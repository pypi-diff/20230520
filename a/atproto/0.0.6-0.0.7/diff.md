# Comparing `tmp/atproto-0.0.6.tar.gz` & `tmp/atproto-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.6.tar", max compression
+gzip compressed data, was "atproto-0.0.7.tar", max compression
```

## Comparing `atproto-0.0.6.tar` & `atproto-0.0.7.tar`

### file list

```diff
@@ -1,170 +1,170 @@
--rw-r--r--   0        0        0     1061 2023-05-19 21:17:17.186501 atproto-0.0.6/LICENSE
--rw-r--r--   0        0        0     9588 2023-05-19 21:17:17.186501 atproto-0.0.6/README.md
--rw-r--r--   0        0        0      332 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/__init__.py
--rw-r--r--   0        0        0     1764 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/car/__init__.py
--rw-r--r--   0        0        0      137 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/cid/__init__.py
--rw-r--r--   0        0        0       23 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/cli/__init__.py
--rw-r--r--   0        0        0     2767 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/clients/__init__.py
--rw-r--r--   0        0        0     1319 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/clients/generate_async_client.py
--rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/models/__init__.py
--rw-r--r--   0        0        0     2353 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/models/builder.py
--rw-r--r--   0        0        0    19303 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/models/generator.py
--rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/namespaces/__init__.py
--rw-r--r--   0        0        0     2562 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/namespaces/builder.py
--rw-r--r--   0        0        0    11855 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/codegen/namespaces/generator.py
--rw-r--r--   0        0        0      944 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/exceptions.py
--rw-r--r--   0        0        0     2569 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/leb128/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:17:17.186501 atproto-0.0.6/atproto/lexicon/__init__.py
--rw-r--r--   0        0        0     4658 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/lexicon/models.py
--rw-r--r--   0        0        0     3871 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/lexicon/parser.py
--rw-r--r--   0        0        0     5298 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/nsid/__init__.py
--rw-r--r--   0        0        0     3075 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/uri/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/__init__.py
--rw-r--r--   0        0        0     7289 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/async_client.py
--rw-r--r--   0        0        0      489 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/async_raw.py
--rw-r--r--   0        0        0      421 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/auth.py
--rw-r--r--   0        0        0     3719 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/base.py
--rw-r--r--   0        0        0     6786 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/client.py
--rw-r--r--   0        0        0       76 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/methods_mixin/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/methods_mixin/session.py
--rw-r--r--   0        0        0      469 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/client/raw.py
--rw-r--r--   0        0        0    11424 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/__init__.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/__init__.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/__init__.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0     4054 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      820 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      836 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      890 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0     1014 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      927 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      670 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0     1061 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      970 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0     1778 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1564 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2457 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1248 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0     4321 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1041 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0     1497 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0     1076 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      855 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0     1181 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0     1066 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      734 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2441 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/post.py
--rw-r--r--   0        0        0      738 2023-05-19 21:17:17.190502 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/repost.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      665 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2446 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      667 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/follow.py
--rw-r--r--   0        0        0     1004 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0     1133 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0     1123 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0     1097 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0     1004 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0     1033 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      999 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0     1121 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/list.py
--rw-r--r--   0        0        0      705 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      574 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      575 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      576 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      577 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      830 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1932 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      586 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0     1735 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      553 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/base.py
--rw-r--r--   0        0        0      713 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/blob_ref.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/__init__.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/__init__.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0    10850 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      595 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      712 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      594 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0     1071 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      839 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0     1097 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      839 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1231 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      890 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      824 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      953 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      911 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0     1129 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1370 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      651 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      621 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      887 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      586 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0     1077 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0     1499 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      825 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0     2140 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0     1236 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      969 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0     1038 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1171 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1817 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1319 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      734 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      644 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      742 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_account.py
--rw-r--r--   0        0        0     1052 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      880 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0     1352 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0     1117 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1296 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/defs.py
--rw-r--r--   0        0        0      659 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0     1271 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0     1028 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      704 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_session.py
--rw-r--r--   0        0        0     1024 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      729 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      589 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      628 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      583 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0      323 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      752 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      744 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      822 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      986 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      764 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      872 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      916 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      969 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0     1253 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      637 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      640 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2782 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      547 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/type_conversion.py
--rw-r--r--   0        0        0     3285 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/models/utils.py
--rw-r--r--   0        0        0        0 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/namespaces/__init__.py
--rw-r--r--   0        0        0    73381 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/namespaces/async_ns.py
--rw-r--r--   0        0        0      361 2023-05-19 21:17:17.194501 atproto-0.0.6/atproto/xrpc_client/namespaces/base.py
--rw-r--r--   0        0        0    72323 2023-05-19 21:17:17.198502 atproto-0.0.6/atproto/xrpc_client/namespaces/sync_ns.py
--rw-r--r--   0        0        0     4353 2023-05-19 21:17:17.198502 atproto-0.0.6/atproto/xrpc_client/request.py
--rw-r--r--   0        0        0       43 2023-05-19 21:17:17.198502 atproto-0.0.6/atproto/xrpc_server/__init__.py
--rw-r--r--   0        0        0     2396 2023-05-19 21:17:44.930884 atproto-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    11262 1970-01-01 00:00:00.000000 atproto-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-20 15:15:38.757786 atproto-0.0.7/LICENSE
+-rw-r--r--   0        0        0     9588 2023-05-20 15:15:38.757786 atproto-0.0.7/README.md
+-rw-r--r--   0        0        0      332 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/__init__.py
+-rw-r--r--   0        0        0     1761 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/car/__init__.py
+-rw-r--r--   0        0        0      137 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/cid/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/cli/__init__.py
+-rw-r--r--   0        0        0     2790 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0     1434 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0     2345 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    19267 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0     2546 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11836 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0      944 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/exceptions.py
+-rw-r--r--   0        0        0     2569 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/leb128/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0     4790 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3857 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5295 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     3064 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/uri/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0     7596 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0      414 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/auth.py
+-rw-r--r--   0        0        0     3748 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     7105 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0       76 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/methods_mixin/__init__.py
+-rw-r--r--   0        0        0     1311 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/methods_mixin/session.py
+-rw-r--r--   0        0        0      469 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    11424 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     4112 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      820 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      833 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      889 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0     1007 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      926 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      670 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0     1056 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      961 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1773 2023-05-20 15:15:38.757786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1563 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2444 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1243 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     4340 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1034 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0     1494 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0     1057 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      854 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1178 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0     1061 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      734 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2426 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      738 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2448 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      667 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      997 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1126 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1116 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0     1090 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      997 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0     1026 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      992 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0     1114 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      705 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      574 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      575 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      576 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      577 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1933 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      586 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1734 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0     1077 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      553 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0    10957 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      595 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      705 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      594 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0     1066 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      836 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0     1092 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      836 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1230 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      879 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      821 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      946 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      908 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1126 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1351 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      651 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      621 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      880 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      586 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1235 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1322 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1066 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0     1488 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      845 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     2121 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1233 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      964 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0     1035 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1166 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1816 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1316 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      727 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      644 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      736 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0     1208 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0     1049 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      873 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1345 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0     1110 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1293 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      659 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1266 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0     1019 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      697 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0     1021 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      729 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      589 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      628 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      583 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      746 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      734 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      808 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      977 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      764 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      858 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      904 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      960 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1246 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      637 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      640 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2774 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      547 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/type_conversion.py
+-rw-r--r--   0        0        0     3254 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0    73557 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      344 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    72513 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4338 2023-05-20 15:15:38.761786 atproto-0.0.7/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-20 15:15:38.765786 atproto-0.0.7/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0     2396 2023-05-20 15:16:02.758155 atproto-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    11262 1970-01-01 00:00:00.000000 atproto-0.0.7/PKG-INFO
```

### Comparing `atproto-0.0.6/LICENSE` & `atproto-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/README.md` & `atproto-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/car/__init__.py` & `atproto-0.0.7/atproto/car/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import typing as t
 from io import BytesIO
-from typing import Dict
 
 import dag_cbor
 
 from .. import leb128
 from ..cid import CID
 
-Nodes = Dict[CID, dict]
+Nodes = t.Dict[CID, dict]
 
 
 class CAR:
     """CAR file."""
 
     _CID_V1_BYTES_LEN = 36
```

### Comparing `atproto-0.0.6/atproto/codegen/__init__.py` & `atproto-0.0.7/atproto/codegen/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 import subprocess
+import typing as t
 from pathlib import Path
-from typing import List, Tuple
 
 from atproto.nsid import NSID
 
 DISCLAIMER = [
     '# THIS IS THE AUTO-GENERATED CODE. DON\'T EDIT IT BY HANDS!',
     '# Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.',
     '# This file is part of Python atproto SDK. Licenced under MIT.',
@@ -39,15 +39,15 @@
     if append:
         mode = 'a'
 
     with open(filepath, mode=mode, encoding='UTF-8') as f:
         f.write(code)
 
 
-def get_file_path_parts(nsid: NSID) -> List[str]:
+def get_file_path_parts(nsid: NSID) -> t.List[str]:
     return nsid.segments[:-1] + [f'{convert_camel_case_to_snake_case(nsid.name)}.py']
 
 
 def get_import_path_old(nsid: NSID) -> str:
     return '.'.join(nsid.segments[:-1] + [f'{convert_camel_case_to_snake_case(nsid.name)}'])
 
 
@@ -58,39 +58,39 @@
 
 
 def convert_camel_case_to_snake_case(string: str) -> str:
     s = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', string)
     return re.sub('([a-z0-9])([A-Z])', r'\1_\2', s).lower()
 
 
-def camel_case_split(string: str):
+def camel_case_split(string: str) -> t.List[str]:
     # regex by chatgpt
     return re.findall(r'[A-Z]?[a-z]+|[A-Z]+(?=[A-Z]|$)', string)
 
 
-def gen_description_by_camel_case_name(name: str):
+def gen_description_by_camel_case_name(name: str) -> str:
     words = camel_case_split(name)
     words = [w.lower() for w in words]
     words[0] = words[0].capitalize()
     return ' '.join(words)
 
 
 def sort_dict_by_key(d: dict) -> dict:
     return dict(sorted(d.items()))
 
 
-def get_code_intent(level: int):
+def get_code_intent(level: int) -> str:
     return ' ' * 4 * level
 
 
-def join_code(lines: List[str]) -> str:
+def join_code(lines: t.List[str]) -> str:
     return '\n'.join(lines)
 
 
-def get_sync_async_keywords(*, sync: bool) -> Tuple[str, str]:
+def get_sync_async_keywords(*, sync: bool) -> t.Tuple[str, str]:
     definition, call = 'async ', 'await '
     if sync:
         definition, call = '', ''
 
     return definition, call
```

### Comparing `atproto-0.0.6/atproto/codegen/clients/generate_async_client.py` & `atproto-0.0.7/atproto/codegen/clients/generate_async_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,18 +14,21 @@
         'send_post',
         'send_image',
         '_get_and_set_session',
         '_refresh_and_set_session',
         '_invoke',
     ]
 
+    code = code.replace('from threading', 'from asyncio')
     code = code.replace('client.raw', 'client.async_raw')
     code = code.replace('class Client', 'class AsyncClient')
     code = code.replace('ClientRaw', 'AsyncClientRaw')
 
+    code = code.replace('with self', 'async with self')
+
     code = code.replace('def', 'async def')
     code = code.replace('async def __', 'def __')
 
     code = code.replace('self.com', 'await self.com')
     code = code.replace('self.bsky', 'await self.bsky')
 
     for method in methods:
```

### Comparing `atproto-0.0.6/atproto/codegen/models/builder.py` & `atproto-0.0.7/atproto/codegen/models/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Union
+import typing as t
 
 from atproto.lexicon import models
 from atproto.lexicon.parser import lexicon_parse_dir
 from atproto.nsid import NSID
 
 _LEX_DEF_TYPES_FOR_PARAMS = {models.LexDefinitionType.QUERY, models.LexDefinitionType.PROCEDURE}
 _LEX_DEF_TYPES_FOR_RESPONSES = {models.LexDefinitionType.QUERY, models.LexDefinitionType.PROCEDURE}
@@ -12,33 +12,33 @@
 _LEX_DEF_TYPES_FOR_DEF = {
     models.LexDefinitionType.OBJECT,
     models.LexPrimitiveType.STRING,
     models.LexDefinitionType.TOKEN,
     models.LexDefinitionType.ARRAY,
 }
 
-LexDefs = Dict[
+LexDefs = t.Dict[
     str,
-    Union[
+    t.Union[
         models.LexXrpcProcedure,
         models.LexXrpcQuery,
         models.LexObject,
         models.LexToken,
         models.LexString,
         models.LexRecord,
     ],
 ]
-LexDB = Dict[NSID, LexDefs]
+LexDB = t.Dict[NSID, LexDefs]
 
 
-def _filter_defs_by_type(defs: Dict[str, models.LexDefinition], def_types: set) -> LexDefs:
+def _filter_defs_by_type(defs: t.Dict[str, models.LexDefinition], def_types: set) -> LexDefs:
     return {k: v for k, v in defs.items() if v.type in def_types}
 
 
-def _build_nsid_to_defs_map(lexicons: List[models.LexiconDoc], def_types: set) -> LexDB:
+def _build_nsid_to_defs_map(lexicons: t.List[models.LexiconDoc], def_types: set) -> LexDB:
     result = {}
 
     for lexicon in lexicons:
         nsid = NSID.from_str(lexicon.id)
         defs = _filter_defs_by_type(lexicon.defs, def_types)
         if defs:
             result[nsid] = defs
```

### Comparing `atproto-0.0.6/atproto/codegen/models/generator.py` & `atproto-0.0.7/atproto/codegen/models/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
+import typing as t
 from enum import Enum
 from pathlib import Path
-from typing import Tuple, Union
 
 from atproto.codegen import (
     DISCLAIMER,
     INPUT_MODEL,
     OUTPUT_MODEL,
     PARAMS_MODEL,
     append_code,
@@ -49,17 +49,17 @@
     append_code(_MODELS_OUTPUT_DIR.joinpath(path_to_file), code)
 
 
 def _get_model_imports() -> str:
     # TODO(MarshalX): isort can't delete unused imports. mb add ruff
     lines = [
         'from dataclasses import dataclass',
-        'from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union',
+        'import typing as t',
         '',
-        'from typing_extensions import Literal',
+        'import typing_extensions as te',
         'from atproto.xrpc_client import models',
         'from atproto.xrpc_client.models import base',
         'from atproto.xrpc_client.models.blob_ref import BlobRef',
         '',
         'from atproto import CID',
         '',
     ]
@@ -101,25 +101,25 @@
     models.LexInteger: 'int',
     models.LexBoolean: 'bool',
 }
 
 
 def _get_optional_typehint(type_hint, *, optional: bool) -> str:
     if optional:
-        return f'Optional[{type_hint}] = None'
+        return f't.Optional[{type_hint}] = None'
     else:
         return type_hint
 
 
 def _get_ref_typehint(nsid: NSID, field_type_def, *, optional: bool) -> str:
     model_path, _ = _resolve_nsid_ref(nsid, field_type_def.ref)
     return _get_optional_typehint(f"'{model_path}'", optional=optional)
 
 
-def _resolve_nsid_ref(nsid: NSID, ref: str, *, local: bool = False) -> Tuple[str, str]:
+def _resolve_nsid_ref(nsid: NSID, ref: str, *, local: bool = False) -> t.Tuple[str, str]:
     """Returns path to the model and model name"""
     if '#' in ref:
         ref_nsid_str, def_name = ref.split('#', 1)
         def_name = get_def_model_name(def_name)
 
         try:
             ref_nsid = NSID.from_str(ref_nsid_str)
@@ -147,18 +147,18 @@
         def_names.append(import_path)
 
     # unbelievable but it's true. If schema doesn't describe the right type in Union
     # we should fall back to the plain data
     # maybe it's for the records that have custom fields... idk
     # ref: https://github.com/bluesky-social/atproto/blob/b01e47b61730d05a780f7a42667b91ccaa192e8e/packages/lex-cli/src/codegen/lex-gen.ts#L325
     # grep by "{$type: string; [k: string]: unknown}" string
-    def_names.append('Dict[str, Any]')
+    def_names.append('t.Dict[str, t.Any]')
 
     def_names = ', '.join([f"'{name}'" for name in def_names])
-    return _get_optional_typehint(f"Union[{def_names}]", optional=optional)
+    return _get_optional_typehint(f"t.Union[{def_names}]", optional=optional)
 
 
 def _get_model_field_typehint(nsid: NSID, field_name: str, field_type_def, *, optional: bool) -> str:
     field_type = type(field_type_def)
 
     if field_type == models.LexUnknown:
         # TODO(MarshalX): some of "unknown" types are well known...
@@ -166,50 +166,50 @@
 
     type_hint = _LEXICON_TYPE_TO_PRIMITIVE_TYPEHINT.get(field_type)
     if type_hint:
         return _get_optional_typehint(type_hint, optional=optional)
 
     if field_type is models.LexArray:
         items_type_hint = _get_model_field_typehint(nsid, field_name, field_type_def.items, optional=False)
-        return _get_optional_typehint(f'List[{items_type_hint}]', optional=optional)
+        return _get_optional_typehint(f't.List[{items_type_hint}]', optional=optional)
 
     if field_type is models.LexRef:
         return _get_ref_typehint(nsid, field_type_def, optional=optional)
 
     if field_type is models.LexRefUnion:
         return _get_ref_union_typehint(nsid, field_type_def, optional=optional)
 
     if field_type is models.LexCidLink:
         return _get_optional_typehint(f'CID', optional=optional)
 
     if field_type is models.LexBytes:
         # CAR file containing relevant blocks
-        return _get_optional_typehint('Union[str, bytes]', optional=optional)
+        return _get_optional_typehint('t.Union[str, bytes]', optional=optional)
 
     if field_type is models.LexBlob:
         # yes, it returns blob,but actually it's blob ref here
         return _get_optional_typehint('BlobRef', optional=optional)
 
     raise ValueError(f'Unknown field type {field_name.__name__}')
 
 
-def _get_req_fields_set(lex_obj: Union[models.LexObject, models.LexXrpcParameters]) -> set:
+def _get_req_fields_set(lex_obj: t.Union[models.LexObject, models.LexXrpcParameters]) -> set:
     required_fields = set()
     if lex_obj.required:
         required_fields = set(lex_obj.required)
 
     if hasattr(lex_obj, 'nullable') and lex_obj.nullable:
         # TODO(MarshalX): not 100% the same thing. think about it
         required_fields = required_fields.difference(set(lex_obj.nullable))
 
     return required_fields
 
 
 def _get_model_docstring(
-    nsid: Union[str, NSID], lex_object: Union[models.LexObject, models.LexXrpcParameters], model_type: ModelType
+    nsid: t.Union[str, NSID], lex_object: t.Union[models.LexObject, models.LexXrpcParameters], model_type: ModelType
 ) -> str:
     model_desc = lex_object.description or ''
     model_desc = f"{model_type.value} model for :obj:`{nsid}`. {model_desc}"
 
     doc_string = [f'{_(1)}"""{model_desc}', '', f'{_(1)}Attributes:']
 
     for field_name, field_type in lex_object.properties.items():
@@ -223,15 +223,15 @@
 
     doc_string.append(f'{_(1)}"""')
     doc_string.append('')
 
     return join_code(doc_string)
 
 
-def _get_model(nsid: NSID, lex_object: Union[models.LexObject, models.LexXrpcParameters]) -> str:
+def _get_model(nsid: NSID, lex_object: t.Union[models.LexObject, models.LexXrpcParameters]) -> str:
     required_fields = _get_req_fields_set(lex_object)
 
     fields = []
     optional_fields = []
 
     for field_name, field_type in lex_object.properties.items():
         is_optional = field_name not in required_fields
@@ -252,33 +252,33 @@
 
     return join_code(fields)
 
 
 def _get_model_ref(nsid: NSID, ref: models.LexRef) -> str:
     # FIXME(MarshalX): "local=True" Is it works well? ;d
     ref_class, _ = _resolve_nsid_ref(nsid, ref.ref, local=True)
-    ref_typehint = f'Type[{ref_class}]'
+    ref_typehint = f't.Type[{ref_class}]'
 
     # "Ref" suffix required to fix name collisions from different namespaces
     lines = [
         f'#: {OUTPUT_MODEL} reference to :obj:`{ref_class}` model.',
         f'{OUTPUT_MODEL}Ref: {ref_typehint} = {ref_class}',
         '',
         '',
     ]
 
     return join_code(lines)
 
 
 def _get_model_raw_data(name: str) -> str:
-    lines = [f'#: {name} raw data type.', f'{name}: Union[Type[str], Type[bytes]] = bytes\n\n']
+    lines = [f'#: {name} raw data type.', f'{name}: t.Union[t.Type[str], t.Type[bytes]] = bytes\n\n']
     return join_code(lines)
 
 
-def _generate_params_model(nsid: NSID, definition: Union[models.LexXrpcProcedure, models.LexXrpcQuery]) -> str:
+def _generate_params_model(nsid: NSID, definition: t.Union[models.LexXrpcProcedure, models.LexXrpcQuery]) -> str:
     lines = [_get_model_class_def(nsid.name, ModelType.PARAMS)]
 
     if definition.parameters:
         lines.append(_get_model_docstring(nsid, definition.parameters, ModelType.PARAMS))
         lines.append(_get_model(nsid, definition.parameters))
 
     return join_code(lines)
@@ -328,15 +328,15 @@
     lines.append('')
 
     return join_code(lines)
 
 
 def _generate_def_token(def_name: str) -> str:
     lines = [
-        f"{get_def_model_name(def_name)}: Literal['{def_name}'] = '{def_name}'",
+        f"{get_def_model_name(def_name)}: te.Literal['{def_name}'] = '{def_name}'",
         '',
         '',
     ]
     return join_code(lines)
 
 
 def _generate_def_array(nsid: NSID, def_name: str, def_model: models.LexArray) -> str:
@@ -349,15 +349,15 @@
     if not def_model.knownValues:
         return ''
 
     # FIXME(MarshalX): Use ref resolver
     known_values = ["'" + get_def_model_name(v.split('#', 1)[1]) + "'" for v in def_model.knownValues]
     known_values = ', '.join(known_values)
 
-    type_ = f'Literal[{known_values}]'
+    type_ = f'te.Literal[{known_values}]'
 
     lines = [
         f"{get_def_model_name(def_name)} = {type_}",
         '',
         '',
     ]
```

### Comparing `atproto-0.0.6/atproto/codegen/namespaces/builder.py` & `atproto-0.0.7/atproto/codegen/namespaces/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from typing import Dict, List, NamedTuple, Union
+import typing as t
 
 from atproto.lexicon.models import (
     LexDefinition,
     LexDefinitionType,
     LexiconDoc,
     LexRecord,
     LexXrpcProcedure,
     LexXrpcQuery,
 )
 from atproto.lexicon.parser import lexicon_parse_dir
 from atproto.nsid import NSID
 
 _VALID_LEX_DEF_TYPES = {LexDefinitionType.QUERY, LexDefinitionType.PROCEDURE, LexDefinitionType.RECORD}
-_VALID_LEX_DEF_TYPE = Union[LexXrpcProcedure, LexXrpcQuery, LexRecord]
+_VALID_LEX_DEF_TYPE = t.Union[LexXrpcProcedure, LexXrpcQuery, LexRecord]
 
 
-def _filter_namespace_valid_definitions(definitions: Dict[str, LexDefinition]) -> Dict[str, LexDefinition]:
+def _filter_namespace_valid_definitions(definitions: t.Dict[str, LexDefinition]) -> t.Dict[str, LexDefinition]:
     result = {}
 
     for def_name, def_content in definitions.items():
         if def_content.type in _VALID_LEX_DEF_TYPES:
             result[def_name] = def_content
 
     return result
 
 
-def get_definition_by_name(name: str, defs: Dict[str, LexDefinition]) -> LexDefinition:
+def get_definition_by_name(name: str, defs: t.Dict[str, LexDefinition]) -> LexDefinition:
     if name in defs:
         return defs[name]
 
     return defs['main']
 
 
-class ObjectInfo(NamedTuple):
+class ObjectInfo(t.NamedTuple):
     name: str
     nsid: NSID
     definition: _VALID_LEX_DEF_TYPE
 
 
 class MethodInfo(ObjectInfo):
     pass
 
 
 class RecordInfo(ObjectInfo):
     pass
 
 
-def _enrich_namespace_tree(root: dict, nsid: NSID, defs: Dict[str, LexDefinition]) -> None:
+def _enrich_namespace_tree(root: dict, nsid: NSID, defs: t.Dict[str, LexDefinition]) -> None:
     segments_count = len(nsid.segments)
     for path_level, segment in enumerate(nsid.segments):
         # if method
         if path_level == segments_count - 1:
             definition = get_definition_by_name(segment, defs)
 
             model_class = MethodInfo
@@ -67,15 +67,15 @@
             if path_level == segments_count - 2:
                 root[segment] = []
             else:
                 root[segment] = {}
         root = root[segment]
 
 
-def build_namespace_tree(lexicons: List[LexiconDoc]) -> dict:
+def build_namespace_tree(lexicons: t.List[LexiconDoc]) -> dict:
     namespace_tree = {}
     for lexicon in lexicons:
         defs = _filter_namespace_valid_definitions(lexicon.defs)
         if not defs:
             continue
 
         nsid = NSID.from_str(lexicon.id)
```

### Comparing `atproto-0.0.6/atproto/codegen/namespaces/generator.py` & `atproto-0.0.7/atproto/codegen/namespaces/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import typing as t
 from pathlib import Path
-from typing import List, Set, Union
 
 from atproto.codegen import (
     DISCLAIMER,
     INPUT_MODEL,
     OUTPUT_MODEL,
     PARAMS_MODEL,
     convert_camel_case_to_snake_case,
@@ -45,15 +45,15 @@
     return f'{path_part.capitalize()}{_RECORD_SUFFIX}'
 
 
 def _get_namespace_imports() -> str:
     lines = [
         DISCLAIMER,
         'from dataclasses import dataclass, field',
-        'from typing import Optional, Union',
+        'import typing as t',
         '',
         'from atproto.xrpc_client import models',
         'from atproto.xrpc_client.models.utils import get_or_create_model, get_response_model',
         'from atproto.xrpc_client.namespaces.base import DefaultNamespace, NamespaceBase',
     ]
 
     return join_code(lines)
@@ -176,23 +176,23 @@
 def _get_namespace_method_signature_arg(
     name: str, nsid: NSID, model_name: str, *, optional: bool, alias: bool = False
 ) -> str:
     if alias:
         return f"{name}: 'models.{get_import_path(nsid)}.{model_name}'"
 
     default_value = ''
-    type_hint = f"Union[dict, 'models.{get_import_path(nsid)}.{model_name}']"
+    type_hint = f"t.Union[dict, 'models.{get_import_path(nsid)}.{model_name}']"
     if optional:
-        type_hint = f'Optional[{type_hint}]'
+        type_hint = f't.Optional[{type_hint}]'
         default_value = ' = None'
 
     return f'{name}: {type_hint}{default_value}'
 
 
-def _get_namespace_method_signature_args_names(method_info: MethodInfo) -> Set[str]:
+def _get_namespace_method_signature_args_names(method_info: MethodInfo) -> t.Set[str]:
     args = {'self'}
     if method_info.definition.parameters:
         args.add('params')
 
     if method_info.definition.type is LexDefinitionType.PROCEDURE and method_info.definition.input:
         if method_info.definition.input.schema:
             args.add('data_schema')
@@ -269,36 +269,36 @@
     name = convert_camel_case_to_snake_case(method_info.name)
     args = _get_namespace_method_signature_args(method_info)
     return_type = _get_namespace_method_return_type(method_info)
 
     return f'{_(1)}{d}def {name}({args}) -> {return_type}:'
 
 
-def _get_namespace_methods_block(methods_info: List[MethodInfo], sync: bool) -> str:
+def _get_namespace_methods_block(methods_info: t.List[MethodInfo], sync: bool) -> str:
     lines = []
 
     methods_info.sort(key=lambda e: e.name)
     for method_info in methods_info:
         lines.append(_get_namespace_method_signature(method_info, sync=sync))
         lines.append(_get_namespace_method_body(method_info, sync=sync))
 
     return join_code(lines)
 
 
-def _get_namespace_records_block(records_info: List[RecordInfo]) -> str:
+def _get_namespace_records_block(records_info: t.List[RecordInfo]) -> str:
     lines = []
 
     records_info.sort(key=lambda e: e.name)
     for record_info in records_info:
         lines.append(f"{_(1)}{record_info.name}: '{get_record_name(record_info.name)}' = DefaultNamespace()")
 
     return join_code(lines)
 
 
-def _generate_namespace_in_output(namespace_tree: Union[dict, list], output: List[str], *, sync: bool) -> None:
+def _generate_namespace_in_output(namespace_tree: t.Union[dict, list], output: t.List[str], *, sync: bool) -> None:
     for node_name, sub_node in namespace_tree.items():
         if isinstance(sub_node, dict):
             output.append(_get_namespace_class_def(node_name))
             output.append(_get_sub_namespaces_block(sub_node))
             output.append(_get_post_init_method(sub_node))
 
             _generate_namespace_in_output(sub_node, output, sync=sync)
```

### Comparing `atproto-0.0.6/atproto/exceptions.py` & `atproto-0.0.7/atproto/exceptions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/leb128/__init__.py` & `atproto-0.0.7/atproto/leb128/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/lexicon/parser.py` & `atproto-0.0.7/atproto/lexicon/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
+import typing as t
 from enum import Enum
 from pathlib import Path
-from typing import List, Optional, Union
 
 import dacite
 
 from atproto.exceptions import (
     LexiconParsingError,
     UnknownDefinitionTypeError,
     UnknownPrimitiveTypeError,
@@ -68,27 +68,27 @@
 def lexicon_parse(data: dict, data_class=None):
     if not data_class:
         data_class = models.LexiconDoc
 
     return dacite.from_dict(data_class=data_class, data=data, config=_DEFAULT_DACITE_CONFIG)
 
 
-def lexicon_parse_file(lexicon_path: Union[Path, str], *, soft_fail: bool = False) -> Optional[models.LexiconDoc]:
+def lexicon_parse_file(lexicon_path: t.Union[Path, str], *, soft_fail: bool = False) -> t.Optional[models.LexiconDoc]:
     try:
         with open(lexicon_path, 'r', encoding='UTF-8') as f:
             plain_lexicon = json.loads(f.read())
             return lexicon_parse(plain_lexicon)
     except Exception as e:
         if soft_fail:
             return None
 
         raise LexiconParsingError("Can't parse lexicon") from e
 
 
-def lexicon_parse_dir(path: Union[Path, str] = None, *, soft_fail: bool = False) -> List[models.LexiconDoc]:
+def lexicon_parse_dir(path: t.Union[Path, str] = None, *, soft_fail: bool = False) -> t.List[models.LexiconDoc]:
     if path is None:
         path = _PATH_TO_LEXICONS
 
     parsed_lexicons = []
 
     for _, _, lexicons in os.walk(path):
         for lexicon in lexicons:
```

### Comparing `atproto-0.0.6/atproto/nsid/__init__.py` & `atproto-0.0.7/atproto/nsid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
+import typing as t
 from dataclasses import dataclass, field
-from typing import List
 
 from atproto.exceptions import InvalidNsidError
 
 _NSID_DELIM = '.'
 _NSID_NAMESPACE = '*'
 
 _MAX_NSID_LEN = 253 + 1 + 128
@@ -14,15 +14,15 @@
 _MIN_NSID_SEGMENTS_COUNT = 3
 
 _NSID_VALID_CHARS_REGEX = r'^[a-zA-Z0-9.-]*$'
 _NSID_PART_VALID_CHARS_REGEX = r'^[a-zA-Z]'
 
 _NSID_PART_FORBIDDEN_END = '-'
 
-Segments = List[str]
+Segments = t.List[str]
 
 
 @dataclass
 class NSID:
     """NameSpaced IDs (NSIDs).
 
     Examples:
```

### Comparing `atproto-0.0.6/atproto/uri/__init__.py` & `atproto-0.0.7/atproto/uri/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
+import typing as t
 import urllib.parse as urlparse
-from typing import Any, List, Tuple
 from urllib.parse import urlencode
 
 from atproto.exceptions import InvalidAtUriError
 
 # ref: https://github.com/bluesky-social/atproto/blob/8c19ce991a766fd9cff5023160853ab1cb106f21/packages/uri/src/index.ts#LL5C38-L5C38
 _ATP_URI_REGEX = r'^(at:\/\/)?((?:did:[a-z0-9:%-]+)|(?:[a-z][a-z0-9.:-]*))(\/[^?#\s]*)?(\?[^#\s]+)?(#[^\s]+)?$'
 
@@ -20,15 +20,15 @@
         Collection: at://alice.host.com/io.example.song
 
         Record: at://alice.host.com/io.example.song/3yI5-c1z-cc2p-1a
 
         Record Field: at://alice.host.com/io.example.song/3yI5-c1z-cc2p-1a#/title
     """
 
-    def __init__(self, host: str, pathname: str, hash_: str, search_params: List[Tuple[str, Any]]):
+    def __init__(self, host: str, pathname: str, hash_: str, search_params: t.List[t.Tuple[str, t.Any]]):
         self.host = host
         self.pathname = pathname
         self.hash = hash_
         self.search_params = search_params
 
     @property
     def protocol(self) -> str:
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/client/async_client.py` & `atproto-0.0.7/atproto/xrpc_client/client/async_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,65 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
+import typing as t
+from asyncio import Lock
 from datetime import datetime
-from typing import TYPE_CHECKING, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.client.async_raw import AsyncClientRaw
 from atproto.xrpc_client.client.methods_mixin import SessionMethodsMixin
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from atproto.xrpc_client.client.auth import JwtPayload
     from atproto.xrpc_client.client.base import InvokeType
     from atproto.xrpc_client.request import Response
 
 
 class AsyncClient(AsyncClientRaw, SessionMethodsMixin):
     """High-level client for XRPC of ATProto."""
 
     def __init__(self, base_url: str = None):
         super().__init__(base_url)
 
-        self._access_jwt: Optional[str] = None
-        self._access_jwt_payload: Optional['JwtPayload'] = None
+        self._access_jwt: t.Optional[str] = None
+        self._access_jwt_payload: t.Optional['JwtPayload'] = None
 
-        self._refresh_jwt: Optional[str] = None
-        self._refresh_jwt_payload: Optional['JwtPayload'] = None
+        self._refresh_jwt: t.Optional[str] = None
+        self._refresh_jwt_payload: t.Optional['JwtPayload'] = None
 
-        self.me: Optional[models.AppBskyActorDefs.ProfileViewDetailed] = None
+        self._refresh_lock = Lock()
+
+        self.me: t.Optional[models.AppBskyActorDefs.ProfileViewDetailed] = None
 
     async def _invoke(self, invoke_type: 'InvokeType', **kwargs) -> 'Response':
-        if self.me and self._should_refresh_session():
-            await self._refresh_and_set_session()
+        session_refreshing = kwargs.pop('session_refreshing', False)
+        if session_refreshing:
+            return await super()._invoke(invoke_type, **kwargs)
+
+        async with self._refresh_lock:
+            if self._access_jwt and self._should_refresh_session():
+                await self._refresh_and_set_session()
 
         return await super()._invoke(invoke_type, **kwargs)
 
     async def _get_and_set_session(self, login: str, password: str) -> models.ComAtprotoServerCreateSession.Response:
         session = await self.com.atproto.server.create_session(
             models.ComAtprotoServerCreateSession.Data(login, password)
         )
         self._set_session(session)
 
         return session
 
     async def _refresh_and_set_session(self) -> models.ComAtprotoServerRefreshSession.Response:
         refresh_session = await self.com.atproto.server.refresh_session(
-            headers=self._get_auth_headers(self._refresh_jwt)
+            headers=self._get_auth_headers(self._refresh_jwt), session_refreshing=True
         )
         self._set_session(refresh_session)
 
         return refresh_session
 
     async def login(self, login: str, password: str) -> models.AppBskyActorGetProfile.ResponseRef:
         """Authorize client and get profile info.
@@ -71,18 +79,18 @@
         self.me = await self.bsky.actor.get_profile(models.AppBskyActorGetProfile.Params(session.handle))
 
         return self.me
 
     async def send_post(
         self,
         text: str,
-        profile_identify: Optional[str] = None,
-        reply_to: Optional[Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
-        embed: Optional[
-            Union[
+        profile_identify: t.Optional[str] = None,
+        reply_to: t.Optional[t.Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
+        embed: t.Optional[
+            t.Union[
                 'models.AppBskyEmbedImages.Main',
                 'models.AppBskyEmbedExternal.Main',
                 'models.AppBskyEmbedRecord.Main',
                 'models.AppBskyEmbedRecordWithMedia.Main',
             ]
         ] = None,
     ) -> models.ComAtprotoRepoCreateRecord.Response:
@@ -119,16 +127,16 @@
         )
 
     async def send_image(
         self,
         text: str,
         image: bytes,
         image_alt: str,
-        profile_identify: Optional[str] = None,
-        reply_to: Optional[Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
+        profile_identify: t.Optional[str] = None,
+        reply_to: t.Optional[t.Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
     ) -> models.ComAtprotoRepoCreateRecord.Response:
         """Send post with attached image.
 
         Note:
             If `profile_identify` is not provided will be sent to the current profile.
 
         Args:
@@ -171,15 +179,15 @@
             models.ComAtprotoRepoCreateRecord.Data(
                 repo=self.me.did,
                 collection='app.bsky.feed.like',
                 record=models.AppBskyFeedLike.Main(createdAt=datetime.now().isoformat(), subject=subject),
             )
         )
 
-    async def unlike(self, record_key: str, profile_identify: Optional[str] = None) -> bool:
+    async def unlike(self, record_key: str, profile_identify: t.Optional[str] = None) -> bool:
         """Unlike the post.
 
         Args:
             record_key: ID (slog) of the post.
             profile_identify: Handler or DID. Who did the like.
 
         Returns:
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/client/base.py` & `atproto-0.0.7/atproto/xrpc_client/client/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import typing as t
 from enum import Enum
-from typing import Optional
 
 from atproto.xrpc_client.models.utils import get_model_as_dict, get_model_as_json
 from atproto.xrpc_client.request import AsyncRequest, Request, Response
 
 # TODO(MarshalX): Generate async version automatically!
 
 
@@ -40,15 +40,15 @@
     kwargs.pop('input_encoding', None)
     kwargs.pop('output_encoding', None)
 
 
 class ClientBase:
     """Low-level methods are here"""
 
-    def __init__(self, base_url: Optional[str] = None, request: Optional[Request] = None):
+    def __init__(self, base_url: t.Optional[str] = None, request: t.Optional[Request] = None):
         if request is None:
             request = Request()
         if base_url is None:
             base_url = _BASE_API_URL
 
         self._request = request
         self._base_url = base_url
@@ -56,19 +56,21 @@
     @property
     def request(self) -> Request:
         return self._request
 
     def _build_url(self, nsid: str) -> str:
         return f'{self._base_url}/{nsid}'
 
-    def invoke_query(self, nsid: str, params: Optional[dict] = None, data: Optional[dict] = None, **kwargs) -> Response:
+    def invoke_query(
+        self, nsid: str, params: t.Optional[dict] = None, data: t.Optional[dict] = None, **kwargs
+    ) -> Response:
         return self._invoke(InvokeType.QUERY, url=self._build_url(nsid), params=params, data=data, **kwargs)
 
     def invoke_procedure(
-        self, nsid: str, params: Optional[dict] = None, data: Optional[dict] = None, **kwargs
+        self, nsid: str, params: t.Optional[dict] = None, data: t.Optional[dict] = None, **kwargs
     ) -> Response:
         return self._invoke(InvokeType.PROCEDURE, url=self._build_url(nsid), params=params, data=data, **kwargs)
 
     def _invoke(self, invoke_type: InvokeType, **kwargs) -> Response:
         _handle_kwagrs(kwargs)
 
         if invoke_type is InvokeType.QUERY:
@@ -76,15 +78,15 @@
         else:
             return self.request.post(**kwargs)
 
 
 class AsyncClientBase:
     """Low-level methods are here"""
 
-    def __init__(self, base_url: Optional[str] = None, request: Optional[AsyncRequest] = None):
+    def __init__(self, base_url: t.Optional[str] = None, request: t.Optional[AsyncRequest] = None):
         if request is None:
             request = AsyncRequest()
         if base_url is None:
             base_url = _BASE_API_URL
 
         self._request = request
         self._base_url = base_url
@@ -93,20 +95,20 @@
     def request(self) -> AsyncRequest:
         return self._request
 
     def _build_url(self, nsid: str) -> str:
         return f'{self._base_url}/{nsid}'
 
     async def invoke_query(
-        self, nsid: str, params: Optional[dict] = None, data: Optional[dict] = None, **kwargs
+        self, nsid: str, params: t.Optional[dict] = None, data: t.Optional[dict] = None, **kwargs
     ) -> Response:
         return await self._invoke(InvokeType.QUERY, url=self._build_url(nsid), params=params, data=data, **kwargs)
 
     async def invoke_procedure(
-        self, nsid: str, params: Optional[dict] = None, data: Optional[dict] = None, **kwargs
+        self, nsid: str, params: t.Optional[dict] = None, data: t.Optional[dict] = None, **kwargs
     ) -> Response:
         return await self._invoke(InvokeType.PROCEDURE, url=self._build_url(nsid), params=params, data=data, **kwargs)
 
     async def _invoke(self, invoke_type: InvokeType, **kwargs) -> Response:
         _handle_kwagrs(kwargs)
 
         if invoke_type is InvokeType.QUERY:
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/client/client.py` & `atproto-0.0.7/atproto/xrpc_client/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,58 @@
+import typing as t
 from datetime import datetime
-from typing import TYPE_CHECKING, Optional, Union
+from threading import Lock
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.client.methods_mixin import SessionMethodsMixin
 from atproto.xrpc_client.client.raw import ClientRaw
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from atproto.xrpc_client.client.auth import JwtPayload
     from atproto.xrpc_client.client.base import InvokeType
     from atproto.xrpc_client.request import Response
 
 
 class Client(ClientRaw, SessionMethodsMixin):
     """High-level client for XRPC of ATProto."""
 
     def __init__(self, base_url: str = None):
         super().__init__(base_url)
 
-        self._access_jwt: Optional[str] = None
-        self._access_jwt_payload: Optional['JwtPayload'] = None
+        self._access_jwt: t.Optional[str] = None
+        self._access_jwt_payload: t.Optional['JwtPayload'] = None
 
-        self._refresh_jwt: Optional[str] = None
-        self._refresh_jwt_payload: Optional['JwtPayload'] = None
+        self._refresh_jwt: t.Optional[str] = None
+        self._refresh_jwt_payload: t.Optional['JwtPayload'] = None
 
-        self.me: Optional[models.AppBskyActorDefs.ProfileViewDetailed] = None
+        self._refresh_lock = Lock()
+
+        self.me: t.Optional[models.AppBskyActorDefs.ProfileViewDetailed] = None
 
     def _invoke(self, invoke_type: 'InvokeType', **kwargs) -> 'Response':
-        if self.me and self._should_refresh_session():
-            self._refresh_and_set_session()
+        session_refreshing = kwargs.pop('session_refreshing', False)
+        if session_refreshing:
+            return super()._invoke(invoke_type, **kwargs)
+
+        with self._refresh_lock:
+            if self._access_jwt and self._should_refresh_session():
+                self._refresh_and_set_session()
 
         return super()._invoke(invoke_type, **kwargs)
 
     def _get_and_set_session(self, login: str, password: str) -> models.ComAtprotoServerCreateSession.Response:
         session = self.com.atproto.server.create_session(models.ComAtprotoServerCreateSession.Data(login, password))
         self._set_session(session)
 
         return session
 
     def _refresh_and_set_session(self) -> models.ComAtprotoServerRefreshSession.Response:
-        refresh_session = self.com.atproto.server.refresh_session(headers=self._get_auth_headers(self._refresh_jwt))
+        refresh_session = self.com.atproto.server.refresh_session(
+            headers=self._get_auth_headers(self._refresh_jwt), session_refreshing=True
+        )
         self._set_session(refresh_session)
 
         return refresh_session
 
     def login(self, login: str, password: str) -> models.AppBskyActorGetProfile.ResponseRef:
         """Authorize client and get profile info.
 
@@ -61,18 +71,18 @@
         self.me = self.bsky.actor.get_profile(models.AppBskyActorGetProfile.Params(session.handle))
 
         return self.me
 
     def send_post(
         self,
         text: str,
-        profile_identify: Optional[str] = None,
-        reply_to: Optional[Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
-        embed: Optional[
-            Union[
+        profile_identify: t.Optional[str] = None,
+        reply_to: t.Optional[t.Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
+        embed: t.Optional[
+            t.Union[
                 'models.AppBskyEmbedImages.Main',
                 'models.AppBskyEmbedExternal.Main',
                 'models.AppBskyEmbedRecord.Main',
                 'models.AppBskyEmbedRecordWithMedia.Main',
             ]
         ] = None,
     ) -> models.ComAtprotoRepoCreateRecord.Response:
@@ -109,16 +119,16 @@
         )
 
     def send_image(
         self,
         text: str,
         image: bytes,
         image_alt: str,
-        profile_identify: Optional[str] = None,
-        reply_to: Optional[Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
+        profile_identify: t.Optional[str] = None,
+        reply_to: t.Optional[t.Union[models.AppBskyFeedPost.ReplyRef, models.AppBskyFeedDefs.ReplyRef]] = None,
     ) -> models.ComAtprotoRepoCreateRecord.Response:
         """Send post with attached image.
 
         Note:
             If `profile_identify` is not provided will be sent to the current profile.
 
         Args:
@@ -161,15 +171,15 @@
             models.ComAtprotoRepoCreateRecord.Data(
                 repo=self.me.did,
                 collection='app.bsky.feed.like',
                 record=models.AppBskyFeedLike.Main(createdAt=datetime.now().isoformat(), subject=subject),
             )
         )
 
-    def unlike(self, record_key: str, profile_identify: Optional[str] = None) -> bool:
+    def unlike(self, record_key: str, profile_identify: t.Optional[str] = None) -> bool:
         """Unlike the post.
 
         Args:
             record_key: ID (slog) of the post.
             profile_identify: Handler or DID. Who did the like.
 
         Returns:
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/client/methods_mixin/session.py` & `atproto-0.0.7/atproto/xrpc_client/client/methods_mixin/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
+import typing as t
 from datetime import datetime, timedelta, timezone
-from typing import TYPE_CHECKING, Dict, Union
 
 from atproto.xrpc_client.client.auth import get_jwt_payload
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from atproto.xrpc_client import models
 
 
 class SessionMethodsMixin:
     def _should_refresh_session(self) -> bool:
         expired_at = datetime.fromtimestamp(self._access_jwt_payload.exp, tz=timezone.utc)
         expired_at = expired_at - timedelta(minutes=15)  # let's update token a bit later than required
 
         datetime_now = datetime.now(timezone.utc)
 
         return datetime_now > expired_at
 
     def _set_session(
         self,
-        session: Union[
+        session: t.Union[
             'models.ComAtprotoServerCreateSession.Response', 'models.ComAtprotoServerRefreshSession.Response'
         ],
     ) -> None:
         self._access_jwt = session.accessJwt
         self._access_jwt_payload = get_jwt_payload(session.accessJwt)
 
         self._refresh_jwt = session.refreshJwt
         self._refresh_jwt_payload = get_jwt_payload(session.refreshJwt)
 
         self._set_auth_headers(session.accessJwt)
 
     @staticmethod
-    def _get_auth_headers(token: str) -> Dict[str, str]:
+    def _get_auth_headers(token: str) -> t.Dict[str, str]:
         return {'Authorization': f'Bearer {token}'}
 
     def _set_auth_headers(self, token: str) -> None:
         self.request.set_additional_headers(self._get_auth_headers(token))  # noqa
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/__init__.py` & `atproto-0.0.7/atproto/xrpc_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/defs.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ProfileViewBasic(base.ModelBase):
@@ -24,18 +24,18 @@
         avatar: Avatar.
         viewer: Viewer.
         labels: Labels.
     """
 
     did: str
     handle: str
-    avatar: Optional[str] = None
-    displayName: Optional[str] = None
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
-    viewer: Optional['models.AppBskyActorDefs.ViewerState'] = None
+    avatar: t.Optional[str] = None
+    displayName: t.Optional[str] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
+    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None
 
     _type: str = 'app.bsky.actor.defs#profileViewBasic'
 
 
 @dataclass
 class ProfileView(base.ModelBase):
 
@@ -50,20 +50,20 @@
         indexedAt: Indexed at.
         viewer: Viewer.
         labels: Labels.
     """
 
     did: str
     handle: str
-    avatar: Optional[str] = None
-    description: Optional[str] = None
-    displayName: Optional[str] = None
-    indexedAt: Optional[str] = None
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
-    viewer: Optional['models.AppBskyActorDefs.ViewerState'] = None
+    avatar: t.Optional[str] = None
+    description: t.Optional[str] = None
+    displayName: t.Optional[str] = None
+    indexedAt: t.Optional[str] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
+    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None
 
     _type: str = 'app.bsky.actor.defs#profileView'
 
 
 @dataclass
 class ProfileViewDetailed(base.ModelBase):
 
@@ -82,24 +82,24 @@
         indexedAt: Indexed at.
         viewer: Viewer.
         labels: Labels.
     """
 
     did: str
     handle: str
-    avatar: Optional[str] = None
-    banner: Optional[str] = None
-    description: Optional[str] = None
-    displayName: Optional[str] = None
-    followersCount: Optional[int] = None
-    followsCount: Optional[int] = None
-    indexedAt: Optional[str] = None
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
-    postsCount: Optional[int] = None
-    viewer: Optional['models.AppBskyActorDefs.ViewerState'] = None
+    avatar: t.Optional[str] = None
+    banner: t.Optional[str] = None
+    description: t.Optional[str] = None
+    displayName: t.Optional[str] = None
+    followersCount: t.Optional[int] = None
+    followsCount: t.Optional[int] = None
+    indexedAt: t.Optional[str] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
+    postsCount: t.Optional[int] = None
+    viewer: t.Optional['models.AppBskyActorDefs.ViewerState'] = None
 
     _type: str = 'app.bsky.actor.defs#profileViewDetailed'
 
 
 @dataclass
 class ViewerState(base.ModelBase):
 
@@ -110,26 +110,28 @@
         mutedByList: Muted by list.
         blockedBy: Blocked by.
         blocking: Blocking.
         following: Following.
         followedBy: Followed by.
     """
 
-    blockedBy: Optional[bool] = None
-    blocking: Optional[str] = None
-    followedBy: Optional[str] = None
-    following: Optional[str] = None
-    muted: Optional[bool] = None
-    mutedByList: Optional['models.AppBskyGraphDefs.ListViewBasic'] = None
+    blockedBy: t.Optional[bool] = None
+    blocking: t.Optional[str] = None
+    followedBy: t.Optional[str] = None
+    following: t.Optional[str] = None
+    muted: t.Optional[bool] = None
+    mutedByList: t.Optional['models.AppBskyGraphDefs.ListViewBasic'] = None
 
     _type: str = 'app.bsky.actor.defs#viewerState'
 
 
-Preferences = List[
-    Union['models.AppBskyActorDefs.AdultContentPref', 'models.AppBskyActorDefs.ContentLabelPref', 'Dict[str, Any]']
+Preferences = t.List[
+    t.Union[
+        'models.AppBskyActorDefs.AdultContentPref', 'models.AppBskyActorDefs.ContentLabelPref', 't.Dict[str, t.Any]'
+    ]
 ]
 
 
 @dataclass
 class AdultContentPref(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.actor.defs`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profile.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Type
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -21,8 +21,8 @@
         actor: Actor.
     """
 
     actor: str
 
 
 #: Response reference to :obj:`models.AppBskyActorDefs.ProfileViewDetailed` model.
-ResponseRef: Type[models.AppBskyActorDefs.ProfileViewDetailed] = models.AppBskyActorDefs.ProfileViewDetailed
+ResponseRef: t.Type[models.AppBskyActorDefs.ProfileViewDetailed] = models.AppBskyActorDefs.ProfileViewDetailed
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
     """Parameters model for :obj:`app.bsky.actor.getProfiles`.
 
     Attributes:
         actors: Actors.
     """
 
-    actors: List[str]
+    actors: t.List[str]
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.actor.getProfiles`.
 
     Attributes:
         profiles: Profiles.
     """
 
-    profiles: List['models.AppBskyActorDefs.ProfileViewDetailed']
+    profiles: t.List['models.AppBskyActorDefs.ProfileViewDetailed']
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.getSuggestions`.
+    """Parameters model for :obj:`app.bsky.feed.getAuthorFeed`.
 
     Attributes:
+        actor: Actor.
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    actor: str
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.actor.getSuggestions`.
+    """Output data model for :obj:`app.bsky.feed.getAuthorFeed`.
 
     Attributes:
         cursor: Cursor.
-        actors: Actors.
+        feed: Feed.
     """
 
-    actors: List['models.AppBskyActorDefs.ProfileView']
-    cursor: Optional[str] = None
+    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/profile.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/profile.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 from atproto.xrpc_client.models.blob_ref import BlobRef
 
 
 @dataclass
 class Main(base.RecordModelBase):
@@ -20,13 +20,13 @@
     Attributes:
         displayName: Display name.
         description: Description.
         avatar: Avatar.
         banner: Banner.
     """
 
-    avatar: Optional[BlobRef] = None
-    banner: Optional[BlobRef] = None
-    description: Optional[str] = None
-    displayName: Optional[str] = None
+    avatar: t.Optional[BlobRef] = None
+    banner: t.Optional[BlobRef] = None
+    description: t.Optional[str] = None
+    displayName: t.Optional[str] = None
 
     _type: str = 'app.bsky.actor.profile'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.searchActors`.
+    """Parameters model for :obj:`app.bsky.actor.searchActorsTypeahead`.
 
     Attributes:
         term: Term.
         limit: Limit.
-        cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
-    term: Optional[str] = None
+    limit: t.Optional[int] = None
+    term: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.actor.searchActors`.
+    """Output data model for :obj:`app.bsky.actor.searchActorsTypeahead`.
 
     Attributes:
-        cursor: Cursor.
         actors: Actors.
     """
 
-    actors: List['models.AppBskyActorDefs.ProfileView']
-    cursor: Optional[str] = None
+    actors: t.List['models.AppBskyActorDefs.ProfileViewBasic']
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/search_actors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.actor.searchActorsTypeahead`.
+    """Parameters model for :obj:`app.bsky.actor.searchActors`.
 
     Attributes:
         term: Term.
         limit: Limit.
+        cursor: Cursor.
     """
 
-    limit: Optional[int] = None
-    term: Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
+    term: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.actor.searchActorsTypeahead`.
+    """Output data model for :obj:`app.bsky.actor.searchActors`.
 
     Attributes:
+        cursor: Cursor.
         actors: Actors.
     """
 
-    actors: List['models.AppBskyActorDefs.ProfileViewBasic']
+    actors: t.List['models.AppBskyActorDefs.ProfileView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/external.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/external.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 from atproto.xrpc_client.models.blob_ref import BlobRef
 
 
 @dataclass
@@ -38,15 +38,15 @@
         description: Description.
         thumb: Thumb.
     """
 
     description: str
     title: str
     uri: str
-    thumb: Optional[BlobRef] = None
+    thumb: t.Optional[BlobRef] = None
 
     _type: str = 'app.bsky.embed.external#external'
 
 
 @dataclass
 class View(base.ModelBase):
 
@@ -72,10 +72,10 @@
         description: Description.
         thumb: Thumb.
     """
 
     description: str
     title: str
     uri: str
-    thumb: Optional[str] = None
+    thumb: t.Optional[str] = None
 
     _type: str = 'app.bsky.embed.external#viewExternal'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/images.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 from atproto.xrpc_client.models.blob_ref import BlobRef
 
 
 @dataclass
@@ -18,15 +18,15 @@
 
     """Definition model for :obj:`app.bsky.embed.images`.
 
     Attributes:
         images: Images.
     """
 
-    images: List['models.AppBskyEmbedImages.Image']
+    images: t.List['models.AppBskyEmbedImages.Image']
 
     _type: str = 'app.bsky.embed.images'
 
 
 @dataclass
 class Image(base.ModelBase):
 
@@ -48,15 +48,15 @@
 
     """Definition model for :obj:`app.bsky.embed.images`.
 
     Attributes:
         images: Images.
     """
 
-    images: List['models.AppBskyEmbedImages.ViewImage']
+    images: t.List['models.AppBskyEmbedImages.ViewImage']
 
     _type: str = 'app.bsky.embed.images#view'
 
 
 @dataclass
 class ViewImage(base.ModelBase):
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
@@ -31,19 +31,19 @@
 
     """Definition model for :obj:`app.bsky.embed.record`.
 
     Attributes:
         record: Record.
     """
 
-    record: Union[
+    record: t.Union[
         'models.AppBskyEmbedRecord.ViewRecord',
         'models.AppBskyEmbedRecord.ViewNotFound',
         'models.AppBskyEmbedRecord.ViewBlocked',
-        'Dict[str, Any]',
+        't.Dict[str, t.Any]',
     ]
 
     _type: str = 'app.bsky.embed.record#view'
 
 
 @dataclass
 class ViewRecord(base.ModelBase):
@@ -61,26 +61,26 @@
     """
 
     author: 'models.AppBskyActorDefs.ProfileViewBasic'
     cid: str
     indexedAt: str
     uri: str
     value: 'base.RecordModelBase'
-    embeds: Optional[
-        List[
-            Union[
+    embeds: t.Optional[
+        t.List[
+            t.Union[
                 'models.AppBskyEmbedImages.View',
                 'models.AppBskyEmbedExternal.View',
                 'models.AppBskyEmbedRecord.View',
                 'models.AppBskyEmbedRecordWithMedia.View',
-                'Dict[str, Any]',
+                't.Dict[str, t.Any]',
             ]
         ]
     ] = None
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
 
     _type: str = 'app.bsky.embed.record#viewRecord'
 
 
 @dataclass
 class ViewNotFound(base.ModelBase):
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
@@ -18,15 +18,15 @@
     """Definition model for :obj:`app.bsky.embed.recordWithMedia`.
 
     Attributes:
         record: Record.
         media: Media.
     """
 
-    media: Union['models.AppBskyEmbedImages.Main', 'models.AppBskyEmbedExternal.Main', 'Dict[str, Any]']
+    media: t.Union['models.AppBskyEmbedImages.Main', 'models.AppBskyEmbedExternal.Main', 't.Dict[str, t.Any]']
     record: 'models.AppBskyEmbedRecord.Main'
 
     _type: str = 'app.bsky.embed.recordWithMedia'
 
 
 @dataclass
 class View(base.ModelBase):
@@ -34,11 +34,11 @@
     """Definition model for :obj:`app.bsky.embed.recordWithMedia`.
 
     Attributes:
         record: Record.
         media: Media.
     """
 
-    media: Union['models.AppBskyEmbedImages.View', 'models.AppBskyEmbedExternal.View', 'Dict[str, Any]']
+    media: t.Union['models.AppBskyEmbedImages.View', 'models.AppBskyEmbedExternal.View', 't.Dict[str, t.Any]']
     record: 'models.AppBskyEmbedRecord.View'
 
     _type: str = 'app.bsky.embed.recordWithMedia#view'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/defs.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class PostView(base.ModelBase):
@@ -32,44 +32,44 @@
     """
 
     author: 'models.AppBskyActorDefs.ProfileViewBasic'
     cid: str
     indexedAt: str
     record: 'base.RecordModelBase'
     uri: str
-    embed: Optional[
-        Union[
+    embed: t.Optional[
+        t.Union[
             'models.AppBskyEmbedImages.View',
             'models.AppBskyEmbedExternal.View',
             'models.AppBskyEmbedRecord.View',
             'models.AppBskyEmbedRecordWithMedia.View',
-            'Dict[str, Any]',
+            't.Dict[str, t.Any]',
         ]
     ] = None
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
-    likeCount: Optional[int] = None
-    replyCount: Optional[int] = None
-    repostCount: Optional[int] = None
-    viewer: Optional['models.AppBskyFeedDefs.ViewerState'] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
+    likeCount: t.Optional[int] = None
+    replyCount: t.Optional[int] = None
+    repostCount: t.Optional[int] = None
+    viewer: t.Optional['models.AppBskyFeedDefs.ViewerState'] = None
 
     _type: str = 'app.bsky.feed.defs#postView'
 
 
 @dataclass
 class ViewerState(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.defs`.
 
     Attributes:
         repost: Repost.
         like: Like.
     """
 
-    like: Optional[str] = None
-    repost: Optional[str] = None
+    like: t.Optional[str] = None
+    repost: t.Optional[str] = None
 
     _type: str = 'app.bsky.feed.defs#viewerState'
 
 
 @dataclass
 class FeedViewPost(base.ModelBase):
 
@@ -78,16 +78,16 @@
     Attributes:
         post: Post.
         reply: Reply.
         reason: Reason.
     """
 
     post: 'models.AppBskyFeedDefs.PostView'
-    reason: Optional[Union['models.AppBskyFeedDefs.ReasonRepost', 'Dict[str, Any]']] = None
-    reply: Optional['models.AppBskyFeedDefs.ReplyRef'] = None
+    reason: t.Optional[t.Union['models.AppBskyFeedDefs.ReasonRepost', 't.Dict[str, t.Any]']] = None
+    reply: t.Optional['models.AppBskyFeedDefs.ReplyRef'] = None
 
     _type: str = 'app.bsky.feed.defs#feedViewPost'
 
 
 @dataclass
 class ReplyRef(base.ModelBase):
 
@@ -128,29 +128,29 @@
     Attributes:
         post: Post.
         parent: Parent.
         replies: Replies.
     """
 
     post: 'models.AppBskyFeedDefs.PostView'
-    parent: Optional[
-        Union[
+    parent: t.Optional[
+        t.Union[
             'models.AppBskyFeedDefs.ThreadViewPost',
             'models.AppBskyFeedDefs.NotFoundPost',
             'models.AppBskyFeedDefs.BlockedPost',
-            'Dict[str, Any]',
+            't.Dict[str, t.Any]',
         ]
     ] = None
-    replies: Optional[
-        List[
-            Union[
+    replies: t.Optional[
+        t.List[
+            t.Union[
                 'models.AppBskyFeedDefs.ThreadViewPost',
                 'models.AppBskyFeedDefs.NotFoundPost',
                 'models.AppBskyFeedDefs.BlockedPost',
-                'Dict[str, Any]',
+                't.Dict[str, t.Any]',
             ]
         ]
     ] = None
 
     _type: str = 'app.bsky.feed.defs#threadViewPost'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_lists.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getAuthorFeed`.
+    """Parameters model for :obj:`app.bsky.graph.getLists`.
 
     Attributes:
         actor: Actor.
         limit: Limit.
         cursor: Cursor.
     """
 
     actor: str
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getAuthorFeed`.
+    """Output data model for :obj:`app.bsky.graph.getLists`.
 
     Attributes:
         cursor: Cursor.
-        feed: Feed.
+        lists: Lists.
     """
 
-    feed: List['models.AppBskyFeedDefs.FeedViewPost']
-    cursor: Optional[str] = None
+    lists: t.List['models.AppBskyGraphDefs.ListView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_likes.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_likes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -21,35 +21,35 @@
         uri: Uri.
         cid: Cid.
         limit: Limit.
         cursor: Cursor.
     """
 
     uri: str
-    cid: Optional[str] = None
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cid: t.Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.feed.getLikes`.
 
     Attributes:
         uri: Uri.
         cid: Cid.
         cursor: Cursor.
         likes: Likes.
     """
 
-    likes: List['models.AppBskyFeedGetLikes.Like']
+    likes: t.List['models.AppBskyFeedGetLikes.Like']
     uri: str
-    cid: Optional[str] = None
-    cursor: Optional[str] = None
+    cid: t.Optional[str] = None
+    cursor: t.Optional[str] = None
 
 
 @dataclass
 class Like(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.feed.getLikes`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -19,25 +19,25 @@
 
     Attributes:
         uri: Uri.
         depth: Depth.
     """
 
     uri: str
-    depth: Optional[int] = None
+    depth: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.feed.getPostThread`.
 
     Attributes:
         thread: Thread.
     """
 
-    thread: Union[
+    thread: t.Union[
         'models.AppBskyFeedDefs.ThreadViewPost',
         'models.AppBskyFeedDefs.NotFoundPost',
         'models.AppBskyFeedDefs.BlockedPost',
-        'Dict[str, Any]',
+        't.Dict[str, t.Any]',
     ]
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_posts.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_head.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,35 +2,33 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import List
 
-from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.feed.getPosts`.
+    """Parameters model for :obj:`com.atproto.sync.getHead`.
 
     Attributes:
-        uris: Uris.
+        did: The DID of the repo.
     """
 
-    uris: List[str]
+    did: str
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.feed.getPosts`.
+    """Output data model for :obj:`com.atproto.sync.getHead`.
 
     Attributes:
-        posts: Posts.
+        root: Root.
     """
 
-    posts: List['models.AppBskyFeedDefs.PostView']
+    root: str
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -21,28 +21,28 @@
         uri: Uri.
         cid: Cid.
         limit: Limit.
         cursor: Cursor.
     """
 
     uri: str
-    cid: Optional[str] = None
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cid: t.Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.feed.getRepostedBy`.
 
     Attributes:
         uri: Uri.
         cid: Cid.
         cursor: Cursor.
         repostedBy: Reposted by.
     """
 
-    repostedBy: List['models.AppBskyActorDefs.ProfileView']
+    repostedBy: t.List['models.AppBskyActorDefs.ProfileView']
     uri: str
-    cid: Optional[str] = None
-    cursor: Optional[str] = None
+    cid: t.Optional[str] = None
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -19,24 +19,24 @@
 
     Attributes:
         algorithm: Algorithm.
         limit: Limit.
         cursor: Cursor.
     """
 
-    algorithm: Optional[str] = None
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    algorithm: t.Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.feed.getTimeline`.
 
     Attributes:
         cursor: Cursor.
         feed: Feed.
     """
 
-    feed: List['models.AppBskyFeedDefs.FeedViewPost']
-    cursor: Optional[str] = None
+    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/like.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/like.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/post.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/post.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ReplyRef(base.ModelBase):
@@ -74,21 +74,21 @@
         reply: Reply.
         embed: Embed.
         createdAt: Created at.
     """
 
     createdAt: str
     text: str
-    embed: Optional[
-        Union[
+    embed: t.Optional[
+        t.Union[
             'models.AppBskyEmbedImages.Main',
             'models.AppBskyEmbedExternal.Main',
             'models.AppBskyEmbedRecord.Main',
             'models.AppBskyEmbedRecordWithMedia.Main',
-            'Dict[str, Any]',
+            't.Dict[str, t.Any]',
         ]
     ] = None
-    entities: Optional[List['models.AppBskyFeedPost.Entity']] = None
-    facets: Optional[List['models.AppBskyRichtextFacet.Main']] = None
-    reply: Optional['models.AppBskyFeedPost.ReplyRef'] = None
+    entities: t.Optional[t.List['models.AppBskyFeedPost.Entity']] = None
+    facets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None
+    reply: t.Optional['models.AppBskyFeedPost.ReplyRef'] = None
 
     _type: str = 'app.bsky.feed.post'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/feed/repost.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/repost.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/block.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/block.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/defs.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
-from typing_extensions import Literal
+import typing_extensions as te
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ListViewBasic(base.ModelBase):
@@ -27,17 +27,17 @@
         viewer: Viewer.
         indexedAt: Indexed at.
     """
 
     name: str
     purpose: 'models.AppBskyGraphDefs.ListPurpose'
     uri: str
-    avatar: Optional[str] = None
-    indexedAt: Optional[str] = None
-    viewer: Optional['models.AppBskyGraphDefs.ListViewerState'] = None
+    avatar: t.Optional[str] = None
+    indexedAt: t.Optional[str] = None
+    viewer: t.Optional['models.AppBskyGraphDefs.ListViewerState'] = None
 
     _type: str = 'app.bsky.graph.defs#listViewBasic'
 
 
 @dataclass
 class ListView(base.ModelBase):
 
@@ -56,18 +56,18 @@
     """
 
     creator: 'models.AppBskyActorDefs.ProfileView'
     indexedAt: str
     name: str
     purpose: 'models.AppBskyGraphDefs.ListPurpose'
     uri: str
-    avatar: Optional[str] = None
-    description: Optional[str] = None
-    descriptionFacets: Optional[List['models.AppBskyRichtextFacet.Main']] = None
-    viewer: Optional['models.AppBskyGraphDefs.ListViewerState'] = None
+    avatar: t.Optional[str] = None
+    description: t.Optional[str] = None
+    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None
+    viewer: t.Optional['models.AppBskyGraphDefs.ListViewerState'] = None
 
     _type: str = 'app.bsky.graph.defs#listView'
 
 
 @dataclass
 class ListItemView(base.ModelBase):
 
@@ -78,24 +78,24 @@
     """
 
     subject: 'models.AppBskyActorDefs.ProfileView'
 
     _type: str = 'app.bsky.graph.defs#listItemView'
 
 
-ListPurpose = Literal['Modlist']
+ListPurpose = te.Literal['Modlist']
 
-Modlist: Literal['modlist'] = 'modlist'
+Modlist: te.Literal['modlist'] = 'modlist'
 
 
 @dataclass
 class ListViewerState(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.graph.defs`.
 
     Attributes:
         muted: Muted.
     """
 
-    muted: Optional[bool] = None
+    muted: t.Optional[bool] = None
 
     _type: str = 'app.bsky.graph.defs#listViewerState'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/follow.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/follow.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getBlocks`.
+    """Parameters model for :obj:`app.bsky.graph.getListMutes`.
 
     Attributes:
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getBlocks`.
+    """Output data model for :obj:`app.bsky.graph.getListMutes`.
 
     Attributes:
         cursor: Cursor.
-        blocks: Blocks.
+        lists: Lists.
     """
 
-    blocks: List['models.AppBskyActorDefs.ProfileView']
-    cursor: Optional[str] = None
+    lists: t.List['models.AppBskyGraphDefs.ListView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_followers.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_followers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -20,25 +20,25 @@
     Attributes:
         actor: Actor.
         limit: Limit.
         cursor: Cursor.
     """
 
     actor: str
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.graph.getFollowers`.
 
     Attributes:
         subject: Subject.
         cursor: Cursor.
         followers: Followers.
     """
 
-    followers: List['models.AppBskyActorDefs.ProfileView']
+    followers: t.List['models.AppBskyActorDefs.ProfileView']
     subject: 'models.AppBskyActorDefs.ProfileView'
-    cursor: Optional[str] = None
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_follows.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getFollows`.
+    """Parameters model for :obj:`app.bsky.unspecced.getPopular`.
 
     Attributes:
-        actor: Actor.
+        includeNsfw: Include nsfw.
         limit: Limit.
         cursor: Cursor.
     """
 
-    actor: str
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    includeNsfw: t.Optional[bool] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getFollows`.
+    """Output data model for :obj:`app.bsky.unspecced.getPopular`.
 
     Attributes:
-        subject: Subject.
         cursor: Cursor.
-        follows: Follows.
+        feed: Feed.
     """
 
-    follows: List['models.AppBskyActorDefs.ProfileView']
-    subject: 'models.AppBskyActorDefs.ProfileView'
-    cursor: Optional[str] = None
+    feed: t.List['models.AppBskyFeedDefs.FeedViewPost']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getList`.
+    """Parameters model for :obj:`app.bsky.actor.getSuggestions`.
 
     Attributes:
-        list: List.
         limit: Limit.
         cursor: Cursor.
     """
 
-    list: str
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getList`.
+    """Output data model for :obj:`app.bsky.actor.getSuggestions`.
 
     Attributes:
         cursor: Cursor.
-        list: List.
-        items: Items.
+        actors: Actors.
     """
 
-    items: List['models.AppBskyGraphDefs.ListItemView']
-    list: 'models.AppBskyGraphDefs.ListView'
-    cursor: Optional[str] = None
+    actors: t.List['models.AppBskyActorDefs.ProfileView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getListMutes`.
+    """Parameters model for :obj:`app.bsky.graph.getList`.
 
     Attributes:
+        list: List.
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    list: str
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getListMutes`.
+    """Output data model for :obj:`app.bsky.graph.getList`.
 
     Attributes:
         cursor: Cursor.
-        lists: Lists.
+        list: List.
+        items: Items.
     """
 
-    lists: List['models.AppBskyGraphDefs.ListView']
-    cursor: Optional[str] = None
+    items: t.List['models.AppBskyGraphDefs.ListItemView']
+    list: 'models.AppBskyGraphDefs.ListView'
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_lists.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.graph.getLists`.
+    """Parameters model for :obj:`app.bsky.graph.getBlocks`.
 
     Attributes:
-        actor: Actor.
         limit: Limit.
         cursor: Cursor.
     """
 
-    actor: str
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.graph.getLists`.
+    """Output data model for :obj:`app.bsky.graph.getBlocks`.
 
     Attributes:
         cursor: Cursor.
-        lists: Lists.
+        blocks: Blocks.
     """
 
-    lists: List['models.AppBskyGraphDefs.ListView']
-    cursor: Optional[str] = None
+    blocks: t.List['models.AppBskyActorDefs.ProfileView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -18,23 +18,23 @@
     """Parameters model for :obj:`app.bsky.graph.getMutes`.
 
     Attributes:
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.graph.getMutes`.
 
     Attributes:
         cursor: Cursor.
         mutes: Mutes.
     """
 
-    mutes: List['models.AppBskyActorDefs.ProfileView']
-    cursor: Optional[str] = None
+    mutes: t.List['models.AppBskyActorDefs.ProfileView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/list.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 from atproto.xrpc_client.models.blob_ref import BlobRef
 
 
 @dataclass
@@ -26,12 +26,12 @@
         avatar: Avatar.
         createdAt: Created at.
     """
 
     createdAt: str
     name: str
     purpose: 'models.AppBskyGraphDefs.ListPurpose'
-    avatar: Optional[BlobRef] = None
-    description: Optional[str] = None
-    descriptionFacets: Optional[List['models.AppBskyRichtextFacet.Main']] = None
+    avatar: t.Optional[BlobRef] = None
+    description: t.Optional[str] = None
+    descriptionFacets: t.Optional[t.List['models.AppBskyRichtextFacet.Main']] = None
 
     _type: str = 'app.bsky.graph.list'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/listitem.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/listitem.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
     """Parameters model for :obj:`app.bsky.notification.getUnreadCount`.
 
     Attributes:
         seenAt: Seen at.
     """
 
-    seenAt: Optional[str] = None
+    seenAt: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.notification.getUnreadCount`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -19,31 +19,31 @@
 
     Attributes:
         limit: Limit.
         cursor: Cursor.
         seenAt: Seen at.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
-    seenAt: Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
+    seenAt: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`app.bsky.notification.listNotifications`.
 
     Attributes:
         cursor: Cursor.
         notifications: Notifications.
     """
 
-    notifications: List['models.AppBskyNotificationListNotifications.Notification']
-    cursor: Optional[str] = None
+    notifications: t.List['models.AppBskyNotificationListNotifications.Notification']
+    cursor: t.Optional[str] = None
 
 
 @dataclass
 class Notification(base.ModelBase):
 
     """Definition model for :obj:`app.bsky.notification.listNotifications`.
 
@@ -62,11 +62,11 @@
     author: 'models.AppBskyActorDefs.ProfileView'
     cid: str
     indexedAt: str
     isRead: bool
     reason: str
     record: 'base.RecordModelBase'
     uri: str
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
-    reasonSubject: Optional[str] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
+    reasonSubject: t.Optional[str] = None
 
     _type: str = 'app.bsky.notification.listNotifications#notification'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/notification/update_seen.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/notification/update_seen.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/richtext/facet.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/richtext/facet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, List, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Main(base.ModelBase):
@@ -18,15 +18,17 @@
     """Definition model for :obj:`app.bsky.richtext.facet`.
 
     Attributes:
         index: Index.
         features: Features.
     """
 
-    features: List[Union['models.AppBskyRichtextFacet.Mention', 'models.AppBskyRichtextFacet.Link', 'Dict[str, Any]']]
+    features: t.List[
+        t.Union['models.AppBskyRichtextFacet.Mention', 'models.AppBskyRichtextFacet.Link', 't.Dict[str, t.Any]']
+    ]
     index: 'models.AppBskyRichtextFacet.ByteSlice'
 
     _type: str = 'app.bsky.richtext.facet'
 
 
 @dataclass
 class Mention(base.ModelBase):
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_repos.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`app.bsky.unspecced.getPopular`.
+    """Parameters model for :obj:`com.atproto.sync.listRepos`.
 
     Attributes:
-        includeNsfw: Include nsfw.
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    includeNsfw: Optional[bool] = None
-    limit: Optional[int] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`app.bsky.unspecced.getPopular`.
+    """Output data model for :obj:`com.atproto.sync.listRepos`.
 
     Attributes:
         cursor: Cursor.
-        feed: Feed.
+        repos: Repos.
     """
 
-    feed: List['models.AppBskyFeedDefs.FeedViewPost']
-    cursor: Optional[str] = None
+    repos: t.List['models.ComAtprotoSyncListRepos.Repo']
+    cursor: t.Optional[str] = None
+
+
+@dataclass
+class Repo(base.ModelBase):
+
+    """Definition model for :obj:`com.atproto.sync.listRepos`.
+
+    Attributes:
+        did: Did.
+        head: Head.
+    """
+
+    did: str
+    head: str
+
+    _type: str = 'com.atproto.sync.listRepos#repo'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/base.py` & `atproto-0.0.7/atproto/xrpc_client/models/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/blob_ref.py` & `atproto-0.0.7/atproto/xrpc_client/models/blob_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/defs.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
 
-from typing_extensions import Literal
+import typing_extensions as te
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class ActionView(base.ModelBase):
@@ -34,20 +34,20 @@
     """
 
     action: 'models.ComAtprotoAdminDefs.ActionType'
     createdAt: str
     createdBy: str
     id: int
     reason: str
-    resolvedReportIds: List[int]
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
-    subjectBlobCids: List[str]
-    createLabelVals: Optional[List[str]] = None
-    negateLabelVals: Optional[List[str]] = None
-    reversal: Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
+    resolvedReportIds: t.List[int]
+    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
+    subjectBlobCids: t.List[str]
+    createLabelVals: t.Optional[t.List[str]] = None
+    negateLabelVals: t.Optional[t.List[str]] = None
+    reversal: t.Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
 
     _type: str = 'com.atproto.admin.defs#actionView'
 
 
 @dataclass
 class ActionViewDetail(base.ModelBase):
 
@@ -68,26 +68,26 @@
     """
 
     action: 'models.ComAtprotoAdminDefs.ActionType'
     createdAt: str
     createdBy: str
     id: int
     reason: str
-    resolvedReports: List['models.ComAtprotoAdminDefs.ReportView']
-    subject: Union[
+    resolvedReports: t.List['models.ComAtprotoAdminDefs.ReportView']
+    subject: t.Union[
         'models.ComAtprotoAdminDefs.RepoView',
         'models.ComAtprotoAdminDefs.RepoViewNotFound',
         'models.ComAtprotoAdminDefs.RecordView',
         'models.ComAtprotoAdminDefs.RecordViewNotFound',
-        'Dict[str, Any]',
+        't.Dict[str, t.Any]',
     ]
-    subjectBlobs: List['models.ComAtprotoAdminDefs.BlobView']
-    createLabelVals: Optional[List[str]] = None
-    negateLabelVals: Optional[List[str]] = None
-    reversal: Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
+    subjectBlobs: t.List['models.ComAtprotoAdminDefs.BlobView']
+    createLabelVals: t.Optional[t.List[str]] = None
+    negateLabelVals: t.Optional[t.List[str]] = None
+    reversal: t.Optional['models.ComAtprotoAdminDefs.ActionReversal'] = None
 
     _type: str = 'com.atproto.admin.defs#actionViewDetail'
 
 
 @dataclass
 class ActionViewCurrent(base.ModelBase):
 
@@ -118,23 +118,23 @@
     createdAt: str
     createdBy: str
     reason: str
 
     _type: str = 'com.atproto.admin.defs#actionReversal'
 
 
-ActionType = Literal['Takedown', 'Flag', 'Acknowledge', 'Escalate']
+ActionType = te.Literal['Takedown', 'Flag', 'Acknowledge', 'Escalate']
 
-Takedown: Literal['takedown'] = 'takedown'
+Takedown: te.Literal['takedown'] = 'takedown'
 
-Flag: Literal['flag'] = 'flag'
+Flag: te.Literal['flag'] = 'flag'
 
-Acknowledge: Literal['acknowledge'] = 'acknowledge'
+Acknowledge: te.Literal['acknowledge'] = 'acknowledge'
 
-Escalate: Literal['escalate'] = 'escalate'
+Escalate: te.Literal['escalate'] = 'escalate'
 
 
 @dataclass
 class ReportView(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
@@ -148,17 +148,17 @@
         resolvedByActionIds: Resolved by action ids.
     """
 
     createdAt: str
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
-    resolvedByActionIds: List[int]
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
-    reason: Optional[str] = None
+    resolvedByActionIds: t.List[int]
+    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
+    reason: t.Optional[str] = None
 
     _type: str = 'com.atproto.admin.defs#reportView'
 
 
 @dataclass
 class ReportViewDetail(base.ModelBase):
 
@@ -174,23 +174,23 @@
         resolvedByActions: Resolved by actions.
     """
 
     createdAt: str
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
-    resolvedByActions: List['models.ComAtprotoAdminDefs.ActionView']
-    subject: Union[
+    resolvedByActions: t.List['models.ComAtprotoAdminDefs.ActionView']
+    subject: t.Union[
         'models.ComAtprotoAdminDefs.RepoView',
         'models.ComAtprotoAdminDefs.RepoViewNotFound',
         'models.ComAtprotoAdminDefs.RecordView',
         'models.ComAtprotoAdminDefs.RecordViewNotFound',
-        'Dict[str, Any]',
+        't.Dict[str, t.Any]',
     ]
-    reason: Optional[str] = None
+    reason: t.Optional[str] = None
 
     _type: str = 'com.atproto.admin.defs#reportViewDetail'
 
 
 @dataclass
 class RepoView(base.ModelBase):
 
@@ -207,18 +207,18 @@
         invitesDisabled: Invites disabled.
     """
 
     did: str
     handle: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.Moderation'
-    relatedRecords: List['base.RecordModelBase']
-    email: Optional[str] = None
-    invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
-    invitesDisabled: Optional[bool] = None
+    relatedRecords: t.List['base.RecordModelBase']
+    email: t.Optional[str] = None
+    invitedBy: t.Optional['models.ComAtprotoServerDefs.InviteCode'] = None
+    invitesDisabled: t.Optional[bool] = None
 
     _type: str = 'com.atproto.admin.defs#repoView'
 
 
 @dataclass
 class RepoViewDetail(base.ModelBase):
 
@@ -237,20 +237,20 @@
         invitesDisabled: Invites disabled.
     """
 
     did: str
     handle: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.ModerationDetail'
-    relatedRecords: List['base.RecordModelBase']
-    email: Optional[str] = None
-    invitedBy: Optional['models.ComAtprotoServerDefs.InviteCode'] = None
-    invites: Optional[List['models.ComAtprotoServerDefs.InviteCode']] = None
-    invitesDisabled: Optional[bool] = None
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
+    relatedRecords: t.List['base.RecordModelBase']
+    email: t.Optional[str] = None
+    invitedBy: t.Optional['models.ComAtprotoServerDefs.InviteCode'] = None
+    invites: t.Optional[t.List['models.ComAtprotoServerDefs.InviteCode']] = None
+    invitesDisabled: t.Optional[bool] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
 
     _type: str = 'com.atproto.admin.defs#repoViewDetail'
 
 
 @dataclass
 class RepoViewNotFound(base.ModelBase):
 
@@ -290,15 +290,15 @@
         value: Value.
         blobCids: Blob cids.
         indexedAt: Indexed at.
         moderation: Moderation.
         repo: Repo.
     """
 
-    blobCids: List[str]
+    blobCids: t.List[str]
     cid: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.Moderation'
     repo: 'models.ComAtprotoAdminDefs.RepoView'
     uri: str
     value: 'base.RecordModelBase'
 
@@ -317,22 +317,22 @@
         blobs: Blobs.
         labels: Labels.
         indexedAt: Indexed at.
         moderation: Moderation.
         repo: Repo.
     """
 
-    blobs: List['models.ComAtprotoAdminDefs.BlobView']
+    blobs: t.List['models.ComAtprotoAdminDefs.BlobView']
     cid: str
     indexedAt: str
     moderation: 'models.ComAtprotoAdminDefs.ModerationDetail'
     repo: 'models.ComAtprotoAdminDefs.RepoView'
     uri: str
     value: 'base.RecordModelBase'
-    labels: Optional[List['models.ComAtprotoLabelDefs.Label']] = None
+    labels: t.Optional[t.List['models.ComAtprotoLabelDefs.Label']] = None
 
     _type: str = 'com.atproto.admin.defs#recordViewDetail'
 
 
 @dataclass
 class RecordViewNotFound(base.ModelBase):
 
@@ -352,15 +352,15 @@
 
     """Definition model for :obj:`com.atproto.admin.defs`.
 
     Attributes:
         currentAction: Current action.
     """
 
-    currentAction: Optional['models.ComAtprotoAdminDefs.ActionViewCurrent'] = None
+    currentAction: t.Optional['models.ComAtprotoAdminDefs.ActionViewCurrent'] = None
 
     _type: str = 'com.atproto.admin.defs#moderation'
 
 
 @dataclass
 class ModerationDetail(base.ModelBase):
 
@@ -368,17 +368,17 @@
 
     Attributes:
         currentAction: Current action.
         actions: Actions.
         reports: Reports.
     """
 
-    actions: List['models.ComAtprotoAdminDefs.ActionView']
-    reports: List['models.ComAtprotoAdminDefs.ReportView']
-    currentAction: Optional['models.ComAtprotoAdminDefs.ActionViewCurrent'] = None
+    actions: t.List['models.ComAtprotoAdminDefs.ActionView']
+    reports: t.List['models.ComAtprotoAdminDefs.ReportView']
+    currentAction: t.Optional['models.ComAtprotoAdminDefs.ActionViewCurrent'] = None
 
     _type: str = 'com.atproto.admin.defs#moderationDetail'
 
 
 @dataclass
 class BlobView(base.ModelBase):
 
@@ -393,18 +393,20 @@
         moderation: Moderation.
     """
 
     cid: str
     createdAt: str
     mimeType: str
     size: int
-    details: Optional[
-        Union['models.ComAtprotoAdminDefs.ImageDetails', 'models.ComAtprotoAdminDefs.VideoDetails', 'Dict[str, Any]']
+    details: t.Optional[
+        t.Union[
+            'models.ComAtprotoAdminDefs.ImageDetails', 'models.ComAtprotoAdminDefs.VideoDetails', 't.Dict[str, t.Any]'
+        ]
     ] = None
-    moderation: Optional['models.ComAtprotoAdminDefs.Moderation'] = None
+    moderation: t.Optional['models.ComAtprotoAdminDefs.Moderation'] = None
 
     _type: str = 'com.atproto.admin.defs#blobView'
 
 
 @dataclass
 class ImageDetails(base.ModelBase):
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
     """Input data model for :obj:`com.atproto.admin.disableInviteCodes`.
 
     Attributes:
         codes: Codes.
         accounts: Accounts.
     """
 
-    accounts: Optional[List[str]] = None
-    codes: Optional[List[str]] = None
+    accounts: t.Optional[t.List[str]] = None
+    codes: t.Optional[t.List[str]] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -19,24 +19,24 @@
 
     Attributes:
         sort: Sort.
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
-    sort: Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
+    sort: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.admin.getInviteCodes`.
 
     Attributes:
         cursor: Cursor.
         codes: Codes.
     """
 
-    codes: List['models.ComAtprotoServerDefs.InviteCode']
-    cursor: Optional[str] = None
+    codes: t.List['models.ComAtprotoServerDefs.InviteCode']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Type
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getModerationAction`.
+    """Parameters model for :obj:`com.atproto.admin.getRepo`.
 
     Attributes:
-        id: Id.
+        did: Did.
     """
 
-    id: int
+    did: str
 
 
-#: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionViewDetail` model.
-ResponseRef: Type[models.ComAtprotoAdminDefs.ActionViewDetail] = models.ComAtprotoAdminDefs.ActionViewDetail
+#: Response reference to :obj:`models.ComAtprotoAdminDefs.RepoViewDetail` model.
+ResponseRef: t.Type[models.ComAtprotoAdminDefs.RepoViewDetail] = models.ComAtprotoAdminDefs.RepoViewDetail
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -19,24 +19,24 @@
 
     Attributes:
         subject: Subject.
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
-    subject: Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
+    subject: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.admin.getModerationActions`.
 
     Attributes:
         cursor: Cursor.
         actions: Actions.
     """
 
-    actions: List['models.ComAtprotoAdminDefs.ActionView']
-    cursor: Optional[str] = None
+    actions: t.List['models.ComAtprotoAdminDefs.ActionView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Type
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -21,8 +21,8 @@
         id: Id.
     """
 
     id: int
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ReportViewDetail` model.
-ResponseRef: Type[models.ComAtprotoAdminDefs.ReportViewDetail] = models.ComAtprotoAdminDefs.ReportViewDetail
+ResponseRef: t.Type[models.ComAtprotoAdminDefs.ReportViewDetail] = models.ComAtprotoAdminDefs.ReportViewDetail
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -21,26 +21,26 @@
         subject: Subject.
         resolved: Resolved.
         actionType: Action type.
         limit: Limit.
         cursor: Cursor.
     """
 
-    actionType: Optional[str] = None
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
-    resolved: Optional[bool] = None
-    subject: Optional[str] = None
+    actionType: t.Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
+    resolved: t.Optional[bool] = None
+    subject: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.admin.getModerationReports`.
 
     Attributes:
         cursor: Cursor.
         reports: Reports.
     """
 
-    reports: List['models.ComAtprotoAdminDefs.ReportView']
-    cursor: Optional[str] = None
+    reports: t.List['models.ComAtprotoAdminDefs.ReportView']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/get_record.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional, Type
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.getRecord`.
+    """Parameters model for :obj:`com.atproto.admin.getModerationAction`.
 
     Attributes:
-        uri: Uri.
-        cid: Cid.
+        id: Id.
     """
 
-    uri: str
-    cid: Optional[str] = None
+    id: int
 
 
-#: Response reference to :obj:`models.ComAtprotoAdminDefs.RecordViewDetail` model.
-ResponseRef: Type[models.ComAtprotoAdminDefs.RecordViewDetail] = models.ComAtprotoAdminDefs.RecordViewDetail
+#: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionViewDetail` model.
+ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionViewDetail] = models.ComAtprotoAdminDefs.ActionViewDetail
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Type
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -21,12 +21,12 @@
         actionId: Action id.
         reportIds: Report ids.
         createdBy: Created by.
     """
 
     actionId: int
     createdBy: str
-    reportIds: List[int]
+    reportIds: t.List[int]
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
-ResponseRef: Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
+ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Type
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -25,8 +25,8 @@
 
     createdBy: str
     id: int
     reason: str
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
-ResponseRef: Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
+ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/search_repos.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/get_record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
-from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.admin.searchRepos`.
+    """Parameters model for :obj:`com.atproto.repo.getRecord`.
 
     Attributes:
-        term: Term.
-        invitedBy: Invited by.
-        limit: Limit.
-        cursor: Cursor.
+        repo: The handle or DID of the repo.
+        collection: The NSID of the record collection.
+        rkey: The key of the record.
+        cid: The CID of the version of the record. If not specified, then return the most recent version.
     """
 
-    cursor: Optional[str] = None
-    invitedBy: Optional[str] = None
-    limit: Optional[int] = None
-    term: Optional[str] = None
+    collection: str
+    repo: str
+    rkey: str
+    cid: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.admin.searchRepos`.
+    """Output data model for :obj:`com.atproto.repo.getRecord`.
 
     Attributes:
-        cursor: Cursor.
-        repos: Repos.
+        uri: Uri.
+        cid: Cid.
+        value: Value.
     """
 
-    repos: List['models.ComAtprotoAdminDefs.RepoView']
-    cursor: Optional[str] = None
+    uri: str
+    value: 'base.RecordModelBase'
+    cid: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Type, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -26,15 +26,15 @@
         reason: Reason.
         createdBy: Created by.
     """
 
     action: str
     createdBy: str
     reason: str
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
-    createLabelVals: Optional[List[str]] = None
-    negateLabelVals: Optional[List[str]] = None
-    subjectBlobCids: Optional[List[str]] = None
+    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
+    createLabelVals: t.Optional[t.List[str]] = None
+    negateLabelVals: t.Optional[t.List[str]] = None
+    subjectBlobCids: t.Optional[t.List[str]] = None
 
 
 #: Response reference to :obj:`models.ComAtprotoAdminDefs.ActionView` model.
-ResponseRef: Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
+ResponseRef: t.Type[models.ComAtprotoAdminDefs.ActionView] = models.ComAtprotoAdminDefs.ActionView
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
     """Parameters model for :obj:`com.atproto.identity.resolveHandle`.
 
     Attributes:
         handle: The handle to resolve. If not supplied, will resolve the host's own handle.
     """
 
-    handle: Optional[str] = None
+    handle: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.identity.resolveHandle`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/identity/update_handle.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/identity/update_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/defs.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Label(base.ModelBase):
 
@@ -25,11 +25,11 @@
         cts: timestamp when this label was created.
     """
 
     cts: str
     src: str
     uri: str
     val: str
-    cid: Optional[str] = None
-    neg: Optional[bool] = None
+    cid: t.Optional[str] = None
+    neg: t.Optional[bool] = None
 
     _type: str = 'com.atproto.label.defs#label'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/query_labels.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/query_labels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -20,25 +20,25 @@
     Attributes:
         uriPatterns: List of AT URI patterns to match (boolean 'OR'). Each may be a prefix (ending with '*'; will match inclusive of the string leading to '*'), or a full URI.
         sources: Optional list of label sources (DIDs) to filter on.
         limit: Limit.
         cursor: Cursor.
     """
 
-    uriPatterns: List[str]
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
-    sources: Optional[List[str]] = None
+    uriPatterns: t.List[str]
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
+    sources: t.Optional[t.List[str]] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.label.queryLabels`.
 
     Attributes:
         cursor: Cursor.
         labels: Labels.
     """
 
-    labels: List['models.ComAtprotoLabelDefs.Label']
-    cursor: Optional[str] = None
+    labels: t.List['models.ComAtprotoLabelDefs.Label']
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Labels(base.ModelBase):
@@ -18,15 +18,15 @@
     """Definition model for :obj:`com.atproto.label.subscribeLabels`.
 
     Attributes:
         seq: Seq.
         labels: Labels.
     """
 
-    labels: List['models.ComAtprotoLabelDefs.Label']
+    labels: t.List['models.ComAtprotoLabelDefs.Label']
     seq: int
 
     _type: str = 'com.atproto.label.subscribeLabels#labels'
 
 
 @dataclass
 class Info(base.ModelBase):
@@ -35,10 +35,10 @@
 
     Attributes:
         name: Name.
         message: Message.
     """
 
     name: str
-    message: Optional[str] = None
+    message: t.Optional[str] = None
 
     _type: str = 'com.atproto.label.subscribeLabels#info'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/create_report.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/create_report.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -20,16 +20,16 @@
     Attributes:
         reasonType: Reason type.
         reason: Reason.
         subject: Subject.
     """
 
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
-    reason: Optional[str] = None
+    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
+    reason: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.moderation.createReport`.
 
@@ -42,9 +42,9 @@
         createdAt: Created at.
     """
 
     createdAt: str
     id: int
     reasonType: 'models.ComAtprotoModerationDefs.ReasonType'
     reportedBy: str
-    subject: Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 'Dict[str, Any]']
-    reason: Optional[str] = None
+    subject: t.Union['models.ComAtprotoAdminDefs.RepoRef', 'models.ComAtprotoRepoStrongRef.Main', 't.Dict[str, t.Any]']
+    reason: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/moderation/defs.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/moderation/defs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
-from typing_extensions import Literal
+import typing_extensions as te
 
-ReasonType = Literal['ReasonSpam', 'ReasonViolation', 'ReasonMisleading', 'ReasonSexual', 'ReasonRude', 'ReasonOther']
+ReasonType = te.Literal[
+    'ReasonSpam', 'ReasonViolation', 'ReasonMisleading', 'ReasonSexual', 'ReasonRude', 'ReasonOther'
+]
 
-ReasonSpam: Literal['reasonSpam'] = 'reasonSpam'
+ReasonSpam: te.Literal['reasonSpam'] = 'reasonSpam'
 
-ReasonViolation: Literal['reasonViolation'] = 'reasonViolation'
+ReasonViolation: te.Literal['reasonViolation'] = 'reasonViolation'
 
-ReasonMisleading: Literal['reasonMisleading'] = 'reasonMisleading'
+ReasonMisleading: te.Literal['reasonMisleading'] = 'reasonMisleading'
 
-ReasonSexual: Literal['reasonSexual'] = 'reasonSexual'
+ReasonSexual: te.Literal['reasonSexual'] = 'reasonSexual'
 
-ReasonRude: Literal['reasonRude'] = 'reasonRude'
+ReasonRude: te.Literal['reasonRude'] = 'reasonRude'
 
-ReasonOther: Literal['reasonOther'] = 'reasonOther'
+ReasonOther: te.Literal['reasonOther'] = 'reasonOther'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -21,24 +21,24 @@
         repo: The handle or DID of the repo.
         validate: Validate the records?
         writes: Writes.
         swapCommit: Swap commit.
     """
 
     repo: str
-    writes: List[
-        Union[
+    writes: t.List[
+        t.Union[
             'models.ComAtprotoRepoApplyWrites.Create',
             'models.ComAtprotoRepoApplyWrites.Update',
             'models.ComAtprotoRepoApplyWrites.Delete',
-            'Dict[str, Any]',
+            't.Dict[str, t.Any]',
         ]
     ]
-    swapCommit: Optional[str] = None
-    validate: Optional[bool] = None
+    swapCommit: t.Optional[str] = None
+    validate: t.Optional[bool] = None
 
 
 @dataclass
 class Create(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.repo.applyWrites`. Create a new record.
 
@@ -46,15 +46,15 @@
         collection: Collection.
         rkey: Rkey.
         value: Value.
     """
 
     collection: str
     value: 'base.RecordModelBase'
-    rkey: Optional[str] = None
+    rkey: t.Optional[str] = None
 
     _type: str = 'com.atproto.repo.applyWrites#create'
 
 
 @dataclass
 class Update(base.ModelBase):
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/create_record.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/create_record.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
@@ -24,17 +24,17 @@
         record: The record to create.
         swapCommit: Compare and swap with the previous commit by cid.
     """
 
     collection: str
     record: 'base.RecordModelBase'
     repo: str
-    rkey: Optional[str] = None
-    swapCommit: Optional[str] = None
-    validate: Optional[bool] = None
+    rkey: t.Optional[str] = None
+    swapCommit: t.Optional[str] = None
+    validate: t.Optional[bool] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.repo.createRecord`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/delete_record.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.deleteRecord`.
+    """Input data model for :obj:`com.atproto.repo.rebaseRepo`.
 
     Attributes:
         repo: The handle or DID of the repo.
-        collection: The NSID of the record collection.
-        rkey: The key of the record.
-        swapRecord: Compare and swap with the previous record by cid.
         swapCommit: Compare and swap with the previous commit by cid.
     """
 
-    collection: str
     repo: str
-    rkey: str
-    swapCommit: Optional[str] = None
-    swapRecord: Optional[str] = None
+    swapCommit: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
@@ -32,12 +32,12 @@
         handle: Handle.
         did: Did.
         didDoc: Did doc.
         collections: Collections.
         handleIsCorrect: Handle is correct.
     """
 
-    collections: List[str]
+    collections: t.List[str]
     did: str
     didDoc: 'base.RecordModelBase'
     handle: str
     handleIsCorrect: bool
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/get_record.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/describe_server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Params(base.ParamsModelBase):
+class Response(base.ResponseModelBase):
 
-    """Parameters model for :obj:`com.atproto.repo.getRecord`.
+    """Output data model for :obj:`com.atproto.server.describeServer`.
 
     Attributes:
-        repo: The handle or DID of the repo.
-        collection: The NSID of the record collection.
-        rkey: The key of the record.
-        cid: The CID of the version of the record. If not specified, then return the most recent version.
+        inviteCodeRequired: Invite code required.
+        availableUserDomains: Available user domains.
+        links: Links.
     """
 
-    collection: str
-    repo: str
-    rkey: str
-    cid: Optional[str] = None
+    availableUserDomains: t.List[str]
+    inviteCodeRequired: t.Optional[bool] = None
+    links: t.Optional['models.ComAtprotoServerDescribeServer.Links'] = None
 
 
 @dataclass
-class Response(base.ResponseModelBase):
+class Links(base.ModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.getRecord`.
+    """Definition model for :obj:`com.atproto.server.describeServer`.
 
     Attributes:
-        uri: Uri.
-        cid: Cid.
-        value: Value.
+        privacyPolicy: Privacy policy.
+        termsOfService: Terms of service.
     """
 
-    uri: str
-    value: 'base.RecordModelBase'
-    cid: Optional[str] = None
+    privacyPolicy: t.Optional[str] = None
+    termsOfService: t.Optional[str] = None
+
+    _type: str = 'com.atproto.server.describeServer#links'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/list_records.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/list_records.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -25,33 +25,33 @@
         rkeyStart: DEPRECATED: The lowest sort-ordered rkey to start from (exclusive).
         rkeyEnd: DEPRECATED: The highest sort-ordered rkey to stop at (exclusive).
         reverse: Reverse the order of the returned records?
     """
 
     collection: str
     repo: str
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
-    reverse: Optional[bool] = None
-    rkeyEnd: Optional[str] = None
-    rkeyStart: Optional[str] = None
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
+    reverse: t.Optional[bool] = None
+    rkeyEnd: t.Optional[str] = None
+    rkeyStart: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.repo.listRecords`.
 
     Attributes:
         cursor: Cursor.
         records: Records.
     """
 
-    records: List['models.ComAtprotoRepoListRecords.Record']
-    cursor: Optional[str] = None
+    records: t.List['models.ComAtprotoRepoListRecords.Record']
+    cursor: t.Optional[str] = None
 
 
 @dataclass
 class Record(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.repo.listRecords`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/put_record.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/put_record.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
@@ -26,17 +26,17 @@
         swapCommit: Compare and swap with the previous commit by cid.
     """
 
     collection: str
     record: 'base.RecordModelBase'
     repo: str
     rkey: str
-    swapCommit: Optional[str] = None
-    swapRecord: Optional[str] = None
-    validate: Optional[bool] = None
+    swapCommit: t.Optional[str] = None
+    swapRecord: t.Optional[str] = None
+    validate: t.Optional[bool] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.repo.putRecord`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Params(base.ParamsModelBase):
 
-    """Input data model for :obj:`com.atproto.repo.rebaseRepo`.
+    """Parameters model for :obj:`com.atproto.sync.getCommitPath`.
 
     Attributes:
-        repo: The handle or DID of the repo.
-        swapCommit: Compare and swap with the previous commit by cid.
+        did: The DID of the repo.
+        latest: The most recent commit.
+        earliest: The earliest commit to start from.
     """
 
-    repo: str
-    swapCommit: Optional[str] = None
+    did: str
+    earliest: t.Optional[str] = None
+    latest: t.Optional[str] = None
+
+
+@dataclass
+class Response(base.ResponseModelBase):
+
+    """Output data model for :obj:`com.atproto.sync.getCommitPath`.
+
+    Attributes:
+        commits: Commits.
+    """
+
+    commits: t.List[str]
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,21 @@
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
 from dataclasses import dataclass
-from typing import Type, Union
 
 from atproto.xrpc_client.models import base
-from atproto.xrpc_client.models.blob_ref import BlobRef
-
-#: Data raw data type.
-Data: Union[Type[str], Type[bytes]] = bytes
 
 
 @dataclass
-class Response(base.ResponseModelBase):
+class Data(base.DataModelBase):
 
-    """Output data model for :obj:`com.atproto.repo.uploadBlob`.
+    """Input data model for :obj:`com.atproto.server.requestPasswordReset`.
 
     Attributes:
-        blob: Blob.
+        email: Email.
     """
 
-    blob: BlobRef
+    email: str
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_account.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
@@ -24,17 +24,17 @@
         password: Password.
         recoveryKey: Recovery key.
     """
 
     email: str
     handle: str
     password: str
-    did: Optional[str] = None
-    inviteCode: Optional[str] = None
-    recoveryKey: Optional[str] = None
+    did: t.Optional[str] = None
+    inviteCode: t.Optional[str] = None
+    recoveryKey: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.server.createAccount`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_app_password.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_app_password.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Type
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
@@ -38,8 +38,8 @@
     name: str
     password: str
 
     _type: str = 'com.atproto.server.createAppPassword#appPassword'
 
 
 #: Response reference to :obj:`AppPassword` model.
-ResponseRef: Type[AppPassword] = AppPassword
+ResponseRef: t.Type[AppPassword] = AppPassword
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
@@ -18,15 +18,15 @@
 
     Attributes:
         useCount: Use count.
         forAccount: For account.
     """
 
     useCount: int
-    forAccount: Optional[str] = None
+    forAccount: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.server.createInviteCode`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
@@ -21,36 +21,36 @@
         codeCount: Code count.
         useCount: Use count.
         forAccounts: For accounts.
     """
 
     codeCount: int
     useCount: int
-    forAccounts: Optional[List[str]] = None
+    forAccounts: t.Optional[t.List[str]] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.server.createInviteCodes`.
 
     Attributes:
         codes: Codes.
     """
 
-    codes: List['models.ComAtprotoServerCreateInviteCodes.AccountCodes']
+    codes: t.List['models.ComAtprotoServerCreateInviteCodes.AccountCodes']
 
 
 @dataclass
 class AccountCodes(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.server.createInviteCodes`.
 
     Attributes:
         account: Account.
         codes: Codes.
     """
 
     account: str
-    codes: List[str]
+    codes: t.List[str]
 
     _type: str = 'com.atproto.server.createInviteCodes#accountCodes'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/create_session.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/create_session.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
@@ -38,8 +38,8 @@
         email: Email.
     """
 
     accessJwt: str
     did: str
     handle: str
     refreshJwt: str
-    email: Optional[str] = None
+    email: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/defs.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class InviteCode(base.ModelBase):
@@ -29,15 +29,15 @@
 
     available: int
     code: str
     createdAt: str
     createdBy: str
     disabled: bool
     forAccount: str
-    uses: List['models.ComAtprotoServerDefs.InviteCodeUse']
+    uses: t.List['models.ComAtprotoServerDefs.InviteCodeUse']
 
     _type: str = 'com.atproto.server.defs#inviteCode'
 
 
 @dataclass
 class InviteCodeUse(base.ModelBase):
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/delete_account.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/delete_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
@@ -18,21 +18,21 @@
     """Parameters model for :obj:`com.atproto.server.getAccountInviteCodes`.
 
     Attributes:
         includeUsed: Include used.
         createAvailable: Create available.
     """
 
-    createAvailable: Optional[bool] = None
-    includeUsed: Optional[bool] = None
+    createAvailable: t.Optional[bool] = None
+    includeUsed: t.Optional[bool] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.server.getAccountInviteCodes`.
 
     Attributes:
         codes: Codes.
     """
 
-    codes: List['models.ComAtprotoServerDefs.InviteCode']
+    codes: t.List['models.ComAtprotoServerDefs.InviteCode']
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/get_session.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/get_session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
@@ -20,8 +20,8 @@
         handle: Handle.
         did: Did.
         email: Email.
     """
 
     did: str
     handle: str
-    email: Optional[str] = None
+    email: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.server.listAppPasswords`.
 
     Attributes:
         passwords: Passwords.
     """
 
-    passwords: List['models.ComAtprotoServerListAppPasswords.AppPassword']
+    passwords: t.List['models.ComAtprotoServerListAppPasswords.AppPassword']
 
 
 @dataclass
 class AppPassword(base.ModelBase):
 
     """Definition model for :obj:`com.atproto.server.listAppPasswords`.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/refresh_session.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/refresh_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Data(base.DataModelBase):
 
-    """Input data model for :obj:`com.atproto.server.requestPasswordReset`.
+    """Input data model for :obj:`com.atproto.server.revokeAppPassword`.
 
     Attributes:
-        email: Email.
+        name: Name.
     """
 
-    email: str
+    name: str
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/reset_password.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/server/reset_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 from dataclasses import dataclass
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
-class Data(base.DataModelBase):
+class Params(base.ParamsModelBase):
 
-    """Input data model for :obj:`com.atproto.server.revokeAppPassword`.
+    """Parameters model for :obj:`com.atproto.sync.requestCrawl`.
 
     Attributes:
-        name: Name.
+        hostname: Hostname of the service that is requesting to be crawled.
     """
 
-    name: str
+    hostname: str
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blob.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Type, Union
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getBlob`.
+    """Parameters model for :obj:`com.atproto.sync.getCheckout`.
 
     Attributes:
         did: The DID of the repo.
-        cid: The CID of the blob to fetch.
+        commit: The commit to get the checkout from. Defaults to current HEAD.
     """
 
-    cid: str
     did: str
+    commit: t.Optional[str] = None
 
 
 #: Response raw data type.
-Response: Union[Type[str], Type[bytes]] = bytes
+Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Type, Union
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
     """Parameters model for :obj:`com.atproto.sync.getBlocks`.
 
     Attributes:
         did: The DID of the repo.
         cids: Cids.
     """
 
-    cids: List[str]
+    cids: t.List[str]
     did: str
 
 
 #: Response raw data type.
-Response: Union[Type[str], Type[bytes]] = bytes
+Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_blob.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional, Type, Union
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getCheckout`.
+    """Parameters model for :obj:`com.atproto.sync.getBlob`.
 
     Attributes:
         did: The DID of the repo.
-        commit: The commit to get the checkout from. Defaults to current HEAD.
+        cid: The CID of the blob to fetch.
     """
 
+    cid: str
     did: str
-    commit: Optional[str] = None
 
 
 #: Response raw data type.
-Response: Union[Type[str], Type[bytes]] = bytes
+Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_head.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,26 +9,14 @@
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.getHead`.
+    """Parameters model for :obj:`com.atproto.sync.notifyOfUpdate`.
 
     Attributes:
-        did: The DID of the repo.
+        hostname: Hostname of the service that is notifying of update.
     """
 
-    did: str
-
-
-@dataclass
-class Response(base.ResponseModelBase):
-
-    """Output data model for :obj:`com.atproto.sync.getHead`.
-
-    Attributes:
-        root: Root.
-    """
-
-    root: str
+    hostname: str
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_record.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_record.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional, Type, Union
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
@@ -22,12 +22,12 @@
         rkey: Rkey.
         commit: An optional past commit CID.
     """
 
     collection: str
     did: str
     rkey: str
-    commit: Optional[str] = None
+    commit: t.Optional[str] = None
 
 
 #: Response raw data type.
-Response: Union[Type[str], Type[bytes]] = bytes
+Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/get_repo.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/get_repo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import Optional, Type, Union
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
@@ -19,13 +19,13 @@
     Attributes:
         did: The DID of the repo.
         earliest: The earliest commit in the commit range (not inclusive).
         latest: The latest commit in the commit range (inclusive).
     """
 
     did: str
-    earliest: Optional[str] = None
-    latest: Optional[str] = None
+    earliest: t.Optional[str] = None
+    latest: t.Optional[str] = None
 
 
 #: Response raw data type.
-Response: Union[Type[str], Type[bytes]] = bytes
+Response: t.Union[t.Type[str], t.Type[bytes]] = bytes
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
@@ -19,21 +19,21 @@
     Attributes:
         did: The DID of the repo.
         latest: The most recent commit.
         earliest: The earliest commit to start from.
     """
 
     did: str
-    earliest: Optional[str] = None
-    latest: Optional[str] = None
+    earliest: t.Optional[str] = None
+    latest: t.Optional[str] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
     """Output data model for :obj:`com.atproto.sync.listBlobs`.
 
     Attributes:
         cids: Cids.
     """
 
-    cids: List[str]
+    cids: t.List[str]
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/list_repos.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/graph/get_follows.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,44 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.listRepos`.
+    """Parameters model for :obj:`app.bsky.graph.getFollows`.
 
     Attributes:
+        actor: Actor.
         limit: Limit.
         cursor: Cursor.
     """
 
-    cursor: Optional[str] = None
-    limit: Optional[int] = None
+    actor: str
+    cursor: t.Optional[str] = None
+    limit: t.Optional[int] = None
 
 
 @dataclass
 class Response(base.ResponseModelBase):
 
-    """Output data model for :obj:`com.atproto.sync.listRepos`.
+    """Output data model for :obj:`app.bsky.graph.getFollows`.
 
     Attributes:
+        subject: Subject.
         cursor: Cursor.
-        repos: Repos.
+        follows: Follows.
     """
 
-    repos: List['models.ComAtprotoSyncListRepos.Repo']
-    cursor: Optional[str] = None
-
-
-@dataclass
-class Repo(base.ModelBase):
-
-    """Definition model for :obj:`com.atproto.sync.listRepos`.
-
-    Attributes:
-        did: Did.
-        head: Head.
-    """
-
-    did: str
-    head: str
-
-    _type: str = 'com.atproto.sync.listRepos#repo'
+    follows: t.List['models.AppBskyActorDefs.ProfileView']
+    subject: 'models.AppBskyActorDefs.ProfileView'
+    cursor: t.Optional[str] = None
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py` & `atproto-0.0.7/atproto/xrpc_client/models/app/bsky/feed/get_posts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
 
+from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
 class Params(base.ParamsModelBase):
 
-    """Parameters model for :obj:`com.atproto.sync.notifyOfUpdate`.
+    """Parameters model for :obj:`app.bsky.feed.getPosts`.
 
     Attributes:
-        hostname: Hostname of the service that is notifying of update.
+        uris: Uris.
     """
 
-    hostname: str
+    uris: t.List[str]
+
+
+@dataclass
+class Response(base.ResponseModelBase):
+
+    """Output data model for :obj:`app.bsky.feed.getPosts`.
+
+    Attributes:
+        posts: Posts.
+    """
+
+    posts: t.List['models.AppBskyFeedDefs.PostView']
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py` & `atproto-0.0.7/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass
-from typing import List, Optional, Union
 
 from atproto import CID
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models import base
 
 
 @dataclass
@@ -27,24 +27,24 @@
         prev: Prev.
         blocks: CAR file containing relevant blocks.
         ops: Ops.
         blobs: Blobs.
         time: Time.
     """
 
-    blobs: List[CID]
-    blocks: Union[str, bytes]
+    blobs: t.List[CID]
+    blocks: t.Union[str, bytes]
     commit: CID
-    ops: List['models.ComAtprotoSyncSubscribeRepos.RepoOp']
+    ops: t.List['models.ComAtprotoSyncSubscribeRepos.RepoOp']
     rebase: bool
     repo: str
     seq: int
     time: str
     tooBig: bool
-    prev: Optional[CID] = None
+    prev: t.Optional[CID] = None
 
     _type: str = 'com.atproto.sync.subscribeRepos#commit'
 
 
 @dataclass
 class Handle(base.ModelBase):
 
@@ -76,15 +76,15 @@
         migrateTo: Migrate to.
         time: Time.
     """
 
     did: str
     seq: int
     time: str
-    migrateTo: Optional[str] = None
+    migrateTo: t.Optional[str] = None
 
     _type: str = 'com.atproto.sync.subscribeRepos#migrate'
 
 
 @dataclass
 class Tombstone(base.ModelBase):
 
@@ -110,15 +110,15 @@
 
     Attributes:
         name: Name.
         message: Message.
     """
 
     name: str
-    message: Optional[str] = None
+    message: t.Optional[str] = None
 
     _type: str = 'com.atproto.sync.subscribeRepos#info'
 
 
 @dataclass
 class RepoOp(base.ModelBase):
 
@@ -128,10 +128,10 @@
         action: Action.
         path: Path.
         cid: Cid.
     """
 
     action: str
     path: str
-    cid: Optional[CID] = None
+    cid: t.Optional[CID] = None
 
     _type: str = 'com.atproto.sync.subscribeRepos#repoOp'
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/type_conversion.py` & `atproto-0.0.7/atproto/xrpc_client/models/type_conversion.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.6/atproto/xrpc_client/models/utils.py` & `atproto-0.0.7/atproto/xrpc_client/models/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 import json
-from typing import TYPE_CHECKING, Any, Optional, Type, TypeVar, Union
+import typing as t
 
 from dacite import Config, exceptions, from_dict
 
 from atproto.cid import CID
 from atproto.exceptions import (
     MissingValueError,
     ModelError,
@@ -12,18 +12,18 @@
     UnexpectedFieldError,
     WrongTypeError,
 )
 from atproto.xrpc_client.models.base import RecordModelBase
 from atproto.xrpc_client.models.blob_ref import BlobRef
 from atproto.xrpc_client.models.type_conversion import RECORD_TYPE_TO_MODEL_CLASS
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     from atproto.xrpc_client.request import Response
 
-M = TypeVar('M')
+M = t.TypeVar('M')
 
 
 def _record_model_type_hook(data: dict) -> RecordModelBase:
     record_type = data.pop('$type')
     return get_or_create_model(data, RECORD_TYPE_TO_MODEL_CLASS[record_type])
 
 
@@ -31,15 +31,15 @@
     BlobRef: lambda ref: BlobRef.from_dict(ref),
     CID: lambda ref: CID.decode(ref),
     RecordModelBase: _record_model_type_hook,
 }
 _DACITE_CONFIG = Config(type_hooks=_TYPE_HOOKS)
 
 
-def get_or_create_model(model_data: Union[dict], model: Type[M]) -> Optional[M]:
+def get_or_create_model(model_data: t.Union[dict], model: t.Type[M]) -> t.Optional[M]:
     if model_data is None:
         return None
 
     if isinstance(model_data, model):
         return model_data
 
     try:
@@ -57,30 +57,30 @@
         raise WrongTypeError(str(e))
     except exceptions.DaciteFieldError as e:
         raise ModelFieldError(str(e))
     except exceptions.DaciteError as e:
         raise ModelError(str(e))
 
 
-def get_response_model(response: 'Response', model: Type[M]) -> Optional[M]:
+def get_response_model(response: 'Response', model: t.Type[M]) -> t.Optional[M]:
     if model is bool:
         # Could not be False? Because the exception with errors will be raised from the server
         return response.success
 
     return get_or_create_model(response.content, model)
 
 
 def _handle_dict_key(key: str) -> str:
     if key == '_type':  # System field. Replaced to original $ symbol because is not allowed in Python.
         return '$type'
 
     return key
 
 
-def _handle_dict_value(ref: Any) -> Any:
+def _handle_dict_value(ref: t.Any) -> t.Any:
     if isinstance(ref, BlobRef):
         return ref.to_dict()
     elif isinstance(ref, CID):
         return ref.encode()
 
     return ref
 
@@ -100,15 +100,15 @@
     return dataclasses.asdict(model, dict_factory=_model_as_dict_factory)
 
 
 def get_model_as_json(model) -> str:
     return json.dumps(get_model_as_dict(model))
 
 
-def is_json(json_data: Union[str, bytes]):
+def is_json(json_data: t.Union[str, bytes]):
     if isinstance(json_data, bytes):
         json_data.decode('UTF-8')
 
     try:
         json.loads(json_data)
         return True
     except Exception:  # noqa
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/namespaces/async_ns.py` & `atproto-0.0.7/atproto/xrpc_client/namespaces/async_ns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass, field
-from typing import Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models.utils import get_or_create_model, get_response_model
 from atproto.xrpc_client.namespaces.base import DefaultNamespace, NamespaceBase
 
 
 @dataclass
@@ -36,15 +36,15 @@
         self.notification = NotificationNamespace(self._client)
         self.unspecced = UnspeccedNamespace(self._client)
 
 
 @dataclass
 class ActorNamespace(NamespaceBase):
     async def get_preferences(
-        self, params: Optional[Union[dict, 'models.AppBskyActorGetPreferences.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorGetPreferences.Params']] = None, **kwargs
     ) -> models.AppBskyActorGetPreferences.Response:
         """Get private preferences attached to the account.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -58,15 +58,15 @@
         params = get_or_create_model(params, models.AppBskyActorGetPreferences.Params)
         response = await self._client.invoke_query(
             'app.bsky.actor.getPreferences', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetPreferences.Response)
 
     async def get_profile(
-        self, params: Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
     ) -> models.AppBskyActorGetProfile.ResponseRef:
         """Get profile.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -80,15 +80,15 @@
         params = get_or_create_model(params, models.AppBskyActorGetProfile.Params)
         response = await self._client.invoke_query(
             'app.bsky.actor.getProfile', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetProfile.ResponseRef)
 
     async def get_profiles(
-        self, params: Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
     ) -> models.AppBskyActorGetProfiles.Response:
         """Get profiles.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -102,15 +102,15 @@
         params = get_or_create_model(params, models.AppBskyActorGetProfiles.Params)
         response = await self._client.invoke_query(
             'app.bsky.actor.getProfiles', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetProfiles.Response)
 
     async def get_suggestions(
-        self, params: Optional[Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
     ) -> models.AppBskyActorGetSuggestions.Response:
         """Get a list of actors suggested for following. Used in discovery UIs.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -123,15 +123,15 @@
 
         params = get_or_create_model(params, models.AppBskyActorGetSuggestions.Params)
         response = await self._client.invoke_query(
             'app.bsky.actor.getSuggestions', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetSuggestions.Response)
 
-    async def put_preferences(self, data: Union[dict, 'models.AppBskyActorPutPreferences.Data'], **kwargs) -> bool:
+    async def put_preferences(self, data: t.Union[dict, 'models.AppBskyActorPutPreferences.Data'], **kwargs) -> bool:
         """Sets the private preferences attached to the account.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -144,15 +144,15 @@
         data = get_or_create_model(data, models.AppBskyActorPutPreferences.Data)
         response = await self._client.invoke_procedure(
             'app.bsky.actor.putPreferences', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def search_actors(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
     ) -> models.AppBskyActorSearchActors.Response:
         """Find actors matching search criteria.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -166,15 +166,15 @@
         params = get_or_create_model(params, models.AppBskyActorSearchActors.Params)
         response = await self._client.invoke_query(
             'app.bsky.actor.searchActors', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorSearchActors.Response)
 
     async def search_actors_typeahead(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
     ) -> models.AppBskyActorSearchActorsTypeahead.Response:
         """Find actor suggestions for a search term.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -191,15 +191,15 @@
         )
         return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
 
 
 @dataclass
 class GraphNamespace(NamespaceBase):
     async def get_blocks(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetBlocks.Response:
         """Who is the requester's account blocking?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -213,15 +213,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetBlocks.Params)
         response = await self._client.invoke_query(
             'app.bsky.graph.getBlocks', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetBlocks.Response)
 
     async def get_followers(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
     ) -> models.AppBskyGraphGetFollowers.Response:
         """Who is following an actor?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -235,15 +235,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetFollowers.Params)
         response = await self._client.invoke_query(
             'app.bsky.graph.getFollowers', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetFollowers.Response)
 
     async def get_follows(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
     ) -> models.AppBskyGraphGetFollows.Response:
         """Who is an actor following?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -257,15 +257,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetFollows.Params)
         response = await self._client.invoke_query(
             'app.bsky.graph.getFollows', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetFollows.Response)
 
     async def get_list(
-        self, params: Union[dict, 'models.AppBskyGraphGetList.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetList.Params'], **kwargs
     ) -> models.AppBskyGraphGetList.Response:
         """Fetch a list of actors.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -279,15 +279,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetList.Params)
         response = await self._client.invoke_query(
             'app.bsky.graph.getList', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetList.Response)
 
     async def get_list_mutes(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetListMutes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetListMutes.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetListMutes.Response:
         """Which lists is the requester's account muting?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -301,15 +301,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetListMutes.Params)
         response = await self._client.invoke_query(
             'app.bsky.graph.getListMutes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetListMutes.Response)
 
     async def get_lists(
-        self, params: Union[dict, 'models.AppBskyGraphGetLists.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetLists.Params'], **kwargs
     ) -> models.AppBskyGraphGetLists.Response:
         """Fetch a list of lists that belong to an actor.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -323,15 +323,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetLists.Params)
         response = await self._client.invoke_query(
             'app.bsky.graph.getLists', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetLists.Response)
 
     async def get_mutes(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetMutes.Response:
         """Who does the viewer mute?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -344,15 +344,15 @@
 
         params = get_or_create_model(params, models.AppBskyGraphGetMutes.Params)
         response = await self._client.invoke_query(
             'app.bsky.graph.getMutes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetMutes.Response)
 
-    async def mute_actor(self, data: Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
+    async def mute_actor(self, data: t.Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
         """Mute an actor by did or handle.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -364,15 +364,15 @@
 
         data = get_or_create_model(data, models.AppBskyGraphMuteActor.Data)
         response = await self._client.invoke_procedure(
             'app.bsky.graph.muteActor', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    async def mute_actor_list(self, data: Union[dict, 'models.AppBskyGraphMuteActorList.Data'], **kwargs) -> bool:
+    async def mute_actor_list(self, data: t.Union[dict, 'models.AppBskyGraphMuteActorList.Data'], **kwargs) -> bool:
         """Mute a list of actors.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -384,15 +384,15 @@
 
         data = get_or_create_model(data, models.AppBskyGraphMuteActorList.Data)
         response = await self._client.invoke_procedure(
             'app.bsky.graph.muteActorList', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    async def unmute_actor(self, data: Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
+    async def unmute_actor(self, data: t.Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
         """Unmute an actor by did or handle.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -404,15 +404,15 @@
 
         data = get_or_create_model(data, models.AppBskyGraphUnmuteActor.Data)
         response = await self._client.invoke_procedure(
             'app.bsky.graph.unmuteActor', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    async def unmute_actor_list(self, data: Union[dict, 'models.AppBskyGraphUnmuteActorList.Data'], **kwargs) -> bool:
+    async def unmute_actor_list(self, data: t.Union[dict, 'models.AppBskyGraphUnmuteActorList.Data'], **kwargs) -> bool:
         """Unmute a list of actors.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -428,15 +428,15 @@
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class FeedNamespace(NamespaceBase):
     async def get_author_feed(
-        self, params: Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
     ) -> models.AppBskyFeedGetAuthorFeed.Response:
         """A view of an actor's feed.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -450,15 +450,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
         response = await self._client.invoke_query(
             'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
 
     async def get_likes(
-        self, params: Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
     ) -> models.AppBskyFeedGetLikes.Response:
         """Get likes.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -472,15 +472,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
         response = await self._client.invoke_query(
             'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetLikes.Response)
 
     async def get_post_thread(
-        self, params: Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
     ) -> models.AppBskyFeedGetPostThread.Response:
         """Get post thread.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -494,15 +494,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
         response = await self._client.invoke_query(
             'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
 
     async def get_posts(
-        self, params: Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
     ) -> models.AppBskyFeedGetPosts.Response:
         """A view of an actor's feed.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -516,15 +516,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
         response = await self._client.invoke_query(
             'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetPosts.Response)
 
     async def get_reposted_by(
-        self, params: Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
     ) -> models.AppBskyFeedGetRepostedBy.Response:
         """Get reposted by.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -538,15 +538,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
         response = await self._client.invoke_query(
             'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
 
     async def get_timeline(
-        self, params: Optional[Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
     ) -> models.AppBskyFeedGetTimeline.Response:
         """A view of the user's home timeline.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -563,15 +563,15 @@
         )
         return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
 
 
 @dataclass
 class UnspeccedNamespace(NamespaceBase):
     async def get_popular(
-        self, params: Optional[Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
     ) -> models.AppBskyUnspeccedGetPopular.Response:
         """An unspecced view of globally popular items.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -588,15 +588,15 @@
         )
         return get_response_model(response, models.AppBskyUnspeccedGetPopular.Response)
 
 
 @dataclass
 class NotificationNamespace(NamespaceBase):
     async def get_unread_count(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
     ) -> models.AppBskyNotificationGetUnreadCount.Response:
         """Get unread count.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -610,15 +610,15 @@
         params = get_or_create_model(params, models.AppBskyNotificationGetUnreadCount.Params)
         response = await self._client.invoke_query(
             'app.bsky.notification.getUnreadCount', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyNotificationGetUnreadCount.Response)
 
     async def list_notifications(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
     ) -> models.AppBskyNotificationListNotifications.Response:
         """List notifications.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -631,15 +631,15 @@
 
         params = get_or_create_model(params, models.AppBskyNotificationListNotifications.Params)
         response = await self._client.invoke_query(
             'app.bsky.notification.listNotifications', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyNotificationListNotifications.Response)
 
-    async def update_seen(self, data: Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
+    async def update_seen(self, data: t.Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
         """Notify server that the user has seen notifications.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -683,15 +683,15 @@
         self.server = ServerNamespace(self._client)
         self.sync = SyncNamespace(self._client)
 
 
 @dataclass
 class SyncNamespace(NamespaceBase):
     async def get_blob(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetBlob.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetBlob.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetBlob.Response:
         """Get a blob associated with a given repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -705,15 +705,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetBlob.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.getBlob', params=params, output_encoding='*/*', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetBlob.Response)
 
     async def get_blocks(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetBlocks.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetBlocks.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetBlocks.Response:
         """Gets blocks from a given repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -727,15 +727,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetBlocks.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.getBlocks', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetBlocks.Response)
 
     async def get_checkout(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetCheckout.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetCheckout.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetCheckout.Response:
         """Gets the repo state.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -749,15 +749,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetCheckout.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.getCheckout', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetCheckout.Response)
 
     async def get_commit_path(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetCommitPath.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetCommitPath.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetCommitPath.Response:
         """Gets the path of repo commits.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -771,15 +771,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetCommitPath.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.getCommitPath', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetCommitPath.Response)
 
     async def get_head(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetHead.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetHead.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetHead.Response:
         """Gets the current HEAD CID of a repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -793,15 +793,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetHead.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.getHead', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetHead.Response)
 
     async def get_record(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetRecord.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetRecord.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetRecord.Response:
         """Gets blocks needed for existence or non-existence of record.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -815,15 +815,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetRecord.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.getRecord', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetRecord.Response)
 
     async def get_repo(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetRepo.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetRepo.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetRepo.Response:
         """Gets the repo state.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -837,15 +837,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetRepo.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.getRepo', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetRepo.Response)
 
     async def list_blobs(
-        self, params: Union[dict, 'models.ComAtprotoSyncListBlobs.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncListBlobs.Params'], **kwargs
     ) -> models.ComAtprotoSyncListBlobs.Response:
         """List blob cids for some range of commits.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -859,15 +859,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncListBlobs.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.listBlobs', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncListBlobs.Response)
 
     async def list_repos(
-        self, params: Optional[Union[dict, 'models.ComAtprotoSyncListRepos.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoSyncListRepos.Params']] = None, **kwargs
     ) -> models.ComAtprotoSyncListRepos.Response:
         """List dids and root cids of hosted repos.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -881,15 +881,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncListRepos.Params)
         response = await self._client.invoke_query(
             'com.atproto.sync.listRepos', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncListRepos.Response)
 
     async def notify_of_update(
-        self, params: Union[dict, 'models.ComAtprotoSyncNotifyOfUpdate.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncNotifyOfUpdate.Params'], **kwargs
     ) -> bool:
         """Notify a crawling service of a recent update. Often when a long break between updates causes the connection with the crawling service to break.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -900,15 +900,15 @@
             :class:`atproto.exceptions.AtProtocolError`: Base exception.
         """
 
         params = get_or_create_model(params, models.ComAtprotoSyncNotifyOfUpdate.Params)
         response = await self._client.invoke_query('com.atproto.sync.notifyOfUpdate', params=params, **kwargs)
         return get_response_model(response, bool)
 
-    async def request_crawl(self, params: Union[dict, 'models.ComAtprotoSyncRequestCrawl.Params'], **kwargs) -> bool:
+    async def request_crawl(self, params: t.Union[dict, 'models.ComAtprotoSyncRequestCrawl.Params'], **kwargs) -> bool:
         """Request a service to persistently crawl hosted repos.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -922,15 +922,15 @@
         response = await self._client.invoke_query('com.atproto.sync.requestCrawl', params=params, **kwargs)
         return get_response_model(response, bool)
 
 
 @dataclass
 class ServerNamespace(NamespaceBase):
     async def create_account(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateAccount.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateAccount.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateAccount.Response:
         """Create an account.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -948,15 +948,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateAccount.Response)
 
     async def create_app_password(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateAppPassword.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateAppPassword.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateAppPassword.ResponseRef:
         """Create an app-specific password.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -974,15 +974,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateAppPassword.ResponseRef)
 
     async def create_invite_code(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateInviteCode.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateInviteCode.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateInviteCode.Response:
         """Create an invite code.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1000,15 +1000,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateInviteCode.Response)
 
     async def create_invite_codes(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateInviteCodes.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateInviteCodes.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateInviteCodes.Response:
         """Create an invite code.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1026,15 +1026,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateInviteCodes.Response)
 
     async def create_session(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateSession.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateSession.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateSession.Response:
         """Create an authentication session.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1051,15 +1051,15 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateSession.Response)
 
-    async def delete_account(self, data: Union[dict, 'models.ComAtprotoServerDeleteAccount.Data'], **kwargs) -> bool:
+    async def delete_account(self, data: t.Union[dict, 'models.ComAtprotoServerDeleteAccount.Data'], **kwargs) -> bool:
         """Delete a user account with a token and password.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1106,15 +1106,15 @@
 
         response = await self._client.invoke_query(
             'com.atproto.server.describeServer', output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoServerDescribeServer.Response)
 
     async def get_account_invite_codes(
-        self, params: Optional[Union[dict, 'models.ComAtprotoServerGetAccountInviteCodes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoServerGetAccountInviteCodes.Params']] = None, **kwargs
     ) -> models.ComAtprotoServerGetAccountInviteCodes.Response:
         """Get all invite codes for a given account.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1198,15 +1198,15 @@
             :class:`atproto.exceptions.AtProtocolError`: Base exception.
         """
 
         response = await self._client.invoke_procedure('com.atproto.server.requestAccountDelete', **kwargs)
         return get_response_model(response, bool)
 
     async def request_password_reset(
-        self, data: Union[dict, 'models.ComAtprotoServerRequestPasswordReset.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerRequestPasswordReset.Data'], **kwargs
     ) -> bool:
         """Initiate a user account password reset via email.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1219,15 +1219,15 @@
 
         data = get_or_create_model(data, models.ComAtprotoServerRequestPasswordReset.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.server.requestPasswordReset', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    async def reset_password(self, data: Union[dict, 'models.ComAtprotoServerResetPassword.Data'], **kwargs) -> bool:
+    async def reset_password(self, data: t.Union[dict, 'models.ComAtprotoServerResetPassword.Data'], **kwargs) -> bool:
         """Reset a user account password using a token.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1240,15 +1240,15 @@
         data = get_or_create_model(data, models.ComAtprotoServerResetPassword.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.server.resetPassword', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def revoke_app_password(
-        self, data: Union[dict, 'models.ComAtprotoServerRevokeAppPassword.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerRevokeAppPassword.Data'], **kwargs
     ) -> bool:
         """Revoke an app-specific password by name.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1264,15 +1264,15 @@
             'com.atproto.server.revokeAppPassword', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class RepoNamespace(NamespaceBase):
-    async def apply_writes(self, data: Union[dict, 'models.ComAtprotoRepoApplyWrites.Data'], **kwargs) -> bool:
+    async def apply_writes(self, data: t.Union[dict, 'models.ComAtprotoRepoApplyWrites.Data'], **kwargs) -> bool:
         """Apply a batch transaction of creates, updates, and deletes.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1285,15 +1285,15 @@
         data = get_or_create_model(data, models.ComAtprotoRepoApplyWrites.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.repo.applyWrites', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def create_record(
-        self, data: Union[dict, 'models.ComAtprotoRepoCreateRecord.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoRepoCreateRecord.Data'], **kwargs
     ) -> models.ComAtprotoRepoCreateRecord.Response:
         """Create a new record.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1310,15 +1310,15 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoRepoCreateRecord.Response)
 
-    async def delete_record(self, data: Union[dict, 'models.ComAtprotoRepoDeleteRecord.Data'], **kwargs) -> bool:
+    async def delete_record(self, data: t.Union[dict, 'models.ComAtprotoRepoDeleteRecord.Data'], **kwargs) -> bool:
         """Delete a record, or ensure it doesn't exist.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1331,15 +1331,15 @@
         data = get_or_create_model(data, models.ComAtprotoRepoDeleteRecord.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.repo.deleteRecord', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def describe_repo(
-        self, params: Union[dict, 'models.ComAtprotoRepoDescribeRepo.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoRepoDescribeRepo.Params'], **kwargs
     ) -> models.ComAtprotoRepoDescribeRepo.Response:
         """Get information about the repo, including the list of collections.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1353,15 +1353,15 @@
         params = get_or_create_model(params, models.ComAtprotoRepoDescribeRepo.Params)
         response = await self._client.invoke_query(
             'com.atproto.repo.describeRepo', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoDescribeRepo.Response)
 
     async def get_record(
-        self, params: Union[dict, 'models.ComAtprotoRepoGetRecord.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoRepoGetRecord.Params'], **kwargs
     ) -> models.ComAtprotoRepoGetRecord.Response:
         """Get a record.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1375,15 +1375,15 @@
         params = get_or_create_model(params, models.ComAtprotoRepoGetRecord.Params)
         response = await self._client.invoke_query(
             'com.atproto.repo.getRecord', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoGetRecord.Response)
 
     async def list_records(
-        self, params: Union[dict, 'models.ComAtprotoRepoListRecords.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoRepoListRecords.Params'], **kwargs
     ) -> models.ComAtprotoRepoListRecords.Response:
         """List a range of records in a collection.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1397,15 +1397,15 @@
         params = get_or_create_model(params, models.ComAtprotoRepoListRecords.Params)
         response = await self._client.invoke_query(
             'com.atproto.repo.listRecords', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoListRecords.Response)
 
     async def put_record(
-        self, data: Union[dict, 'models.ComAtprotoRepoPutRecord.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoRepoPutRecord.Data'], **kwargs
     ) -> models.ComAtprotoRepoPutRecord.Response:
         """Write a record, creating or updating it as needed.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1422,15 +1422,15 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoRepoPutRecord.Response)
 
-    async def rebase_repo(self, data: Union[dict, 'models.ComAtprotoRepoRebaseRepo.Data'], **kwargs) -> bool:
+    async def rebase_repo(self, data: t.Union[dict, 'models.ComAtprotoRepoRebaseRepo.Data'], **kwargs) -> bool:
         """Simple rebase of repo that deletes history.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1467,15 +1467,15 @@
         )
         return get_response_model(response, models.ComAtprotoRepoUploadBlob.Response)
 
 
 @dataclass
 class AdminNamespace(NamespaceBase):
     async def disable_account_invites(
-        self, data: Union[dict, 'models.ComAtprotoAdminDisableAccountInvites.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminDisableAccountInvites.Data'], **kwargs
     ) -> bool:
         """Disable an account from receiving new invite codes, but does not invalidate existing codes.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1489,15 +1489,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminDisableAccountInvites.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.admin.disableAccountInvites', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def disable_invite_codes(
-        self, data: Optional[Union[dict, 'models.ComAtprotoAdminDisableInviteCodes.Data']] = None, **kwargs
+        self, data: t.Optional[t.Union[dict, 'models.ComAtprotoAdminDisableInviteCodes.Data']] = None, **kwargs
     ) -> bool:
         """Disable some set of codes and/or all codes associated with a set of users.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1511,15 +1511,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminDisableInviteCodes.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.admin.disableInviteCodes', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def enable_account_invites(
-        self, data: Union[dict, 'models.ComAtprotoAdminEnableAccountInvites.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminEnableAccountInvites.Data'], **kwargs
     ) -> bool:
         """Re-enable an accounts ability to receive invite codes.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1533,15 +1533,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminEnableAccountInvites.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.admin.enableAccountInvites', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def get_invite_codes(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetInviteCodes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminGetInviteCodes.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetInviteCodes.Response:
         """Admin view of invite codes.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1555,15 +1555,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetInviteCodes.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.getInviteCodes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetInviteCodes.Response)
 
     async def get_moderation_action(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetModerationAction.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetModerationAction.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetModerationAction.ResponseRef:
         """View details about a moderation action.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1577,15 +1577,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationAction.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.getModerationAction', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationAction.ResponseRef)
 
     async def get_moderation_actions(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetModerationActions.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminGetModerationActions.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetModerationActions.Response:
         """List moderation actions related to a subject.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1599,15 +1599,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationActions.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.getModerationActions', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationActions.Response)
 
     async def get_moderation_report(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetModerationReport.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetModerationReport.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetModerationReport.ResponseRef:
         """View details about a moderation report.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1621,15 +1621,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationReport.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.getModerationReport', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationReport.ResponseRef)
 
     async def get_moderation_reports(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetModerationReports.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminGetModerationReports.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetModerationReports.Response:
         """List moderation reports related to a subject.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1643,15 +1643,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationReports.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.getModerationReports', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationReports.Response)
 
     async def get_record(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetRecord.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetRecord.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetRecord.ResponseRef:
         """View details about a record.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1665,15 +1665,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetRecord.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.getRecord', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetRecord.ResponseRef)
 
     async def get_repo(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetRepo.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetRepo.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetRepo.ResponseRef:
         """View details about a repository.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1687,15 +1687,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetRepo.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.getRepo', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetRepo.ResponseRef)
 
     async def resolve_moderation_reports(
-        self, data: Union[dict, 'models.ComAtprotoAdminResolveModerationReports.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminResolveModerationReports.Data'], **kwargs
     ) -> models.ComAtprotoAdminResolveModerationReports.ResponseRef:
         """Resolve moderation reports by an action.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1713,15 +1713,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoAdminResolveModerationReports.ResponseRef)
 
     async def reverse_moderation_action(
-        self, data: Union[dict, 'models.ComAtprotoAdminReverseModerationAction.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminReverseModerationAction.Data'], **kwargs
     ) -> models.ComAtprotoAdminReverseModerationAction.ResponseRef:
         """Reverse a moderation action.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1739,15 +1739,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoAdminReverseModerationAction.ResponseRef)
 
     async def search_repos(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminSearchRepos.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminSearchRepos.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminSearchRepos.Response:
         """Find repositories based on a search term.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1761,15 +1761,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminSearchRepos.Params)
         response = await self._client.invoke_query(
             'com.atproto.admin.searchRepos', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminSearchRepos.Response)
 
     async def take_moderation_action(
-        self, data: Union[dict, 'models.ComAtprotoAdminTakeModerationAction.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminTakeModerationAction.Data'], **kwargs
     ) -> models.ComAtprotoAdminTakeModerationAction.ResponseRef:
         """Take a moderation action on a repo.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1787,15 +1787,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoAdminTakeModerationAction.ResponseRef)
 
     async def update_account_email(
-        self, data: Union[dict, 'models.ComAtprotoAdminUpdateAccountEmail.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminUpdateAccountEmail.Data'], **kwargs
     ) -> bool:
         """Administrative action to update an account's email.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1809,15 +1809,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminUpdateAccountEmail.Data)
         response = await self._client.invoke_procedure(
             'com.atproto.admin.updateAccountEmail', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     async def update_account_handle(
-        self, data: Union[dict, 'models.ComAtprotoAdminUpdateAccountHandle.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminUpdateAccountHandle.Data'], **kwargs
     ) -> bool:
         """Administrative action to update an account's handle.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1834,15 +1834,15 @@
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class IdentityNamespace(NamespaceBase):
     async def resolve_handle(
-        self, params: Optional[Union[dict, 'models.ComAtprotoIdentityResolveHandle.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoIdentityResolveHandle.Params']] = None, **kwargs
     ) -> models.ComAtprotoIdentityResolveHandle.Response:
         """Provides the DID of a repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1855,15 +1855,15 @@
 
         params = get_or_create_model(params, models.ComAtprotoIdentityResolveHandle.Params)
         response = await self._client.invoke_query(
             'com.atproto.identity.resolveHandle', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoIdentityResolveHandle.Response)
 
-    async def update_handle(self, data: Union[dict, 'models.ComAtprotoIdentityUpdateHandle.Data'], **kwargs) -> bool:
+    async def update_handle(self, data: t.Union[dict, 'models.ComAtprotoIdentityUpdateHandle.Data'], **kwargs) -> bool:
         """Updates the handle of the account.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1879,15 +1879,15 @@
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class ModerationNamespace(NamespaceBase):
     async def create_report(
-        self, data: Union[dict, 'models.ComAtprotoModerationCreateReport.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoModerationCreateReport.Data'], **kwargs
     ) -> models.ComAtprotoModerationCreateReport.Response:
         """Report a repo or a record.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1908,15 +1908,15 @@
         )
         return get_response_model(response, models.ComAtprotoModerationCreateReport.Response)
 
 
 @dataclass
 class LabelNamespace(NamespaceBase):
     async def query_labels(
-        self, params: Union[dict, 'models.ComAtprotoLabelQueryLabels.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoLabelQueryLabels.Params'], **kwargs
     ) -> models.ComAtprotoLabelQueryLabels.Response:
         """Find labels relevant to the provided URI patterns.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/namespaces/sync_ns.py` & `atproto-0.0.7/atproto/xrpc_client/namespaces/sync_ns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ##################################################################
 # THIS IS THE AUTO-GENERATED CODE. DON'T EDIT IT BY HANDS!
 # Copyright (C) 2023 Ilya (Marshal) <https://github.com/MarshalX>.
 # This file is part of Python atproto SDK. Licenced under MIT.
 ##################################################################
 
 
+import typing as t
 from dataclasses import dataclass, field
-from typing import Optional, Union
 
 from atproto.xrpc_client import models
 from atproto.xrpc_client.models.utils import get_or_create_model, get_response_model
 from atproto.xrpc_client.namespaces.base import DefaultNamespace, NamespaceBase
 
 
 @dataclass
@@ -36,15 +36,15 @@
         self.notification = NotificationNamespace(self._client)
         self.unspecced = UnspeccedNamespace(self._client)
 
 
 @dataclass
 class ActorNamespace(NamespaceBase):
     def get_preferences(
-        self, params: Optional[Union[dict, 'models.AppBskyActorGetPreferences.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorGetPreferences.Params']] = None, **kwargs
     ) -> models.AppBskyActorGetPreferences.Response:
         """Get private preferences attached to the account.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -58,15 +58,15 @@
         params = get_or_create_model(params, models.AppBskyActorGetPreferences.Params)
         response = self._client.invoke_query(
             'app.bsky.actor.getPreferences', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetPreferences.Response)
 
     def get_profile(
-        self, params: Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyActorGetProfile.Params'], **kwargs
     ) -> models.AppBskyActorGetProfile.ResponseRef:
         """Get profile.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -80,15 +80,15 @@
         params = get_or_create_model(params, models.AppBskyActorGetProfile.Params)
         response = self._client.invoke_query(
             'app.bsky.actor.getProfile', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetProfile.ResponseRef)
 
     def get_profiles(
-        self, params: Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyActorGetProfiles.Params'], **kwargs
     ) -> models.AppBskyActorGetProfiles.Response:
         """Get profiles.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -102,15 +102,15 @@
         params = get_or_create_model(params, models.AppBskyActorGetProfiles.Params)
         response = self._client.invoke_query(
             'app.bsky.actor.getProfiles', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetProfiles.Response)
 
     def get_suggestions(
-        self, params: Optional[Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorGetSuggestions.Params']] = None, **kwargs
     ) -> models.AppBskyActorGetSuggestions.Response:
         """Get a list of actors suggested for following. Used in discovery UIs.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -123,15 +123,15 @@
 
         params = get_or_create_model(params, models.AppBskyActorGetSuggestions.Params)
         response = self._client.invoke_query(
             'app.bsky.actor.getSuggestions', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorGetSuggestions.Response)
 
-    def put_preferences(self, data: Union[dict, 'models.AppBskyActorPutPreferences.Data'], **kwargs) -> bool:
+    def put_preferences(self, data: t.Union[dict, 'models.AppBskyActorPutPreferences.Data'], **kwargs) -> bool:
         """Sets the private preferences attached to the account.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -144,15 +144,15 @@
         data = get_or_create_model(data, models.AppBskyActorPutPreferences.Data)
         response = self._client.invoke_procedure(
             'app.bsky.actor.putPreferences', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     def search_actors(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorSearchActors.Params']] = None, **kwargs
     ) -> models.AppBskyActorSearchActors.Response:
         """Find actors matching search criteria.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -166,15 +166,15 @@
         params = get_or_create_model(params, models.AppBskyActorSearchActors.Params)
         response = self._client.invoke_query(
             'app.bsky.actor.searchActors', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyActorSearchActors.Response)
 
     def search_actors_typeahead(
-        self, params: Optional[Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyActorSearchActorsTypeahead.Params']] = None, **kwargs
     ) -> models.AppBskyActorSearchActorsTypeahead.Response:
         """Find actor suggestions for a search term.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -191,15 +191,15 @@
         )
         return get_response_model(response, models.AppBskyActorSearchActorsTypeahead.Response)
 
 
 @dataclass
 class GraphNamespace(NamespaceBase):
     def get_blocks(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetBlocks.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetBlocks.Response:
         """Who is the requester's account blocking?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -213,15 +213,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetBlocks.Params)
         response = self._client.invoke_query(
             'app.bsky.graph.getBlocks', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetBlocks.Response)
 
     def get_followers(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetFollowers.Params'], **kwargs
     ) -> models.AppBskyGraphGetFollowers.Response:
         """Who is following an actor?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -235,15 +235,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetFollowers.Params)
         response = self._client.invoke_query(
             'app.bsky.graph.getFollowers', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetFollowers.Response)
 
     def get_follows(
-        self, params: Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetFollows.Params'], **kwargs
     ) -> models.AppBskyGraphGetFollows.Response:
         """Who is an actor following?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -257,15 +257,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetFollows.Params)
         response = self._client.invoke_query(
             'app.bsky.graph.getFollows', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetFollows.Response)
 
     def get_list(
-        self, params: Union[dict, 'models.AppBskyGraphGetList.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetList.Params'], **kwargs
     ) -> models.AppBskyGraphGetList.Response:
         """Fetch a list of actors.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -279,15 +279,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetList.Params)
         response = self._client.invoke_query(
             'app.bsky.graph.getList', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetList.Response)
 
     def get_list_mutes(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetListMutes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetListMutes.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetListMutes.Response:
         """Which lists is the requester's account muting?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -301,15 +301,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetListMutes.Params)
         response = self._client.invoke_query(
             'app.bsky.graph.getListMutes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetListMutes.Response)
 
     def get_lists(
-        self, params: Union[dict, 'models.AppBskyGraphGetLists.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyGraphGetLists.Params'], **kwargs
     ) -> models.AppBskyGraphGetLists.Response:
         """Fetch a list of lists that belong to an actor.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -323,15 +323,15 @@
         params = get_or_create_model(params, models.AppBskyGraphGetLists.Params)
         response = self._client.invoke_query(
             'app.bsky.graph.getLists', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetLists.Response)
 
     def get_mutes(
-        self, params: Optional[Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyGraphGetMutes.Params']] = None, **kwargs
     ) -> models.AppBskyGraphGetMutes.Response:
         """Who does the viewer mute?
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -344,15 +344,15 @@
 
         params = get_or_create_model(params, models.AppBskyGraphGetMutes.Params)
         response = self._client.invoke_query(
             'app.bsky.graph.getMutes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyGraphGetMutes.Response)
 
-    def mute_actor(self, data: Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
+    def mute_actor(self, data: t.Union[dict, 'models.AppBskyGraphMuteActor.Data'], **kwargs) -> bool:
         """Mute an actor by did or handle.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -364,15 +364,15 @@
 
         data = get_or_create_model(data, models.AppBskyGraphMuteActor.Data)
         response = self._client.invoke_procedure(
             'app.bsky.graph.muteActor', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    def mute_actor_list(self, data: Union[dict, 'models.AppBskyGraphMuteActorList.Data'], **kwargs) -> bool:
+    def mute_actor_list(self, data: t.Union[dict, 'models.AppBskyGraphMuteActorList.Data'], **kwargs) -> bool:
         """Mute a list of actors.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -384,15 +384,15 @@
 
         data = get_or_create_model(data, models.AppBskyGraphMuteActorList.Data)
         response = self._client.invoke_procedure(
             'app.bsky.graph.muteActorList', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    def unmute_actor(self, data: Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
+    def unmute_actor(self, data: t.Union[dict, 'models.AppBskyGraphUnmuteActor.Data'], **kwargs) -> bool:
         """Unmute an actor by did or handle.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -404,15 +404,15 @@
 
         data = get_or_create_model(data, models.AppBskyGraphUnmuteActor.Data)
         response = self._client.invoke_procedure(
             'app.bsky.graph.unmuteActor', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    def unmute_actor_list(self, data: Union[dict, 'models.AppBskyGraphUnmuteActorList.Data'], **kwargs) -> bool:
+    def unmute_actor_list(self, data: t.Union[dict, 'models.AppBskyGraphUnmuteActorList.Data'], **kwargs) -> bool:
         """Unmute a list of actors.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -428,15 +428,15 @@
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class FeedNamespace(NamespaceBase):
     def get_author_feed(
-        self, params: Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetAuthorFeed.Params'], **kwargs
     ) -> models.AppBskyFeedGetAuthorFeed.Response:
         """A view of an actor's feed.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -450,15 +450,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetAuthorFeed.Params)
         response = self._client.invoke_query(
             'app.bsky.feed.getAuthorFeed', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetAuthorFeed.Response)
 
     def get_likes(
-        self, params: Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetLikes.Params'], **kwargs
     ) -> models.AppBskyFeedGetLikes.Response:
         """Get likes.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -472,15 +472,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetLikes.Params)
         response = self._client.invoke_query(
             'app.bsky.feed.getLikes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetLikes.Response)
 
     def get_post_thread(
-        self, params: Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPostThread.Params'], **kwargs
     ) -> models.AppBskyFeedGetPostThread.Response:
         """Get post thread.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -494,15 +494,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetPostThread.Params)
         response = self._client.invoke_query(
             'app.bsky.feed.getPostThread', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetPostThread.Response)
 
     def get_posts(
-        self, params: Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetPosts.Params'], **kwargs
     ) -> models.AppBskyFeedGetPosts.Response:
         """A view of an actor's feed.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -516,15 +516,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetPosts.Params)
         response = self._client.invoke_query(
             'app.bsky.feed.getPosts', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetPosts.Response)
 
     def get_reposted_by(
-        self, params: Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
+        self, params: t.Union[dict, 'models.AppBskyFeedGetRepostedBy.Params'], **kwargs
     ) -> models.AppBskyFeedGetRepostedBy.Response:
         """Get reposted by.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -538,15 +538,15 @@
         params = get_or_create_model(params, models.AppBskyFeedGetRepostedBy.Params)
         response = self._client.invoke_query(
             'app.bsky.feed.getRepostedBy', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyFeedGetRepostedBy.Response)
 
     def get_timeline(
-        self, params: Optional[Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyFeedGetTimeline.Params']] = None, **kwargs
     ) -> models.AppBskyFeedGetTimeline.Response:
         """A view of the user's home timeline.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -563,15 +563,15 @@
         )
         return get_response_model(response, models.AppBskyFeedGetTimeline.Response)
 
 
 @dataclass
 class UnspeccedNamespace(NamespaceBase):
     def get_popular(
-        self, params: Optional[Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyUnspeccedGetPopular.Params']] = None, **kwargs
     ) -> models.AppBskyUnspeccedGetPopular.Response:
         """An unspecced view of globally popular items.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -588,15 +588,15 @@
         )
         return get_response_model(response, models.AppBskyUnspeccedGetPopular.Response)
 
 
 @dataclass
 class NotificationNamespace(NamespaceBase):
     def get_unread_count(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyNotificationGetUnreadCount.Params']] = None, **kwargs
     ) -> models.AppBskyNotificationGetUnreadCount.Response:
         """Get unread count.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -610,15 +610,15 @@
         params = get_or_create_model(params, models.AppBskyNotificationGetUnreadCount.Params)
         response = self._client.invoke_query(
             'app.bsky.notification.getUnreadCount', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyNotificationGetUnreadCount.Response)
 
     def list_notifications(
-        self, params: Optional[Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.AppBskyNotificationListNotifications.Params']] = None, **kwargs
     ) -> models.AppBskyNotificationListNotifications.Response:
         """List notifications.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -631,15 +631,15 @@
 
         params = get_or_create_model(params, models.AppBskyNotificationListNotifications.Params)
         response = self._client.invoke_query(
             'app.bsky.notification.listNotifications', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.AppBskyNotificationListNotifications.Response)
 
-    def update_seen(self, data: Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
+    def update_seen(self, data: t.Union[dict, 'models.AppBskyNotificationUpdateSeen.Data'], **kwargs) -> bool:
         """Notify server that the user has seen notifications.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -683,15 +683,15 @@
         self.server = ServerNamespace(self._client)
         self.sync = SyncNamespace(self._client)
 
 
 @dataclass
 class SyncNamespace(NamespaceBase):
     def get_blob(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetBlob.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetBlob.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetBlob.Response:
         """Get a blob associated with a given repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -703,15 +703,15 @@
         """
 
         params = get_or_create_model(params, models.ComAtprotoSyncGetBlob.Params)
         response = self._client.invoke_query('com.atproto.sync.getBlob', params=params, output_encoding='*/*', **kwargs)
         return get_response_model(response, models.ComAtprotoSyncGetBlob.Response)
 
     def get_blocks(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetBlocks.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetBlocks.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetBlocks.Response:
         """Gets blocks from a given repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -725,15 +725,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetBlocks.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.getBlocks', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetBlocks.Response)
 
     def get_checkout(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetCheckout.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetCheckout.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetCheckout.Response:
         """Gets the repo state.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -747,15 +747,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetCheckout.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.getCheckout', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetCheckout.Response)
 
     def get_commit_path(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetCommitPath.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetCommitPath.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetCommitPath.Response:
         """Gets the path of repo commits.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -769,15 +769,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetCommitPath.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.getCommitPath', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetCommitPath.Response)
 
     def get_head(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetHead.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetHead.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetHead.Response:
         """Gets the current HEAD CID of a repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -791,15 +791,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetHead.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.getHead', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetHead.Response)
 
     def get_record(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetRecord.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetRecord.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetRecord.Response:
         """Gets blocks needed for existence or non-existence of record.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -813,15 +813,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetRecord.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.getRecord', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetRecord.Response)
 
     def get_repo(
-        self, params: Union[dict, 'models.ComAtprotoSyncGetRepo.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncGetRepo.Params'], **kwargs
     ) -> models.ComAtprotoSyncGetRepo.Response:
         """Gets the repo state.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -835,15 +835,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncGetRepo.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.getRepo', params=params, output_encoding='application/vnd.ipld.car', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncGetRepo.Response)
 
     def list_blobs(
-        self, params: Union[dict, 'models.ComAtprotoSyncListBlobs.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoSyncListBlobs.Params'], **kwargs
     ) -> models.ComAtprotoSyncListBlobs.Response:
         """List blob cids for some range of commits.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -857,15 +857,15 @@
         params = get_or_create_model(params, models.ComAtprotoSyncListBlobs.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.listBlobs', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncListBlobs.Response)
 
     def list_repos(
-        self, params: Optional[Union[dict, 'models.ComAtprotoSyncListRepos.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoSyncListRepos.Params']] = None, **kwargs
     ) -> models.ComAtprotoSyncListRepos.Response:
         """List dids and root cids of hosted repos.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -878,15 +878,15 @@
 
         params = get_or_create_model(params, models.ComAtprotoSyncListRepos.Params)
         response = self._client.invoke_query(
             'com.atproto.sync.listRepos', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoSyncListRepos.Response)
 
-    def notify_of_update(self, params: Union[dict, 'models.ComAtprotoSyncNotifyOfUpdate.Params'], **kwargs) -> bool:
+    def notify_of_update(self, params: t.Union[dict, 'models.ComAtprotoSyncNotifyOfUpdate.Params'], **kwargs) -> bool:
         """Notify a crawling service of a recent update. Often when a long break between updates causes the connection with the crawling service to break.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -896,15 +896,15 @@
             :class:`atproto.exceptions.AtProtocolError`: Base exception.
         """
 
         params = get_or_create_model(params, models.ComAtprotoSyncNotifyOfUpdate.Params)
         response = self._client.invoke_query('com.atproto.sync.notifyOfUpdate', params=params, **kwargs)
         return get_response_model(response, bool)
 
-    def request_crawl(self, params: Union[dict, 'models.ComAtprotoSyncRequestCrawl.Params'], **kwargs) -> bool:
+    def request_crawl(self, params: t.Union[dict, 'models.ComAtprotoSyncRequestCrawl.Params'], **kwargs) -> bool:
         """Request a service to persistently crawl hosted repos.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -918,15 +918,15 @@
         response = self._client.invoke_query('com.atproto.sync.requestCrawl', params=params, **kwargs)
         return get_response_model(response, bool)
 
 
 @dataclass
 class ServerNamespace(NamespaceBase):
     def create_account(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateAccount.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateAccount.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateAccount.Response:
         """Create an account.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -944,15 +944,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateAccount.Response)
 
     def create_app_password(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateAppPassword.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateAppPassword.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateAppPassword.ResponseRef:
         """Create an app-specific password.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -970,15 +970,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateAppPassword.ResponseRef)
 
     def create_invite_code(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateInviteCode.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateInviteCode.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateInviteCode.Response:
         """Create an invite code.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -996,15 +996,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateInviteCode.Response)
 
     def create_invite_codes(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateInviteCodes.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateInviteCodes.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateInviteCodes.Response:
         """Create an invite code.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1022,15 +1022,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateInviteCodes.Response)
 
     def create_session(
-        self, data: Union[dict, 'models.ComAtprotoServerCreateSession.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerCreateSession.Data'], **kwargs
     ) -> models.ComAtprotoServerCreateSession.Response:
         """Create an authentication session.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1047,15 +1047,15 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoServerCreateSession.Response)
 
-    def delete_account(self, data: Union[dict, 'models.ComAtprotoServerDeleteAccount.Data'], **kwargs) -> bool:
+    def delete_account(self, data: t.Union[dict, 'models.ComAtprotoServerDeleteAccount.Data'], **kwargs) -> bool:
         """Delete a user account with a token and password.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1102,15 +1102,15 @@
 
         response = self._client.invoke_query(
             'com.atproto.server.describeServer', output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoServerDescribeServer.Response)
 
     def get_account_invite_codes(
-        self, params: Optional[Union[dict, 'models.ComAtprotoServerGetAccountInviteCodes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoServerGetAccountInviteCodes.Params']] = None, **kwargs
     ) -> models.ComAtprotoServerGetAccountInviteCodes.Response:
         """Get all invite codes for a given account.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1194,15 +1194,15 @@
             :class:`atproto.exceptions.AtProtocolError`: Base exception.
         """
 
         response = self._client.invoke_procedure('com.atproto.server.requestAccountDelete', **kwargs)
         return get_response_model(response, bool)
 
     def request_password_reset(
-        self, data: Union[dict, 'models.ComAtprotoServerRequestPasswordReset.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoServerRequestPasswordReset.Data'], **kwargs
     ) -> bool:
         """Initiate a user account password reset via email.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1215,15 +1215,15 @@
 
         data = get_or_create_model(data, models.ComAtprotoServerRequestPasswordReset.Data)
         response = self._client.invoke_procedure(
             'com.atproto.server.requestPasswordReset', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    def reset_password(self, data: Union[dict, 'models.ComAtprotoServerResetPassword.Data'], **kwargs) -> bool:
+    def reset_password(self, data: t.Union[dict, 'models.ComAtprotoServerResetPassword.Data'], **kwargs) -> bool:
         """Reset a user account password using a token.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1235,15 +1235,17 @@
 
         data = get_or_create_model(data, models.ComAtprotoServerResetPassword.Data)
         response = self._client.invoke_procedure(
             'com.atproto.server.resetPassword', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
-    def revoke_app_password(self, data: Union[dict, 'models.ComAtprotoServerRevokeAppPassword.Data'], **kwargs) -> bool:
+    def revoke_app_password(
+        self, data: t.Union[dict, 'models.ComAtprotoServerRevokeAppPassword.Data'], **kwargs
+    ) -> bool:
         """Revoke an app-specific password by name.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1258,15 +1260,15 @@
             'com.atproto.server.revokeAppPassword', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class RepoNamespace(NamespaceBase):
-    def apply_writes(self, data: Union[dict, 'models.ComAtprotoRepoApplyWrites.Data'], **kwargs) -> bool:
+    def apply_writes(self, data: t.Union[dict, 'models.ComAtprotoRepoApplyWrites.Data'], **kwargs) -> bool:
         """Apply a batch transaction of creates, updates, and deletes.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1279,15 +1281,15 @@
         data = get_or_create_model(data, models.ComAtprotoRepoApplyWrites.Data)
         response = self._client.invoke_procedure(
             'com.atproto.repo.applyWrites', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     def create_record(
-        self, data: Union[dict, 'models.ComAtprotoRepoCreateRecord.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoRepoCreateRecord.Data'], **kwargs
     ) -> models.ComAtprotoRepoCreateRecord.Response:
         """Create a new record.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1304,15 +1306,15 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoRepoCreateRecord.Response)
 
-    def delete_record(self, data: Union[dict, 'models.ComAtprotoRepoDeleteRecord.Data'], **kwargs) -> bool:
+    def delete_record(self, data: t.Union[dict, 'models.ComAtprotoRepoDeleteRecord.Data'], **kwargs) -> bool:
         """Delete a record, or ensure it doesn't exist.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1325,15 +1327,15 @@
         data = get_or_create_model(data, models.ComAtprotoRepoDeleteRecord.Data)
         response = self._client.invoke_procedure(
             'com.atproto.repo.deleteRecord', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     def describe_repo(
-        self, params: Union[dict, 'models.ComAtprotoRepoDescribeRepo.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoRepoDescribeRepo.Params'], **kwargs
     ) -> models.ComAtprotoRepoDescribeRepo.Response:
         """Get information about the repo, including the list of collections.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1347,15 +1349,15 @@
         params = get_or_create_model(params, models.ComAtprotoRepoDescribeRepo.Params)
         response = self._client.invoke_query(
             'com.atproto.repo.describeRepo', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoDescribeRepo.Response)
 
     def get_record(
-        self, params: Union[dict, 'models.ComAtprotoRepoGetRecord.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoRepoGetRecord.Params'], **kwargs
     ) -> models.ComAtprotoRepoGetRecord.Response:
         """Get a record.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1369,15 +1371,15 @@
         params = get_or_create_model(params, models.ComAtprotoRepoGetRecord.Params)
         response = self._client.invoke_query(
             'com.atproto.repo.getRecord', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoGetRecord.Response)
 
     def list_records(
-        self, params: Union[dict, 'models.ComAtprotoRepoListRecords.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoRepoListRecords.Params'], **kwargs
     ) -> models.ComAtprotoRepoListRecords.Response:
         """List a range of records in a collection.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1391,15 +1393,15 @@
         params = get_or_create_model(params, models.ComAtprotoRepoListRecords.Params)
         response = self._client.invoke_query(
             'com.atproto.repo.listRecords', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoRepoListRecords.Response)
 
     def put_record(
-        self, data: Union[dict, 'models.ComAtprotoRepoPutRecord.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoRepoPutRecord.Data'], **kwargs
     ) -> models.ComAtprotoRepoPutRecord.Response:
         """Write a record, creating or updating it as needed.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1416,15 +1418,15 @@
             data=data,
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoRepoPutRecord.Response)
 
-    def rebase_repo(self, data: Union[dict, 'models.ComAtprotoRepoRebaseRepo.Data'], **kwargs) -> bool:
+    def rebase_repo(self, data: t.Union[dict, 'models.ComAtprotoRepoRebaseRepo.Data'], **kwargs) -> bool:
         """Simple rebase of repo that deletes history.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1461,15 +1463,15 @@
         )
         return get_response_model(response, models.ComAtprotoRepoUploadBlob.Response)
 
 
 @dataclass
 class AdminNamespace(NamespaceBase):
     def disable_account_invites(
-        self, data: Union[dict, 'models.ComAtprotoAdminDisableAccountInvites.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminDisableAccountInvites.Data'], **kwargs
     ) -> bool:
         """Disable an account from receiving new invite codes, but does not invalidate existing codes.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1483,15 +1485,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminDisableAccountInvites.Data)
         response = self._client.invoke_procedure(
             'com.atproto.admin.disableAccountInvites', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     def disable_invite_codes(
-        self, data: Optional[Union[dict, 'models.ComAtprotoAdminDisableInviteCodes.Data']] = None, **kwargs
+        self, data: t.Optional[t.Union[dict, 'models.ComAtprotoAdminDisableInviteCodes.Data']] = None, **kwargs
     ) -> bool:
         """Disable some set of codes and/or all codes associated with a set of users.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1505,15 +1507,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminDisableInviteCodes.Data)
         response = self._client.invoke_procedure(
             'com.atproto.admin.disableInviteCodes', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     def enable_account_invites(
-        self, data: Union[dict, 'models.ComAtprotoAdminEnableAccountInvites.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminEnableAccountInvites.Data'], **kwargs
     ) -> bool:
         """Re-enable an accounts ability to receive invite codes.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1527,15 +1529,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminEnableAccountInvites.Data)
         response = self._client.invoke_procedure(
             'com.atproto.admin.enableAccountInvites', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     def get_invite_codes(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetInviteCodes.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminGetInviteCodes.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetInviteCodes.Response:
         """Admin view of invite codes.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1549,15 +1551,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetInviteCodes.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.getInviteCodes', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetInviteCodes.Response)
 
     def get_moderation_action(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetModerationAction.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetModerationAction.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetModerationAction.ResponseRef:
         """View details about a moderation action.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1571,15 +1573,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationAction.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.getModerationAction', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationAction.ResponseRef)
 
     def get_moderation_actions(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetModerationActions.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminGetModerationActions.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetModerationActions.Response:
         """List moderation actions related to a subject.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1593,15 +1595,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationActions.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.getModerationActions', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationActions.Response)
 
     def get_moderation_report(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetModerationReport.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetModerationReport.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetModerationReport.ResponseRef:
         """View details about a moderation report.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1615,15 +1617,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationReport.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.getModerationReport', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationReport.ResponseRef)
 
     def get_moderation_reports(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminGetModerationReports.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminGetModerationReports.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminGetModerationReports.Response:
         """List moderation reports related to a subject.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1637,15 +1639,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetModerationReports.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.getModerationReports', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetModerationReports.Response)
 
     def get_record(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetRecord.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetRecord.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetRecord.ResponseRef:
         """View details about a record.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1659,15 +1661,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetRecord.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.getRecord', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetRecord.ResponseRef)
 
     def get_repo(
-        self, params: Union[dict, 'models.ComAtprotoAdminGetRepo.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoAdminGetRepo.Params'], **kwargs
     ) -> models.ComAtprotoAdminGetRepo.ResponseRef:
         """View details about a repository.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1681,15 +1683,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminGetRepo.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.getRepo', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminGetRepo.ResponseRef)
 
     def resolve_moderation_reports(
-        self, data: Union[dict, 'models.ComAtprotoAdminResolveModerationReports.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminResolveModerationReports.Data'], **kwargs
     ) -> models.ComAtprotoAdminResolveModerationReports.ResponseRef:
         """Resolve moderation reports by an action.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1707,15 +1709,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoAdminResolveModerationReports.ResponseRef)
 
     def reverse_moderation_action(
-        self, data: Union[dict, 'models.ComAtprotoAdminReverseModerationAction.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminReverseModerationAction.Data'], **kwargs
     ) -> models.ComAtprotoAdminReverseModerationAction.ResponseRef:
         """Reverse a moderation action.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1733,15 +1735,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoAdminReverseModerationAction.ResponseRef)
 
     def search_repos(
-        self, params: Optional[Union[dict, 'models.ComAtprotoAdminSearchRepos.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoAdminSearchRepos.Params']] = None, **kwargs
     ) -> models.ComAtprotoAdminSearchRepos.Response:
         """Find repositories based on a search term.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1755,15 +1757,15 @@
         params = get_or_create_model(params, models.ComAtprotoAdminSearchRepos.Params)
         response = self._client.invoke_query(
             'com.atproto.admin.searchRepos', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoAdminSearchRepos.Response)
 
     def take_moderation_action(
-        self, data: Union[dict, 'models.ComAtprotoAdminTakeModerationAction.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminTakeModerationAction.Data'], **kwargs
     ) -> models.ComAtprotoAdminTakeModerationAction.ResponseRef:
         """Take a moderation action on a repo.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1781,15 +1783,15 @@
             input_encoding='application/json',
             output_encoding='application/json',
             **kwargs,
         )
         return get_response_model(response, models.ComAtprotoAdminTakeModerationAction.ResponseRef)
 
     def update_account_email(
-        self, data: Union[dict, 'models.ComAtprotoAdminUpdateAccountEmail.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminUpdateAccountEmail.Data'], **kwargs
     ) -> bool:
         """Administrative action to update an account's email.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1803,15 +1805,15 @@
         data = get_or_create_model(data, models.ComAtprotoAdminUpdateAccountEmail.Data)
         response = self._client.invoke_procedure(
             'com.atproto.admin.updateAccountEmail', data=data, input_encoding='application/json', **kwargs
         )
         return get_response_model(response, bool)
 
     def update_account_handle(
-        self, data: Union[dict, 'models.ComAtprotoAdminUpdateAccountHandle.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoAdminUpdateAccountHandle.Data'], **kwargs
     ) -> bool:
         """Administrative action to update an account's handle.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1828,15 +1830,15 @@
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class IdentityNamespace(NamespaceBase):
     def resolve_handle(
-        self, params: Optional[Union[dict, 'models.ComAtprotoIdentityResolveHandle.Params']] = None, **kwargs
+        self, params: t.Optional[t.Union[dict, 'models.ComAtprotoIdentityResolveHandle.Params']] = None, **kwargs
     ) -> models.ComAtprotoIdentityResolveHandle.Response:
         """Provides the DID of a repo.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1849,15 +1851,15 @@
 
         params = get_or_create_model(params, models.ComAtprotoIdentityResolveHandle.Params)
         response = self._client.invoke_query(
             'com.atproto.identity.resolveHandle', params=params, output_encoding='application/json', **kwargs
         )
         return get_response_model(response, models.ComAtprotoIdentityResolveHandle.Response)
 
-    def update_handle(self, data: Union[dict, 'models.ComAtprotoIdentityUpdateHandle.Data'], **kwargs) -> bool:
+    def update_handle(self, data: t.Union[dict, 'models.ComAtprotoIdentityUpdateHandle.Data'], **kwargs) -> bool:
         """Updates the handle of the account.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
         Returns:
@@ -1873,15 +1875,15 @@
         )
         return get_response_model(response, bool)
 
 
 @dataclass
 class ModerationNamespace(NamespaceBase):
     def create_report(
-        self, data: Union[dict, 'models.ComAtprotoModerationCreateReport.Data'], **kwargs
+        self, data: t.Union[dict, 'models.ComAtprotoModerationCreateReport.Data'], **kwargs
     ) -> models.ComAtprotoModerationCreateReport.Response:
         """Report a repo or a record.
 
         Args:
             data: Input data.
             **kwargs: Arbitrary arguments to HTTP request.
 
@@ -1902,15 +1904,15 @@
         )
         return get_response_model(response, models.ComAtprotoModerationCreateReport.Response)
 
 
 @dataclass
 class LabelNamespace(NamespaceBase):
     def query_labels(
-        self, params: Union[dict, 'models.ComAtprotoLabelQueryLabels.Params'], **kwargs
+        self, params: t.Union[dict, 'models.ComAtprotoLabelQueryLabels.Params'], **kwargs
     ) -> models.ComAtprotoLabelQueryLabels.Response:
         """Find labels relevant to the provided URI patterns.
 
         Args:
             params: Parameters.
             **kwargs: Arbitrary arguments to HTTP request.
```

### Comparing `atproto-0.0.6/atproto/xrpc_client/request.py` & `atproto-0.0.7/atproto/xrpc_client/request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import json
+import typing as t
 from dataclasses import dataclass
-from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from atproto import exceptions
 from atproto.xrpc_client.models.utils import get_or_create_model, is_json
 
 
 @dataclass
 class Response:
     success: bool
     status_code: int
-    content: Optional[Union[dict, bytes, 'XrpcError']]
-    headers: Dict[str, Any]
+    content: t.Optional[t.Union[dict, bytes, 'XrpcError']]
+    headers: t.Dict[str, t.Any]
 
 
 @dataclass
 class XrpcError:
     error: str
-    message: Optional[str]
+    message: t.Optional[str]
 
 
 def _parse_response(response: httpx.Response) -> Response:
     content = response.content
     if response.headers.get('content-type') == 'application/json; charset=utf-8':
         content = response.json()
 
@@ -71,15 +71,15 @@
 
 class RequestBase:
     MANDATORY_HEADERS = {'User-Agent': f'atproto/alpha (Python SDK)'}
 
     def __init__(self):
         self._additional_headers: dict = {}
 
-    def get_headers(self, additional_headers: Optional[dict] = None) -> dict:
+    def get_headers(self, additional_headers: t.Optional[dict] = None) -> dict:
         headers = {**self.MANDATORY_HEADERS, **self._additional_headers}
 
         if additional_headers:
             headers.update(additional_headers)
 
         return headers
```

### Comparing `atproto-0.0.6/pyproject.toml` & `atproto-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atproto"
-version = "0.0.6" # placeholder. Dynamic version from Git Tag
+version = "0.0.7" # placeholder. Dynamic version from Git Tag
 description = "The AT Protocol SDK"
 authors = ["Ilya (Marshal) <ilya@marshal.dev>"]
 license = "MIT"
 repository = "https://github.com/MarshalX/atproto"
 readme = "README.md"
 keywords = ["library", "sdk", "codegen", "xrpc", "xrpc-client", "atprotocol", "atproto", "lexicon", "parser", "schema", "bluesky", "bluesky-api", "at", "uri", "atp", "nsid", "did", "cid"]
 classifiers = [
```

### Comparing `atproto-0.0.6/PKG-INFO` & `atproto-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atproto
-Version: 0.0.6
+Version: 0.0.7
 Summary: The AT Protocol SDK
 Home-page: https://github.com/MarshalX/atproto
 License: MIT
 Keywords: library,sdk,codegen,xrpc,xrpc-client,atprotocol,atproto,lexicon,parser,schema,bluesky,bluesky-api,at,uri,atp,nsid,did,cid
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 Requires-Python: >=3.7,<3.12
```

