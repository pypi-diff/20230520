# Comparing `tmp/pyrofork_dev-2.1.8.dev202305201733.tar.gz` & `tmp/PyroFork-dev-2.1.8.dev202305201740.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrofork_dev-2.1.8.dev202305201733.tar", max compression
+gzip compressed data, was "PyroFork-dev-2.1.8.dev202305201740.tar", last modified: Sat May 20 17:40:44 2023, max compression
```

## Comparing `pyrofork_dev-2.1.8.dev202305201733.tar` & `PyroFork-dev-2.1.8.dev202305201740.tar`

### file list

```diff
@@ -1,1684 +1,523 @@
--rw-r--r--   0        0        0     2155 2023-05-20 17:33:19.923593 pyrofork_dev-2.1.8.dev202305201733/README.md
--rw-r--r--   0        0        0     1931 2023-05-20 17:34:01.181056 pyrofork_dev-2.1.8.dev202305201733/pyproject.toml
--rw-r--r--   0        0        0     1446 2023-05-20 17:33:33.452332 pyrofork_dev-2.1.8.dev202305201733/pyrogram/__init__.py
--rw-r--r--   0        0        0    40792 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/client.py
--rw-r--r--   0        0        0      854 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2830 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4100 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1768 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2830 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2453 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4013 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4767 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2446 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13437 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0    10085 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   208021 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/emoji.py
--rw-r--r--   0        0        0     1736 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     1002 2023-05-20 17:33:19.927595 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     2307 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4520 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1265 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     2464 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1599 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     2468 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2406 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1723 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1299 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2489 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     1066 2023-05-20 17:34:01.169056 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/__init__.py
--rw-r--r--   0        0        0    25520 2023-05-20 17:34:01.173056 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/all.py
--rw-r--r--   0        0        0    64535 2023-05-20 17:34:01.173056 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/bad_request_400.py
--rw-r--r--   0        0        0     1941 2023-05-20 17:34:01.165055 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/flood_420.py
--rw-r--r--   0        0        0     6046 2023-05-20 17:34:01.165055 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/forbidden_403.py
--rw-r--r--   0        0        0    10644 2023-05-20 17:34:01.165055 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/internal_server_error_500.py
--rw-r--r--   0        0        0     3580 2023-05-20 17:34:01.169056 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/not_acceptable_406.py
--rw-r--r--   0        0        0     1952 2023-05-20 17:34:01.165055 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/see_other_303.py
--rw-r--r--   0        0        0     1351 2023-05-20 17:34:01.165055 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/service_unavailable_503.py
--rw-r--r--   0        0        0     2672 2023-05-20 17:34:01.165055 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/unauthorized_401.py
--rw-r--r--   0        0        0     3315 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0    15154 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/file_id.py
--rw-r--r--   0        0        0    24836 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/filters.py
--rw-r--r--   0        0        0     1475 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2101 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2543 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1550 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1935 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     1914 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1989 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1365 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      988 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3133 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4560 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8164 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1655 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1468 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1942 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1749 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1664 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1831 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2150 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2786 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3085 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2723 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2355 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     1859 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2041 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3311 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     4990 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1989 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2051 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2319 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2798 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3365 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     2847 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     4191 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     2886 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3186 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2048 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     3946 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0     4299 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     3364 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2216 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     4620 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     1848 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0        0        0     1711 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0        0        0     1817 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2333 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0        0        0     2281 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     1955 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1585 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2307 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1943 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0        0        0     1603 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     1969 2023-05-20 17:33:19.931598 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     2177 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0        0        0     1830 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0        0        0     3282 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4032 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3338 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5282 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2264 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1723 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3360 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2096 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2285 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0        0        0     3145 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0        0        0     2401 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2136 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     1715 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0        0        0     2694 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2605 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1528 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3157 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3925 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     1853 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0        0        0     1734 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0        0        0     4381 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     3136 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2247 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     3484 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4601 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1727 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2572 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2296 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     1982 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2083 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2230 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2305 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     1724 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2139 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1154 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2566 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2448 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1605 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1422 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1934 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1624 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2169 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2190 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2217 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2183 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1553 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2172 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2167 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2138 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2120 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1818 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2154 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2435 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1894 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1924 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3369 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1895 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1925 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2031 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1751 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3533 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2582 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3566 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2335 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     1997 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1925 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2928 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1929 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     2947 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2329 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     3921 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     5963 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     5423 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     3148 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     7530 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     2271 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10375 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2464 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     3115 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     2978 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    13022 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     2976 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     3906 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     5018 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     4501 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2389 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     1980 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2229 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2808 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     1950 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2946 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     4741 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2175 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2527 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2124 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4160 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2156 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5349 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3203 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    12828 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    11362 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     5723 2023-05-20 17:33:19.935600 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     3076 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     5111 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     5085 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    10712 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     4820 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    20821 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0     7509 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0     9682 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0     8315 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0     2361 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0        0        0     8582 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     5641 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    12198 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0     9556 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0     9672 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     2819 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3937 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2504 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1088 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2797 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3006 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2143 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0     1049 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2819 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0        0        0     4292 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0        0        0     1752 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/get_sticker_set.py
--rw-r--r--   0        0        0     1659 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     1771 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     2237 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     4421 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2509 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2359 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1664 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1565 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2562 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1882 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2718 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1876 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     1781 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2376 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1253 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2346 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2232 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1557 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2750 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2210 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2294 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2857 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2117 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1724 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0    61915 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/mime_types.py
--rw-r--r--   0        0        0      846 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     8681 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/html.py
--rw-r--r--   0        0        0     5770 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2077 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1545 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/py.typed
--rw-r--r--   0        0        0     1040 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0   105239 2023-05-20 17:34:01.133055 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/all.py
--rw-r--r--   0        0        0    14050 2023-05-20 17:34:01.113054 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/__init__.py
--rw-r--r--   0        0        0     1934 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/access_point_rule.py
--rw-r--r--   0        0        0     2134 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/account_days_ttl.py
--rw-r--r--   0        0        0     2158 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/app_web_view_result.py
--rw-r--r--   0        0        0     1922 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bot.py
--rw-r--r--   0        0        0     1947 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bot_icon.py
--rw-r--r--   0        0        0     1978 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bot_icon_color.py
--rw-r--r--   0        0        0     2215 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bots.py
--rw-r--r--   0        0        0     2157 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bots_bot.py
--rw-r--r--   0        0        0     2256 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_peer_type.py
--rw-r--r--   0        0        0     2126 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/authorization.py
--rw-r--r--   0        0        0     1964 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/auto_download_settings.py
--rw-r--r--   0        0        0     1946 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/auto_save_exception.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/auto_save_settings.py
--rw-r--r--   0        0        0     1945 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/available_reaction.py
--rw-r--r--   0        0        0     2004 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bad_msg_notification.py
--rw-r--r--   0        0        0     1935 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bank_card_open_url.py
--rw-r--r--   0        0        0     2124 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/base_theme.py
--rw-r--r--   0        0        0     1941 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bind_auth_key_inner.py
--rw-r--r--   0        0        0     1939 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_app.py
--rw-r--r--   0        0        0     2107 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_command.py
--rw-r--r--   0        0        0     2363 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_command_scope.py
--rw-r--r--   0        0        0     1885 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_info.py
--rw-r--r--   0        0        0     2336 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_inline_message.py
--rw-r--r--   0        0        0     2000 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_inline_result.py
--rw-r--r--   0        0        0     2261 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_menu_button.py
--rw-r--r--   0        0        0     2099 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/cdn_config.py
--rw-r--r--   0        0        0     1916 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/cdn_public_key.py
--rw-r--r--   0        0        0     1965 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/channel_admin_log_event.py
--rw-r--r--   0        0        0     6564 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/channel_admin_log_event_action.py
--rw-r--r--   0        0        0     2008 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/channel_admin_log_events_filter.py
--rw-r--r--   0        0        0     1999 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/channel_location.py
--rw-r--r--   0        0        0     2048 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/channel_messages_filter.py
--rw-r--r--   0        0        0     2309 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/channel_participant.py
--rw-r--r--   0        0        0     2524 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/channel_participants_filter.py
--rw-r--r--   0        0        0     2057 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat.py
--rw-r--r--   0        0        0     1934 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_admin_rights.py
--rw-r--r--   0        0        0     1965 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_admin_with_invites.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_banned_rights.py
--rw-r--r--   0        0        0     1939 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_full.py
--rw-r--r--   0        0        0     2225 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_invite.py
--rw-r--r--   0        0        0     1952 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_invite_importer.py
--rw-r--r--   0        0        0     2113 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_onlines.py
--rw-r--r--   0        0        0     2068 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_participant.py
--rw-r--r--   0        0        0     2015 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_participants.py
--rw-r--r--   0        0        0     1951 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_photo.py
--rw-r--r--   0        0        0     2046 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_reactions.py
--rw-r--r--   0        0        0     1947 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/client_dh_inner_data.py
--rw-r--r--   0        0        0     1915 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/code_settings.py
--rw-r--r--   0        0        0     2077 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/config.py
--rw-r--r--   0        0        0     1884 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/contact.py
--rw-r--r--   0        0        0     2126 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/contact_status.py
--rw-r--r--   0        0        0     2131 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/data_json.py
--rw-r--r--   0        0        0     1891 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/dc_option.py
--rw-r--r--   0        0        0     2160 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/default_history_ttl.py
--rw-r--r--   0        0        0     2267 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/destroy_auth_key_res.py
--rw-r--r--   0        0        0     2205 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/destroy_session_res.py
--rw-r--r--   0        0        0     1928 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/dialog.py
--rw-r--r--   0        0        0     2254 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/dialog_filter.py
--rw-r--r--   0        0        0     2189 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/dialog_filter_suggested.py
--rw-r--r--   0        0        0     2175 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/dialog_peer.py
--rw-r--r--   0        0        0     2266 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/document.py
--rw-r--r--   0        0        0     2487 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/document_attribute.py
--rw-r--r--   0        0        0     1975 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/draft_message.py
--rw-r--r--   0        0        0     2094 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/email_verification.py
--rw-r--r--   0        0        0     2133 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/email_verify_purpose.py
--rw-r--r--   0        0        0     1903 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_group.py
--rw-r--r--   0        0        0     1979 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_keyword.py
--rw-r--r--   0        0        0     2241 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_keywords_difference.py
--rw-r--r--   0        0        0     2140 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_language.py
--rw-r--r--   0        0        0     2271 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_list.py
--rw-r--r--   0        0        0     2024 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_status.py
--rw-r--r--   0        0        0     2096 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_url.py
--rw-r--r--   0        0        0     2436 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/encrypted_chat.py
--rw-r--r--   0        0        0     2196 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/encrypted_file.py
--rw-r--r--   0        0        0     2011 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/encrypted_message.py
--rw-r--r--   0        0        0     1872 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/error.py
--rw-r--r--   0        0        0     2244 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/exported_chat_invite.py
--rw-r--r--   0        0        0     2189 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/exported_chatlist_invite.py
--rw-r--r--   0        0        0     2176 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/exported_contact_token.py
--rw-r--r--   0        0        0     2169 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/exported_message_link.py
--rw-r--r--   0        0        0     2168 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/file_hash.py
--rw-r--r--   0        0        0     1878 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/folder.py
--rw-r--r--   0        0        0     1903 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/folder_peer.py
--rw-r--r--   0        0        0     1963 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/forum_topic.py
--rw-r--r--   0        0        0     1866 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/game.py
--rw-r--r--   0        0        0     1943 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/geo_point.py
--rw-r--r--   0        0        0     2233 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/global_privacy_settings.py
--rw-r--r--   0        0        0     1959 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/group_call.py
--rw-r--r--   0        0        0     1964 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/group_call_participant.py
--rw-r--r--   0        0        0     1995 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/group_call_participant_video.py
--rw-r--r--   0        0        0     2063 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/group_call_participant_video_source_group.py
--rw-r--r--   0        0        0     1977 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/group_call_stream_channel.py
--rw-r--r--   0        0        0     1897 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/high_score.py
--rw-r--r--   0        0        0     1891 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/http_wait.py
--rw-r--r--   0        0        0     1933 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/imported_contact.py
--rw-r--r--   0        0        0     1947 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/inline_bot_switch_pm.py
--rw-r--r--   0        0        0     1941 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/inline_bot_web_view.py
--rw-r--r--   0        0        0     2351 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/inline_query_peer_type.py
--rw-r--r--   0        0        0     1922 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_app_event.py
--rw-r--r--   0        0        0     1980 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_bot_app.py
--rw-r--r--   0        0        0     2492 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_bot_inline_message.py
--rw-r--r--   0        0        0     2060 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_bot_inline_message_id.py
--rw-r--r--   0        0        0     2195 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_bot_inline_result.py
--rw-r--r--   0        0        0     2046 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_channel.py
--rw-r--r--   0        0        0     2061 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_chat_photo.py
--rw-r--r--   0        0        0     1945 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_chatlist.py
--rw-r--r--   0        0        0     2043 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_check_password_srp.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_client_proxy.py
--rw-r--r--   0        0        0     1925 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_contact.py
--rw-r--r--   0        0        0     2002 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_dialog_peer.py
--rw-r--r--   0        0        0     1983 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_document.py
--rw-r--r--   0        0        0     1952 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_encrypted_chat.py
--rw-r--r--   0        0        0     2184 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_encrypted_file.py
--rw-r--r--   0        0        0     1947 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_file.py
--rw-r--r--   0        0        0     2601 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_file_location.py
--rw-r--r--   0        0        0     1934 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_folder_peer.py
--rw-r--r--   0        0        0     1963 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_game.py
--rw-r--r--   0        0        0     1984 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_geo_point.py
--rw-r--r--   0        0        0     1928 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_group_call.py
--rw-r--r--   0        0        0     1987 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_invoice.py
--rw-r--r--   0        0        0     2779 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_media.py
--rw-r--r--   0        0        0     2119 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_message.py
--rw-r--r--   0        0        0     2183 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_notify_peer.py
--rw-r--r--   0        0        0     2240 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_payment_credentials.py
--rw-r--r--   0        0        0     2270 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_peer.py
--rw-r--r--   0        0        0     1983 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_peer_notify_settings.py
--rw-r--r--   0        0        0     1928 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_phone_call.py
--rw-r--r--   0        0        0     1959 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_photo.py
--rw-r--r--   0        0        0     2571 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_privacy_key.py
--rw-r--r--   0        0        0     2588 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_privacy_rule.py
--rw-r--r--   0        0        0     2006 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_secure_file.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_secure_value.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_single_media.py
--rw-r--r--   0        0        0     2695 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_sticker_set.py
--rw-r--r--   0        0        0     1959 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_sticker_set_item.py
--rw-r--r--   0        0        0     2048 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_stickered_media.py
--rw-r--r--   0        0        0     2095 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_store_payment_purpose.py
--rw-r--r--   0        0        0     1957 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_theme.py
--rw-r--r--   0        0        0     1952 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_theme_settings.py
--rw-r--r--   0        0        0     2067 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_user.py
--rw-r--r--   0        0        0     2055 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_wall_paper.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_web_document.py
--rw-r--r--   0        0        0     2142 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_web_file_location.py
--rw-r--r--   0        0        0     1884 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/invoice.py
--rw-r--r--   0        0        0     1929 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/ip_port.py
--rw-r--r--   0        0        0     1934 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/json_object_value.py
--rw-r--r--   0        0        0     2115 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/json_value.py
--rw-r--r--   0        0        0     3020 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/keyboard_button.py
--rw-r--r--   0        0        0     1946 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/keyboard_button_row.py
--rw-r--r--   0        0        0     1915 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/labeled_price.py
--rw-r--r--   0        0        0     2193 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/lang_pack_difference.py
--rw-r--r--   0        0        0     2180 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/lang_pack_language.py
--rw-r--r--   0        0        0     2273 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/lang_pack_string.py
--rw-r--r--   0        0        0     1903 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/mask_coords.py
--rw-r--r--   0        0        0     1987 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message.py
--rw-r--r--   0        0        0     4917 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_action.py
--rw-r--r--   0        0        0     3249 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_entity.py
--rw-r--r--   0        0        0     2044 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_extended_media.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_fwd_header.py
--rw-r--r--   0        0        0     2000 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_interaction_counters.py
--rw-r--r--   0        0        0     2945 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_media.py
--rw-r--r--   0        0        0     1958 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_peer_reaction.py
--rw-r--r--   0        0        0     2123 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_range.py
--rw-r--r--   0        0        0     1939 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_reactions.py
--rw-r--r--   0        0        0     1927 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_replies.py
--rw-r--r--   0        0        0     1952 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_reply_header.py
--rw-r--r--   0        0        0     2083 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_user_vote.py
--rw-r--r--   0        0        0     1915 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_views.py
--rw-r--r--   0        0        0     3181 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/messages_filter.py
--rw-r--r--   0        0        0     1996 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/msg_detailed_info.py
--rw-r--r--   0        0        0     1972 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/msg_resend_req.py
--rw-r--r--   0        0        0     1885 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/msgs_ack.py
--rw-r--r--   0        0        0     1910 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/msgs_all_info.py
--rw-r--r--   0        0        0     1922 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/msgs_state_info.py
--rw-r--r--   0        0        0     1916 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/msgs_state_req.py
--rw-r--r--   0        0        0     2099 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/nearest_dc.py
--rw-r--r--   0        0        0     1917 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/new_session.py
--rw-r--r--   0        0        0     2171 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/notification_sound.py
--rw-r--r--   0        0        0     2112 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/notify_peer.py
--rw-r--r--   0        0        0     1866 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/null.py
--rw-r--r--   0        0        0     1866 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page.py
--rw-r--r--   0        0        0     3535 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page_block.py
--rw-r--r--   0        0        0     1909 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page_caption.py
--rw-r--r--   0        0        0     1986 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page_list_item.py
--rw-r--r--   0        0        0     2043 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page_list_ordered_item.py
--rw-r--r--   0        0        0     1952 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page_related_article.py
--rw-r--r--   0        0        0     1922 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page_table_cell.py
--rw-r--r--   0        0        0     1916 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page_table_row.py
--rw-r--r--   0        0        0     2104 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/password_kdf_algo.py
--rw-r--r--   0        0        0     1921 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/payment_charge.py
--rw-r--r--   0        0        0     1946 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/payment_form_method.py
--rw-r--r--   0        0        0     1964 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/payment_requested_info.py
--rw-r--r--   0        0        0     1990 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/payment_saved_credentials.py
--rw-r--r--   0        0        0     2185 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/peer.py
--rw-r--r--   0        0        0     1909 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/peer_blocked.py
--rw-r--r--   0        0        0     1965 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/peer_located.py
--rw-r--r--   0        0        0     2162 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/peer_notify_settings.py
--rw-r--r--   0        0        0     1915 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/peer_settings.py
--rw-r--r--   0        0        0     2189 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/phone_call.py
--rw-r--r--   0        0        0     2237 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/phone_call_discard_reason.py
--rw-r--r--   0        0        0     1946 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/phone_call_protocol.py
--rw-r--r--   0        0        0     2001 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/phone_connection.py
--rw-r--r--   0        0        0     1918 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/photo.py
--rw-r--r--   0        0        0     2181 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/photo_size.py
--rw-r--r--   0        0        0     1866 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/poll.py
--rw-r--r--   0        0        0     1903 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/poll_answer.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/poll_answer_voters.py
--rw-r--r--   0        0        0     1909 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/poll_results.py
--rw-r--r--   0        0        0     2088 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/pong.py
--rw-r--r--   0        0        0     1927 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/popular_contact.py
--rw-r--r--   0        0        0     1909 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/post_address.py
--rw-r--r--   0        0        0     2076 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/pq_inner_data.py
--rw-r--r--   0        0        0     1946 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/premium_gift_option.py
--rw-r--r--   0        0        0     1994 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/premium_subscription_option.py
--rw-r--r--   0        0        0     2460 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/privacy_key.py
--rw-r--r--   0        0        0     2487 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/privacy_rule.py
--rw-r--r--   0        0        0     2015 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/reaction.py
--rw-r--r--   0        0        0     1921 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/reaction_count.py
--rw-r--r--   0        0        0     2178 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/read_participant_date.py
--rw-r--r--   0        0        0     2180 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/received_notify_message.py
--rw-r--r--   0        0        0     2169 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/recent_me_url.py
--rw-r--r--   0        0        0     2115 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/reply_markup.py
--rw-r--r--   0        0        0     2640 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/report_reason.py
--rw-r--r--   0        0        0     2079 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/request_peer_type.py
--rw-r--r--   0        0        0     2087 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/res_pq.py
--rw-r--r--   0        0        0     1945 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/restriction_reason.py
--rw-r--r--   0        0        0     2572 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/rich_text.py
--rw-r--r--   0        0        0     2255 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/rpc_drop_answer.py
--rw-r--r--   0        0        0     1891 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/rpc_error.py
--rw-r--r--   0        0        0     1897 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/rpc_result.py
--rw-r--r--   0        0        0     2127 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/saved_contact.py
--rw-r--r--   0        0        0     2007 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/search_results_calendar_period.py
--rw-r--r--   0        0        0     1968 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/search_results_position.py
--rw-r--r--   0        0        0     2000 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_credentials_encrypted.py
--rw-r--r--   0        0        0     1903 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_data.py
--rw-r--r--   0        0        0     1959 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_file.py
--rw-r--r--   0        0        0     2184 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_password_kdf_algo.py
--rw-r--r--   0        0        0     1994 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_plain_data.py
--rw-r--r--   0        0        0     2024 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_required_type.py
--rw-r--r--   0        0        0     1964 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_secret_settings.py
--rw-r--r--   0        0        0     2192 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_value.py
--rw-r--r--   0        0        0     2537 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_value_error.py
--rw-r--r--   0        0        0     1934 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_value_hash.py
--rw-r--r--   0        0        0     2918 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_value_type.py
--rw-r--r--   0        0        0     1904 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/send_as_peer.py
--rw-r--r--   0        0        0     3337 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/send_message_action.py
--rw-r--r--   0        0        0     1947 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/server_dh_inner_data.py
--rw-r--r--   0        0        0     2190 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/server_dh_params.py
--rw-r--r--   0        0        0     2243 2023-05-20 17:34:00.837048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/set_client_dh_params_answer.py
--rw-r--r--   0        0        0     1927 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/shipping_option.py
--rw-r--r--   0        0        0     2179 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/simple_web_view_result.py
--rw-r--r--   0        0        0     1939 2023-05-20 17:34:00.873049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/sponsored_message.py
--rw-r--r--   0        0        0     1966 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_abs_value_and_prev.py
--rw-r--r--   0        0        0     1953 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_date_range_days.py
--rw-r--r--   0        0        0     2219 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_graph.py
--rw-r--r--   0        0        0     1953 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_group_top_admin.py
--rw-r--r--   0        0        0     1965 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_group_top_inviter.py
--rw-r--r--   0        0        0     1959 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_group_top_poster.py
--rw-r--r--   0        0        0     1946 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_percent_value.py
--rw-r--r--   0        0        0     1891 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/stats_url.py
--rw-r--r--   0        0        0     1927 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/sticker_keyword.py
--rw-r--r--   0        0        0     1909 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/sticker_pack.py
--rw-r--r--   0        0        0     1903 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/sticker_set.py
--rw-r--r--   0        0        0     2359 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/sticker_set_covered.py
--rw-r--r--   0        0        0     1940 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/text_with_entities.py
--rw-r--r--   0        0        0     2138 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/theme.py
--rw-r--r--   0        0        0     1921 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/theme_settings.py
--rw-r--r--   0        0        0     1885 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/top_peer.py
--rw-r--r--   0        0        0     2476 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/top_peer_category.py
--rw-r--r--   0        0        0     1965 2023-05-20 17:34:00.853048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/top_peer_category_peers.py
--rw-r--r--   0        0        0     9329 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/update.py
--rw-r--r--   0        0        0     5681 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/updates_t.py
--rw-r--r--   0        0        0     2313 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/url_auth_result.py
--rw-r--r--   0        0        0     2251 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/user.py
--rw-r--r--   0        0        0     1891 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/user_full.py
--rw-r--r--   0        0        0     2008 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/user_profile_photo.py
--rw-r--r--   0        0        0     2215 2023-05-20 17:34:00.841048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/user_status.py
--rw-r--r--   0        0        0     1890 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/username.py
--rw-r--r--   0        0        0     2032 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/video_size.py
--rw-r--r--   0        0        0     2234 2023-05-20 17:34:00.845048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/wall_paper.py
--rw-r--r--   0        0        0     1946 2023-05-20 17:34:00.865049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/wall_paper_settings.py
--rw-r--r--   0        0        0     1939 2023-05-20 17:34:00.861049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/web_authorization.py
--rw-r--r--   0        0        0     1971 2023-05-20 17:34:00.857048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/web_document.py
--rw-r--r--   0        0        0     2253 2023-05-20 17:34:00.849048 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/web_page.py
--rw-r--r--   0        0        0     1950 2023-05-20 17:34:00.869049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/web_page_attribute.py
--rw-r--r--   0        0        0     2171 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/web_view_message_sent.py
--rw-r--r--   0        0        0     2136 2023-05-20 17:34:00.877049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/web_view_result.py
--rw-r--r--   0        0        0     1312 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1814 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1048 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     1012 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1759 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2022 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0     2495 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1998 2023-05-20 17:34:01.125054 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/__init__.py
--rw-r--r--   0        0        0     2010 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/destroy_auth_key.py
--rw-r--r--   0        0        0     2211 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/destroy_session.py
--rw-r--r--   0        0        0     2133 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/get_future_salts.py
--rw-r--r--   0        0        0     4863 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/init_connection.py
--rw-r--r--   0        0        0     2397 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/invoke_after_msg.py
--rw-r--r--   0        0        0     2450 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/invoke_after_msgs.py
--rw-r--r--   0        0        0     2389 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/invoke_with_layer.py
--rw-r--r--   0        0        0     2492 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/invoke_with_messages_range.py
--rw-r--r--   0        0        0     2445 2023-05-20 17:34:01.045053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/invoke_with_takeout.py
--rw-r--r--   0        0        0     2209 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/invoke_without_updates.py
--rw-r--r--   0        0        0     2118 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/ping.py
--rw-r--r--   0        0        0     2477 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/ping_delay_disconnect.py
--rw-r--r--   0        0        0     3390 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/req_dh_params.py
--rw-r--r--   0        0        0     2113 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/req_pq.py
--rw-r--r--   0        0        0     2133 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/req_pq_multi.py
--rw-r--r--   0        0        0     2199 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/rpc_drop_answer.py
--rw-r--r--   0        0        0     2750 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/set_client_dh_params.py
--rw-r--r--   0        0        0    56200 2023-05-20 17:34:01.121054 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/access_point_rule.py
--rw-r--r--   0        0        0     2329 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/account_days_ttl.py
--rw-r--r--   0        0        0     2345 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/app_web_view_result_url.py
--rw-r--r--   0        0        0     4075 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_bot.py
--rw-r--r--   0        0        0     2923 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_bot_icon.py
--rw-r--r--   0        0        0     2362 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_bot_icon_color.py
--rw-r--r--   0        0        0     2886 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_bots.py
--rw-r--r--   0        0        0     2675 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_bots_bot.py
--rw-r--r--   0        0        0     2234 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_bots_not_modified.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_peer_type_bot_pm.py
--rw-r--r--   0        0        0     2036 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_peer_type_broadcast.py
--rw-r--r--   0        0        0     2014 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_peer_type_chat.py
--rw-r--r--   0        0        0     2008 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_peer_type_pm.py
--rw-r--r--   0        0        0     2036 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_peer_type_same_bot_pm.py
--rw-r--r--   0        0        0     6710 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/authorization.py
--rw-r--r--   0        0        0     4611 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/auto_download_settings.py
--rw-r--r--   0        0        0     2492 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/auto_save_exception.py
--rw-r--r--   0        0        0     2962 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/auto_save_settings.py
--rw-r--r--   0        0        0     5709 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/available_reaction.py
--rw-r--r--   0        0        0     2718 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bad_msg_notification.py
--rw-r--r--   0        0        0     2991 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bad_server_salt.py
--rw-r--r--   0        0        0     2307 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bank_card_open_url.py
--rw-r--r--   0        0        0     1979 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/base_theme_arctic.py
--rw-r--r--   0        0        0     1983 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/base_theme_classic.py
--rw-r--r--   0        0        0     1967 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/base_theme_day.py
--rw-r--r--   0        0        0     1975 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/base_theme_night.py
--rw-r--r--   0        0        0     1979 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/base_theme_tinted.py
--rw-r--r--   0        0        0     3288 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bind_auth_key_inner.py
--rw-r--r--   0        0        0     3944 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_app.py
--rw-r--r--   0        0        0     1984 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_app_not_modified.py
--rw-r--r--   0        0        0     2584 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command.py
--rw-r--r--   0        0        0     2025 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_chat_admins.py
--rw-r--r--   0        0        0     2005 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_chats.py
--rw-r--r--   0        0        0     2013 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_default.py
--rw-r--r--   0        0        0     2204 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_peer.py
--rw-r--r--   0        0        0     2228 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_peer_admins.py
--rw-r--r--   0        0        0     2495 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_peer_user.py
--rw-r--r--   0        0        0     2005 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_users.py
--rw-r--r--   0        0        0     4814 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_info.py
--rw-r--r--   0        0        0     4328 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_media_result.py
--rw-r--r--   0        0        0     3220 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_media_auto.py
--rw-r--r--   0        0        0     3471 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_media_contact.py
--rw-r--r--   0        0        0     4119 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_media_geo.py
--rw-r--r--   0        0        0     4576 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_media_invoice.py
--rw-r--r--   0        0        0     3871 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_media_venue.py
--rw-r--r--   0        0        0     3494 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_text.py
--rw-r--r--   0        0        0     4665 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_result.py
--rw-r--r--   0        0        0     2502 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_menu_button.py
--rw-r--r--   0        0        0     2212 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_menu_button_commands.py
--rw-r--r--   0        0        0     2208 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_menu_button_default.py
--rw-r--r--   0        0        0     2456 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/cdn_config.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/cdn_public_key.py
--rw-r--r--   0        0        0    12591 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel.py
--rw-r--r--   0        0        0     2887 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event.py
--rw-r--r--   0        0        0     2514 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_about.py
--rw-r--r--   0        0        0     2720 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_available_reactions.py
--rw-r--r--   0        0        0     2538 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_history_ttl.py
--rw-r--r--   0        0        0     2542 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_linked_chat.py
--rw-r--r--   0        0        0     2694 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_location.py
--rw-r--r--   0        0        0     2604 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_photo.py
--rw-r--r--   0        0        0     2794 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_sticker_set.py
--rw-r--r--   0        0        0     2514 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_title.py
--rw-r--r--   0        0        0     2526 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_username.py
--rw-r--r--   0        0        0     2610 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_change_usernames.py
--rw-r--r--   0        0        0     2300 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_create_topic.py
--rw-r--r--   0        0        0     2868 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_default_banned_rights.py
--rw-r--r--   0        0        0     2314 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_delete_message.py
--rw-r--r--   0        0        0     2300 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_delete_topic.py
--rw-r--r--   0        0        0     2327 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_discard_group_call.py
--rw-r--r--   0        0        0     2656 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_edit_message.py
--rw-r--r--   0        0        0     2636 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_edit_topic.py
--rw-r--r--   0        0        0     2377 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_delete.py
--rw-r--r--   0        0        0     2754 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_edit.py
--rw-r--r--   0        0        0     2377 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_revoke.py
--rw-r--r--   0        0        0     2410 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_invite.py
--rw-r--r--   0        0        0     2100 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_join.py
--rw-r--r--   0        0        0     2746 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_invite.py
--rw-r--r--   0        0        0     2650 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_request.py
--rw-r--r--   0        0        0     2104 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_leave.py
--rw-r--r--   0        0        0     2410 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_mute.py
--rw-r--r--   0        0        0     2860 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_admin.py
--rw-r--r--   0        0        0     2852 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_ban.py
--rw-r--r--   0        0        0     2418 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_unmute.py
--rw-r--r--   0        0        0     2418 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_participant_volume.py
--rw-r--r--   0        0        0     3005 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_pin_topic.py
--rw-r--r--   0        0        0     2306 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_send_message.py
--rw-r--r--   0        0        0     2319 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_start_group_call.py
--rw-r--r--   0        0        0     2294 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_stop_poll.py
--rw-r--r--   0        0        0     2279 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_anti_spam.py
--rw-r--r--   0        0        0     2265 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_forum.py
--rw-r--r--   0        0        0     2320 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_group_call_setting.py
--rw-r--r--   0        0        0     2275 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_invites.py
--rw-r--r--   0        0        0     2287 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_no_forwards.py
--rw-r--r--   0        0        0     2311 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_pre_history_hidden.py
--rw-r--r--   0        0        0     2287 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_signatures.py
--rw-r--r--   0        0        0     2530 2023-05-20 17:34:00.993051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_toggle_slow_mode.py
--rw-r--r--   0        0        0     2310 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_update_pinned.py
--rw-r--r--   0        0        0     6648 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_events_filter.py
--rw-r--r--   0        0        0     3591 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_forbidden.py
--rw-r--r--   0        0        0    21188 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_full.py
--rw-r--r--   0        0        0     2445 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_location.py
--rw-r--r--   0        0        0     2005 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_location_empty.py
--rw-r--r--   0        0        0     2699 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_messages_filter.py
--rw-r--r--   0        0        0     2035 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_messages_filter_empty.py
--rw-r--r--   0        0        0     2365 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participant.py
--rw-r--r--   0        0        0     4333 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participant_admin.py
--rw-r--r--   0        0        0     3281 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participant_banned.py
--rw-r--r--   0        0        0     2936 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participant_creator.py
--rw-r--r--   0        0        0     2199 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participant_left.py
--rw-r--r--   0        0        0     2977 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participant_self.py
--rw-r--r--   0        0        0     2035 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_admins.py
--rw-r--r--   0        0        0     2150 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_banned.py
--rw-r--r--   0        0        0     2027 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_bots.py
--rw-r--r--   0        0        0     2158 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_contacts.py
--rw-r--r--   0        0        0     2150 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_kicked.py
--rw-r--r--   0        0        0     2762 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_mentions.py
--rw-r--r--   0        0        0     2035 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_recent.py
--rw-r--r--   0        0        0     2148 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_search.py
--rw-r--r--   0        0        0     6664 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat.py
--rw-r--r--   0        0        0     5640 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_admin_rights.py
--rw-r--r--   0        0        0     2809 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_admin_with_invites.py
--rw-r--r--   0        0        0     8389 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_banned_rights.py
--rw-r--r--   0        0        0     2079 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_empty.py
--rw-r--r--   0        0        0     2293 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_forbidden.py
--rw-r--r--   0        0        0     9951 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_full.py
--rw-r--r--   0        0        0     5192 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_invite.py
--rw-r--r--   0        0        0     2379 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_invite_already.py
--rw-r--r--   0        0        0     6062 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_invite_exported.py
--rw-r--r--   0        0        0     3786 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_invite_importer.py
--rw-r--r--   0        0        0     2585 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_invite_peek.py
--rw-r--r--   0        0        0     2249 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_invite_public_join_requests.py
--rw-r--r--   0        0        0     2339 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_onlines.py
--rw-r--r--   0        0        0     2598 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_participant.py
--rw-r--r--   0        0        0     2618 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_participant_admin.py
--rw-r--r--   0        0        0     2187 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_participant_creator.py
--rw-r--r--   0        0        0     2750 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_participants.py
--rw-r--r--   0        0        0     2804 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_participants_forbidden.py
--rw-r--r--   0        0        0     3122 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_photo.py
--rw-r--r--   0        0        0     1975 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_photo_empty.py
--rw-r--r--   0        0        0     2297 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_reactions_all.py
--rw-r--r--   0        0        0     1991 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_reactions_none.py
--rw-r--r--   0        0        0     2257 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_reactions_some.py
--rw-r--r--   0        0        0     2842 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/client_dh_inner_data.py
--rw-r--r--   0        0        0     4902 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/code_settings.py
--rw-r--r--   0        0        0    19235 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/config.py
--rw-r--r--   0        0        0     2322 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/contact.py
--rw-r--r--   0        0        0     2625 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/contact_status.py
--rw-r--r--   0        0        0     2331 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/data_json.py
--rw-r--r--   0        0        0     4562 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dc_option.py
--rw-r--r--   0        0        0     2370 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/default_history_ttl.py
--rw-r--r--   0        0        0     2197 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/destroy_auth_key_fail.py
--rw-r--r--   0        0        0     2197 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/destroy_auth_key_none.py
--rw-r--r--   0        0        0     2189 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/destroy_auth_key_ok.py
--rw-r--r--   0        0        0     2398 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/destroy_session_none.py
--rw-r--r--   0        0        0     2390 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/destroy_session_ok.py
--rw-r--r--   0        0        0     2906 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dh_gen_fail.py
--rw-r--r--   0        0        0     2898 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dh_gen_ok.py
--rw-r--r--   0        0        0     2910 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dh_gen_retry.py
--rw-r--r--   0        0        0     6524 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog.py
--rw-r--r--   0        0        0     6358 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog_filter.py
--rw-r--r--   0        0        0     4000 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog_filter_chatlist.py
--rw-r--r--   0        0        0     2207 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog_filter_default.py
--rw-r--r--   0        0        0     2718 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog_filter_suggested.py
--rw-r--r--   0        0        0     4534 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog_folder.py
--rw-r--r--   0        0        0     2356 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog_peer.py
--rw-r--r--   0        0        0     2386 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/dialog_peer_folder.py
--rw-r--r--   0        0        0     5113 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document.py
--rw-r--r--   0        0        0     2027 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_animated.py
--rw-r--r--   0        0        0     3632 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_audio.py
--rw-r--r--   0        0        0     3079 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_custom_emoji.py
--rw-r--r--   0        0        0     2214 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_filename.py
--rw-r--r--   0        0        0     2039 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_has_stickers.py
--rw-r--r--   0        0        0     2312 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_image_size.py
--rw-r--r--   0        0        0     3253 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_sticker.py
--rw-r--r--   0        0        0     3253 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_attribute_video.py
--rw-r--r--   0        0        0     2422 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/document_empty.py
--rw-r--r--   0        0        0     3616 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/draft_message.py
--rw-r--r--   0        0        0     2333 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/draft_message_empty.py
--rw-r--r--   0        0        0     2166 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/email_verification_apple.py
--rw-r--r--   0        0        0     2153 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/email_verification_code.py
--rw-r--r--   0        0        0     2170 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/email_verification_google.py
--rw-r--r--   0        0        0     2044 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/email_verify_purpose_login_change.py
--rw-r--r--   0        0        0     2542 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/email_verify_purpose_login_setup.py
--rw-r--r--   0        0        0     2032 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/email_verify_purpose_passport.py
--rw-r--r--   0        0        0     2660 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_group.py
--rw-r--r--   0        0        0     2413 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_keyword.py
--rw-r--r--   0        0        0     2441 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_keyword_deleted.py
--rw-r--r--   0        0        0     3271 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_keywords_difference.py
--rw-r--r--   0        0        0     2380 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_language.py
--rw-r--r--   0        0        0     2706 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_list.py
--rw-r--r--   0        0        0     2306 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_list_not_modified.py
--rw-r--r--   0        0        0     2175 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_status.py
--rw-r--r--   0        0        0     1985 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_status_empty.py
--rw-r--r--   0        0        0     2395 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_status_until.py
--rw-r--r--   0        0        0     2287 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_url.py
--rw-r--r--   0        0        0     3831 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_chat.py
--rw-r--r--   0        0        0     2770 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_chat_discarded.py
--rw-r--r--   0        0        0     2370 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_chat_empty.py
--rw-r--r--   0        0        0     3974 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_chat_requested.py
--rw-r--r--   0        0        0     3340 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_chat_waiting.py
--rw-r--r--   0        0        0     3257 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_file.py
--rw-r--r--   0        0        0     2207 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_file_empty.py
--rw-r--r--   0        0        0     3056 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_message.py
--rw-r--r--   0        0        0     2818 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_message_service.py
--rw-r--r--   0        0        0     2268 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/error.py
--rw-r--r--   0        0        0     2876 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/exported_chatlist_invite.py
--rw-r--r--   0        0        0     2572 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/exported_contact_token.py
--rw-r--r--   0        0        0     2546 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/exported_message_link.py
--rw-r--r--   0        0        0     2781 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/file_hash.py
--rw-r--r--   0        0        0     3983 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/folder.py
--rw-r--r--   0        0        0     2379 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/folder_peer.py
--rw-r--r--   0        0        0     7364 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/forum_topic.py
--rw-r--r--   0        0        0     2112 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/forum_topic_deleted.py
--rw-r--r--   0        0        0     3740 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/game.py
--rw-r--r--   0        0        0     3070 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/geo_point.py
--rw-r--r--   0        0        0     1970 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/geo_point_empty.py
--rw-r--r--   0        0        0     2977 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/global_privacy_settings.py
--rw-r--r--   0        0        0     8290 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/group_call.py
--rw-r--r--   0        0        0     2604 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/group_call_discarded.py
--rw-r--r--   0        0        0     8200 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/group_call_participant.py
--rw-r--r--   0        0        0     3410 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/group_call_participant_video.py
--rw-r--r--   0        0        0     2535 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/group_call_participant_video_source_group.py
--rw-r--r--   0        0        0     2702 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/group_call_stream_channel.py
--rw-r--r--   0        0        0     2511 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/high_score.py
--rw-r--r--   0        0        0     2611 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/http_wait.py
--rw-r--r--   0        0        0     2398 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/imported_contact.py
--rw-r--r--   0        0        0     2389 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_bot_switch_pm.py
--rw-r--r--   0        0        0     2312 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_bot_web_view.py
--rw-r--r--   0        0        0     2023 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_query_peer_type_bot_pm.py
--rw-r--r--   0        0        0     2041 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_query_peer_type_broadcast.py
--rw-r--r--   0        0        0     2021 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_query_peer_type_chat.py
--rw-r--r--   0        0        0     2041 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_query_peer_type_megagroup.py
--rw-r--r--   0        0        0     2013 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_query_peer_type_pm.py
--rw-r--r--   0        0        0     2041 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/inline_query_peer_type_same_bot_pm.py
--rw-r--r--   0        0        0     2765 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_app_event.py
--rw-r--r--   0        0        0     2359 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_app_id.py
--rw-r--r--   0        0        0     2465 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_app_short_name.py
--rw-r--r--   0        0        0     2528 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_game.py
--rw-r--r--   0        0        0     2611 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_id.py
--rw-r--r--   0        0        0     2846 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_id64.py
--rw-r--r--   0        0        0     3245 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_media_auto.py
--rw-r--r--   0        0        0     3496 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_media_contact.py
--rw-r--r--   0        0        0     4220 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_media_geo.py
--rw-r--r--   0        0        0     4490 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_media_invoice.py
--rw-r--r--   0        0        0     3970 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_media_venue.py
--rw-r--r--   0        0        0     3519 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_text.py
--rw-r--r--   0        0        0     4750 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_result.py
--rw-r--r--   0        0        0     3846 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_result_document.py
--rw-r--r--   0        0        0     2763 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_result_game.py
--rw-r--r--   0        0        0     2976 2023-05-20 17:34:00.965051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_result_photo.py
--rw-r--r--   0        0        0     2428 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_channel.py
--rw-r--r--   0        0        0     1990 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_channel_empty.py
--rw-r--r--   0        0        0     2674 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_channel_from_message.py
--rw-r--r--   0        0        0     2169 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_chat_photo.py
--rw-r--r--   0        0        0     2000 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_chat_photo_empty.py
--rw-r--r--   0        0        0     3852 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_chat_uploaded_photo.py
--rw-r--r--   0        0        0     2212 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_chatlist_dialog_filter.py
--rw-r--r--   0        0        0     2023 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_check_password_empty.py
--rw-r--r--   0        0        0     2515 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_check_password_srp.py
--rw-r--r--   0        0        0     2350 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_client_proxy.py
--rw-r--r--   0        0        0     2188 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_dialog_peer.py
--rw-r--r--   0        0        0     2198 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_dialog_peer_folder.py
--rw-r--r--   0        0        0     2641 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_document.py
--rw-r--r--   0        0        0     1995 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_document_empty.py
--rw-r--r--   0        0        0     2936 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_document_file_location.py
--rw-r--r--   0        0        0     2428 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_encrypted_chat.py
--rw-r--r--   0        0        0     2386 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_encrypted_file.py
--rw-r--r--   0        0        0     2663 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_encrypted_file_big_uploaded.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_encrypted_file_empty.py
--rw-r--r--   0        0        0     2417 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_encrypted_file_location.py
--rw-r--r--   0        0        0     2912 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_encrypted_file_uploaded.py
--rw-r--r--   0        0        0     2734 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_file.py
--rw-r--r--   0        0        0     2485 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_file_big.py
--rw-r--r--   0        0        0     2906 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_file_location.py
--rw-r--r--   0        0        0     2424 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_folder_peer.py
--rw-r--r--   0        0        0     2347 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_game_id.py
--rw-r--r--   0        0        0     2455 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_game_short_name.py
--rw-r--r--   0        0        0     2838 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_geo_point.py
--rw-r--r--   0        0        0     1995 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_geo_point_empty.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_group_call.py
--rw-r--r--   0        0        0     3582 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_group_call_stream.py
--rw-r--r--   0        0        0     2410 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_invoice_message.py
--rw-r--r--   0        0        0     2128 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_invoice_slug.py
--rw-r--r--   0        0        0     3407 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_keyboard_button_url_auth.py
--rw-r--r--   0        0        0     2463 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_keyboard_button_user_profile.py
--rw-r--r--   0        0        0     2877 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_contact.py
--rw-r--r--   0        0        0     2154 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_dice.py
--rw-r--r--   0        0        0     3281 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_document.py
--rw-r--r--   0        0        0     2891 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_document_external.py
--rw-r--r--   0        0        0     1980 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_empty.py
--rw-r--r--   0        0        0     2161 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_game.py
--rw-r--r--   0        0        0     3929 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_geo_live.py
--rw-r--r--   0        0        0     2256 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_geo_point.py
--rw-r--r--   0        0        0     4853 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_invoice.py
--rw-r--r--   0        0        0     2903 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_photo.py
--rw-r--r--   0        0        0     2879 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_photo_external.py
--rw-r--r--   0        0        0     3669 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_poll.py
--rw-r--r--   0        0        0     5063 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_uploaded_document.py
--rw-r--r--   0        0        0     3430 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_uploaded_photo.py
--rw-r--r--   0        0        0     3351 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_media_venue.py
--rw-r--r--   0        0        0     2378 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_message_callback_query.py
--rw-r--r--   0        0        0     2687 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_message_entity_mention_name.py
--rw-r--r--   0        0        0     2104 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_message_id.py
--rw-r--r--   0        0        0     1994 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_message_pinned.py
--rw-r--r--   0        0        0     2124 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_message_reply_to.py
--rw-r--r--   0        0        0     2040 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_chat_photos.py
--rw-r--r--   0        0        0     2032 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_contacts.py
--rw-r--r--   0        0        0     2032 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_document.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_empty.py
--rw-r--r--   0        0        0     2012 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_geo.py
--rw-r--r--   0        0        0     2012 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_gif.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_music.py
--rw-r--r--   0        0        0     2040 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_my_mentions.py
--rw-r--r--   0        0        0     2296 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_phone_calls.py
--rw-r--r--   0        0        0     2040 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_photo_video.py
--rw-r--r--   0        0        0     2024 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_photos.py
--rw-r--r--   0        0        0     2024 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_pinned.py
--rw-r--r--   0        0        0     2040 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_round_video.py
--rw-r--r--   0        0        0     2040 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_round_voice.py
--rw-r--r--   0        0        0     2012 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_url.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_video.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:00.917050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_messages_filter_voice.py
--rw-r--r--   0        0        0     2009 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_notify_broadcasts.py
--rw-r--r--   0        0        0     1989 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_notify_chats.py
--rw-r--r--   0        0        0     2457 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_notify_forum_topic.py
--rw-r--r--   0        0        0     2188 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_notify_peer.py
--rw-r--r--   0        0        0     1989 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_notify_users.py
--rw-r--r--   0        0        0     2509 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_payment_credentials.py
--rw-r--r--   0        0        0     2326 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_payment_credentials_apple_pay.py
--rw-r--r--   0        0        0     2341 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_payment_credentials_google_pay.py
--rw-r--r--   0        0        0     2431 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_payment_credentials_saved.py
--rw-r--r--   0        0        0     2441 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_channel.py
--rw-r--r--   0        0        0     2687 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_channel_from_message.py
--rw-r--r--   0        0        0     2145 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_chat.py
--rw-r--r--   0        0        0     1975 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_empty.py
--rw-r--r--   0        0        0     3679 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_notify_settings.py
--rw-r--r--   0        0        0     2740 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_photo_file_location.py
--rw-r--r--   0        0        0     1971 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_self.py
--rw-r--r--   0        0        0     2402 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_user.py
--rw-r--r--   0        0        0     2648 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_user_from_message.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_phone_call.py
--rw-r--r--   0        0        0     2857 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_phone_contact.py
--rw-r--r--   0        0        0     2626 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_photo.py
--rw-r--r--   0        0        0     1980 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_photo_empty.py
--rw-r--r--   0        0        0     2924 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_photo_file_location.py
--rw-r--r--   0        0        0     3383 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_photo_legacy_file_location.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_added_by_phone.py
--rw-r--r--   0        0        0     2025 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_chat_invite.py
--rw-r--r--   0        0        0     2017 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_forwards.py
--rw-r--r--   0        0        0     2021 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_phone_call.py
--rw-r--r--   0        0        0     2027 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_phone_number.py
--rw-r--r--   0        0        0     2017 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_phone_p2_p.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_profile_photo.py
--rw-r--r--   0        0        0     2045 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_status_timestamp.py
--rw-r--r--   0        0        0     2037 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_key_voice_messages.py
--rw-r--r--   0        0        0     2026 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_allow_all.py
--rw-r--r--   0        0        0     2274 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_allow_chat_participants.py
--rw-r--r--   0        0        0     2044 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_allow_contacts.py
--rw-r--r--   0        0        0     2268 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_allow_users.py
--rw-r--r--   0        0        0     2038 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_disallow_all.py
--rw-r--r--   0        0        0     2286 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_disallow_chat_participants.py
--rw-r--r--   0        0        0     2056 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_disallow_contacts.py
--rw-r--r--   0        0        0     2280 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_privacy_value_disallow_users.py
--rw-r--r--   0        0        0     2030 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_child_abuse.py
--rw-r--r--   0        0        0     2026 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_copyright.py
--rw-r--r--   0        0        0     2006 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_fake.py
--rw-r--r--   0        0        0     2042 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_geo_irrelevant.py
--rw-r--r--   0        0        0     2036 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_illegal_drugs.py
--rw-r--r--   0        0        0     2010 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_other.py
--rw-r--r--   0        0        0     2050 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_personal_details.py
--rw-r--r--   0        0        0     2034 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_pornography.py
--rw-r--r--   0        0        0     2006 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_spam.py
--rw-r--r--   0        0        0     2022 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_report_reason_violence.py
--rw-r--r--   0        0        0     2371 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_secure_file.py
--rw-r--r--   0        0        0     2405 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_secure_file_location.py
--rw-r--r--   0        0        0     3050 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_secure_file_uploaded.py
--rw-r--r--   0        0        0     5597 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_secure_value.py
--rw-r--r--   0        0        0     3187 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_single_media.py
--rw-r--r--   0        0        0     2035 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_animated_emoji.py
--rw-r--r--   0        0        0     2075 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_animated_emoji_animations.py
--rw-r--r--   0        0        0     2179 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_dice.py
--rw-r--r--   0        0        0     2065 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_emoji_default_statuses.py
--rw-r--r--   0        0        0     2073 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_emoji_default_topic_icons.py
--rw-r--r--   0        0        0     2071 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_emoji_generic_animations.py
--rw-r--r--   0        0        0     2005 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_empty.py
--rw-r--r--   0        0        0     2379 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_id.py
--rw-r--r--   0        0        0     3374 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_item.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_premium_gifts.py
--rw-r--r--   0        0        0     2217 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_short_name.py
--rw-r--r--   0        0        0     2560 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_sticker_set_thumb.py
--rw-r--r--   0        0        0     2236 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_stickered_media_document.py
--rw-r--r--   0        0        0     2214 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_stickered_media_photo.py
--rw-r--r--   0        0        0     2713 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_store_payment_gift_premium.py
--rw-r--r--   0        0        0     2610 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_store_payment_premium_subscription.py
--rw-r--r--   0        0        0     2023 2023-05-20 17:34:00.893049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_takeout_file_location.py
--rw-r--r--   0        0        0     2346 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_theme.py
--rw-r--r--   0        0        0     5043 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_theme_settings.py
--rw-r--r--   0        0        0     2118 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_theme_slug.py
--rw-r--r--   0        0        0     2386 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_user.py
--rw-r--r--   0        0        0     1975 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_user_empty.py
--rw-r--r--   0        0        0     2632 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_user_from_message.py
--rw-r--r--   0        0        0     1971 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_user_self.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_wall_paper.py
--rw-r--r--   0        0        0     2133 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_wall_paper_no_file.py
--rw-r--r--   0        0        0     2138 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_wall_paper_slug.py
--rw-r--r--   0        0        0     2906 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_web_document.py
--rw-r--r--   0        0        0     3532 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_web_file_audio_album_thumb_location.py
--rw-r--r--   0        0        0     3282 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_web_file_geo_point_location.py
--rw-r--r--   0        0        0     2400 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_web_file_location.py
--rw-r--r--   0        0        0     6967 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/invoice.py
--rw-r--r--   0        0        0     2275 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/ip_port.py
--rw-r--r--   0        0        0     2507 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/ip_port_secret.py
--rw-r--r--   0        0        0     2189 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/json_array.py
--rw-r--r--   0        0        0     2098 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/json_bool.py
--rw-r--r--   0        0        0     1951 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/json_null.py
--rw-r--r--   0        0        0     2125 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/json_number.py
--rw-r--r--   0        0        0     2217 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/json_object.py
--rw-r--r--   0        0        0     2377 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/json_object_value.py
--rw-r--r--   0        0        0     2110 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/json_string.py
--rw-r--r--   0        0        0     2122 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button.py
--rw-r--r--   0        0        0     2134 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_buy.py
--rw-r--r--   0        0        0     2746 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_callback.py
--rw-r--r--   0        0        0     2138 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_game.py
--rw-r--r--   0        0        0     2194 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_request_geo_location.py
--rw-r--r--   0        0        0     2719 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_request_peer.py
--rw-r--r--   0        0        0     2170 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_request_phone.py
--rw-r--r--   0        0        0     2550 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_request_poll.py
--rw-r--r--   0        0        0     2267 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_row.py
--rw-r--r--   0        0        0     2354 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_simple_web_view.py
--rw-r--r--   0        0        0     3225 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_switch_inline.py
--rw-r--r--   0        0        0     2314 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_url.py
--rw-r--r--   0        0        0     2998 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_url_auth.py
--rw-r--r--   0        0        0     2387 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_user_profile.py
--rw-r--r--   0        0        0     2330 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_web_view.py
--rw-r--r--   0        0        0     2333 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/labeled_price.py
--rw-r--r--   0        0        0     3227 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/lang_pack_difference.py
--rw-r--r--   0        0        0     5222 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/lang_pack_language.py
--rw-r--r--   0        0        0     2514 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/lang_pack_string.py
--rw-r--r--   0        0        0     2344 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/lang_pack_string_deleted.py
--rw-r--r--   0        0        0     4665 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/lang_pack_string_pluralized.py
--rw-r--r--   0        0        0     2635 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/mask_coords.py
--rw-r--r--   0        0        0    12715 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message.py
--rw-r--r--   0        0        0     3061 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_bot_allowed.py
--rw-r--r--   0        0        0     2178 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_channel_create.py
--rw-r--r--   0        0        0     2419 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_channel_migrate_from.py
--rw-r--r--   0        0        0     2215 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_add_user.py
--rw-r--r--   0        0        0     2409 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_create.py
--rw-r--r--   0        0        0     2035 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_delete_photo.py
--rw-r--r--   0        0        0     2205 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_delete_user.py
--rw-r--r--   0        0        0     2223 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_edit_photo.py
--rw-r--r--   0        0        0     2178 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_edit_title.py
--rw-r--r--   0        0        0     2238 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_joined_by_link.py
--rw-r--r--   0        0        0     2051 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_joined_by_request.py
--rw-r--r--   0        0        0     2228 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_chat_migrate_to.py
--rw-r--r--   0        0        0     2027 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_contact_sign_up.py
--rw-r--r--   0        0        0     2192 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_custom_action.py
--rw-r--r--   0        0        0     1995 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_empty.py
--rw-r--r--   0        0        0     2385 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_game_score.py
--rw-r--r--   0        0        0     2727 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_geo_proximity_reached.py
--rw-r--r--   0        0        0     3574 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_gift_premium.py
--rw-r--r--   0        0        0     2668 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_group_call.py
--rw-r--r--   0        0        0     2542 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_group_call_scheduled.py
--rw-r--r--   0        0        0     2023 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_history_clear.py
--rw-r--r--   0        0        0     2509 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_invite_to_group_call.py
--rw-r--r--   0        0        0     3599 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_payment_sent.py
--rw-r--r--   0        0        0     4621 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_payment_sent_me.py
--rw-r--r--   0        0        0     3345 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_phone_call.py
--rw-r--r--   0        0        0     2015 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_pin_message.py
--rw-r--r--   0        0        0     2446 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_requested_peer.py
--rw-r--r--   0        0        0     2035 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_screenshot_taken.py
--rw-r--r--   0        0        0     2297 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_secure_values_sent.py
--rw-r--r--   0        0        0     2679 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_secure_values_sent_me.py
--rw-r--r--   0        0        0     2201 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_set_chat_theme.py
--rw-r--r--   0        0        0     2287 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_set_chat_wall_paper.py
--rw-r--r--   0        0        0     2729 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_set_messages_ttl.py
--rw-r--r--   0        0        0     2303 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_set_same_chat_wall_paper.py
--rw-r--r--   0        0        0     2247 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_suggest_profile_photo.py
--rw-r--r--   0        0        0     2905 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_topic_create.py
--rw-r--r--   0        0        0     3532 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_topic_edit.py
--rw-r--r--   0        0        0     2177 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_web_view_data_sent.py
--rw-r--r--   0        0        0     2374 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_action_web_view_data_sent_me.py
--rw-r--r--   0        0        0     2552 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_empty.py
--rw-r--r--   0        0        0     2378 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_bank_card.py
--rw-r--r--   0        0        0     2384 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_blockquote.py
--rw-r--r--   0        0        0     2362 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_bold.py
--rw-r--r--   0        0        0     2386 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_bot_command.py
--rw-r--r--   0        0        0     2374 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_cashtag.py
--rw-r--r--   0        0        0     2362 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_code.py
--rw-r--r--   0        0        0     2647 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_custom_emoji.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_email.py
--rw-r--r--   0        0        0     2374 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_hashtag.py
--rw-r--r--   0        0        0     2370 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_italic.py
--rw-r--r--   0        0        0     2374 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_mention.py
--rw-r--r--   0        0        0     2611 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_mention_name.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_phone.py
--rw-r--r--   0        0        0     2583 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_pre.py
--rw-r--r--   0        0        0     2374 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_spoiler.py
--rw-r--r--   0        0        0     2370 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_strike.py
--rw-r--r--   0        0        0     2554 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_text_url.py
--rw-r--r--   0        0        0     2382 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_underline.py
--rw-r--r--   0        0        0     2374 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_unknown.py
--rw-r--r--   0        0        0     2358 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_entity_url.py
--rw-r--r--   0        0        0     2234 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_extended_media.py
--rw-r--r--   0        0        0     3529 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_extended_media_preview.py
--rw-r--r--   0        0        0     5501 2023-05-20 17:34:00.969051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_fwd_header.py
--rw-r--r--   0        0        0     2629 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_interaction_counters.py
--rw-r--r--   0        0        0     3393 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_contact.py
--rw-r--r--   0        0        0     2649 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_dice.py
--rw-r--r--   0        0        0     3702 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_document.py
--rw-r--r--   0        0        0     2275 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_empty.py
--rw-r--r--   0        0        0     2454 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_game.py
--rw-r--r--   0        0        0     2457 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_geo.py
--rw-r--r--   0        0        0     3725 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_geo_live.py
--rw-r--r--   0        0        0     5586 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_invoice.py
--rw-r--r--   0        0        0     3360 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_photo.py
--rw-r--r--   0        0        0     2739 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_poll.py
--rw-r--r--   0        0        0     2299 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_unsupported.py
--rw-r--r--   0        0        0     3572 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_venue.py
--rw-r--r--   0        0        0     2505 2023-05-20 17:34:00.905049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_media_web_page.py
--rw-r--r--   0        0        0     3222 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_peer_reaction.py
--rw-r--r--   0        0        0     2546 2023-05-20 17:34:00.961051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_range.py
--rw-r--r--   0        0        0     3439 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_reactions.py
--rw-r--r--   0        0        0     4451 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_replies.py
--rw-r--r--   0        0        0     3938 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_reply_header.py
--rw-r--r--   0        0        0     5782 2023-05-20 17:34:00.901049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_service.py
--rw-r--r--   0        0        0     2558 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_user_vote.py
--rw-r--r--   0        0        0     2394 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_user_vote_input_option.py
--rw-r--r--   0        0        0     2639 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_user_vote_multiple.py
--rw-r--r--   0        0        0     3169 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/message_views.py
--rw-r--r--   0        0        0     2834 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msg_detailed_info.py
--rw-r--r--   0        0        0     2634 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msg_new_detailed_info.py
--rw-r--r--   0        0        0     2196 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msg_resend_ans_req.py
--rw-r--r--   0        0        0     2184 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msg_resend_req.py
--rw-r--r--   0        0        0     2159 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msgs_ack.py
--rw-r--r--   0        0        0     2368 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msgs_all_info.py
--rw-r--r--   0        0        0     2365 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msgs_state_info.py
--rw-r--r--   0        0        0     2184 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/msgs_state_req.py
--rw-r--r--   0        0        0     2788 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/nearest_dc.py
--rw-r--r--   0        0        0     2703 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/new_session_created.py
--rw-r--r--   0        0        0     2023 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notification_sound_default.py
--rw-r--r--   0        0        0     2355 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notification_sound_local.py
--rw-r--r--   0        0        0     2011 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notification_sound_none.py
--rw-r--r--   0        0        0     2156 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notification_sound_ringtone.py
--rw-r--r--   0        0        0     1984 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notify_broadcasts.py
--rw-r--r--   0        0        0     1964 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notify_chats.py
--rw-r--r--   0        0        0     2412 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notify_forum_topic.py
--rw-r--r--   0        0        0     2143 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notify_peer.py
--rw-r--r--   0        0        0     1964 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/notify_users.py
--rw-r--r--   0        0        0     1930 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/null.py
--rw-r--r--   0        0        0     4034 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page.py
--rw-r--r--   0        0        0     2121 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_anchor.py
--rw-r--r--   0        0        0     2443 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_audio.py
--rw-r--r--   0        0        0     2493 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_author_date.py
--rw-r--r--   0        0        0     2467 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_blockquote.py
--rw-r--r--   0        0        0     2193 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_channel.py
--rw-r--r--   0        0        0     2502 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_collage.py
--rw-r--r--   0        0        0     2187 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_cover.py
--rw-r--r--   0        0        0     2766 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_details.py
--rw-r--r--   0        0        0     1983 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_divider.py
--rw-r--r--   0        0        0     4659 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_embed.py
--rw-r--r--   0        0        0     3638 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_embed_post.py
--rw-r--r--   0        0        0     2178 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_footer.py
--rw-r--r--   0        0        0     2178 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_header.py
--rw-r--r--   0        0        0     2178 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_kicker.py
--rw-r--r--   0        0        0     2217 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_list.py
--rw-r--r--   0        0        0     2961 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_map.py
--rw-r--r--   0        0        0     2273 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_ordered_list.py
--rw-r--r--   0        0        0     2190 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_paragraph.py
--rw-r--r--   0        0        0     3234 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_photo.py
--rw-r--r--   0        0        0     2427 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_preformatted.py
--rw-r--r--   0        0        0     2463 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_pullquote.py
--rw-r--r--   0        0        0     2567 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_related_articles.py
--rw-r--r--   0        0        0     2508 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_slideshow.py
--rw-r--r--   0        0        0     2190 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_subheader.py
--rw-r--r--   0        0        0     2186 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_subtitle.py
--rw-r--r--   0        0        0     3055 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_table.py
--rw-r--r--   0        0        0     2174 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_title.py
--rw-r--r--   0        0        0     1999 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_unsupported.py
--rw-r--r--   0        0        0     3004 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_block_video.py
--rw-r--r--   0        0        0     2428 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_caption.py
--rw-r--r--   0        0        0     2237 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_list_item_blocks.py
--rw-r--r--   0        0        0     2185 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_list_item_text.py
--rw-r--r--   0        0        0     2452 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_list_ordered_item_blocks.py
--rw-r--r--   0        0        0     2400 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_list_ordered_item_text.py
--rw-r--r--   0        0        0     4412 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_related_article.py
--rw-r--r--   0        0        0     4643 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_table_cell.py
--rw-r--r--   0        0        0     2220 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/page_table_row.py
--rw-r--r--   0        0        0     2863 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/password_kdf_algo_sha256_sha256_pbkdf2_hmacsha512iter100000_sha256_mod_pow.py
--rw-r--r--   0        0        0     2013 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/password_kdf_algo_unknown.py
--rw-r--r--   0        0        0     2414 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/payment_charge.py
--rw-r--r--   0        0        0     2326 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/payment_form_method.py
--rw-r--r--   0        0        0     3602 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/payment_requested_info.py
--rw-r--r--   0        0        0     2363 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/payment_saved_credentials_card.py
--rw-r--r--   0        0        0     2366 2023-05-20 17:34:01.021052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_blocked.py
--rw-r--r--   0        0        0     2380 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_channel.py
--rw-r--r--   0        0        0     2341 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_chat.py
--rw-r--r--   0        0        0     2593 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_located.py
--rw-r--r--   0        0        0     4953 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_notify_settings.py
--rw-r--r--   0        0        0     2152 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_self_located.py
--rw-r--r--   0        0        0     6386 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_settings.py
--rw-r--r--   0        0        0     2341 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/peer_user.py
--rw-r--r--   0        0        0     5084 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call.py
--rw-r--r--   0        0        0     3871 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_accepted.py
--rw-r--r--   0        0        0     2036 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_discard_reason_busy.py
--rw-r--r--   0        0        0     2060 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_discard_reason_disconnect.py
--rw-r--r--   0        0        0     2044 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_discard_reason_hangup.py
--rw-r--r--   0        0        0     2044 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_discard_reason_missed.py
--rw-r--r--   0        0        0     3877 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_discarded.py
--rw-r--r--   0        0        0     2104 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_empty.py
--rw-r--r--   0        0        0     3390 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_protocol.py
--rw-r--r--   0        0        0     3920 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_requested.py
--rw-r--r--   0        0        0     4119 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_call_waiting.py
--rw-r--r--   0        0        0     3167 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_connection.py
--rw-r--r--   0        0        0     3664 2023-05-20 17:34:00.989051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/phone_connection_webrtc.py
--rw-r--r--   0        0        0     4128 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo.py
--rw-r--r--   0        0        0     2646 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo_cached_size.py
--rw-r--r--   0        0        0     2084 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo_empty.py
--rw-r--r--   0        0        0     2312 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo_path_size.py
--rw-r--r--   0        0        0     2616 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo_size.py
--rw-r--r--   0        0        0     2115 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo_size_empty.py
--rw-r--r--   0        0        0     2709 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo_size_progressive.py
--rw-r--r--   0        0        0     2328 2023-05-20 17:34:00.909050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/photo_stripped_size.py
--rw-r--r--   0        0        0     4634 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/poll.py
--rw-r--r--   0        0        0     2310 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/poll_answer.py
--rw-r--r--   0        0        0     2930 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/poll_answer_voters.py
--rw-r--r--   0        0        0     4558 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/poll_results.py
--rw-r--r--   0        0        0     2537 2023-05-20 17:34:00.889049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/pong.py
--rw-r--r--   0        0        0     2408 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/popular_contact.py
--rw-r--r--   0        0        0     3322 2023-05-20 17:34:00.981051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/post_address.py
--rw-r--r--   0        0        0     3145 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/pq_inner_data.py
--rw-r--r--   0        0        0     3326 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/pq_inner_data_dc.py
--rw-r--r--   0        0        0     3406 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/pq_inner_data_temp.py
--rw-r--r--   0        0        0     3587 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/pq_inner_data_temp_dc.py
--rw-r--r--   0        0        0     3297 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/premium_gift_option.py
--rw-r--r--   0        0        0     4408 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/premium_subscription_option.py
--rw-r--r--   0        0        0     2008 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_added_by_phone.py
--rw-r--r--   0        0        0     2000 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_chat_invite.py
--rw-r--r--   0        0        0     1992 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_forwards.py
--rw-r--r--   0        0        0     1996 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_phone_call.py
--rw-r--r--   0        0        0     2004 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_phone_number.py
--rw-r--r--   0        0        0     1992 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_phone_p2_p.py
--rw-r--r--   0        0        0     2008 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_profile_photo.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_status_timestamp.py
--rw-r--r--   0        0        0     2010 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_key_voice_messages.py
--rw-r--r--   0        0        0     2001 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_allow_all.py
--rw-r--r--   0        0        0     2249 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_allow_chat_participants.py
--rw-r--r--   0        0        0     2021 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_allow_contacts.py
--rw-r--r--   0        0        0     2205 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_allow_users.py
--rw-r--r--   0        0        0     2013 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_disallow_all.py
--rw-r--r--   0        0        0     2261 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_disallow_chat_participants.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_disallow_contacts.py
--rw-r--r--   0        0        0     2217 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/privacy_value_disallow_users.py
--rw-r--r--   0        0        0     2888 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reaction_count.py
--rw-r--r--   0        0        0     2204 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reaction_custom_emoji.py
--rw-r--r--   0        0        0     2148 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reaction_emoji.py
--rw-r--r--   0        0        0     1970 2023-05-20 17:34:01.033052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reaction_empty.py
--rw-r--r--   0        0        0     2589 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/read_participant_date.py
--rw-r--r--   0        0        0     2550 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/received_notify_message.py
--rw-r--r--   0        0        0     2335 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/recent_me_url_chat.py
--rw-r--r--   0        0        0     2455 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/recent_me_url_chat_invite.py
--rw-r--r--   0        0        0     2411 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/recent_me_url_sticker_set.py
--rw-r--r--   0        0        0     2126 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/recent_me_url_unknown.py
--rw-r--r--   0        0        0     2335 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/recent_me_url_user.py
--rw-r--r--   0        0        0     2246 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reply_inline_markup.py
--rw-r--r--   0        0        0     3010 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reply_keyboard_force_reply.py
--rw-r--r--   0        0        0     2272 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reply_keyboard_hide.py
--rw-r--r--   0        0        0     3850 2023-05-20 17:34:00.957051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/reply_keyboard_markup.py
--rw-r--r--   0        0        0     3842 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/request_peer_type_broadcast.py
--rw-r--r--   0        0        0     4511 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/request_peer_type_chat.py
--rw-r--r--   0        0        0     2699 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/request_peer_type_user.py
--rw-r--r--   0        0        0     3224 2023-05-20 17:34:00.881049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/res_pq.py
--rw-r--r--   0        0        0     2569 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/restriction_reason.py
--rw-r--r--   0        0        0     2758 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/rpc_answer_dropped.py
--rw-r--r--   0        0        0     2212 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/rpc_answer_dropped_running.py
--rw-r--r--   0        0        0     2184 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/rpc_answer_unknown.py
--rw-r--r--   0        0        0     2418 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/rpc_error.py
--rw-r--r--   0        0        0     2403 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/rpc_result.py
--rw-r--r--   0        0        0     3010 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/saved_phone_contact.py
--rw-r--r--   0        0        0     2573 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/search_result_position.py
--rw-r--r--   0        0        0     2879 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/search_results_calendar_period.py
--rw-r--r--   0        0        0     2581 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_credentials_encrypted.py
--rw-r--r--   0        0        0     2546 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_data.py
--rw-r--r--   0        0        0     3374 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_file.py
--rw-r--r--   0        0        0     1980 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_file_empty.py
--rw-r--r--   0        0        0     2262 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_password_kdf_algo_pbkdf2_hmacsha512iter100000.py
--rw-r--r--   0        0        0     2182 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_password_kdf_algo_sha512.py
--rw-r--r--   0        0        0     2039 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_password_kdf_algo_unknown.py
--rw-r--r--   0        0        0     2140 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_plain_email.py
--rw-r--r--   0        0        0     2140 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_plain_phone.py
--rw-r--r--   0        0        0     3307 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_required_type.py
--rw-r--r--   0        0        0     2288 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_required_type_one_of.py
--rw-r--r--   0        0        0     2897 2023-05-20 17:34:01.005052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_secret_settings.py
--rw-r--r--   0        0        0     5944 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value.py
--rw-r--r--   0        0        0     2596 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error.py
--rw-r--r--   0        0        0     2855 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_data.py
--rw-r--r--   0        0        0     2657 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_file.py
--rw-r--r--   0        0        0     2701 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_files.py
--rw-r--r--   0        0        0     2673 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_front_side.py
--rw-r--r--   0        0        0     2685 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_reverse_side.py
--rw-r--r--   0        0        0     2665 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_selfie.py
--rw-r--r--   0        0        0     2701 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_translation_file.py
--rw-r--r--   0        0        0     2745 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_error_translation_files.py
--rw-r--r--   0        0        0     2402 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_hash.py
--rw-r--r--   0        0        0     2013 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_address.py
--rw-r--r--   0        0        0     2037 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_bank_statement.py
--rw-r--r--   0        0        0     2035 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_driver_license.py
--rw-r--r--   0        0        0     2005 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_email.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_identity_card.py
--rw-r--r--   0        0        0     2049 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_internal_passport.py
--rw-r--r--   0        0        0     2017 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_passport.py
--rw-r--r--   0        0        0     2065 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_passport_registration.py
--rw-r--r--   0        0        0     2045 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_personal_details.py
--rw-r--r--   0        0        0     2005 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_phone.py
--rw-r--r--   0        0        0     2045 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_rental_agreement.py
--rw-r--r--   0        0        0     2069 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_temporary_registration.py
--rw-r--r--   0        0        0     2029 2023-05-20 17:34:01.001052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/secure_value_type_utility_bill.py
--rw-r--r--   0        0        0     2536 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_as_peer.py
--rw-r--r--   0        0        0     2019 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_cancel_action.py
--rw-r--r--   0        0        0     2047 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_choose_contact_action.py
--rw-r--r--   0        0        0     2047 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_choose_sticker_action.py
--rw-r--r--   0        0        0     2731 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_emoji_interaction.py
--rw-r--r--   0        0        0     2229 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_emoji_interaction_seen.py
--rw-r--r--   0        0        0     2027 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_game_play_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_geo_location_action.py
--rw-r--r--   0        0        0     2227 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_history_import_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_record_audio_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_record_round_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_record_video_action.py
--rw-r--r--   0        0        0     2019 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_typing_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_upload_audio_action.py
--rw-r--r--   0        0        0     2231 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_upload_document_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_upload_photo_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_upload_round_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 17:34:00.941050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/send_message_upload_video_action.py
--rw-r--r--   0        0        0     3256 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/server_dh_inner_data.py
--rw-r--r--   0        0        0     2918 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/server_dh_params_fail.py
--rw-r--r--   0        0        0     2917 2023-05-20 17:34:00.885049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/server_dh_params_ok.py
--rw-r--r--   0        0        0     2604 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/shipping_option.py
--rw-r--r--   0        0        0     2363 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/simple_web_view_result_url.py
--rw-r--r--   0        0        0     2027 2023-05-20 17:34:00.945050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/speaking_in_group_call_action.py
--rw-r--r--   0        0        0     6685 2023-05-20 17:34:01.025052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sponsored_message.py
--rw-r--r--   0        0        0     2434 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_abs_value_and_prev.py
--rw-r--r--   0        0        0     2407 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_date_range_days.py
--rw-r--r--   0        0        0     2817 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_graph.py
--rw-r--r--   0        0        0     2335 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_graph_async.py
--rw-r--r--   0        0        0     2335 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_graph_error.py
--rw-r--r--   0        0        0     2810 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_group_top_admin.py
--rw-r--r--   0        0        0     2438 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_group_top_inviter.py
--rw-r--r--   0        0        0     2642 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_group_top_poster.py
--rw-r--r--   0        0        0     2365 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_percent_value.py
--rw-r--r--   0        0        0     2083 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/stats_url.py
--rw-r--r--   0        0        0     2446 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sticker_keyword.py
--rw-r--r--   0        0        0     2422 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sticker_pack.py
--rw-r--r--   0        0        0     7071 2023-05-20 17:34:00.953050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sticker_set.py
--rw-r--r--   0        0        0     2660 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sticker_set_covered.py
--rw-r--r--   0        0        0     3351 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sticker_set_full_covered.py
--rw-r--r--   0        0        0     2711 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sticker_set_multi_covered.py
--rw-r--r--   0        0        0     2413 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/sticker_set_no_covered.py
--rw-r--r--   0        0        0     2346 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_anchor.py
--rw-r--r--   0        0        0     2149 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_bold.py
--rw-r--r--   0        0        0     2188 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_concat.py
--rw-r--r--   0        0        0     2351 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_email.py
--rw-r--r--   0        0        0     1954 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_empty.py
--rw-r--r--   0        0        0     2153 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_fixed.py
--rw-r--r--   0        0        0     2490 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_image.py
--rw-r--r--   0        0        0     2157 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_italic.py
--rw-r--r--   0        0        0     2155 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_marked.py
--rw-r--r--   0        0        0     2351 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_phone.py
--rw-r--r--   0        0        0     2096 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_plain.py
--rw-r--r--   0        0        0     2157 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_strike.py
--rw-r--r--   0        0        0     2169 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_subscript.py
--rw-r--r--   0        0        0     2177 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_superscript.py
--rw-r--r--   0        0        0     2169 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_underline.py
--rw-r--r--   0        0        0     2573 2023-05-20 17:34:00.977051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_url.py
--rw-r--r--   0        0        0     2456 2023-05-20 17:34:01.041053 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/text_with_entities.py
--rw-r--r--   0        0        0     5594 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/theme.py
--rw-r--r--   0        0        0     4409 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/theme_settings.py
--rw-r--r--   0        0        0     2350 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer.py
--rw-r--r--   0        0        0     2025 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_bots_inline.py
--rw-r--r--   0        0        0     2009 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_bots_pm.py
--rw-r--r--   0        0        0     2017 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_channels.py
--rw-r--r--   0        0        0     2039 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_correspondents.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_forward_chats.py
--rw-r--r--   0        0        0     2033 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_forward_users.py
--rw-r--r--   0        0        0     2009 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_groups.py
--rw-r--r--   0        0        0     2746 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_peers.py
--rw-r--r--   0        0        0     2025 2023-05-20 17:34:00.973051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/top_peer_category_phone_calls.py
--rw-r--r--   0        0        0     1996 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_attach_menu_bots.py
--rw-r--r--   0        0        0     2004 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_auto_save_settings.py
--rw-r--r--   0        0        0     3975 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_callback_query.py
--rw-r--r--   0        0        0     3307 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_chat_invite_requester.py
--rw-r--r--   0        0        0     2691 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_commands.py
--rw-r--r--   0        0        0     3736 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_inline_query.py
--rw-r--r--   0        0        0     3449 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_inline_send.py
--rw-r--r--   0        0        0     2441 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_menu_button.py
--rw-r--r--   0        0        0     4117 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_precheckout_query.py
--rw-r--r--   0        0        0     2991 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_shipping_query.py
--rw-r--r--   0        0        0     2739 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_stopped.py
--rw-r--r--   0        0        0     2195 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_webhook_json.py
--rw-r--r--   0        0        0     2663 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_bot_webhook_json_query.py
--rw-r--r--   0        0        0     2169 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel.py
--rw-r--r--   0        0        0     2536 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_available_messages.py
--rw-r--r--   0        0        0     2629 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_message_forwards.py
--rw-r--r--   0        0        0     2590 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_message_views.py
--rw-r--r--   0        0        0     4986 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_participant.py
--rw-r--r--   0        0        0     2743 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_pinned_topic.py
--rw-r--r--   0        0        0     2653 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_pinned_topics.py
--rw-r--r--   0        0        0     2972 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_read_messages_contents.py
--rw-r--r--   0        0        0     2576 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_too_long.py
--rw-r--r--   0        0        0     3222 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_user_typing.py
--rw-r--r--   0        0        0     2884 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_channel_web_page.py
--rw-r--r--   0        0        0     2130 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat.py
--rw-r--r--   0        0        0     2864 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat_default_banned_rights.py
--rw-r--r--   0        0        0     4611 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat_participant.py
--rw-r--r--   0        0        0     3064 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat_participant_add.py
--rw-r--r--   0        0        0     2854 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat_participant_admin.py
--rw-r--r--   0        0        0     2637 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat_participant_delete.py
--rw-r--r--   0        0        0     2305 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat_participants.py
--rw-r--r--   0        0        0     2727 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_chat_user_typing.py
--rw-r--r--   0        0        0     1964 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_config.py
--rw-r--r--   0        0        0     1992 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_contacts_reset.py
--rw-r--r--   0        0        0     2251 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_dc_options.py
--rw-r--r--   0        0        0     2910 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_delete_channel_messages.py
--rw-r--r--   0        0        0     2634 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_delete_messages.py
--rw-r--r--   0        0        0     2482 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_delete_scheduled_messages.py
--rw-r--r--   0        0        0     2596 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_dialog_filter.py
--rw-r--r--   0        0        0     2201 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_dialog_filter_order.py
--rw-r--r--   0        0        0     1992 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_dialog_filters.py
--rw-r--r--   0        0        0     2898 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_dialog_pinned.py
--rw-r--r--   0        0        0     2514 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_dialog_unread_mark.py
--rw-r--r--   0        0        0     2898 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_draft_message.py
--rw-r--r--   0        0        0     2652 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_edit_channel_message.py
--rw-r--r--   0        0        0     2624 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_edit_message.py
--rw-r--r--   0        0        0     2187 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_encrypted_chat_typing.py
--rw-r--r--   0        0        0     2613 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_encrypted_messages_read.py
--rw-r--r--   0        0        0     2390 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_encryption.py
--rw-r--r--   0        0        0     1992 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_faved_stickers.py
--rw-r--r--   0        0        0     2703 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_folder_peers.py
--rw-r--r--   0        0        0     2384 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_geo_live_viewed.py
--rw-r--r--   0        0        0     2400 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_group_call.py
--rw-r--r--   0        0        0     2588 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_group_call_connection.py
--rw-r--r--   0        0        0     2853 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_group_call_participants.py
--rw-r--r--   0        0        0     2222 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_group_invite_privacy_forbidden.py
--rw-r--r--   0        0        0     3884 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_inline_bot_callback_query.py
--rw-r--r--   0        0        0     2265 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_lang_pack.py
--rw-r--r--   0        0        0     2187 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_lang_pack_too_long.py
--rw-r--r--   0        0        0     1980 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_login_token.py
--rw-r--r--   0        0        0     2796 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_message_extended_media.py
--rw-r--r--   0        0        0     2341 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_message_id.py
--rw-r--r--   0        0        0     2871 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_message_poll.py
--rw-r--r--   0        0        0     2834 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_message_poll_vote.py
--rw-r--r--   0        0        0     3175 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_message_reactions.py
--rw-r--r--   0        0        0     2769 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_move_sticker_set_to_top.py
--rw-r--r--   0        0        0     2648 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_new_channel_message.py
--rw-r--r--   0        0        0     2456 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_new_encrypted_message.py
--rw-r--r--   0        0        0     2620 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_new_message.py
--rw-r--r--   0        0        0     2238 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_new_scheduled_message.py
--rw-r--r--   0        0        0     2289 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_new_sticker_set.py
--rw-r--r--   0        0        0     2588 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_notify_settings.py
--rw-r--r--   0        0        0     2406 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_peer_blocked.py
--rw-r--r--   0        0        0     2635 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_peer_history_ttl.py
--rw-r--r--   0        0        0     2226 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_peer_located.py
--rw-r--r--   0        0        0     2469 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_peer_settings.py
--rw-r--r--   0        0        0     2849 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_pending_join_requests.py
--rw-r--r--   0        0        0     2233 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_phone_call.py
--rw-r--r--   0        0        0     2446 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_phone_call_signaling_data.py
--rw-r--r--   0        0        0     3213 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_pinned_channel_messages.py
--rw-r--r--   0        0        0     2826 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_pinned_dialogs.py
--rw-r--r--   0        0        0     3167 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_pinned_messages.py
--rw-r--r--   0        0        0     2455 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_privacy.py
--rw-r--r--   0        0        0     1980 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_pts_changed.py
--rw-r--r--   0        0        0     3680 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_channel_discussion_inbox.py
--rw-r--r--   0        0        0     2748 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_channel_discussion_outbox.py
--rw-r--r--   0        0        0     3358 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_channel_inbox.py
--rw-r--r--   0        0        0     2418 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_channel_outbox.py
--rw-r--r--   0        0        0     2040 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_featured_emoji_stickers.py
--rw-r--r--   0        0        0     2020 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_featured_stickers.py
--rw-r--r--   0        0        0     3576 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_history_inbox.py
--rw-r--r--   0        0        0     2818 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_history_outbox.py
--rw-r--r--   0        0        0     2658 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_read_messages_contents.py
--rw-r--r--   0        0        0     2016 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_recent_emoji_statuses.py
--rw-r--r--   0        0        0     2000 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_recent_reactions.py
--rw-r--r--   0        0        0     1996 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_recent_stickers.py
--rw-r--r--   0        0        0     1976 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_saved_gifs.py
--rw-r--r--   0        0        0     1996 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_saved_ringtones.py
--rw-r--r--   0        0        0     3674 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_service_notification.py
--rw-r--r--   0        0        0     5802 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_short.py
--rw-r--r--   0        0        0    10243 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_short_chat_message.py
--rw-r--r--   0        0        0    10006 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_short_message.py
--rw-r--r--   0        0        0     7778 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_short_sent_message.py
--rw-r--r--   0        0        0     2489 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_sticker_sets.py
--rw-r--r--   0        0        0     2750 2023-05-20 17:34:00.925050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_sticker_sets_order.py
--rw-r--r--   0        0        0     2156 2023-05-20 17:34:00.929050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_theme.py
--rw-r--r--   0        0        0     3195 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_transcribed_audio.py
--rw-r--r--   0        0        0     2130 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_user.py
--rw-r--r--   0        0        0     2504 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_user_emoji_status.py
--rw-r--r--   0        0        0     2936 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_user_name.py
--rw-r--r--   0        0        0     2346 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_user_phone.py
--rw-r--r--   0        0        0     2426 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_user_status.py
--rw-r--r--   0        0        0     2454 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_user_typing.py
--rw-r--r--   0        0        0     2608 2023-05-20 17:34:00.921050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_web_page.py
--rw-r--r--   0        0        0     2191 2023-05-20 17:34:00.933050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/update_web_view_result_sent.py
--rw-r--r--   0        0        0     6789 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/updates_combined.py
--rw-r--r--   0        0        0     6521 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/updates_t.py
--rw-r--r--   0        0        0     5414 2023-05-20 17:34:00.937050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/updates_too_long.py
--rw-r--r--   0        0        0     2383 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/url_auth_result_accepted.py
--rw-r--r--   0        0        0     2246 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/url_auth_result_default.py
--rw-r--r--   0        0        0     3056 2023-05-20 17:34:01.013052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/url_auth_result_request.py
--rw-r--r--   0        0        0    13966 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user.py
--rw-r--r--   0        0        0     2419 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_empty.py
--rw-r--r--   0        0        0    12871 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_full.py
--rw-r--r--   0        0        0     3433 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_profile_photo.py
--rw-r--r--   0        0        0     2010 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_profile_photo_empty.py
--rw-r--r--   0        0        0     1978 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_status_empty.py
--rw-r--r--   0        0        0     1996 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_status_last_month.py
--rw-r--r--   0        0        0     1990 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_status_last_week.py
--rw-r--r--   0        0        0     2182 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_status_offline.py
--rw-r--r--   0        0        0     2155 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_status_online.py
--rw-r--r--   0        0        0     1992 2023-05-20 17:34:00.897049 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/user_status_recently.py
--rw-r--r--   0        0        0     2707 2023-05-20 17:34:01.037052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/username.py
--rw-r--r--   0        0        0     3129 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/video_size.py
--rw-r--r--   0        0        0     2530 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/video_size_emoji_markup.py
--rw-r--r--   0        0        0     2882 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/video_size_sticker_markup.py
--rw-r--r--   0        0        0     4657 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/wall_paper.py
--rw-r--r--   0        0        0     3419 2023-05-20 17:34:00.913050 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/wall_paper_no_file.py
--rw-r--r--   0        0        0     5408 2023-05-20 17:34:01.009052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/wall_paper_settings.py
--rw-r--r--   0        0        0     3892 2023-05-20 17:34:00.997052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_authorization.py
--rw-r--r--   0        0        0     3138 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_document.py
--rw-r--r--   0        0        0     2909 2023-05-20 17:34:00.985051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_document_no_proxy.py
--rw-r--r--   0        0        0     8698 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_page.py
--rw-r--r--   0        0        0     2943 2023-05-20 17:34:01.017052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_page_attribute_theme.py
--rw-r--r--   0        0        0     2297 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_page_empty.py
--rw-r--r--   0        0        0     2678 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_page_not_modified.py
--rw-r--r--   0        0        0     2496 2023-05-20 17:34:00.949051 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_page_pending.py
--rw-r--r--   0        0        0     2694 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_view_message_sent.py
--rw-r--r--   0        0        0     2555 2023-05-20 17:34:01.029052 pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/web_view_result_url.py
--rw-r--r--   0        0        0      871 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    10513 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/auth.py
--rw-r--r--   0        0        0      917 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2452 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1374 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1587 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1257 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0    12440 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/session.py
--rw-r--r--   0        0        0      968 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     2741 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0     5428 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/mongo_storage.py
--rw-r--r--   0        0        0     6382 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     2781 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     3739 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/sync.py
--rw-r--r--   0        0        0     1109 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/__init__.py
--rw-r--r--   0        0        0      938 2023-05-20 17:33:19.939603 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2288 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1930 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     2830 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1293 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1258 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1249 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1817 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1029 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    12797 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2383 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2216 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0     8120 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2460 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0     3514 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     3712 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1209 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1212 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1809 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4575 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2339 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1564 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     1313 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     2755 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3662 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7298 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2411 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     5782 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3304 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4505 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4245 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4029 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4388 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4312 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3031 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4394 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4202 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4132 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5240 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4619 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5261 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4754 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5474 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4360 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1314 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1638 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3428 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3282 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2771 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2685 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     3620 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1737 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     1006 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0     1413 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     2638 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     1093 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/list.py
--rw-r--r--   0        0        0     1885 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4044 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4069 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     2207 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1587 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3409 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     3044 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     1660 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   153585 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4352 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     1800 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4309 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     8016 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1532 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     2617 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     6909 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0     2765 2023-05-20 17:33:19.943605 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0        0        0     1431 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3755 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2291 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4389 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     3601 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3204 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1565 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6351 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     3862 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/object.py
--rw-r--r--   0        0        0     1030 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/update.py
--rw-r--r--   0        0        0     3063 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0    33966 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2236 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0    22023 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5514 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4579 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4245 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     1054 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0        0        0     2564 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9444 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     3674 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0     4718 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3967 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     2592 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0        0        0     5300 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2356 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     2682 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2422 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     4970 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0        0        0     1043 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0        0        0     1850 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0        0        0     1861 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0        0        0     1047 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0        0        0     1047 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1051 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     1951 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1329 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0        0        0     1293 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0        0        0     1663 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    13658 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1691 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1346 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1610 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0        0        0     1531 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0    10911 2023-05-20 17:33:19.947608 pyrofork_dev-2.1.8.dev202305201733/pyrogram/utils.py
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 pyrofork_dev-2.1.8.dev202305201733/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.844792 PyroFork-dev-2.1.8.dev202305201740/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-20 17:40:44.844792 PyroFork-dev-2.1.8.dev202305201740/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.712792 PyroFork-dev-2.1.8.dev202305201740/PyroFork_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-20 17:40:44.000000 PyroFork-dev-2.1.8.dev202305201740/PyroFork_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-05-20 17:40:44.000000 PyroFork-dev-2.1.8.dev202305201740/PyroFork_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:40:44.000000 PyroFork-dev-2.1.8.dev202305201740/PyroFork_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 17:40:44.000000 PyroFork-dev-2.1.8.dev202305201740/PyroFork_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 17:40:44.000000 PyroFork-dev-2.1.8.dev202305201740/PyroFork_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-20 17:40:44.000000 PyroFork-dev-2.1.8.dev202305201740/PyroFork_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.712792 PyroFork-dev-2.1.8.dev202305201740/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.712792 PyroFork-dev-2.1.8.dev202305201740/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.712792 PyroFork-dev-2.1.8.dev202305201740/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   169763 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.716792 PyroFork-dev-2.1.8.dev202305201740/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.716792 PyroFork-dev-2.1.8.dev202305201740/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.716792 PyroFork-dev-2.1.8.dev202305201740/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.716792 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.716792 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22642 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.716792 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.720792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-20 17:40:35.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40792 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.720792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.720792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.724792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.724792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.728792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.728792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.732792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.732792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.736792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.740792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.744792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.756792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.756792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.760792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.764792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.780792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12828 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20821 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12198 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.780792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.780792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.784792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.788792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.792792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.792792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.796792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.796792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.796792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.800792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.800792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.804792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.804792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.812792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.820792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.820792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.820792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.828792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153585 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.840792 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 17:40:44.844792 PyroFork-dev-2.1.8.dev202305201740/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-20 17:40:35.000000 PyroFork-dev-2.1.8.dev202305201740/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.844792 PyroFork-dev-2.1.8.dev202305201740/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.844792 PyroFork-dev-2.1.8.dev202305201740/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 17:40:44.844792 PyroFork-dev-2.1.8.dev202305201740/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-20 17:40:22.000000 PyroFork-dev-2.1.8.dev202305201740/tests/test_file_id.py
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/README.md` & `PyroFork-dev-2.1.8.dev202305201740/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -52,20 +52,12 @@
 
 ### Installing
 
 ``` bash
 pip3 install pyrofork
 ```
 
-### Install from source
-
-```bash
-git clone https://github.com/Mayuri-Chan/pyrofork.git -b master
-cd pyrofork
-make install
-```
-
 ### Resources
 
 - Check out the docs at https://pyrofork.mayuri.my.id to learn more about PyroFork, get started right
 away and discover more in-depth material for building your client applications.
```

#### html2text {}

```diff
@@ -15,12 +15,10 @@
 usages. - **Elegant**: Low-level details are abstracted and re-presented in a
 more convenient way. - **Fast**: Boosted up by [TgCrypto](https://github.com/
 pyrogram/tgcrypto), a high-performance cryptography library written in C. -
 **Type-hinted**: Types and methods are all type-hinted, enabling excellent
 editor support. - **Async**: Fully asynchronous (also usable synchronously if
 wanted, for convenience). - **Powerful**: Full access to Telegram's API to
 execute any official client action and more. ### Installing ``` bash pip3
-install pyrofork ``` ### Install from source ```bash git clone https://
-github.com/Mayuri-Chan/pyrofork.git -b master cd pyrofork make install ``` ###
-Resources - Check out the docs at https://pyrofork.mayuri.my.id to learn more
-about PyroFork, get started right away and discover more in-depth material for
-building your client applications.
+install pyrofork ``` ### Resources - Check out the docs at https://
+pyrofork.mayuri.my.id to learn more about PyroFork, get started right away and
+discover more in-depth material for building your client applications.
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork-dev"
-__version__ = "2.1.8.dev202305201733"
+__version__ = "2.1.8.dev202305201740"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/client.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/connection.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/aes.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/mtproto.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/prime.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/crypto/rsa.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/dispatcher.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/emoji.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/auto_name.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_action.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_event_action.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_member_status.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_members_filter.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/chat_type.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/message_entity_type.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/message_media_type.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/message_service_type.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/messages_filter.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/next_code_type.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/parse_mode.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/poll_type.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/sent_code_type.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/enums/user_status.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# Pyrogram - Telegram MTProto API Client Library for Python
-# Copyright (C) 2017-present Dan <https://github.com/delivrance>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-# This file is part of Pyrogram.
+#  This file is part of Pyrogram.
 #
-# Pyrogram is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published
-# by the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+#  Pyrogram is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
 #
-# Pyrogram is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#  Pyrogram is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+#  You should have received a copy of the GNU Lesser General Public License
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .see_other_303 import *
-from .service_unavailable_503 import *
-from .internal_server_error_500 import *
-from .forbidden_403 import *
-from .flood_420 import *
-from .unauthorized_401 import *
-from .not_acceptable_406 import *
-from .bad_request_400 import *
+from .bool import Bool, BoolFalse, BoolTrue
+from .bytes import Bytes
+from .double import Double
+from .int import Int, Long, Int128, Int256
+from .string import String
+from .vector import Vector
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/exceptions/service_unavailable_503.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-# Pyrogram - Telegram MTProto API Client Library for Python
-# Copyright (C) 2017-present Dan <https://github.com/delivrance>
+#  Pyrogram - Telegram MTProto API Client Library for Python
+#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
 #
-# This file is part of Pyrogram.
+#  This file is part of Pyrogram.
 #
-# Pyrogram is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published
-# by the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
+#  Pyrogram is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU Lesser General Public License as published
+#  by the Free Software Foundation, either version 3 of the License, or
+#  (at your option) any later version.
 #
-# Pyrogram is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Lesser General Public License for more details.
+#  Pyrogram is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU Lesser General Public License for more details.
 #
-# You should have received a copy of the GNU Lesser General Public License
-# along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
-
-from ..rpc_error import RPCError
-
-
-class ServiceUnavailable(RPCError):
-    """Service Unavailable"""
-    CODE = 503
-    """``int``: RPC Error Code"""
-    NAME = __doc__
-
-
-class ApiCallError(ServiceUnavailable):
-    """Telegram is having internal problems. Please try again later."""
-    ID = "ApiCallError"
-    """``str``: RPC Error ID"""
-    MESSAGE = __doc__
-
-
-class Timeout(ServiceUnavailable):
-    """Telegram is having internal problems. Please try again later."""
-    ID = "Timeout"
-    """``str``: RPC Error ID"""
-    MESSAGE = __doc__
-
-
+#  You should have received a copy of the GNU Lesser General Public License
+#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+import pyrogram
+from pyrogram import raw
+from pyrogram import types
+from typing import Union
+
+
+class ReopenGeneralTopic:
+    async def reopen_general_topic(
+        self: "pyrogram.Client",
+        chat_id: Union[int, str]
+    ) -> bool:
+        """Reopen a general forum topic.
+
+        .. include:: /_includes/usable-by/users-bots.rst
+
+        Parameters:
+            chat_id (``int`` | ``str``):
+                Unique identifier (int) or username (str) of the target chat.
+
+        Returns:
+            `bool`: On success, a True is returned.
+
+        Example:
+            .. code-block:: python
+
+                await app.reopen_general_topic(chat_id, topic_id)
+        """
+        await self.invoke(
+            raw.functions.channels.EditForumTopic(
+                channel=await self.resolve_peer(chat_id),
+                topic_id=1,
+                closed=False
+            )
+        )
+        return True
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/errors/rpc_error.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/file_id.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/filters.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/callback_query_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/disconnect_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/edited_message_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/inline_query_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/message_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/poll_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/raw_update_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/handlers/user_status_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/invoke.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/advanced/save_file.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/check_password.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/connect.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/disconnect.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/initialize.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/log_out.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/recover_password.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/resend_code.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/send_code.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/sign_in.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/sign_up.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/auth/terminate.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/send_game.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/bots/set_game_score.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/archive_chats.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_channel.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_group.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_channel.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/join_chat.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/leave_chat.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,42 +11,31 @@
 #  Pyrogram is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+
 import pyrogram
 from pyrogram import raw
-from pyrogram import types
-from typing import Union
 
 
-class ReopenGeneralTopic:
-    async def reopen_general_topic(
-        self: "pyrogram.Client",
-        chat_id: Union[int, str]
-    ) -> bool:
-        """Reopen a general forum topic.
-
-        .. include:: /_includes/usable-by/users-bots.rst
-
-        Parameters:
-            chat_id (``int`` | ``str``):
-                Unique identifier (int) or username (str) of the target chat.
+class GetContactsCount:
+    async def get_contacts_count(
+        self: "pyrogram.Client"
+    ) -> int:
+        """Get the total count of contacts from your Telegram address book.
+
+        .. include:: /_includes/usable-by/users.rst
 
         Returns:
-            `bool`: On success, a True is returned.
+            ``int``: On success, the contacts count is returned.
 
         Example:
             .. code-block:: python
 
-                await app.reopen_general_topic(chat_id, topic_id)
+                count = await app.get_contacts_count()
+                print(count)
         """
-        await self.invoke(
-            raw.functions.channels.EditForumTopic(
-                channel=await self.resolve_peer(chat_id),
-                topic_id=1,
-                closed=False
-            )
-        )
-        return True
+
+        return len((await self.invoke(raw.functions.contacts.GetContacts(hash=0))).contacts)
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/add_contact.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/update.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,29 +13,17 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
-from pyrogram import raw
 
 
-class GetContactsCount:
-    async def get_contacts_count(
-        self: "pyrogram.Client"
-    ) -> int:
-        """Get the total count of contacts from your Telegram address book.
-
-        .. include:: /_includes/usable-by/users.rst
-
-        Returns:
-            ``int``: On success, the contacts count is returned.
-
-        Example:
-            .. code-block:: python
-
-                count = await app.get_contacts_count()
-                print(count)
-        """
-
-        return len((await self.invoke(raw.functions.contacts.GetContacts(hash=0))).contacts)
+class Update:
+    @staticmethod
+    def stop_propagation():
+        raise pyrogram.StopPropagation
+
+    @staticmethod
+    def continue_propagation():
+        raise pyrogram.ContinuePropagation
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_poll.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/copy_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/delete_messages.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/download_media.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/forward_messages.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_media_group.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/get_messages.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/inline_session.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/retract_vote.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_global.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_global_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_messages.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_animation.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_audio.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_contact.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_dice.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_document.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_location.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_media_group.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_photo.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_poll.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_reaction.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_sticker.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_venue.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_video.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_video_note.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/send_voice.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/stop_poll.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/stream_media.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/messages/vote_poll.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/add_sticker_to_set.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/create_sticker_set.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/stickers/get_sticker_set.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/block_user.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_common_chats.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_me.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/get_users.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/set_username.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/unblock_user.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/users/update_profile.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/add_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/compose.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/idle.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/restart.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/run.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/start.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/stop.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/mime_types.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/html.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/markdown.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/parser.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/parser/utils.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/access_point_rule.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,42 +12,47 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-AccessPointRule = Union[raw.types.AccessPointRule]
+from ..object import Object
 
 
-# noinspection PyRedeclaration
-class AccessPointRule:  # type: ignore
-    """Telegram API base type.
+class ForumTopicEdited(Object):
+    """A service message about a forum topic renamed in the chat.
 
-    Constructors:
-        This base type has 1 constructor available.
 
-        .. currentmodule:: pyrogram.raw.types
+    Parameters:
+        title (``String``):
+            Name of the topic.
 
-        .. autosummary::
-            :nosignatures:
+        icon_color (``Integer``):
+            Color of the topic icon in RGB format
 
-            AccessPointRule
+        icon_custom_emoji_id (``String``, *optional*):
+            Unique identifier of the custom emoji shown as the topic icon
     """
 
-    QUALNAME = "pyrogram.raw.base.AccessPointRule"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/access-point-rule")
+    def __init__(
+        self, *,
+        title: str = None,
+        icon_color: int = None,
+        icon_emoji_id: str = None
+    ):
+        super().__init__()
+
+        self.title = title
+        self.icon_color = icon_color
+        self.icon_emoji_id = icon_emoji_id
+
+    @staticmethod
+    def _parse(action: "raw.types.MessageActionTopicEdit") -> "ForumTopicEdited":
+
+
+        return ForumTopicEdited(
+            title=getattr(action,"title", None),
+            icon_color=getattr(action,"icon_color", None),
+            icon_emoji_id=getattr(action,"icon_emoji_id", None)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/account_days_ttl.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,52 +12,37 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
 from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-AccountDaysTTL = Union[raw.types.AccountDaysTTL]
-
-
-# noinspection PyRedeclaration
-class AccountDaysTTL:  # type: ignore
-    """Telegram API base type.
 
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            AccountDaysTTL
+import pyrogram
+from pyrogram import raw
+from .bot_command_scope import BotCommandScope
 
-    Functions:
-        This object can be returned by 1 function.
 
-        .. currentmodule:: pyrogram.raw.functions
+class BotCommandScopeChatMember(BotCommandScope):
+    """Represents the scope of bot commands, covering a specific member of a group or supergroup chat.
 
-        .. autosummary::
-            :nosignatures:
+    Parameters:
+        chat_id (``int`` | ``str``):
+            Unique identifier for the target chat or username of the target supergroup (in the format
+            @supergroupusername).
 
-            account.GetAccountTTL
+        user_id (``int`` | ``str``):
+            Unique identifier of the target user.
     """
 
-    QUALNAME = "pyrogram.raw.base.AccountDaysTTL"
+    def __init__(self, chat_id: Union[int, str], user_id: Union[int, str]):
+        super().__init__("chat_member")
+
+        self.chat_id = chat_id
+        self.user_id = user_id
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/account-days-ttl")
+    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
+        return raw.types.BotCommandScopePeerUser(
+            peer=await client.resolve_peer(self.chat_id),
+            user_id=await client.resolve_peer(self.user_id)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/app_web_view_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,52 +12,39 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from typing import List, Dict
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from pyrogram import raw, types
+from ..object import Object
 
-AppWebViewResult = Union[raw.types.AppWebViewResultUrl]
 
+class VideoChatMembersInvited(Object):
+    """A service message about new members invited to a voice chat.
 
-# noinspection PyRedeclaration
-class AppWebViewResult:  # type: ignore
-    """Telegram API base type.
 
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            AppWebViewResultUrl
-
-    Functions:
-        This object can be returned by 1 function.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            messages.RequestAppWebView
+    Parameters:
+        users (List of :obj:`~pyrogram.types.User`):
+            New members that were invited to the voice chat.
     """
 
-    QUALNAME = "pyrogram.raw.base.AppWebViewResult"
+    def __init__(
+        self, *,
+        users: List["types.User"]
+    ):
+        super().__init__()
+
+        self.users = users
+
+    @staticmethod
+    def _parse(
+        client,
+        action: "raw.types.MessageActionInviteToGroupCall",
+        users: Dict[int, "raw.types.User"]
+    ) -> "VideoChatMembersInvited":
+        users = [types.User._parse(client, users[i]) for i in action.users]
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/app-web-view-result")
+        return VideoChatMembersInvited(users=users)
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bot.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,42 +12,47 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-AttachMenuBot = Union[raw.types.AttachMenuBot]
+from ..object import Object
 
 
-# noinspection PyRedeclaration
-class AttachMenuBot:  # type: ignore
-    """Telegram API base type.
+class ForumTopicCreated(Object):
+    """A service message about a new forum topic created in the chat.
 
-    Constructors:
-        This base type has 1 constructor available.
 
-        .. currentmodule:: pyrogram.raw.types
+    Parameters:
+        title (``String``):
+            Name of the topic.
 
-        .. autosummary::
-            :nosignatures:
+        icon_color (``Integer``):
+            Color of the topic icon in RGB format
 
-            AttachMenuBot
+        icon_emoji_id (``Integer``, *optional*):
+            Unique identifier of the custom emoji shown as the topic icon
     """
 
-    QUALNAME = "pyrogram.raw.base.AttachMenuBot"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/attach-menu-bot")
+    def __init__(
+        self, *,
+        title: str,
+        icon_color: int,
+        icon_emoji_id: int = None
+    ):
+        super().__init__()
+
+        self.title = title
+        self.icon_color = icon_color
+        self.icon_emoji_id = icon_emoji_id
+
+    @staticmethod
+    def _parse(action: "raw.types.MessageActionTopicCreate") -> "ForumTopicCreated":
+
+
+        return ForumTopicCreated(
+            title=getattr(action,"title", None),
+            icon_color=getattr(action,"icon_color", None),
+            icon_emoji_id=getattr(action,"icon_emoji_id", None)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bot_icon.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/location.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,42 +12,44 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+import pyrogram
 
-from typing import Union
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from ..object import Object
 
-AttachMenuBotIcon = Union[raw.types.AttachMenuBotIcon]
 
+class Location(Object):
+    """A point on the map.
 
-# noinspection PyRedeclaration
-class AttachMenuBotIcon:  # type: ignore
-    """Telegram API base type.
+    Parameters:
+        longitude (``float``):
+            Longitude as defined by sender.
 
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            AttachMenuBotIcon
+        latitude (``float``):
+            Latitude as defined by sender.
     """
 
-    QUALNAME = "pyrogram.raw.base.AttachMenuBotIcon"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/attach-menu-bot-icon")
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        longitude: float,
+        latitude: float
+    ):
+        super().__init__(client)
+
+        self.longitude = longitude
+        self.latitude = latitude
+
+    @staticmethod
+    def _parse(client, geo_point: "raw.types.GeoPoint") -> "Location":
+        if isinstance(geo_point, raw.types.GeoPoint):
+            return Location(
+                longitude=geo_point.long,
+                latitude=geo_point.lat,
+                client=client
+            )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bot_icon_color.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,42 +12,45 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from typing import Optional, List
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+import pyrogram
+from pyrogram import raw, types
+from ..object import Object
 
-AttachMenuBotIconColor = Union[raw.types.AttachMenuBotIconColor]
 
+class MessageReactions(Object):
+    """Contains information about a message reactions.
 
-# noinspection PyRedeclaration
-class AttachMenuBotIconColor:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            AttachMenuBotIconColor
+    Parameters:
+        reactions (List of :obj:`~pyrogram.types.Reaction`):
+            Reactions list.
     """
 
-    QUALNAME = "pyrogram.raw.base.AttachMenuBotIconColor"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/attach-menu-bot-icon-color")
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        reactions: Optional[List["types.Reaction"]] = None,
+    ):
+        super().__init__(client)
+
+        self.reactions = reactions
+
+    @staticmethod
+    def _parse(
+        client: "pyrogram.Client",
+        message_reactions: Optional["raw.base.MessageReactions"] = None
+    ) -> Optional["MessageReactions"]:
+        if not message_reactions:
+            return None
+
+        return MessageReactions(
+            client=client,
+            reactions=[types.Reaction._parse_count(client, reaction)
+                       for reaction in message_reactions.results]
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/attach_menu_bots_bot.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/poll_option.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,52 +12,39 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+import pyrogram
+from ..object import Object
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
 
-AttachMenuBotsBot = Union[raw.types.AttachMenuBotsBot]
+class PollOption(Object):
+    """Contains information about one answer option in a poll.
 
+    Parameters:
+        text (``str``):
+            Option text, 1-100 characters.
 
-# noinspection PyRedeclaration
-class AttachMenuBotsBot:  # type: ignore
-    """Telegram API base type.
+        voter_count (``int``):
+            Number of users that voted for this option.
+            Equals to 0 until you vote.
 
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            AttachMenuBotsBot
-
-    Functions:
-        This object can be returned by 1 function.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            messages.GetAttachMenuBot
+        data (``bytes``):
+            The data this poll option is holding.
     """
 
-    QUALNAME = "pyrogram.raw.base.AttachMenuBotsBot"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/attach-menu-bots-bot")
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        text: str,
+        voter_count: int,
+        data: bytes
+    ):
+        super().__init__(client)
+
+        self.text = text
+        self.voter_count = voter_count
+        self.data = data
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/auto_save_settings.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/msg_id.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,42 +12,34 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-AutoSaveSettings = Union[raw.types.AutoSaveSettings]
-
-
-# noinspection PyRedeclaration
-class AutoSaveSettings:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            AutoSaveSettings
-    """
-
-    QUALNAME = "pyrogram.raw.base.AutoSaveSettings"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/auto-save-settings")
+import logging
+from datetime import datetime
+from time import perf_counter
+
+log = logging.getLogger(__name__)
+
+
+class MsgId:
+    reference_clock = 0
+    last_time = 0
+    msg_id_offset = 0
+    server_time = 0
+
+    def __new__(cls) -> int:
+        now = perf_counter() - cls.reference_clock + cls.server_time
+        cls.msg_id_offset = cls.msg_id_offset + 4 if now == cls.last_time else 0
+        msg_id = int(now * 2 ** 32) + cls.msg_id_offset
+        cls.last_time = now
+
+        return msg_id
+
+    @classmethod
+    def set_server_time(cls, server_time: int):
+        if not cls.server_time:
+            cls.reference_clock = perf_counter()
+            cls.server_time = server_time
+            log.info(f"Time synced: {datetime.utcfromtimestamp(server_time)} UTC")
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/available_reaction.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,42 +12,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from datetime import datetime
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from pyrogram import raw, utils
+from ..object import Object
 
-AvailableReaction = Union[raw.types.AvailableReaction]
 
+class VideoChatScheduled(Object):
+    """A service message about a voice chat scheduled in the chat.
 
-# noinspection PyRedeclaration
-class AvailableReaction:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            AvailableReaction
+    Parameters:
+        start_date (:py:obj:`~datetime.datetime`):
+            Point in time when the voice chat is supposed to be started by a chat administrator.
     """
 
-    QUALNAME = "pyrogram.raw.base.AvailableReaction"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/available-reaction")
+    def __init__(
+        self, *,
+        start_date: datetime
+    ):
+        super().__init__()
+
+        self.start_date = start_date
+
+    @staticmethod
+    def _parse(action: "raw.types.MessageActionGroupCallScheduled") -> "VideoChatScheduled":
+        return VideoChatScheduled(start_date=utils.timestamp_to_datetime(action.schedule_date))
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bank_card_open_url.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,42 +12,38 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from typing import List, Union, BinaryIO
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from ..messages_and_media import MessageEntity
+from ..object import Object
 
-BankCardOpenUrl = Union[raw.types.BankCardOpenUrl]
 
+class InputMedia(Object):
+    """Content of a media message to be sent.
 
-# noinspection PyRedeclaration
-class BankCardOpenUrl:  # type: ignore
-    """Telegram API base type.
+    It should be one of:
 
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            BankCardOpenUrl
+    - :obj:`~pyrogram.types.InputMediaAnimation`
+    - :obj:`~pyrogram.types.InputMediaDocument`
+    - :obj:`~pyrogram.types.InputMediaAudio`
+    - :obj:`~pyrogram.types.InputMediaPhoto`
+    - :obj:`~pyrogram.types.InputMediaVideo`
     """
 
-    QUALNAME = "pyrogram.raw.base.BankCardOpenUrl"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/bank-card-open-url")
+    def __init__(
+        self,
+        media: Union[str, BinaryIO],
+        caption: str = "",
+        parse_mode: str = None,
+        caption_entities: List[MessageEntity] = None
+    ):
+        super().__init__()
+
+        self.media = media
+        self.caption = caption
+        self.parse_mode = parse_mode
+        self.caption_entities = caption_entities
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/base_theme.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,46 +12,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
 from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-BaseTheme = Union[raw.types.BaseThemeArctic, raw.types.BaseThemeClassic, raw.types.BaseThemeDay, raw.types.BaseThemeNight, raw.types.BaseThemeTinted]
-
 
-# noinspection PyRedeclaration
-class BaseTheme:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 5 constructors available.
+import pyrogram
+from pyrogram import raw
+from .bot_command_scope import BotCommandScope
 
-        .. currentmodule:: pyrogram.raw.types
 
-        .. autosummary::
-            :nosignatures:
+class BotCommandScopeChat(BotCommandScope):
+    """Represents the scope of bot commands, covering a specific chat.
 
-            BaseThemeArctic
-            BaseThemeClassic
-            BaseThemeDay
-            BaseThemeNight
-            BaseThemeTinted
+    Parameters:
+        chat_id (``int`` | ``str``):
+            Unique identifier for the target chat or username of the target supergroup (in the format
+            @supergroupusername).
     """
 
-    QUALNAME = "pyrogram.raw.base.BaseTheme"
+    def __init__(self, chat_id: Union[int, str]):
+        super().__init__("chat")
+
+        self.chat_id = chat_id
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/base-theme")
+    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
+        return raw.types.BotCommandScopePeer(
+            peer=await client.resolve_peer(self.chat_id)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_app.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/double.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,43 +12,21 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from io import BytesIO
+from struct import unpack, pack
+from typing import cast, Any
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from ..tl_object import TLObject
 
-BotApp = Union[raw.types.BotApp, raw.types.BotAppNotModified]
 
+class Double(bytes, TLObject):
+    @classmethod
+    def read(cls, data: BytesIO, *args: Any) -> float:
+        return cast(float, unpack("d", data.read(8))[0])
 
-# noinspection PyRedeclaration
-class BotApp:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 2 constructors available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            BotApp
-            BotAppNotModified
-    """
-
-    QUALNAME = "pyrogram.raw.base.BotApp"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/bot-app")
+    def __new__(cls, value: float) -> bytes:  # type: ignore
+        return pack("d", value)
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_command.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,52 +12,26 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from ..object import Object
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
 
-BotCommand = Union[raw.types.BotCommand]
+class WebAppInfo(Object):
+    """Contains information about a `Web App <https://core.telegram.org/bots/webapps>`_.
 
-
-# noinspection PyRedeclaration
-class BotCommand:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            BotCommand
-
-    Functions:
-        This object can be returned by 1 function.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            bots.GetBotCommands
+    Parameters:
+        url (``str``):
+            An HTTPS URL of a Web App to be opened with additional data as specified in
+            `Initializing Web Apps <https://core.telegram.org/bots/webapps#initializing-web-apps>`_.
     """
 
-    QUALNAME = "pyrogram.raw.base.BotCommand"
+    def __init__(
+        self, *,
+        url: str,
+    ):
+        super().__init__()
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/bot-command")
+        self.url = url
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/bot_inline_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,43 +12,31 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from pyrogram import raw, utils
+from ..object import Object
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
 
-BotInlineResult = Union[raw.types.BotInlineMediaResult, raw.types.BotInlineResult]
+class SentWebAppMessage(Object):
+    """Contains information about an inline message sent by a `Web App <https://core.telegram.org/bots/webapps>`_ on behalf of a user.
 
-
-# noinspection PyRedeclaration
-class BotInlineResult:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 2 constructors available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            BotInlineMediaResult
-            BotInlineResult
+    Parameters:
+        inline_message_id (``str``):
+            Identifier of the sent inline message.
+            Available only if there is an inline keyboard attached to the message.
     """
 
-    QUALNAME = "pyrogram.raw.base.BotInlineResult"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/bot-inline-result")
+    def __init__(
+        self, *,
+        inline_message_id: str,
+    ):
+        super().__init__()
+
+        self.inline_message_id = inline_message_id
+
+    @staticmethod
+    def _parse(obj: "raw.types.WebViewMessageSent"):
+        return SentWebAppMessage(inline_message_id=utils.pack_inline_message_id(obj.msg_id))
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_participant.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/dice.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,44 +12,36 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
+import pyrogram
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-ChatParticipant = Union[raw.types.ChatParticipant, raw.types.ChatParticipantAdmin, raw.types.ChatParticipantCreator]
-
+from ..object import Object
 
-# noinspection PyRedeclaration
-class ChatParticipant:  # type: ignore
-    """Telegram API base type.
 
-    Constructors:
-        This base type has 3 constructors available.
+class Dice(Object):
+    """A dice with a random value from 1 to 6 for currently supported base emoji.
 
-        .. currentmodule:: pyrogram.raw.types
+    Parameters:
+        emoji (``string``):
+            Emoji on which the dice throw animation is based.
 
-        .. autosummary::
-            :nosignatures:
-
-            ChatParticipant
-            ChatParticipantAdmin
-            ChatParticipantCreator
+        value (``int``):
+            Value of the dice, 1-6 for currently supported base emoji.
     """
 
-    QUALNAME = "pyrogram.raw.base.ChatParticipant"
+    def __init__(self, *, client: "pyrogram.Client" = None, emoji: str, value: int):
+        super().__init__(client)
+
+        self.emoji = emoji
+        self.value = value
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/chat-participant")
+    @staticmethod
+    def _parse(client, dice: "raw.types.MessageMediaDice") -> "Dice":
+        return Dice(
+            emoji=dice.emoticon,
+            value=dice.value,
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_photo.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,43 +12,30 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-ChatPhoto = Union[raw.types.ChatPhoto, raw.types.ChatPhotoEmpty]
-
+from ..object import Object
 
-# noinspection PyRedeclaration
-class ChatPhoto:  # type: ignore
-    """Telegram API base type.
 
-    Constructors:
-        This base type has 2 constructors available.
+class VideoChatEnded(Object):
+    """A service message about a voice chat ended in the chat.
 
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            ChatPhoto
-            ChatPhotoEmpty
+    Parameters:
+        duration (``int``):
+            Voice chat duration; in seconds.
     """
 
-    QUALNAME = "pyrogram.raw.base.ChatPhoto"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/chat-photo")
+    def __init__(
+        self, *,
+        duration: int
+    ):
+        super().__init__()
+
+        self.duration = duration
+
+    @staticmethod
+    def _parse(action: "raw.types.MessageActionGroupCall") -> "VideoChatEnded":
+        return VideoChatEnded(duration=action.duration)
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/chat_reactions.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,44 +12,68 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from typing import List
 
-from typing import Union
+import pyrogram
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from pyrogram import types
+from ..object import Object
 
-ChatReactions = Union[raw.types.ChatReactionsAll, raw.types.ChatReactionsNone, raw.types.ChatReactionsSome]
 
+class ChatPreview(Object):
+    """A chat preview.
 
-# noinspection PyRedeclaration
-class ChatReactions:  # type: ignore
-    """Telegram API base type.
+    Parameters:
+        title (``str``):
+            Title of the chat.
 
-    Constructors:
-        This base type has 3 constructors available.
+        type (``str``):
+            Type of chat, can be either, "group", "supergroup" or "channel".
 
-        .. currentmodule:: pyrogram.raw.types
+        members_count (``int``):
+            Chat members count.
 
-        .. autosummary::
-            :nosignatures:
+        photo (:obj:`~pyrogram.types.Photo`, *optional*):
+            Chat photo.
 
-            ChatReactionsAll
-            ChatReactionsNone
-            ChatReactionsSome
+        members (List of :obj:`~pyrogram.types.User`, *optional*):
+            Preview of some of the chat members.
     """
 
-    QUALNAME = "pyrogram.raw.base.ChatReactions"
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        title: str,
+        type: str,
+        members_count: int,
+        photo: "types.Photo" = None,
+        members: List["types.User"] = None
+    ):
+        super().__init__(client)
+
+        self.title = title
+        self.type = type
+        self.members_count = members_count
+        self.photo = photo
+        self.members = members
+
+    @staticmethod
+    def _parse(client, chat_invite: "raw.types.ChatInvite") -> "ChatPreview":
+        return ChatPreview(
+            title=chat_invite.title,
+            type=("group" if not chat_invite.channel else
+                  "channel" if chat_invite.broadcast else
+                  "supergroup"),
+            members_count=chat_invite.participants_count,
+            photo=types.Photo._parse(client, chat_invite.photo),
+            members=[types.User._parse(client, user) for user in chat_invite.participants] or None,
+            client=client
+        )
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/chat-reactions")
+    # TODO: Maybe just merge this object into Chat itself by adding the "members" field.
+    #  get_chat can be used as well instead of get_chat_preview
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/contact_status.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,52 +12,65 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from typing import List
 
-from typing import Union
+import pyrogram
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from pyrogram import types
+from ..object import Object
 
-ContactStatus = Union[raw.types.ContactStatus]
 
+class InlineKeyboardMarkup(Object):
+    """An inline keyboard that appears right next to the message it belongs to.
 
-# noinspection PyRedeclaration
-class ContactStatus:  # type: ignore
-    """Telegram API base type.
+    Parameters:
+        inline_keyboard (List of List of :obj:`~pyrogram.types.InlineKeyboardButton`):
+            List of button rows, each represented by a List of InlineKeyboardButton objects.
+    """
 
-    Constructors:
-        This base type has 1 constructor available.
+    def __init__(self, inline_keyboard: List[List["types.InlineKeyboardButton"]]):
+        super().__init__()
 
-        .. currentmodule:: pyrogram.raw.types
+        self.inline_keyboard = inline_keyboard
 
-        .. autosummary::
-            :nosignatures:
+    @staticmethod
+    def read(o):
+        inline_keyboard = []
 
-            ContactStatus
+        for i in o.rows:
+            row = []
 
-    Functions:
-        This object can be returned by 1 function.
+            for j in i.buttons:
+                row.append(types.InlineKeyboardButton.read(j))
 
-        .. currentmodule:: pyrogram.raw.functions
+            inline_keyboard.append(row)
 
-        .. autosummary::
-            :nosignatures:
+        return InlineKeyboardMarkup(
+            inline_keyboard=inline_keyboard
+        )
 
-            contacts.GetStatuses
-    """
+    async def write(self, client: "pyrogram.Client"):
+        rows = []
+
+        for r in self.inline_keyboard:
+            buttons = []
+
+            for b in r:
+                buttons.append(await b.write(client))
+
+            rows.append(raw.types.KeyboardButtonRow(buttons=buttons))
 
-    QUALNAME = "pyrogram.raw.base.ContactStatus"
+        return raw.types.ReplyInlineMarkup(rows=rows)
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/contact-status")
+        # There seems to be a Python issues with nested async comprehensions.
+        # See: https://bugs.python.org/issue33346
+        #
+        # return raw.types.ReplyInlineMarkup(
+        #     rows=[raw.types.KeyboardButtonRow(
+        #         buttons=[await j.write(client) for j in i]
+        #     ) for i in self.inline_keyboard]
+        # )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/data_json.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/msg_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,53 +12,27 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from pyrogram.raw.core import Message, MsgContainer, TLObject
+from pyrogram.raw.functions import Ping
+from pyrogram.raw.types import MsgsAck, HttpWait
+from .msg_id import MsgId
+from .seq_no import SeqNo
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+not_content_related = (Ping, HttpWait, MsgsAck, MsgContainer)
 
-DataJSON = Union[raw.types.DataJSON]
-
-
-# noinspection PyRedeclaration
-class DataJSON:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            DataJSON
-
-    Functions:
-        This object can be returned by 2 functions.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            bots.SendCustomRequest
-            phone.GetCallConfig
-    """
-
-    QUALNAME = "pyrogram.raw.base.DataJSON"
 
+class MsgFactory:
     def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/data-json")
+        self.seq_no = SeqNo()
+
+    def __call__(self, body: TLObject) -> Message:
+        return Message(
+            body,
+            MsgId(),
+            self.seq_no(not isinstance(body, not_content_related)),
+            len(body)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/destroy_auth_key_res.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/bytes.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,54 +12,44 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from io import BytesIO
+from typing import Any
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from ..tl_object import TLObject
 
-DestroyAuthKeyRes = Union[raw.types.DestroyAuthKeyFail, raw.types.DestroyAuthKeyNone, raw.types.DestroyAuthKeyOk]
 
-
-# noinspection PyRedeclaration
-class DestroyAuthKeyRes:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 3 constructors available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            DestroyAuthKeyFail
-            DestroyAuthKeyNone
-            DestroyAuthKeyOk
-
-    Functions:
-        This object can be returned by 1 function.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            DestroyAuthKey
-    """
-
-    QUALNAME = "pyrogram.raw.base.DestroyAuthKeyRes"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/destroy-auth-key-res")
+class Bytes(bytes, TLObject):
+    @classmethod
+    def read(cls, data: BytesIO, *args: Any) -> bytes:
+        length = int.from_bytes(data.read(1), "little")
+
+        if length <= 253:
+            x = data.read(length)
+            data.read(-(length + 1) % 4)
+        else:
+            length = int.from_bytes(data.read(3), "little")
+            x = data.read(length)
+            data.read(-length % 4)
+
+        return x
+
+    def __new__(cls, value: bytes) -> bytes:  # type: ignore
+        length = len(value)
+
+        if length <= 253:
+            return (
+                bytes([length])
+                + value
+                + bytes(-(length + 1) % 4)
+            )
+        else:
+            return (
+                bytes([254])
+                + length.to_bytes(3, "little")
+                + value
+                + bytes(-length % 4)
+            )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/destroy_session_res.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/msg_container.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,53 +12,42 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from io import BytesIO
+from typing import List, Any
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from .message import Message
+from .primitives.int import Int
+from .tl_object import TLObject
 
-DestroySessionRes = Union[raw.types.DestroySessionNone, raw.types.DestroySessionOk]
 
+class MsgContainer(TLObject):
+    ID = 0x73F1F8DC
 
-# noinspection PyRedeclaration
-class DestroySessionRes:  # type: ignore
-    """Telegram API base type.
+    __slots__ = ["messages"]
 
-    Constructors:
-        This base type has 2 constructors available.
+    QUALNAME = "MsgContainer"
 
-        .. currentmodule:: pyrogram.raw.types
+    def __init__(self, messages: List[Message]):
+        self.messages = messages
 
-        .. autosummary::
-            :nosignatures:
+    @staticmethod
+    def read(data: BytesIO, *args: Any) -> "MsgContainer":
+        count = Int.read(data)
+        return MsgContainer([Message.read(data) for _ in range(count)])
 
-            DestroySessionNone
-            DestroySessionOk
+    def write(self, *args: Any) -> bytes:
+        b = BytesIO()
 
-    Functions:
-        This object can be returned by 1 function.
+        b.write(Int(self.ID, False))
 
-        .. currentmodule:: pyrogram.raw.functions
+        count = len(self.messages)
+        b.write(Int(count))
 
-        .. autosummary::
-            :nosignatures:
+        for message in self.messages:
+            b.write(message.write())
 
-            DestroySession
-    """
-
-    QUALNAME = "pyrogram.raw.base.DestroySessionRes"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/destroy-session-res")
+        return b.getvalue()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/dialog_filter_suggested.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/venue.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,52 +12,63 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
+import pyrogram
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-DialogFilterSuggested = Union[raw.types.DialogFilterSuggested]
-
+from pyrogram import types
+from ..object import Object
 
-# noinspection PyRedeclaration
-class DialogFilterSuggested:  # type: ignore
-    """Telegram API base type.
 
-    Constructors:
-        This base type has 1 constructor available.
+class Venue(Object):
+    """A venue.
 
-        .. currentmodule:: pyrogram.raw.types
+    Parameters:
+        location (:obj:`~pyrogram.types.Location`):
+            Venue location.
 
-        .. autosummary::
-            :nosignatures:
+        title (``str``):
+            Name of the venue.
 
-            DialogFilterSuggested
+        address (``str``):
+            Address of the venue.
 
-    Functions:
-        This object can be returned by 1 function.
+        foursquare_id (``str``, *optional*):
+            Foursquare identifier of the venue.
 
-        .. currentmodule:: pyrogram.raw.functions
+        foursquare_type (``str``, *optional*):
+            Foursquare type of the venue.
+            (For example, "arts_entertainment/default", "arts_entertainment/aquarium" or "food/icecream".)
 
-        .. autosummary::
-            :nosignatures:
-
-            messages.GetSuggestedDialogFilters
     """
 
-    QUALNAME = "pyrogram.raw.base.DialogFilterSuggested"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/dialog-filter-suggested")
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        location: "types.Location",
+        title: str,
+        address: str,
+        foursquare_id: str = None,
+        foursquare_type: str = None
+    ):
+        super().__init__(client)
+
+        self.location = location
+        self.title = title
+        self.address = address
+        self.foursquare_id = foursquare_id
+        self.foursquare_type = foursquare_type
+
+    @staticmethod
+    def _parse(client, venue: "raw.types.MessageMediaVenue"):
+        return Venue(
+            location=types.Location._parse(client, venue.geo),
+            title=venue.title,
+            address=venue.address,
+            foursquare_id=venue.venue_id or None,
+            foursquare_type=venue.venue_type,
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/document.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,56 +12,59 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+import pyrogram
+from pyrogram import raw, utils
+from pyrogram import types
+from ..object import Object
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
 
-Document = Union[raw.types.Document, raw.types.DocumentEmpty]
+class GameHighScore(Object):
+    """One row of the high scores table for a game.
 
+    Parameters:
+        user (:obj:`~pyrogram.types.User`):
+            User.
 
-# noinspection PyRedeclaration
-class Document:  # type: ignore
-    """Telegram API base type.
+        score (``int``):
+            Score.
 
-    Constructors:
-        This base type has 2 constructors available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            Document
-            DocumentEmpty
-
-    Functions:
-        This object can be returned by 4 functions.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            account.UploadTheme
-            account.UploadRingtone
-            messages.GetDocumentByHash
-            messages.GetCustomEmojiDocuments
+        position (``int``, *optional*):
+            Position in high score table for the game.
     """
 
-    QUALNAME = "pyrogram.raw.base.Document"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/document")
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        user: "types.User",
+        score: int,
+        position: int = None
+    ):
+        super().__init__(client)
+
+        self.user = user
+        self.score = score
+        self.position = position
+
+    @staticmethod
+    def _parse(client, game_high_score: raw.types.HighScore, users: dict) -> "GameHighScore":
+        users = {i.id: i for i in users}
+
+        return GameHighScore(
+            user=types.User._parse(client, users[game_high_score.user_id]),
+            score=game_high_score.score,
+            position=game_high_score.pos,
+            client=client
+        )
+
+    @staticmethod
+    def _parse_action(client, service: raw.types.MessageService, users: dict):
+        return GameHighScore(
+            user=types.User._parse(client, users[utils.get_raw_peer_id(service.from_id or service.peer_id)]),
+            score=service.action.score,
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/email_verify_purpose.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/contact.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,44 +12,60 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
+import pyrogram
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from ..object import Object
 
-EmailVerifyPurpose = Union[raw.types.EmailVerifyPurposeLoginChange, raw.types.EmailVerifyPurposeLoginSetup, raw.types.EmailVerifyPurposePassport]
 
+class Contact(Object):
+    """A phone contact.
 
-# noinspection PyRedeclaration
-class EmailVerifyPurpose:  # type: ignore
-    """Telegram API base type.
+    Parameters:
+        phone_number (``str``):
+            Contact's phone number.
 
-    Constructors:
-        This base type has 3 constructors available.
+        first_name (``str``):
+            Contact's first name.
 
-        .. currentmodule:: pyrogram.raw.types
+        last_name (``str``, *optional*):
+            Contact's last name.
 
-        .. autosummary::
-            :nosignatures:
+        user_id (``int``, *optional*):
+            Contact's user identifier in Telegram.
 
-            EmailVerifyPurposeLoginChange
-            EmailVerifyPurposeLoginSetup
-            EmailVerifyPurposePassport
+        vcard (``str``, *optional*):
+            Additional data about the contact in the form of a vCard.
     """
 
-    QUALNAME = "pyrogram.raw.base.EmailVerifyPurpose"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/email-verify-purpose")
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        phone_number: str,
+        first_name: str,
+        last_name: str = None,
+        user_id: int = None,
+        vcard: str = None
+    ):
+        super().__init__(client)
+
+        self.phone_number = phone_number
+        self.first_name = first_name
+        self.last_name = last_name
+        self.user_id = user_id
+        self.vcard = vcard
+
+    @staticmethod
+    def _parse(client: "pyrogram.Client", contact: "raw.types.MessageMediaContact") -> "Contact":
+        return Contact(
+            phone_number=contact.phone_number,
+            first_name=contact.first_name,
+            last_name=contact.last_name or None,
+            vcard=contact.vcard or None,
+            user_id=contact.user_id or None,
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_keyword.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/string.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,43 +12,20 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from io import BytesIO
+from typing import cast
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from .bytes import Bytes
 
-EmojiKeyword = Union[raw.types.EmojiKeyword, raw.types.EmojiKeywordDeleted]
 
+class String(Bytes):
+    @classmethod
+    def read(cls, data: BytesIO, *args) -> str:  # type: ignore
+        return cast(bytes, super(String, String).read(data)).decode(errors="replace")
 
-# noinspection PyRedeclaration
-class EmojiKeyword:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 2 constructors available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            EmojiKeyword
-            EmojiKeywordDeleted
-    """
-
-    QUALNAME = "pyrogram.raw.base.EmojiKeyword"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/emoji-keyword")
+    def __new__(cls, value: str) -> bytes:  # type: ignore
+        return super().__new__(cls, value.encode())
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/emoji_list.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/future_salt.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,55 +12,42 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from io import BytesIO
+from typing import Any
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from .primitives.int import Int, Long
+from .tl_object import TLObject
 
-EmojiList = Union[raw.types.EmojiList, raw.types.EmojiListNotModified]
 
+class FutureSalt(TLObject):
+    ID = 0x0949D9DC
 
-# noinspection PyRedeclaration
-class EmojiList:  # type: ignore
-    """Telegram API base type.
+    __slots__ = ["valid_since", "valid_until", "salt"]
 
-    Constructors:
-        This base type has 2 constructors available.
+    QUALNAME = "FutureSalt"
 
-        .. currentmodule:: pyrogram.raw.types
+    def __init__(self, valid_since: int, valid_until: int, salt: int):
+        self.valid_since = valid_since
+        self.valid_until = valid_until
+        self.salt = salt
 
-        .. autosummary::
-            :nosignatures:
+    @staticmethod
+    def read(data: BytesIO, *args: Any) -> "FutureSalt":
+        valid_since = Int.read(data)
+        valid_until = Int.read(data)
+        salt = Long.read(data)
 
-            EmojiList
-            EmojiListNotModified
+        return FutureSalt(valid_since, valid_until, salt)
 
-    Functions:
-        This object can be returned by 3 functions.
+    def write(self, *args: Any) -> bytes:
+        b = BytesIO()
 
-        .. currentmodule:: pyrogram.raw.functions
+        b.write(Int(self.valid_since))
+        b.write(Int(self.valid_until))
+        b.write(Long(self.salt))
 
-        .. autosummary::
-            :nosignatures:
-
-            account.GetDefaultProfilePhotoEmojis
-            account.GetDefaultGroupPhotoEmojis
-            messages.SearchCustomEmoji
-    """
-
-    QUALNAME = "pyrogram.raw.base.EmojiList"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/emoji-list")
+        return b.getvalue()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/error.py` & `PyroFork-dev-2.1.8.dev202305201740/compiler/errors/sort.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,42 +12,24 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+import csv
+from pathlib import Path
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+for p in Path("source").glob("*.tsv"):
+    with open(p) as f:
+        reader = csv.reader(f, delimiter="\t")
+        dct = {k: v for k, v in reader if k != "id"}
+        keys = sorted(dct)
 
-Error = Union[raw.types.Error]
+    with open(p, "w") as f:
+        f.write("id\tmessage\n")
 
+        for i, item in enumerate(keys, start=1):
+            f.write(f"{item}\t{dct[item]}")
 
-# noinspection PyRedeclaration
-class Error:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            Error
-    """
-
-    QUALNAME = "pyrogram.raw.base.Error"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/error")
+            if i != len(keys):
+                f.write("\n")
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/game.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,42 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from ..object import Object
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
 
-Game = Union[raw.types.Game]
+class VideoChatStarted(Object):
+    """A service message about a voice chat started in the chat.
 
-
-# noinspection PyRedeclaration
-class Game:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            Game
+    Currently holds no information.
     """
 
-    QUALNAME = "pyrogram.raw.base.Game"
-
     def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/game")
+        super().__init__()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/input_peer.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,48 +12,67 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-InputPeer = Union[raw.types.InputPeerChannel, raw.types.InputPeerChannelFromMessage, raw.types.InputPeerChat, raw.types.InputPeerEmpty, raw.types.InputPeerSelf, raw.types.InputPeerUser, raw.types.InputPeerUserFromMessage]
-
-
-# noinspection PyRedeclaration
-class InputPeer:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 7 constructors available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            InputPeerChannel
-            InputPeerChannelFromMessage
-            InputPeerChat
-            InputPeerEmpty
-            InputPeerSelf
-            InputPeerUser
-            InputPeerUserFromMessage
-    """
+import pyrogram
+from pyrogram import raw, types
+from .inline_query_result import InlineQueryResult
+from ...file_id import FileId
+
+
+class InlineQueryResultCachedSticker(InlineQueryResult):
+    """A link to a sticker stored on the Telegram servers
+
+    By default, this sticker will be sent by the user. Alternatively, you can use *input_message_content* to send a
+    message with the specified content instead of the sticker.
 
-    QUALNAME = "pyrogram.raw.base.InputPeer"
+    Parameters:
+        sticker_file_id (``str``):
+            A valid file identifier of the sticker.
+
+        id (``str``, *optional*):
+            Unique identifier for this result, 1-64 bytes.
+            Defaults to a randomly generated UUID4.
+
+        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
+            An InlineKeyboardMarkup object.
+
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
+            Content of the message to be sent instead of the photo.
+    """
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/input-peer")
+    def __init__(
+        self,
+        sticker_file_id: str,
+        id: str = None,
+        reply_markup: "types.InlineKeyboardMarkup" = None,
+        input_message_content: "types.InputMessageContent" = None
+    ):
+        super().__init__("sticker", id, input_message_content, reply_markup)
+
+        self.sticker_file_id = sticker_file_id
+        self.reply_markup = reply_markup
+        self.input_message_content = input_message_content
+
+    async def write(self, client: "pyrogram.Client"):
+        file_id = FileId.decode(self.sticker_file_id)
+
+        return raw.types.InputBotInlineResultDocument(
+            id=self.id,
+            type=self.type,
+            document=raw.types.InputDocument(
+                id=file_id.media_id,
+                access_hash=file_id.access_hash,
+                file_reference=file_id.file_reference,
+            ),
+            send_message=(
+                await self.input_message_content.write(client, self.reply_markup)
+                if self.input_message_content
+                else raw.types.InputBotInlineMessageMediaAuto(
+                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
+                    message="",
+                )
+            )
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/message_extended_media.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_document.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,43 +12,54 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from typing import Optional, List, Union, BinaryIO
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from .input_media import InputMedia
+from ..messages_and_media import MessageEntity
+from ... import enums
+
+
+class InputMediaDocument(InputMedia):
+    """A generic file to be sent inside an album.
+
+    Parameters:
+        media (``str`` | ``BinaryIO``):
+            File to send.
+            Pass a file_id as string to send a file that exists on the Telegram servers or
+            pass a file path as string to upload a new file that exists on your local machine or
+            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
+            pass an HTTP URL as a string for Telegram to get a file from the Internet.
+
+        thumb (``str``):
+            Thumbnail of the file sent.
+            The thumbnail should be in JPEG format and less than 200 KB in size.
+            A thumbnail's width and height should not exceed 320 pixels.
+            Thumbnails can't be reused and can be only uploaded as a new file.
+
+        caption (``str``, *optional*):
+            Caption of the document to be sent, 0-1024 characters.
+            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
+
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
 
-MessageExtendedMedia = Union[raw.types.MessageExtendedMedia, raw.types.MessageExtendedMediaPreview]
-
-
-# noinspection PyRedeclaration
-class MessageExtendedMedia:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 2 constructors available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            MessageExtendedMedia
-            MessageExtendedMediaPreview
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
     """
 
-    QUALNAME = "pyrogram.raw.base.MessageExtendedMedia"
+    def __init__(
+        self,
+        media: Union[str, BinaryIO],
+        thumb: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List[MessageEntity] = None
+    ):
+        super().__init__(media, caption, parse_mode, caption_entities)
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/message-extended-media")
+        self.thumb = thumb
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/msg_resend_req.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,43 +12,33 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-from typing import Union
+import pyrogram
 from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-MsgResendReq = Union[raw.types.MsgResendAnsReq, raw.types.MsgResendReq]
+from ..object import Object
 
 
-# noinspection PyRedeclaration
-class MsgResendReq:  # type: ignore
-    """Telegram API base type.
+class MenuButton(Object):
+    """Describes the bot's menu button in a private chat.
 
-    Constructors:
-        This base type has 2 constructors available.
+    It should be one of:
 
-        .. currentmodule:: pyrogram.raw.types
+    - :obj:`~pyrogram.types.MenuButtonCommands`
+    - :obj:`~pyrogram.types.MenuButtonWebApp`
+    - :obj:`~pyrogram.types.MenuButtonDefault`
 
-        .. autosummary::
-            :nosignatures:
-
-            MsgResendAnsReq
-            MsgResendReq
+    If a menu button other than :obj:`~pyrogram.types.MenuButtonDefault` is set for a private chat, then it is applied
+    in the chat. Otherwise the default menu button is applied. By default, the menu button opens the list of bot
+    commands.
     """
 
-    QUALNAME = "pyrogram.raw.base.MsgResendReq"
+    def __init__(self, type: str):
+        super().__init__()
+
+        self.type = type
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/msg-resend-req")
+    async def write(self, client: "pyrogram.Client") -> "raw.base.BotMenuButton":
+        raise NotImplementedError
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/page.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/seq_no.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,42 +12,23 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from threading import Lock
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
 
-Page = Union[raw.types.Page]
-
-
-# noinspection PyRedeclaration
-class Page:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
+class SeqNo:
+    def __init__(self):
+        self.content_related_messages_sent = 0
+        self.lock = Lock()
 
-            Page
-    """
+    def __call__(self, is_content_related: bool) -> int:
+        with self.lock:
+            seq_no = (self.content_related_messages_sent * 2) + (1 if is_content_related else 0)
 
-    QUALNAME = "pyrogram.raw.base.Page"
+            if is_content_related:
+                self.content_related_messages_sent += 1
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/page")
+            return seq_no
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/phone_connection.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,43 +12,58 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from typing import Optional, List
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+import pyrogram
+from pyrogram import raw, types
+from ..object import Object
 
-PhoneConnection = Union[raw.types.PhoneConnection, raw.types.PhoneConnectionWebrtc]
 
+class ChatReactions(Object):
+    """A chat reactions
 
-# noinspection PyRedeclaration
-class PhoneConnection:  # type: ignore
-    """Telegram API base type.
+    Parameters:
+        all_are_enabled (``bool``, *optional*)
 
-    Constructors:
-        This base type has 2 constructors available.
+        allow_custom_emoji (``bool``, *optional*):
+            Whether custom emoji are allowed or not.
 
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            PhoneConnection
-            PhoneConnectionWebrtc
+        reactions (List of :obj:`~pyrogram.types.Reaction`, *optional*):
+            Reactions available.
     """
 
-    QUALNAME = "pyrogram.raw.base.PhoneConnection"
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        all_are_enabled: Optional[bool] = None,
+        allow_custom_emoji: Optional[bool] = None,
+        reactions: Optional[List["types.Reaction"]] = None,
+    ):
+        super().__init__(client)
+
+        self.all_are_enabled = all_are_enabled
+        self.allow_custom_emoji = allow_custom_emoji
+        self.reactions = reactions
+
+    @staticmethod
+    def _parse(client, chat_reactions: "raw.base.ChatReactions") -> Optional["ChatReactions"]:
+        if isinstance(chat_reactions, raw.types.ChatReactionsAll):
+            return ChatReactions(
+                client=client,
+                all_are_enabled=True,
+                allow_custom_emoji=chat_reactions.allow_custom
+            )
+
+        if isinstance(chat_reactions, raw.types.ChatReactionsSome):
+            return ChatReactions(
+                client=client,
+                reactions=[types.Reaction._parse(client, reaction)
+                           for reaction in chat_reactions.reactions]
+            )
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/phone-connection")
+        return None
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/pong.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,53 +12,50 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from datetime import datetime
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from pyrogram import raw, utils
+from pyrogram import types
+from ..object import Object
 
-Pong = Union[raw.types.Pong]
 
+class InviteLinkImporter(Object):
+    """The date and user of when someone has joined with an invite link.
 
-# noinspection PyRedeclaration
-class Pong:  # type: ignore
-    """Telegram API base type.
+    Parameters:
+        date (:py:obj:`~datetime.datetime`):
+            The time of when this user used the given link
 
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            Pong
-
-    Functions:
-        This object can be returned by 2 functions.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            Ping
-            PingDelayDisconnect
+        user (:obj:`~pyrogram.types.User`):
+            The user that has used the given invite link
     """
 
-    QUALNAME = "pyrogram.raw.base.Pong"
+    def __init__(
+        self, *,
+        date: datetime,
+        user: "types.User"
+    ):
+        super().__init__(None)
+
+        self.date = date
+        self.user = user
+
+    @staticmethod
+    def _parse(client, invite_importers: "raw.types.messages.ChatInviteImporters"):
+        importers = types.List()
+
+        d = {i.id: i for i in invite_importers.users}
+
+        for j in invite_importers.importers:
+            importers.append(
+                InviteLinkImporter(
+                    date=utils.timestamp_to_datetime(j.date),
+                    user=types.User._parse(client=None, user=d[j.user_id])
+                )
+            )
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/pong")
+        return importers
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/recent_me_url.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,46 +12,32 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
 from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-RecentMeUrl = Union[raw.types.RecentMeUrlChat, raw.types.RecentMeUrlChatInvite, raw.types.RecentMeUrlStickerSet, raw.types.RecentMeUrlUnknown, raw.types.RecentMeUrlUser]
-
 
-# noinspection PyRedeclaration
-class RecentMeUrl:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 5 constructors available.
+import pyrogram
+from pyrogram import raw
+from .bot_command_scope import BotCommandScope
 
-        .. currentmodule:: pyrogram.raw.types
 
-        .. autosummary::
-            :nosignatures:
+class BotCommandScopeChatAdministrators(BotCommandScope):
+    """Represents the scope of bot commands, covering all administrators of a specific group or supergroup chat.
 
-            RecentMeUrlChat
-            RecentMeUrlChatInvite
-            RecentMeUrlStickerSet
-            RecentMeUrlUnknown
-            RecentMeUrlUser
+    Parameters:
+        chat_id (``int`` | ``str``):
+            Unique identifier for the target chat or username of the target supergroup (in the format
+            @supergroupusername).
     """
 
-    QUALNAME = "pyrogram.raw.base.RecentMeUrl"
+    def __init__(self, chat_id: Union[int, str]):
+        super().__init__("chat_administrators")
+
+        self.chat_id = chat_id
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/recent-me-url")
+    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
+        return raw.types.BotCommandScopePeerAdmins(
+            peer=await client.resolve_peer(self.chat_id)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/secure_value_hash.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/file_storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,42 +12,60 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+import logging
+import os
+import aiosqlite
+from pathlib import Path
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
+from .sqlite_storage import SQLiteStorage
 
-SecureValueHash = Union[raw.types.SecureValueHash]
+log = logging.getLogger(__name__)
 
 
-# noinspection PyRedeclaration
-class SecureValueHash:  # type: ignore
-    """Telegram API base type.
+class FileStorage(SQLiteStorage):
+    FILE_EXTENSION = ".session"
 
-    Constructors:
-        This base type has 1 constructor available.
+    def __init__(self, name: str, workdir: Path):
+        super().__init__(name)
 
-        .. currentmodule:: pyrogram.raw.types
+        self.database = workdir / (self.name + self.FILE_EXTENSION)
 
-        .. autosummary::
-            :nosignatures:
+    async def update(self):
+        version = await self.version()
 
-            SecureValueHash
-    """
+        if version == 1:
+            await self.conn.execute("DELETE FROM peers")
 
-    QUALNAME = "pyrogram.raw.base.SecureValueHash"
+            version += 1
 
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/secure-value-hash")
+        if version == 2:
+            await self.conn.execute("ALTER TABLE sessions ADD api_id INTEGER")
+
+            version += 1
+
+        await self.version(version)
+
+    async def open(self):
+        path = self.database
+        file_exists = path.is_file()
+
+        self.conn = await aiosqlite.connect(str(path), timeout=1)
+
+        await self.conn.execute("PRAGMA journal_mode=WAL")
+
+        if not file_exists:
+            await self.create()
+        else:
+            await self.update()
+
+        try:  # Python 3.6.0 (exactly this version) is bugged and won't successfully execute the vacuum
+            await self.conn.execute("VACUUM")
+        except aiosqlite.OperationalError:
+            pass
+
+    async def delete(self):
+        os.remove(self.database)
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/base/simple_web_view_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/vector.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,52 +12,48 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from io import BytesIO
+from typing import cast, Union, Any
 
-from typing import Union
-from pyrogram import raw
-from pyrogram.raw.core import TLObject
-
-SimpleWebViewResult = Union[raw.types.SimpleWebViewResultUrl]
-
-
-# noinspection PyRedeclaration
-class SimpleWebViewResult:  # type: ignore
-    """Telegram API base type.
-
-    Constructors:
-        This base type has 1 constructor available.
-
-        .. currentmodule:: pyrogram.raw.types
-
-        .. autosummary::
-            :nosignatures:
-
-            SimpleWebViewResultUrl
-
-    Functions:
-        This object can be returned by 1 function.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            messages.RequestSimpleWebView
-    """
-
-    QUALNAME = "pyrogram.raw.base.SimpleWebViewResult"
-
-    def __init__(self):
-        raise TypeError("Base types can only be used for type checking purposes: "
-                        "you tried to use a base type instance as argument, "
-                        "but you need to instantiate one of its constructors instead. "
-                        "More info: https://docs.pyrogram.org/telegram/base/simple-web-view-result")
+from .int import Int, Long
+from ..list import List
+from ..tl_object import TLObject
+
+
+class Vector(bytes, TLObject):
+    ID = 0x1CB5C415
+
+    # Method added to handle the special case when a query returns a bare Vector (of Ints);
+    # i.e., RpcResult body starts with 0x1cb5c415 (Vector Id) - e.g., messages.GetMessagesViews.
+    @staticmethod
+    def read_bare(b: BytesIO, size: int) -> Union[int, Any]:
+        if size == 4:
+            return Int.read(b)
+
+        if size == 8:
+            return Long.read(b)
+
+        return TLObject.read(b)
+
+    @classmethod
+    def read(cls, data: BytesIO, t: Any = None, *args: Any) -> List:
+        count = Int.read(data)
+        left = len(data.read())
+        size = (left / count) if count else 0
+        data.seek(-left, 1)
+
+        return List(
+            t.read(data) if t
+            else Vector.read_bare(data, size)
+            for _ in range(count)
+        )
+
+    def __new__(cls, value: list, t: Any = None) -> bytes:  # type: ignore
+        return b"".join(
+            [Int(cls.ID, False), Int(len(value))]
+            + [cast(bytes, t(i)) if t else i.write() for i in value]
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/future_salt.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/peer_user.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,42 +12,35 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-from typing import Any
+from pyrogram import raw
+from ..object import Object
 
-from .primitives.int import Int, Long
-from .tl_object import TLObject
 
+class PeerUser(Object):
+    """A PeerUser.
 
-class FutureSalt(TLObject):
-    ID = 0x0949D9DC
 
-    __slots__ = ["valid_since", "valid_until", "salt"]
+    Parameters:
+        user_id (``Integer``):
+            Id of the user.
+    """
 
-    QUALNAME = "FutureSalt"
+    def __init__(
+        self, *,
+        user_id: int
+    ):
+        super().__init__()
 
-    def __init__(self, valid_since: int, valid_until: int, salt: int):
-        self.valid_since = valid_since
-        self.valid_until = valid_until
-        self.salt = salt
+        self.user_id = user_id
 
     @staticmethod
-    def read(data: BytesIO, *args: Any) -> "FutureSalt":
-        valid_since = Int.read(data)
-        valid_until = Int.read(data)
-        salt = Long.read(data)
+    def _parse(action: "raw.types.PeerUser") -> "PeerUser":
 
-        return FutureSalt(valid_since, valid_until, salt)
 
-    def write(self, *args: Any) -> bytes:
-        b = BytesIO()
-
-        b.write(Int(self.valid_since))
-        b.write(Int(self.valid_until))
-        b.write(Long(self.salt))
-
-        return b.getvalue()
+        return PeerUser(
+            user_id=getattr(action,"user_id", None)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/future_salts.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/gzip_packed.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/list.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/msg_container.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,42 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-from typing import List, Any
+from ..object import Object
 
-from .message import Message
-from .primitives.int import Int
-from .tl_object import TLObject
 
+class ForumTopicReopened(Object):
+    """A service message about a forum topic reopened in the chat.
 
-class MsgContainer(TLObject):
-    ID = 0x73F1F8DC
+    Currently holds no information.
+    """
 
-    __slots__ = ["messages"]
-
-    QUALNAME = "MsgContainer"
-
-    def __init__(self, messages: List[Message]):
-        self.messages = messages
-
-    @staticmethod
-    def read(data: BytesIO, *args: Any) -> "MsgContainer":
-        count = Int.read(data)
-        return MsgContainer([Message.read(data) for _ in range(count)])
-
-    def write(self, *args: Any) -> bytes:
-        b = BytesIO()
-
-        b.write(Int(self.ID, False))
-
-        count = len(self.messages)
-        b.write(Int(count))
-
-        for message in self.messages:
-            b.write(message.write())
-
-        return b.getvalue()
+    def __init__(self):
+        super().__init__()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,13 +12,9 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .bool import Bool, BoolFalse, BoolTrue
-from .bytes import Bytes
-from .double import Double
-from .int import Int, Long, Int128, Int256
-from .string import String
-from .vector import Vector
+from .auth import Auth
+from .session import Session
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/bool.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/username.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,44 +12,47 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-from typing import Any
+from pyrogram import raw
+from ..object import Object
 
-from ..tl_object import TLObject
 
+class Username(Object):
+    """A Username.
 
-class Bytes(bytes, TLObject):
-    @classmethod
-    def read(cls, data: BytesIO, *args: Any) -> bytes:
-        length = int.from_bytes(data.read(1), "little")
-
-        if length <= 253:
-            x = data.read(length)
-            data.read(-(length + 1) % 4)
-        else:
-            length = int.from_bytes(data.read(3), "little")
-            x = data.read(length)
-            data.read(-length % 4)
-
-        return x
-
-    def __new__(cls, value: bytes) -> bytes:  # type: ignore
-        length = len(value)
-
-        if length <= 253:
-            return (
-                bytes([length])
-                + value
-                + bytes(-(length + 1) % 4)
-            )
-        else:
-            return (
-                bytes([254])
-                + length.to_bytes(3, "little")
-                + value
-                + bytes(-length % 4)
-            )
+
+    Parameters:
+        username (``String``):
+            The channel/user username.
+
+        editable (``bool``, *optional*):
+            Can the username edited.
+
+        active (``bool``, *optional*)
+            Is the username active.
+    """
+
+    def __init__(
+        self, *,
+        username: str,
+        editable: bool = None,
+        active: bool = None
+    ):
+        super().__init__()
+
+        self.username = username
+        self.editable = editable
+        self.active = active
+
+    @staticmethod
+    def _parse(action: "raw.types.Username") -> "Username":
+
+
+        return Username(
+            username=getattr(action,"username", None),
+            editable=getattr(action,"editable", None),
+            active=getattr(action,"active", None)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/double.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,21 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-from struct import unpack, pack
-from typing import cast, Any
+from ..object import Object
 
-from ..tl_object import TLObject
 
+class ForumTopicClosed(Object):
+    """A service message about a forum topic closed in the chat.
 
-class Double(bytes, TLObject):
-    @classmethod
-    def read(cls, data: BytesIO, *args: Any) -> float:
-        return cast(float, unpack("d", data.read(8))[0])
+    Currently holds no information.
+    """
 
-    def __new__(cls, value: float) -> bytes:  # type: ignore
-        return pack("d", value)
+    def __init__(self):
+        super().__init__()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/int.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/string.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-from typing import cast
+from ..object import Object
 
-from .bytes import Bytes
 
+class GeneralTopicHidden(Object):
+    """A service message about a general topic hidden in the chat.
 
-class String(Bytes):
-    @classmethod
-    def read(cls, data: BytesIO, *args) -> str:  # type: ignore
-        return cast(bytes, super(String, String).read(data)).decode(errors="replace")
+    Currently holds no information.
+    """
 
-    def __new__(cls, value: str) -> bytes:  # type: ignore
-        return super().__new__(cls, value.encode())
+    def __init__(self):
+        super().__init__()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/core/primitives/vector.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/raw/core/tl_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,47 +13,70 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from io import BytesIO
-from typing import cast, Union, Any
+from json import dumps
+from typing import cast, List, Any, Union, Dict
 
-from .int import Int, Long
-from ..list import List
-from ..tl_object import TLObject
+from ..all import objects
 
 
-class Vector(bytes, TLObject):
-    ID = 0x1CB5C415
+class TLObject:
+    __slots__: List[str] = []
 
-    # Method added to handle the special case when a query returns a bare Vector (of Ints);
-    # i.e., RpcResult body starts with 0x1cb5c415 (Vector Id) - e.g., messages.GetMessagesViews.
-    @staticmethod
-    def read_bare(b: BytesIO, size: int) -> Union[int, Any]:
-        if size == 4:
-            return Int.read(b)
+    QUALNAME = "Base"
 
-        if size == 8:
-            return Long.read(b)
+    @classmethod
+    def read(cls, b: BytesIO, *args: Any) -> Any:
+        return cast(TLObject, objects[int.from_bytes(b.read(4), "little")]).read(b, *args)
 
-        return TLObject.read(b)
+    def write(self, *args: Any) -> bytes:
+        pass
 
-    @classmethod
-    def read(cls, data: BytesIO, t: Any = None, *args: Any) -> List:
-        count = Int.read(data)
-        left = len(data.read())
-        size = (left / count) if count else 0
-        data.seek(-left, 1)
-
-        return List(
-            t.read(data) if t
-            else Vector.read_bare(data, size)
-            for _ in range(count)
+    @staticmethod
+    def default(obj: "TLObject") -> Union[str, Dict[str, str]]:
+        if isinstance(obj, bytes):
+            return repr(obj)
+
+        return {
+            "_": obj.QUALNAME,
+            **{
+                attr: getattr(obj, attr)
+                for attr in obj.__slots__
+                if getattr(obj, attr) is not None
+            }
+        }
+
+    def __str__(self) -> str:
+        return dumps(self, indent=4, default=TLObject.default, ensure_ascii=False)
+
+    def __repr__(self) -> str:
+        if not hasattr(self, "QUALNAME"):
+            return repr(self)
+
+        return "pyrogram.raw.{}({})".format(
+            self.QUALNAME,
+            ", ".join(
+                f"{attr}={repr(getattr(self, attr))}"
+                for attr in self.__slots__
+                if getattr(self, attr) is not None
+            )
         )
 
-    def __new__(cls, value: list, t: Any = None) -> bytes:  # type: ignore
-        return b"".join(
-            [Int(cls.ID, False), Int(len(value))]
-            + [cast(bytes, t(i)) if t else i.write() for i in value]
-        )
+    def __eq__(self, other: Any) -> bool:
+        for attr in self.__slots__:
+            try:
+                if getattr(self, attr) != getattr(other, attr):
+                    return False
+            except AttributeError:
+                return False
+
+        return True
+
+    def __len__(self) -> int:
+        return len(self.write())
+
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
+        pass
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/destroy_session.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,61 +12,55 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from ..object import Object
+
 
+class ForceReply(Object):
+    """Object used to force clients to show a reply interface.
 
-class DestroySession(TLObject):  # type: ignore
-    """Telegram API function.
+    Upon receiving a message with this object, Telegram clients will display a reply interface to the user.
 
-    Details:
-        - Layer: ``158``
-        - ID: ``E7512126``
+    This acts as if the user has selected the bot's message and tapped "Reply".
+    This can be extremely useful if you want to create user-friendly step-by-step interfaces without having to
+    sacrifice privacy mode.
 
     Parameters:
-        session_id (``int`` ``64-bit``):
-            N/A
+        selective (``bool``, *optional*):
+            Use this parameter if you want to force reply from specific users only. Targets:
+            1) users that are @mentioned in the text of the Message object;
+            2) if the bot's message is a reply (has reply_to_message_id), sender of the original message.
 
-    Returns:
-        :obj:`DestroySessionRes <pyrogram.raw.base.DestroySessionRes>`
+        placeholder (``str``, *optional*):
+            The placeholder to be shown in the input field when the reply is active; 1-64 characters.
     """
 
-    __slots__: List[str] = ["session_id"]
-
-    ID = 0xe7512126
-    QUALNAME = "functions.DestroySession"
+    def __init__(
+        self,
+        selective: bool = None,
+        placeholder: str = None
+    ):
+        super().__init__()
 
-    def __init__(self, *, session_id: int) -> None:
-        self.session_id = session_id  # long
+        self.selective = selective
+        self.placeholder = placeholder
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "DestroySession":
-        # No flags
-        
-        session_id = Long.read(b)
-        
-        return DestroySession(session_id=session_id)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(Long(self.session_id))
-        
-        return b.getvalue()
+    def read(b):
+        return ForceReply(
+            selective=b.selective,
+            placeholder=b.placeholder
+        )
+
+    async def write(self, _: "pyrogram.Client"):
+        return raw.types.ReplyKeyboardForceReply(
+            single_use=True,
+            selective=self.selective or None,
+            placeholder=self.placeholder or None
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/get_future_salts.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,61 +12,21 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-
-class GetFutureSalts(TLObject):  # type: ignore
-    """Telegram API function.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``B921BD04``
+from .menu_button import MenuButton
 
-    Parameters:
-        num (``int`` ``32-bit``):
-            N/A
 
-    Returns:
-        :obj:`FutureSalts <pyrogram.raw.base.FutureSalts>`
+class MenuButtonDefault(MenuButton):
+    """Describes that no specific value for the menu button was set.
     """
 
-    __slots__: List[str] = ["num"]
-
-    ID = 0xb921bd04
-    QUALNAME = "functions.GetFutureSalts"
-
-    def __init__(self, *, num: int) -> None:
-        self.num = num  # int
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "GetFutureSalts":
-        # No flags
-        
-        num = Int.read(b)
-        
-        return GetFutureSalts(num=num)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
+    def __init__(self):
+        super().__init__("default")
 
-        # No flags
-        
-        b.write(Int(self.num))
-        
-        return b.getvalue()
+    async def write(self, client: "pyrogram.Client") -> "raw.types.BotMenuButtonDefault":
+        return raw.types.BotMenuButtonDefault()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/invoke_with_layer.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_phone_contact.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,69 +12,40 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
+from pyrogram.session.internals import MsgId
+from ..object import Object
 
 
-class InvokeWithLayer(TLObject):  # type: ignore
-    """Telegram API function.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``DA9B0D0D``
+class InputPhoneContact(Object):
+    """A Phone Contact to be added in your Telegram address book.
+    It is intended to be used with :meth:`~pyrogram.Client.add_contacts()`
 
     Parameters:
-        layer (``int`` ``32-bit``):
-            N/A
+        phone (``str``):
+            Contact's phone number
 
-        query (Any function from :obj:`~pyrogram.raw.functions`):
-            N/A
+        first_name (``str``):
+            Contact's first name
 
-    Returns:
-        Any object from :obj:`~pyrogram.raw.types`
+        last_name (``str``, *optional*):
+            Contact's last name
     """
 
-    __slots__: List[str] = ["layer", "query"]
-
-    ID = 0xda9b0d0d
-    QUALNAME = "functions.InvokeWithLayer"
+    def __init__(self, phone: str, first_name: str, last_name: str = ""):
+        super().__init__(None)
 
-    def __init__(self, *, layer: int, query: TLObject) -> None:
-        self.layer = layer  # int
-        self.query = query  # !X
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "InvokeWithLayer":
-        # No flags
-        
-        layer = Int.read(b)
-        
-        query = TLObject.read(b)
-        
-        return InvokeWithLayer(layer=layer, query=query)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(Int(self.layer))
-        
-        b.write(self.query.write())
-        
-        return b.getvalue()
+    def __new__(cls,
+                phone: str,
+                first_name: str,
+                last_name: str = ""):
+        return raw.types.InputPhoneContact(
+            client_id=MsgId(),
+            phone="+" + phone.strip("+"),
+            first_name=first_name,
+            last_name=last_name
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/functions/rpc_drop_answer.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,61 +12,40 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
+from ..object import Object
 
-class RpcDropAnswer(TLObject):  # type: ignore
-    """Telegram API function.
 
-    Details:
-        - Layer: ``158``
-        - ID: ``58E4A740``
+class WebAppData(Object):
+    """Contains data sent from a `Web App <https://core.telegram.org/bots/webapps>`_ to the bot.
 
     Parameters:
-        req_msg_id (``int`` ``64-bit``):
-            N/A
+        data (``str``):
+            The data.
 
-    Returns:
-        :obj:`RpcDropAnswer <pyrogram.raw.base.RpcDropAnswer>`
-    """
+        button_text (``str``):
+            Text of the *web_app* keyboard button, from which the Web App was opened.
 
-    __slots__: List[str] = ["req_msg_id"]
+    """
 
-    ID = 0x58e4a740
-    QUALNAME = "functions.RpcDropAnswer"
+    def __init__(
+        self,
+        *,
+        data: str,
+        button_text: str,
+    ):
+        super().__init__()
 
-    def __init__(self, *, req_msg_id: int) -> None:
-        self.req_msg_id = req_msg_id  # long
+        self.data = data
+        self.button_text = button_text
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "RpcDropAnswer":
-        # No flags
-        
-        req_msg_id = Long.read(b)
-        
-        return RpcDropAnswer(req_msg_id=req_msg_id)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(Long(self.req_msg_id))
-        
-        return b.getvalue()
+    def _parse(action: "raw.types.MessageActionWebViewDataSentMe"):
+        return WebAppData(
+            data=action.data,
+            button_text=action.text
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/attach_menu_bots.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/document.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,86 +12,87 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from datetime import datetime
+from typing import List
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, utils
+from pyrogram import types
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
+from ..object import Object
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
-
-class AttachMenuBots(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.AttachMenuBots`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``3C4301C0``
+class Document(Object):
+    """A generic file (as opposed to photos, voice messages, audio files, ...).
 
     Parameters:
-        hash (``int`` ``64-bit``):
-            N/A
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        bots (List of :obj:`AttachMenuBot <pyrogram.raw.base.AttachMenuBot>`):
-            N/A
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-        users (List of :obj:`User <pyrogram.raw.base.User>`):
-            N/A
+        file_name (``str``, *optional*):
+            Original filename as defined by sender.
 
-    Functions:
-        This object can be returned by 1 function.
+        mime_type (``str``, *optional*):
+            MIME type of the file as defined by sender.
 
-        .. currentmodule:: pyrogram.raw.functions
+        file_size (``int``, *optional*):
+            File size.
 
-        .. autosummary::
-            :nosignatures:
+        date (:py:obj:`~datetime.datetime`, *optional*):
+            Date the document was sent.
 
-            messages.GetAttachMenuBots
+        thumbs (List of :obj:`~pyrogram.types.Thumbnail`, *optional*):
+            Document thumbnails as defined by sender.
     """
 
-    __slots__: List[str] = ["hash", "bots", "users"]
-
-    ID = 0x3c4301c0
-    QUALNAME = "types.AttachMenuBots"
-
-    def __init__(self, *, hash: int, bots: List["raw.base.AttachMenuBot"], users: List["raw.base.User"]) -> None:
-        self.hash = hash  # long
-        self.bots = bots  # Vector<AttachMenuBot>
-        self.users = users  # Vector<User>
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        file_name: str = None,
+        mime_type: str = None,
+        file_size: int = None,
+        date: datetime = None,
+        thumbs: List["types.Thumbnail"] = None
+    ):
+        super().__init__(client)
+
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.file_name = file_name
+        self.mime_type = mime_type
+        self.file_size = file_size
+        self.date = date
+        self.thumbs = thumbs
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "AttachMenuBots":
-        # No flags
-        
-        hash = Long.read(b)
-        
-        bots = TLObject.read(b)
-        
-        users = TLObject.read(b)
-        
-        return AttachMenuBots(hash=hash, bots=bots, users=users)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(Long(self.hash))
-        
-        b.write(Vector(self.bots))
-        
-        b.write(Vector(self.users))
-        
-        return b.getvalue()
+    def _parse(client, document: "raw.types.Document", file_name: str) -> "Document":
+        return Document(
+            file_id=FileId(
+                file_type=FileType.DOCUMENT,
+                dc_id=document.dc_id,
+                media_id=document.id,
+                access_hash=document.access_hash,
+                file_reference=document.file_reference
+            ).encode(),
+            file_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=document.id
+            ).encode(),
+            file_name=file_name,
+            mime_type=document.mime_type,
+            file_size=document.size,
+            date=utils.timestamp_to_datetime(document.date),
+            thumbs=types.Thumbnail._parse(client, document),
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/available_reaction.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/web_page.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,143 +12,176 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
+from pyrogram import types
+from ..object import Object
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class WebPage(Object):
+    # TODO: hash, cached_page
+    """A webpage preview
 
-class AvailableReaction(TLObject):  # type: ignore
-    """Telegram API type.
+    Parameters:
+        id (``str``):
+            Unique identifier for this webpage.
 
-    Constructor of :obj:`~pyrogram.raw.base.AvailableReaction`.
+        url (``str``):
+            Full URL for this webpage.
 
-    Details:
-        - Layer: ``158``
-        - ID: ``C077EC01``
+        display_url (``str``):
+            Display URL for this webpage.
 
-    Parameters:
-        reaction (``str``):
-            N/A
+        type (``str``, *optional*):
+            Type of webpage preview, known types (at the time of writing) are:
+            *"article"*, *"photo"*, *"gif"*, *"video"* and *"document"*,
+            *"telegram_user"*, *"telegram_bot"*, *"telegram_channel"*, *"telegram_megagroup"*.
 
-        title (``str``):
-            N/A
+        site_name (``str``, *optional*):
+            Webpage site name.
 
-        static_icon (:obj:`Document <pyrogram.raw.base.Document>`):
-            N/A
+        title (``str``, *optional*):
+            Title of this webpage.
 
-        appear_animation (:obj:`Document <pyrogram.raw.base.Document>`):
-            N/A
+        description (``str``, *optional*):
+            Description of this webpage.
 
-        select_animation (:obj:`Document <pyrogram.raw.base.Document>`):
-            N/A
+        audio (:obj:`~pyrogram.types.Audio`, *optional*):
+            Webpage preview is an audio file, information about the file.
 
-        activate_animation (:obj:`Document <pyrogram.raw.base.Document>`):
-            N/A
+        document (:obj:`~pyrogram.types.Document`, *optional*):
+            Webpage preview is a general file, information about the file.
 
-        effect_animation (:obj:`Document <pyrogram.raw.base.Document>`):
-            N/A
+        photo (:obj:`~pyrogram.types.Photo`, *optional*):
+            Webpage preview is a photo, information about the photo.
 
-        inactive (``bool``, *optional*):
-            N/A
+        animation (:obj:`~pyrogram.types.Animation`, *optional*):
+            Webpage preview is an animation, information about the animation.
 
-        premium (``bool``, *optional*):
-            N/A
+        video (:obj:`~pyrogram.types.Video`, *optional*):
+            Webpage preview is a video, information about the video.
 
-        around_animation (:obj:`Document <pyrogram.raw.base.Document>`, *optional*):
-            N/A
+        embed_url (``str``, *optional*):
+            Embedded content URL.
 
-        center_icon (:obj:`Document <pyrogram.raw.base.Document>`, *optional*):
-            N/A
+        embed_type (``str``, *optional*):
+            Embedded content type, like `iframe`
 
-    """
+        embed_width (``int``, *optional*):
+            Embedded content width.
+
+        embed_height (``int``, *optional*):
+            Embedded content height.
 
-    __slots__: List[str] = ["reaction", "title", "static_icon", "appear_animation", "select_animation", "activate_animation", "effect_animation", "inactive", "premium", "around_animation", "center_icon"]
+        duration (``int``, *optional*):
+            Unknown at the time of writing.
 
-    ID = 0xc077ec01
-    QUALNAME = "types.AvailableReaction"
+        author (``str``, *optional*):
+            Author of the webpage, eg the Twitter user for a tweet, or the author in an article.
+    """
 
-    def __init__(self, *, reaction: str, title: str, static_icon: "raw.base.Document", appear_animation: "raw.base.Document", select_animation: "raw.base.Document", activate_animation: "raw.base.Document", effect_animation: "raw.base.Document", inactive: Optional[bool] = None, premium: Optional[bool] = None, around_animation: "raw.base.Document" = None, center_icon: "raw.base.Document" = None) -> None:
-        self.reaction = reaction  # string
-        self.title = title  # string
-        self.static_icon = static_icon  # Document
-        self.appear_animation = appear_animation  # Document
-        self.select_animation = select_animation  # Document
-        self.activate_animation = activate_animation  # Document
-        self.effect_animation = effect_animation  # Document
-        self.inactive = inactive  # flags.0?true
-        self.premium = premium  # flags.2?true
-        self.around_animation = around_animation  # flags.1?Document
-        self.center_icon = center_icon  # flags.1?Document
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        id: str,
+        url: str,
+        display_url: str,
+        type: str = None,
+        site_name: str = None,
+        title: str = None,
+        description: str = None,
+        audio: "types.Audio" = None,
+        document: "types.Document" = None,
+        photo: "types.Photo" = None,
+        animation: "types.Animation" = None,
+        video: "types.Video" = None,
+        embed_url: str = None,
+        embed_type: str = None,
+        embed_width: int = None,
+        embed_height: int = None,
+        duration: int = None,
+        author: str = None
+    ):
+        super().__init__(client)
+
+        self.id = id
+        self.url = url
+        self.display_url = display_url
+        self.type = type
+        self.site_name = site_name
+        self.title = title
+        self.description = description
+        self.audio = audio
+        self.document = document
+        self.photo = photo
+        self.animation = animation
+        self.video = video
+        self.embed_url = embed_url
+        self.embed_type = embed_type
+        self.embed_width = embed_width
+        self.embed_height = embed_height
+        self.duration = duration
+        self.author = author
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "AvailableReaction":
-        
-        flags = Int.read(b)
-        
-        inactive = True if flags & (1 << 0) else False
-        premium = True if flags & (1 << 2) else False
-        reaction = String.read(b)
-        
-        title = String.read(b)
-        
-        static_icon = TLObject.read(b)
-        
-        appear_animation = TLObject.read(b)
-        
-        select_animation = TLObject.read(b)
-        
-        activate_animation = TLObject.read(b)
-        
-        effect_animation = TLObject.read(b)
-        
-        around_animation = TLObject.read(b) if flags & (1 << 1) else None
-        
-        center_icon = TLObject.read(b) if flags & (1 << 1) else None
-        
-        return AvailableReaction(reaction=reaction, title=title, static_icon=static_icon, appear_animation=appear_animation, select_animation=select_animation, activate_animation=activate_animation, effect_animation=effect_animation, inactive=inactive, premium=premium, around_animation=around_animation, center_icon=center_icon)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.inactive else 0
-        flags |= (1 << 2) if self.premium else 0
-        flags |= (1 << 1) if self.around_animation is not None else 0
-        flags |= (1 << 1) if self.center_icon is not None else 0
-        b.write(Int(flags))
-        
-        b.write(String(self.reaction))
-        
-        b.write(String(self.title))
-        
-        b.write(self.static_icon.write())
-        
-        b.write(self.appear_animation.write())
-        
-        b.write(self.select_animation.write())
-        
-        b.write(self.activate_animation.write())
-        
-        b.write(self.effect_animation.write())
-        
-        if self.around_animation is not None:
-            b.write(self.around_animation.write())
-        
-        if self.center_icon is not None:
-            b.write(self.center_icon.write())
-        
-        return b.getvalue()
+    def _parse(client, webpage: "raw.types.WebPage") -> "WebPage":
+        audio = None
+        document = None
+        photo = None
+        animation = None
+        video = None
+
+        if isinstance(webpage.photo, raw.types.Photo):
+            photo = types.Photo._parse(client, webpage.photo)
+
+        doc = webpage.document
+
+        if isinstance(doc, raw.types.Document):
+            attributes = {type(i): i for i in doc.attributes}
+
+            file_name = getattr(
+                attributes.get(
+                    raw.types.DocumentAttributeFilename, None
+                ), "file_name", None
+            )
+
+            if raw.types.DocumentAttributeAudio in attributes:
+                audio_attributes = attributes[raw.types.DocumentAttributeAudio]
+                audio = types.Audio._parse(client, doc, audio_attributes, file_name)
+
+            elif raw.types.DocumentAttributeAnimated in attributes:
+                video_attributes = attributes.get(raw.types.DocumentAttributeVideo, None)
+                animation = types.Animation._parse(client, doc, video_attributes, file_name)
+
+            elif raw.types.DocumentAttributeVideo in attributes:
+                video_attributes = attributes[raw.types.DocumentAttributeVideo]
+                video = types.Video._parse(client, doc, video_attributes, file_name)
+
+            else:
+                document = types.Document._parse(client, doc, file_name)
+
+        return WebPage(
+            id=str(webpage.id),
+            url=webpage.url,
+            display_url=webpage.display_url,
+            type=webpage.type,
+            site_name=webpage.site_name,
+            title=webpage.title,
+            description=webpage.description,
+            audio=audio,
+            document=document,
+            photo=photo,
+            animation=animation,
+            video=video,
+            embed_url=webpage.embed_url,
+            embed_type=webpage.embed_type,
+            embed_width=webpage.embed_width,
+            embed_height=webpage.embed_height,
+            duration=webpage.duration,
+            author=webpage.author
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_command_scope_users.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,56 +12,22 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-
-class BotCommandScopeUsers(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.BotCommandScope`.
+from .bot_command_scope import BotCommandScope
 
-    Details:
-        - Layer: ``158``
-        - ID: ``3C4F04D8``
-
-    Parameters:
-        No parameters required.
 
+class BotCommandScopeDefault(BotCommandScope):
+    """Represents the default scope of bot commands.
+    Default commands are used if no commands with a narrower scope are specified for the user.
     """
 
-    __slots__: List[str] = []
-
-    ID = 0x3c4f04d8
-    QUALNAME = "types.BotCommandScopeUsers"
-
-    def __init__(self) -> None:
-        pass
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "BotCommandScopeUsers":
-        # No flags
-        
-        return BotCommandScopeUsers()
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
+    def __init__(self):
+        super().__init__("default")
 
-        # No flags
-        
-        return b.getvalue()
+    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
+        return raw.types.BotCommandScopeDefault()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_media_invoice.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,119 +12,103 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import List, Optional
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, types, utils, enums
+from .inline_query_result import InlineQueryResult
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-
-class BotInlineMessageMediaInvoice(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.BotInlineMessage`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``354A9B09``
 
+class InlineQueryResultVoice(InlineQueryResult):
+    """Link to a voice recording in an .OGG container encoded with OPUS.
+    
+    By default, this voice recording will be sent by the user.
+    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
+    voice message.
+    
     Parameters:
+        voice_url (``str``):
+            A valid URL for the voice recording.
+            
         title (``str``):
-            N/A
-
-        description (``str``):
-            N/A
-
-        currency (``str``):
-            N/A
-
-        total_amount (``int`` ``64-bit``):
-            N/A
-
-        shipping_address_requested (``bool``, *optional*):
-            N/A
-
-        test (``bool``, *optional*):
-            N/A
-
-        photo (:obj:`WebDocument <pyrogram.raw.base.WebDocument>`, *optional*):
-            N/A
-
-        reply_markup (:obj:`ReplyMarkup <pyrogram.raw.base.ReplyMarkup>`, *optional*):
-            N/A
-
+            Title for the result.
+            
+        id (``str``, *optional*):
+            Unique identifier for this result, 1-64 bytes.
+            Defaults to a randomly generated UUID4.
+            
+        voice_duration (``int``, *optional*):
+            Recording duration in seconds.
+
+        caption (``str``, *optional*):
+            Caption of the audio to be sent, 0-1024 characters.
+            
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
+
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+            
+        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
+            Inline keyboard attached to the message.
+            
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`, *optional*):
+            Content of the message to be sent instead of the audio.
     """
 
-    __slots__: List[str] = ["title", "description", "currency", "total_amount", "shipping_address_requested", "test", "photo", "reply_markup"]
-
-    ID = 0x354a9b09
-    QUALNAME = "types.BotInlineMessageMediaInvoice"
-
-    def __init__(self, *, title: str, description: str, currency: str, total_amount: int, shipping_address_requested: Optional[bool] = None, test: Optional[bool] = None, photo: "raw.base.WebDocument" = None, reply_markup: "raw.base.ReplyMarkup" = None) -> None:
-        self.title = title  # string
-        self.description = description  # string
-        self.currency = currency  # string
-        self.total_amount = total_amount  # long
-        self.shipping_address_requested = shipping_address_requested  # flags.1?true
-        self.test = test  # flags.3?true
-        self.photo = photo  # flags.0?WebDocument
-        self.reply_markup = reply_markup  # flags.2?ReplyMarkup
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "BotInlineMessageMediaInvoice":
-        
-        flags = Int.read(b)
-        
-        shipping_address_requested = True if flags & (1 << 1) else False
-        test = True if flags & (1 << 3) else False
-        title = String.read(b)
-        
-        description = String.read(b)
-        
-        photo = TLObject.read(b) if flags & (1 << 0) else None
-        
-        currency = String.read(b)
-        
-        total_amount = Long.read(b)
-        
-        reply_markup = TLObject.read(b) if flags & (1 << 2) else None
-        
-        return BotInlineMessageMediaInvoice(title=title, description=description, currency=currency, total_amount=total_amount, shipping_address_requested=shipping_address_requested, test=test, photo=photo, reply_markup=reply_markup)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 1) if self.shipping_address_requested else 0
-        flags |= (1 << 3) if self.test else 0
-        flags |= (1 << 0) if self.photo is not None else 0
-        flags |= (1 << 2) if self.reply_markup is not None else 0
-        b.write(Int(flags))
-        
-        b.write(String(self.title))
-        
-        b.write(String(self.description))
-        
-        if self.photo is not None:
-            b.write(self.photo.write())
-        
-        b.write(String(self.currency))
-        
-        b.write(Long(self.total_amount))
-        
-        if self.reply_markup is not None:
-            b.write(self.reply_markup.write())
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        voice_url: str,
+        title: str,
+        id: str = None,
+        voice_duration: int = 0,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List["types.MessageEntity"] = None,
+        reply_markup: "types.InlineKeyboardMarkup" = None,
+        input_message_content: "types.InputMessageContent" = None
+    ):
+        super().__init__("voice", id, input_message_content, reply_markup)
+
+        self.voice_url = voice_url
+        self.title = title
+        self.voice_duration = voice_duration
+        self.caption = caption
+        self.parse_mode = parse_mode
+        self.caption_entities = caption_entities
+
+    async def write(self, client: "pyrogram.Client"):
+        audio = raw.types.InputWebDocument(
+            url=self.voice_url,
+            size=0,
+            mime_type="audio/mpeg",
+            attributes=[raw.types.DocumentAttributeAudio(
+                duration=self.voice_duration,
+                title=self.title,
+            )]
+        )
+
+        message, entities = (await utils.parse_text_entities(
+            client, self.caption, self.parse_mode, self.caption_entities
+        )).values()
+
+        return raw.types.InputBotInlineResult(
+            id=self.id,
+            type=self.type,
+            title=self.title,
+            content=audio,
+            send_message=(
+                await self.input_message_content.write(client, self.reply_markup)
+                if self.input_message_content
+                else raw.types.InputBotInlineMessageMediaAuto(
+                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
+                    message=message,
+                    entities=entities
+                )
+            )
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_message_text.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,89 +12,97 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import Optional, List
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, types, utils, enums
+from .inline_query_result import InlineQueryResult
+from ...file_id import FileId
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class InlineQueryResultCachedVoice(InlineQueryResult):
+    """A link to a voice message stored on the Telegram servers.
 
-class BotInlineMessageText(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.BotInlineMessage`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``8C7F65E2``
+    By default, this voice message will be sent by the user.
+    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the voice
+    message.
 
     Parameters:
-        message (``str``):
-            N/A
+        voice_file_id (``str``):
+            A valid file identifier for the voice message.
 
-        no_webpage (``bool``, *optional*):
-            N/A
+        id (``str``, *optional*):
+            Unique identifier for this result, 1-64 bytes.
+            Defaults to a randomly generated UUID4.
 
-        entities (List of :obj:`MessageEntity <pyrogram.raw.base.MessageEntity>`, *optional*):
-            N/A
+        title (``str``, *optional*):
+            Title for the result.
 
-        reply_markup (:obj:`ReplyMarkup <pyrogram.raw.base.ReplyMarkup>`, *optional*):
-            N/A
+        caption (``str``, *optional*):
+            Caption of the photo to be sent, 0-1024 characters.
 
-    """
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
 
-    __slots__: List[str] = ["message", "no_webpage", "entities", "reply_markup"]
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
-    ID = 0x8c7f65e2
-    QUALNAME = "types.BotInlineMessageText"
+        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
+            An InlineKeyboardMarkup object.
+
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
+            Content of the message to be sent instead of the photo.
+    """
 
-    def __init__(self, *, message: str, no_webpage: Optional[bool] = None, entities: Optional[List["raw.base.MessageEntity"]] = None, reply_markup: "raw.base.ReplyMarkup" = None) -> None:
-        self.message = message  # string
-        self.no_webpage = no_webpage  # flags.0?true
-        self.entities = entities  # flags.1?Vector<MessageEntity>
-        self.reply_markup = reply_markup  # flags.2?ReplyMarkup
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "BotInlineMessageText":
-        
-        flags = Int.read(b)
-        
-        no_webpage = True if flags & (1 << 0) else False
-        message = String.read(b)
-        
-        entities = TLObject.read(b) if flags & (1 << 1) else []
-        
-        reply_markup = TLObject.read(b) if flags & (1 << 2) else None
-        
-        return BotInlineMessageText(message=message, no_webpage=no_webpage, entities=entities, reply_markup=reply_markup)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.no_webpage else 0
-        flags |= (1 << 1) if self.entities else 0
-        flags |= (1 << 2) if self.reply_markup is not None else 0
-        b.write(Int(flags))
-        
-        b.write(String(self.message))
-        
-        if self.entities is not None:
-            b.write(Vector(self.entities))
-        
-        if self.reply_markup is not None:
-            b.write(self.reply_markup.write())
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        voice_file_id: str,
+        id: str = None,
+        title: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List["types.MessageEntity"] = None,
+        reply_markup: "types.InlineKeyboardMarkup" = None,
+        input_message_content: "types.InputMessageContent" = None
+    ):
+        super().__init__("voice", id, input_message_content, reply_markup)
+
+        self.voice_file_id = voice_file_id
+        self.title = title
+        self.caption = caption
+        self.parse_mode = parse_mode
+        self.caption_entities = caption_entities
+        self.reply_markup = reply_markup
+        self.input_message_content = input_message_content
+
+    async def write(self, client: "pyrogram.Client"):
+        message, entities = (await utils.parse_text_entities(
+            client, self.caption, self.parse_mode, self.caption_entities
+        )).values()
+
+        file_id = FileId.decode(self.voice_file_id)
+
+        return raw.types.InputBotInlineResultDocument(
+            id=self.id,
+            type=self.type,
+            title=self.title,
+            document=raw.types.InputDocument(
+                id=file_id.media_id,
+                access_hash=file_id.access_hash,
+                file_reference=file_id.file_reference,
+            ),
+            send_message=(
+                await self.input_message_content.write(client, self.reply_markup)
+                if self.input_message_content
+                else raw.types.InputBotInlineMessageMediaAuto(
+                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
+                    message=message,
+                    entities=entities
+                )
+            )
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_inline_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,126 +12,134 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import Optional, List
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, types, utils, enums
+from .inline_query_result import InlineQueryResult
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class InlineQueryResultDocument(InlineQueryResult):
+    """Link to a file.
 
-class BotInlineResult(TLObject):  # type: ignore
-    """Telegram API type.
+    By default, this file will be sent by the user with an optional caption.
+    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the file.
 
-    Constructor of :obj:`~pyrogram.raw.base.BotInlineResult`.
+    Parameters:
+        document_url (``str``):
+            A valid URL for the file.
 
-    Details:
-        - Layer: ``158``
-        - ID: ``11965F3A``
+        title (``str``):
+            Title for the result.
 
-    Parameters:
-        id (``str``):
-            N/A
+        mime_type (``str``, *optional*):
+            Mime type of the content of the file, either “application/pdf” or “application/zip”.
+            Defaults to "application/zip".
 
-        type (``str``):
-            N/A
+        id (``str``, *optional*):
+            Unique identifier for this result, 1-64 bytes.
+            Defaults to a randomly generated UUID4.
 
-        send_message (:obj:`BotInlineMessage <pyrogram.raw.base.BotInlineMessage>`):
-            N/A
+        caption (``str``, *optional*):
+            Caption of the video to be sent, 0-1024 characters.
 
-        title (``str``, *optional*):
-            N/A
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
 
-        description (``str``, *optional*):
-            N/A
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
-        url (``str``, *optional*):
-            N/A
+        description (``str``, *optional*):
+            Short description of the result.
 
-        thumb (:obj:`WebDocument <pyrogram.raw.base.WebDocument>`, *optional*):
-            N/A
+        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
+            Inline keyboard attached to the message.
 
-        content (:obj:`WebDocument <pyrogram.raw.base.WebDocument>`, *optional*):
-            N/A
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
+            Content of the message to be sent instead of the file.
 
-    """
+        thumb_url (``str``, *optional*):
+            Url of the thumbnail for the result.
 
-    __slots__: List[str] = ["id", "type", "send_message", "title", "description", "url", "thumb", "content"]
+        thumb_width (``int``, *optional*):
+            Thumbnail width.
 
-    ID = 0x11965f3a
-    QUALNAME = "types.BotInlineResult"
+        thumb_height (``int``, *optional*):
+            Thumbnail height.
+    """
 
-    def __init__(self, *, id: str, type: str, send_message: "raw.base.BotInlineMessage", title: Optional[str] = None, description: Optional[str] = None, url: Optional[str] = None, thumb: "raw.base.WebDocument" = None, content: "raw.base.WebDocument" = None) -> None:
-        self.id = id  # string
-        self.type = type  # string
-        self.send_message = send_message  # BotInlineMessage
-        self.title = title  # flags.1?string
-        self.description = description  # flags.2?string
-        self.url = url  # flags.3?string
-        self.thumb = thumb  # flags.4?WebDocument
-        self.content = content  # flags.5?WebDocument
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "BotInlineResult":
-        
-        flags = Int.read(b)
-        
-        id = String.read(b)
-        
-        type = String.read(b)
-        
-        title = String.read(b) if flags & (1 << 1) else None
-        description = String.read(b) if flags & (1 << 2) else None
-        url = String.read(b) if flags & (1 << 3) else None
-        thumb = TLObject.read(b) if flags & (1 << 4) else None
-        
-        content = TLObject.read(b) if flags & (1 << 5) else None
-        
-        send_message = TLObject.read(b)
-        
-        return BotInlineResult(id=id, type=type, send_message=send_message, title=title, description=description, url=url, thumb=thumb, content=content)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 1) if self.title is not None else 0
-        flags |= (1 << 2) if self.description is not None else 0
-        flags |= (1 << 3) if self.url is not None else 0
-        flags |= (1 << 4) if self.thumb is not None else 0
-        flags |= (1 << 5) if self.content is not None else 0
-        b.write(Int(flags))
-        
-        b.write(String(self.id))
-        
-        b.write(String(self.type))
-        
-        if self.title is not None:
-            b.write(String(self.title))
-        
-        if self.description is not None:
-            b.write(String(self.description))
-        
-        if self.url is not None:
-            b.write(String(self.url))
-        
-        if self.thumb is not None:
-            b.write(self.thumb.write())
-        
-        if self.content is not None:
-            b.write(self.content.write())
-        
-        b.write(self.send_message.write())
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        document_url: str,
+        title: str,
+        mime_type: str = "application/zip",
+        id: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List["types.MessageEntity"] = None,
+        description: str = "",
+        reply_markup: "types.InlineKeyboardMarkup" = None,
+        input_message_content: "types.InputMessageContent" = None,
+        thumb_url: str = None,
+        thumb_width: int = 0,
+        thumb_height: int = 0
+    ):
+        super().__init__("file", id, input_message_content, reply_markup)
+
+        self.document_url = document_url
+        self.title = title
+        self.mime_type = mime_type
+        self.caption = caption
+        self.parse_mode = parse_mode
+        self.caption_entities = caption_entities
+        self.description = description
+        self.thumb_url = thumb_url
+        self.thumb_width = thumb_width
+        self.thumb_height = thumb_height
+
+    async def write(self, client: "pyrogram.Client"):
+        document = raw.types.InputWebDocument(
+            url=self.document_url,
+            size=0,
+            mime_type=self.mime_type,
+            attributes=[]
+        )
+
+        thumb = raw.types.InputWebDocument(
+            url=self.thumb_url,
+            size=0,
+            mime_type="image/jpeg",
+            attributes=[
+                raw.types.DocumentAttributeImageSize(
+                    w=self.thumb_width,
+                    h=self.thumb_height
+                )
+            ]
+        ) if self.thumb_url else None
+
+        message, entities = (await utils.parse_text_entities(
+            client, self.caption, self.parse_mode, self.caption_entities
+        )).values()
+
+        return raw.types.InputBotInlineResult(
+            id=self.id,
+            type=self.type,
+            title=self.title,
+            description=self.description,
+            thumb=thumb,
+            content=document,
+            send_message=(
+                await self.input_message_content.write(client, self.reply_markup)
+                if self.input_message_content
+                else raw.types.InputBotInlineMessageMediaAuto(
+                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
+                    message=message,
+                    entities=entities
+                )
+            )
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/bot_menu_button.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/voice.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,78 +12,85 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from datetime import datetime
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, utils
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
+from ..object import Object
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
-
-class BotMenuButton(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.BotMenuButton`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``C7B57CE6``
+class Voice(Object):
+    """A voice note.
 
     Parameters:
-        text (``str``):
-            N/A
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        url (``str``):
-            N/A
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-    Functions:
-        This object can be returned by 1 function.
+        duration (``int``):
+            Duration of the audio in seconds as defined by sender.
 
-        .. currentmodule:: pyrogram.raw.functions
+        waveform (``bytes``, *optional*):
+            Voice waveform.
 
-        .. autosummary::
-            :nosignatures:
+        mime_type (``str``, *optional*):
+            MIME type of the file as defined by sender.
 
-            bots.GetBotMenuButton
-    """
-
-    __slots__: List[str] = ["text", "url"]
+        file_size (``int``, *optional*):
+            File size.
 
-    ID = 0xc7b57ce6
-    QUALNAME = "types.BotMenuButton"
+        date (:py:obj:`~datetime.datetime`, *optional*):
+            Date the voice was sent.
+    """
 
-    def __init__(self, *, text: str, url: str) -> None:
-        self.text = text  # string
-        self.url = url  # string
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        duration: int,
+        waveform: bytes = None,
+        mime_type: str = None,
+        file_size: int = None,
+        date: datetime = None
+    ):
+        super().__init__(client)
+
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.duration = duration
+        self.waveform = waveform
+        self.mime_type = mime_type
+        self.file_size = file_size
+        self.date = date
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "BotMenuButton":
-        # No flags
-        
-        text = String.read(b)
-        
-        url = String.read(b)
-        
-        return BotMenuButton(text=text, url=url)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(String(self.text))
-        
-        b.write(String(self.url))
-        
-        return b.getvalue()
+    def _parse(client, voice: "raw.types.Document", attributes: "raw.types.DocumentAttributeAudio") -> "Voice":
+        return Voice(
+            file_id=FileId(
+                file_type=FileType.VOICE,
+                dc_id=voice.dc_id,
+                media_id=voice.id,
+                access_hash=voice.access_hash,
+                file_reference=voice.file_reference
+            ).encode(),
+            file_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=voice.id
+            ).encode(),
+            duration=attributes.duration,
+            mime_type=voice.mime_type,
+            file_size=voice.size,
+            waveform=attributes.waveform,
+            date=utils.timestamp_to_datetime(voice.date),
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_admin_log_event_action_update_pinned.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,61 +12,47 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
+from ..object import Object
 
-class ChannelAdminLogEventActionUpdatePinned(TLObject):  # type: ignore
-    """Telegram API type.
 
-    Constructor of :obj:`~pyrogram.raw.base.ChannelAdminLogEventAction`.
+class ReplyKeyboardRemove(Object):
+    """Object used to tell clients to remove a bot keyboard.
 
-    Details:
-        - Layer: ``158``
-        - ID: ``E9E82C18``
+    Upon receiving a message with this object, Telegram clients will remove the current custom keyboard and display
+    the default letter-keyboard. By default, custom keyboards are displayed until a new keyboard is sent by a bot.
+    An exception is made for one-time keyboards that are hidden immediately after the user presses a button
+    (see ReplyKeyboardMarkup).
 
     Parameters:
-        message (:obj:`Message <pyrogram.raw.base.Message>`):
-            N/A
-
+        selective (``bool``, *optional*):
+            Use this parameter if you want to remove the keyboard for specific users only. Targets:
+            1) users that are @mentioned in the text of the Message object;
+            2) if the bot's message is a reply (has reply_to_message_id), sender of the original message.
+            Example: A user votes in a poll, bot returns confirmation message in reply to the vote and removes the
+            keyboard for that user, while still showing the keyboard with poll options to users who haven't voted yet.
     """
 
-    __slots__: List[str] = ["message"]
-
-    ID = 0xe9e82c18
-    QUALNAME = "types.ChannelAdminLogEventActionUpdatePinned"
+    def __init__(
+        self,
+        selective: bool = None
+    ):
+        super().__init__()
 
-    def __init__(self, *, message: "raw.base.Message") -> None:
-        self.message = message  # Message
+        self.selective = selective
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "ChannelAdminLogEventActionUpdatePinned":
-        # No flags
-        
-        message = TLObject.read(b)
-        
-        return ChannelAdminLogEventActionUpdatePinned(message=message)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(self.message.write())
-        
-        return b.getvalue()
+    def read(b):
+        return ReplyKeyboardRemove(
+            selective=b.selective
+        )
+
+    async def write(self, _: "pyrogram.Client"):
+        return raw.types.ReplyKeyboardHide(
+            selective=self.selective or None
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/channel_participants_admins.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,56 +12,40 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+import pyrogram
+from pyrogram import raw, types
+from .menu_button import MenuButton
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-
-class ChannelParticipantsAdmins(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.ChannelParticipantsFilter`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``B4608969``
+class MenuButtonWebApp(MenuButton):
+    """A menu button, which launches a `Web App <https://core.telegram.org/bots/webapps>`_.
 
     Parameters:
-        No parameters required.
+        text (``str``):
+            Text on the button
 
+        web_app (:obj:`~pyrogram.types.WebAppInfo`):
+            Description of the Web App that will be launched when the user presses the button.
+            The Web App will be able to send an arbitrary message on behalf of the user using the method
+            :meth:`~pyrogram.Client.answer_web_app_query`.
     """
 
-    __slots__: List[str] = []
-
-    ID = 0xb4608969
-    QUALNAME = "types.ChannelParticipantsAdmins"
-
-    def __init__(self) -> None:
-        pass
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "ChannelParticipantsAdmins":
-        # No flags
-        
-        return ChannelParticipantsAdmins()
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        text: str,
+        web_app: "types.WebAppInfo"
+    ):
+        super().__init__("web_app")
+
+        self.text = text
+        self.web_app = web_app
+
+    async def write(self, client: "pyrogram.Client") -> "raw.types.BotMenuButton":
+        return raw.types.BotMenuButton(
+            text=self.text,
+            url=self.web_app.url
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/chat_admin_rights.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,127 +12,108 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
+from ..object import Object
 
-class ChatAdminRights(TLObject):  # type: ignore
-    """Telegram API type.
 
-    Constructor of :obj:`~pyrogram.raw.base.ChatAdminRights`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``5FB224D5``
+class ChatPrivileges(Object):
+    """Describes privileged actions an administrator is able to take in a chat.
 
     Parameters:
-        change_info (``bool``, *optional*):
-            N/A
-
-        post_messages (``bool``, *optional*):
-            N/A
-
-        edit_messages (``bool``, *optional*):
-            N/A
-
-        delete_messages (``bool``, *optional*):
-            N/A
-
-        ban_users (``bool``, *optional*):
-            N/A
-
-        invite_users (``bool``, *optional*):
-            N/A
-
-        pin_messages (``bool``, *optional*):
-            N/A
-
-        add_admins (``bool``, *optional*):
-            N/A
-
-        anonymous (``bool``, *optional*):
-            N/A
-
-        manage_call (``bool``, *optional*):
-            N/A
-
-        other (``bool``, *optional*):
-            N/A
-
-        manage_topics (``bool``, *optional*):
-            N/A
+        can_manage_chat (``bool``, *optional*):
+            True, if the administrator can access the chat event log, chat statistics, message statistics in channels,
+            see channel members, see anonymous administrators in supergroups and ignore slow mode.
+            Implied by any other administrator privilege.
+
+        can_delete_messages (``bool``, *optional*):
+            True, if the administrator can delete messages of other users.
+
+        can_manage_video_chats (``bool``, *optional*):
+            Groups and supergroups only.
+            True, if the administrator can manage video chats (also called group calls).
+
+        can_restrict_members (``bool``, *optional*):
+            True, if the administrator can restrict, ban or unban chat members.
+
+        can_promote_members (``bool``, *optional*):
+            True, if the administrator can add new administrators with a subset of his own privileges or demote
+            administrators that he has promoted, directly or indirectly (promoted by administrators that were appointed
+            by the user).
+
+        can_change_info (``bool``, *optional*):
+            True, if the user is allowed to change the chat title, photo and other settings.
+
+        can_post_messages (``bool``, *optional*):
+            Channels only.
+            True, if the administrator can post messages in the channel.
+
+        can_edit_messages (``bool``, *optional*):
+            Channels only.
+            True, if the administrator can edit messages of other users and can pin messages.
+
+        can_invite_users (``bool``, *optional*):
+            True, if the user is allowed to invite new users to the chat.
+
+        can_pin_messages (``bool``, *optional*):
+            Groups and supergroups only.
+            True, if the user is allowed to pin messages.
+
+        can_manage_topics (``bool``, *optional*):
+            supergroups only.
+            True, if the user is allowed to create, rename, close, and reopen forum topics.
 
+        is_anonymous (``bool``, *optional*):
+            True, if the user's presence in the chat is hidden.
     """
 
-    __slots__: List[str] = ["change_info", "post_messages", "edit_messages", "delete_messages", "ban_users", "invite_users", "pin_messages", "add_admins", "anonymous", "manage_call", "other", "manage_topics"]
-
-    ID = 0x5fb224d5
-    QUALNAME = "types.ChatAdminRights"
-
-    def __init__(self, *, change_info: Optional[bool] = None, post_messages: Optional[bool] = None, edit_messages: Optional[bool] = None, delete_messages: Optional[bool] = None, ban_users: Optional[bool] = None, invite_users: Optional[bool] = None, pin_messages: Optional[bool] = None, add_admins: Optional[bool] = None, anonymous: Optional[bool] = None, manage_call: Optional[bool] = None, other: Optional[bool] = None, manage_topics: Optional[bool] = None) -> None:
-        self.change_info = change_info  # flags.0?true
-        self.post_messages = post_messages  # flags.1?true
-        self.edit_messages = edit_messages  # flags.2?true
-        self.delete_messages = delete_messages  # flags.3?true
-        self.ban_users = ban_users  # flags.4?true
-        self.invite_users = invite_users  # flags.5?true
-        self.pin_messages = pin_messages  # flags.7?true
-        self.add_admins = add_admins  # flags.9?true
-        self.anonymous = anonymous  # flags.10?true
-        self.manage_call = manage_call  # flags.11?true
-        self.other = other  # flags.12?true
-        self.manage_topics = manage_topics  # flags.13?true
+    def __init__(
+        self,
+        *,
+        can_manage_chat: bool = True,
+        can_delete_messages: bool = False,
+        can_manage_video_chats: bool = False,  # Groups and supergroups only
+        can_restrict_members: bool = False,
+        can_promote_members: bool = False,
+        can_change_info: bool = False,
+        can_post_messages: bool = False,  # Channels only
+        can_edit_messages: bool = False,  # Channels only
+        can_invite_users: bool = False,
+        can_pin_messages: bool = False,  # Groups and supergroups only
+        can_manage_topics: bool = False, # supergroups only.
+        is_anonymous: bool = False
+    ):
+        super().__init__(None)
+
+        self.can_manage_chat: bool = can_manage_chat
+        self.can_delete_messages: bool = can_delete_messages
+        self.can_manage_video_chats: bool = can_manage_video_chats
+        self.can_restrict_members: bool = can_restrict_members
+        self.can_promote_members: bool = can_promote_members
+        self.can_change_info: bool = can_change_info
+        self.can_post_messages: bool = can_post_messages
+        self.can_edit_messages: bool = can_edit_messages
+        self.can_invite_users: bool = can_invite_users
+        self.can_pin_messages: bool = can_pin_messages
+        self.can_manage_topics: bool = can_manage_topics
+        self.is_anonymous: bool = is_anonymous
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "ChatAdminRights":
-        
-        flags = Int.read(b)
-        
-        change_info = True if flags & (1 << 0) else False
-        post_messages = True if flags & (1 << 1) else False
-        edit_messages = True if flags & (1 << 2) else False
-        delete_messages = True if flags & (1 << 3) else False
-        ban_users = True if flags & (1 << 4) else False
-        invite_users = True if flags & (1 << 5) else False
-        pin_messages = True if flags & (1 << 7) else False
-        add_admins = True if flags & (1 << 9) else False
-        anonymous = True if flags & (1 << 10) else False
-        manage_call = True if flags & (1 << 11) else False
-        other = True if flags & (1 << 12) else False
-        manage_topics = True if flags & (1 << 13) else False
-        return ChatAdminRights(change_info=change_info, post_messages=post_messages, edit_messages=edit_messages, delete_messages=delete_messages, ban_users=ban_users, invite_users=invite_users, pin_messages=pin_messages, add_admins=add_admins, anonymous=anonymous, manage_call=manage_call, other=other, manage_topics=manage_topics)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.change_info else 0
-        flags |= (1 << 1) if self.post_messages else 0
-        flags |= (1 << 2) if self.edit_messages else 0
-        flags |= (1 << 3) if self.delete_messages else 0
-        flags |= (1 << 4) if self.ban_users else 0
-        flags |= (1 << 5) if self.invite_users else 0
-        flags |= (1 << 7) if self.pin_messages else 0
-        flags |= (1 << 9) if self.add_admins else 0
-        flags |= (1 << 10) if self.anonymous else 0
-        flags |= (1 << 11) if self.manage_call else 0
-        flags |= (1 << 12) if self.other else 0
-        flags |= (1 << 13) if self.manage_topics else 0
-        b.write(Int(flags))
-        
-        return b.getvalue()
+    def _parse(admin_rights: "raw.base.ChatAdminRights") -> "ChatPrivileges":
+        return ChatPrivileges(
+            can_manage_chat=admin_rights.other,
+            can_delete_messages=admin_rights.delete_messages,
+            can_manage_video_chats=admin_rights.manage_call,
+            can_restrict_members=admin_rights.ban_users,
+            can_promote_members=admin_rights.add_admins,
+            can_change_info=admin_rights.change_info,
+            can_post_messages=admin_rights.post_messages,
+            can_edit_messages=admin_rights.edit_messages,
+            can_invite_users=admin_rights.invite_users,
+            can_pin_messages=admin_rights.pin_messages,
+            can_manage_topics=admin_rights.manage_topics,
+            is_anonymous=admin_rights.anonymous
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/contact.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/stickerset.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,69 +12,78 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import List, Optional, Union
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
+from ..object import Object
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class StickerSet(Object):
+    """A stickerset.
 
-class Contact(TLObject):  # type: ignore
-    """Telegram API type.
+    Parameters:
+        id (``Integer``):
+            Identifier for this stickerset.
 
-    Constructor of :obj:`~pyrogram.raw.base.Contact`.
+        title (``String``):
+            Title of stickerset.
 
-    Details:
-        - Layer: ``158``
-        - ID: ``145ADE0B``
+        short_name (``String``):
+            Short name of stickerset, used when sharing stickerset using stickerset deep links.
 
-    Parameters:
-        user_id (``int`` ``64-bit``):
-            N/A
+        count (``Integer``):
+            Number of stickers in stickerset.
 
-        mutual (``bool``):
-            N/A
+        masks (``Boolean``):
+            Is this a mask stickerset.
 
-    """
+        animated (``Boolean``):
+            Is this a animated stickerset.
 
-    __slots__: List[str] = ["user_id", "mutual"]
+        videos (``Boolean``):
+            Is this a videos stickerset.
 
-    ID = 0x145ade0b
-    QUALNAME = "types.Contact"
+        emojis (``Boolean``):
+            Is this a emojis stickerset.
+    """
 
-    def __init__(self, *, user_id: int, mutual: bool) -> None:
-        self.user_id = user_id  # long
-        self.mutual = mutual  # Bool
+    def __init__(
+        self,
+        *,
+        id: int,
+        title: str,
+        short_name: str,
+        count: int,
+        masks: bool = None,
+        animated: bool = None,
+        videos: bool = None,
+        emojis: bool = None
+    ):
+        self.id = id
+        self.title = title
+        self.short_name = short_name
+        self.count = count
+        self.masks = masks
+        self.animated = animated
+        self.videos = videos
+        self.emojis = emojis
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "Contact":
-        # No flags
-        
-        user_id = Long.read(b)
-        
-        mutual = Bool.read(b)
-        
-        return Contact(user_id=user_id, mutual=mutual)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(Long(self.user_id))
-        
-        b.write(Bool(self.mutual))
-        
-        return b.getvalue()
+    def _parse(stickerset: "raw.types.StickerSet") -> "StickerSet":
+
+        return StickerSet(
+            id=getattr(stickerset,"id", None),
+            title=getattr(stickerset,"title", None),
+            short_name=getattr(stickerset,"short_name", None),
+            count=getattr(stickerset,"count", None),
+            masks=getattr(stickerset,"masks", None),
+            animated=getattr(stickerset,"animated", None),
+            videos=getattr(stickerset,"videos", None),
+            emojis=getattr(stickerset,"emojis", None)
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/destroy_auth_key_fail.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,65 +12,21 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-
-class DestroyAuthKeyFail(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.DestroyAuthKeyRes`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``EA109B13``
-
-    Parameters:
-        No parameters required.
+from .bot_command_scope import BotCommandScope
 
-    Functions:
-        This object can be returned by 1 function.
 
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            DestroyAuthKey
+class BotCommandScopeAllGroupChats(BotCommandScope):
+    """Represents the scope of bot commands, covering all group and supergroup chats.
     """
 
-    __slots__: List[str] = []
-
-    ID = 0xea109b13
-    QUALNAME = "types.DestroyAuthKeyFail"
-
-    def __init__(self) -> None:
-        pass
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "DestroyAuthKeyFail":
-        # No flags
-        
-        return DestroyAuthKeyFail()
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
+    def __init__(self):
+        super().__init__("all_group_chats")
 
-        # No flags
-        
-        return b.getvalue()
+    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
+        return raw.types.BotCommandScopeChats()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/draft_message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,96 +12,90 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import Optional, List
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, types, utils, enums
+from .inline_query_result import InlineQueryResult
+from ...file_id import FileId
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class InlineQueryResultCachedAudio(InlineQueryResult):
+    """A link to an MP3 audio file stored on the Telegram servers
 
-class DraftMessage(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.DraftMessage`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``FD8E711F``
+    By default, this audio file will be sent by the user. Alternatively, you can use *input_message_content* to send a
+    message with the specified content instead of the audio.
 
     Parameters:
-        message (``str``):
-            N/A
+        audio_file_id (``str``):
+            A valid file identifier for the audio file.
 
-        date (``int`` ``32-bit``):
-            N/A
+        id (``str``, *optional*):
+            Unique identifier for this result, 1-64 bytes.
+            Defaults to a randomly generated UUID4.
 
-        no_webpage (``bool``, *optional*):
-            N/A
+        caption (``str``, *optional*):
+            Caption of the photo to be sent, 0-1024 characters.
 
-        reply_to_msg_id (``int`` ``32-bit``, *optional*):
-            N/A
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
 
-        entities (List of :obj:`MessageEntity <pyrogram.raw.base.MessageEntity>`, *optional*):
-            N/A
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
-    """
+        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
+            An InlineKeyboardMarkup object.
 
-    __slots__: List[str] = ["message", "date", "no_webpage", "reply_to_msg_id", "entities"]
-
-    ID = 0xfd8e711f
-    QUALNAME = "types.DraftMessage"
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
+            Content of the message to be sent instead of the photo.
+    """
 
-    def __init__(self, *, message: str, date: int, no_webpage: Optional[bool] = None, reply_to_msg_id: Optional[int] = None, entities: Optional[List["raw.base.MessageEntity"]] = None) -> None:
-        self.message = message  # string
-        self.date = date  # int
-        self.no_webpage = no_webpage  # flags.1?true
-        self.reply_to_msg_id = reply_to_msg_id  # flags.0?int
-        self.entities = entities  # flags.3?Vector<MessageEntity>
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "DraftMessage":
-        
-        flags = Int.read(b)
-        
-        no_webpage = True if flags & (1 << 1) else False
-        reply_to_msg_id = Int.read(b) if flags & (1 << 0) else None
-        message = String.read(b)
-        
-        entities = TLObject.read(b) if flags & (1 << 3) else []
-        
-        date = Int.read(b)
-        
-        return DraftMessage(message=message, date=date, no_webpage=no_webpage, reply_to_msg_id=reply_to_msg_id, entities=entities)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 1) if self.no_webpage else 0
-        flags |= (1 << 0) if self.reply_to_msg_id is not None else 0
-        flags |= (1 << 3) if self.entities else 0
-        b.write(Int(flags))
-        
-        if self.reply_to_msg_id is not None:
-            b.write(Int(self.reply_to_msg_id))
-        
-        b.write(String(self.message))
-        
-        if self.entities is not None:
-            b.write(Vector(self.entities))
-        
-        b.write(Int(self.date))
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        audio_file_id: str,
+        id: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List["types.MessageEntity"] = None,
+        reply_markup: "types.InlineKeyboardMarkup" = None,
+        input_message_content: "types.InputMessageContent" = None
+    ):
+        super().__init__("audio", id, input_message_content, reply_markup)
+
+        self.audio_file_id = audio_file_id
+        self.caption = caption
+        self.parse_mode = parse_mode
+        self.caption_entities = caption_entities
+        self.reply_markup = reply_markup
+        self.input_message_content = input_message_content
+
+    async def write(self, client: "pyrogram.Client"):
+        message, entities = (await utils.parse_text_entities(
+            client, self.caption, self.parse_mode, self.caption_entities
+        )).values()
+
+        file_id = FileId.decode(self.audio_file_id)
+
+        return raw.types.InputBotInlineResultDocument(
+            id=self.id,
+            type=self.type,
+            document=raw.types.InputDocument(
+                id=file_id.media_id,
+                access_hash=file_id.access_hash,
+                file_reference=file_id.file_reference,
+            ),
+            send_message=(
+                await self.input_message_content.write(client, self.reply_markup)
+                if self.input_message_content
+                else raw.types.InputBotInlineMessageMediaAuto(
+                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
+                    message=message,
+                    entities=entities
+                )
+            )
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/email_verification_apple.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,61 +12,71 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from datetime import datetime
+from typing import Dict
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, types, utils
+from ..object import Object
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class ChatJoiner(Object):
+    """Contains information about a joiner member of a chat.
 
-class EmailVerificationApple(TLObject):  # type: ignore
-    """Telegram API type.
+    Parameters:
+        user (:obj:`~pyrogram.types.User`):
+            Information about the user.
 
-    Constructor of :obj:`~pyrogram.raw.base.EmailVerification`.
+        date (:py:obj:`~datetime.datetime`):
+            Date when the user joined.
 
-    Details:
-        - Layer: ``158``
-        - ID: ``96D074FD``
+        bio (``str``, *optional*):
+            Bio of the user.
 
-    Parameters:
-        token (``str``):
-            N/A
+        pending (``bool``, *optional*):
+            True in case the chat joiner has a pending request.
 
+        approved_by (:obj:`~pyrogram.types.User`, *optional*):
+            Administrator who approved this chat joiner.
     """
 
-    __slots__: List[str] = ["token"]
-
-    ID = 0x96d074fd
-    QUALNAME = "types.EmailVerificationApple"
-
-    def __init__(self, *, token: str) -> None:
-        self.token = token  # string
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client",
+        user: "types.User",
+        date: datetime = None,
+        bio: str = None,
+        pending: bool = None,
+        approved_by: "types.User" = None,
+    ):
+        super().__init__(client)
+
+        self.user = user
+        self.date = date
+        self.bio = bio
+        self.pending = pending
+        self.approved_by = approved_by
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "EmailVerificationApple":
-        # No flags
-        
-        token = String.read(b)
-        
-        return EmailVerificationApple(token=token)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(String(self.token))
-        
-        return b.getvalue()
+    def _parse(
+        client: "pyrogram.Client",
+        joiner: "raw.base.ChatInviteImporter",
+        users: Dict[int, "raw.base.User"],
+    ) -> "ChatJoiner":
+        return ChatJoiner(
+            user=types.User._parse(client, users[joiner.user_id]),
+            date=utils.timestamp_to_datetime(joiner.date),
+            pending=joiner.requested,
+            bio=joiner.about,
+            approved_by=(
+                types.User._parse(client, users[joiner.approved_by])
+                if joiner.approved_by
+                else None
+            ),
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/emoji_list_not_modified.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,67 +12,36 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
-
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
+import pyrogram
 from pyrogram import raw
-from typing import List, Optional, Any
-
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
+from ..object import Object
 
-class EmojiListNotModified(TLObject):  # type: ignore
-    """Telegram API type.
 
-    Constructor of :obj:`~pyrogram.raw.base.EmojiList`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``481EADFA``
+class StrippedThumbnail(Object):
+    """A stripped thumbnail
 
     Parameters:
-        No parameters required.
-
-    Functions:
-        This object can be returned by 3 functions.
-
-        .. currentmodule:: pyrogram.raw.functions
-
-        .. autosummary::
-            :nosignatures:
-
-            account.GetDefaultProfilePhotoEmojis
-            account.GetDefaultGroupPhotoEmojis
-            messages.SearchCustomEmoji
+        data (``bytes``):
+            Thumbnail data
     """
 
-    __slots__: List[str] = []
-
-    ID = 0x481eadfa
-    QUALNAME = "types.EmojiListNotModified"
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        data: bytes
+    ):
+        super().__init__(client)
 
-    def __init__(self) -> None:
-        pass
+        self.data = data
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "EmojiListNotModified":
-        # No flags
-        
-        return EmojiListNotModified()
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        return b.getvalue()
+    def _parse(client, stripped_thumbnail: "raw.types.PhotoStrippedSize") -> "StrippedThumbnail":
+        return StrippedThumbnail(
+            data=stripped_thumbnail.bytes,
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/encrypted_file.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/video_note.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,102 +12,97 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from datetime import datetime
+from typing import List
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, utils
+from pyrogram import types
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
+from ..object import Object
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
-
-class EncryptedFile(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.EncryptedFile`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``A8008CD8``
+class VideoNote(Object):
+    """A video note.
 
     Parameters:
-        id (``int`` ``64-bit``):
-            N/A
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        access_hash (``int`` ``64-bit``):
-            N/A
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-        size (``int`` ``64-bit``):
-            N/A
+        length (``int``):
+            Video width and height as defined by sender.
 
-        dc_id (``int`` ``32-bit``):
-            N/A
+        duration (``int``):
+            Duration of the video in seconds as defined by sender.
 
-        key_fingerprint (``int`` ``32-bit``):
-            N/A
+        mime_type (``str``, *optional*):
+            MIME type of the file as defined by sender.
 
-    Functions:
-        This object can be returned by 1 function.
+        file_size (``int``, *optional*):
+            File size.
 
-        .. currentmodule:: pyrogram.raw.functions
+        date (:py:obj:`~datetime.datetime`, *optional*):
+            Date the video note was sent.
 
-        .. autosummary::
-            :nosignatures:
-
-            messages.UploadEncryptedFile
+        thumbs (List of :obj:`~pyrogram.types.Thumbnail`, *optional*):
+            Video thumbnails.
     """
 
-    __slots__: List[str] = ["id", "access_hash", "size", "dc_id", "key_fingerprint"]
-
-    ID = 0xa8008cd8
-    QUALNAME = "types.EncryptedFile"
-
-    def __init__(self, *, id: int, access_hash: int, size: int, dc_id: int, key_fingerprint: int) -> None:
-        self.id = id  # long
-        self.access_hash = access_hash  # long
-        self.size = size  # long
-        self.dc_id = dc_id  # int
-        self.key_fingerprint = key_fingerprint  # int
+    def __init__(
+        self,
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        length: int,
+        duration: int,
+        thumbs: List["types.Thumbnail"] = None,
+        mime_type: str = None,
+        file_size: int = None,
+        date: datetime = None
+    ):
+        super().__init__(client)
+
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.mime_type = mime_type
+        self.file_size = file_size
+        self.date = date
+        self.length = length
+        self.duration = duration
+        self.thumbs = thumbs
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "EncryptedFile":
-        # No flags
-        
-        id = Long.read(b)
-        
-        access_hash = Long.read(b)
-        
-        size = Long.read(b)
-        
-        dc_id = Int.read(b)
-        
-        key_fingerprint = Int.read(b)
-        
-        return EncryptedFile(id=id, access_hash=access_hash, size=size, dc_id=dc_id, key_fingerprint=key_fingerprint)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        # No flags
-        
-        b.write(Long(self.id))
-        
-        b.write(Long(self.access_hash))
-        
-        b.write(Long(self.size))
-        
-        b.write(Int(self.dc_id))
-        
-        b.write(Int(self.key_fingerprint))
-        
-        return b.getvalue()
+    def _parse(
+        client,
+        video_note: "raw.types.Document",
+        video_attributes: "raw.types.DocumentAttributeVideo"
+    ) -> "VideoNote":
+        return VideoNote(
+            file_id=FileId(
+                file_type=FileType.VIDEO_NOTE,
+                dc_id=video_note.dc_id,
+                media_id=video_note.id,
+                access_hash=video_note.access_hash,
+                file_reference=video_note.file_reference
+            ).encode(),
+            file_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=video_note.id
+            ).encode(),
+            length=video_attributes.w,
+            duration=video_attributes.duration,
+            file_size=video_note.size,
+            mime_type=video_note.mime_type,
+            date=utils.timestamp_to_datetime(video_note.date),
+            thumbs=types.Thumbnail._parse(client, video_note),
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/folder.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,99 +12,100 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import Optional, List
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, types, utils, enums
+from .inline_query_result import InlineQueryResult
+from ...file_id import FileId
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class InlineQueryResultCachedPhoto(InlineQueryResult):
+    """A link to a photo stored on the Telegram servers.
 
-class Folder(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.Folder`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``FF544E65``
+    By default, this photo will be sent by the user with an optional caption. Alternatively, you can use
+    *input_message_content* to send a message with the specified content instead of the photo.
 
     Parameters:
-        id (``int`` ``32-bit``):
-            N/A
+        photo_file_id (``str``):
+            A valid file identifier of the photo.
 
-        title (``str``):
-            N/A
+        id (``str``, *optional*):
+            Unique identifier for this result, 1-64 bytes.
+            Defaults to a randomly generated UUID4.
 
-        autofill_new_broadcasts (``bool``, *optional*):
-            N/A
+        title (``str``, *optional*):
+            Title for the result.
 
-        autofill_public_groups (``bool``, *optional*):
-            N/A
+        description (``str``, *optional*):
+            Short description of the result.
 
-        autofill_new_correspondents (``bool``, *optional*):
-            N/A
+        caption (``str``, *optional*):
+            Caption of the photo to be sent, 0-1024 characters.
 
-        photo (:obj:`ChatPhoto <pyrogram.raw.base.ChatPhoto>`, *optional*):
-            N/A
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
 
-    """
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
-    __slots__: List[str] = ["id", "title", "autofill_new_broadcasts", "autofill_public_groups", "autofill_new_correspondents", "photo"]
+        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
+            An InlineKeyboardMarkup object.
 
-    ID = 0xff544e65
-    QUALNAME = "types.Folder"
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
+            Content of the message to be sent instead of the photo.
+    """
 
-    def __init__(self, *, id: int, title: str, autofill_new_broadcasts: Optional[bool] = None, autofill_public_groups: Optional[bool] = None, autofill_new_correspondents: Optional[bool] = None, photo: "raw.base.ChatPhoto" = None) -> None:
-        self.id = id  # int
-        self.title = title  # string
-        self.autofill_new_broadcasts = autofill_new_broadcasts  # flags.0?true
-        self.autofill_public_groups = autofill_public_groups  # flags.1?true
-        self.autofill_new_correspondents = autofill_new_correspondents  # flags.2?true
-        self.photo = photo  # flags.3?ChatPhoto
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "Folder":
-        
-        flags = Int.read(b)
-        
-        autofill_new_broadcasts = True if flags & (1 << 0) else False
-        autofill_public_groups = True if flags & (1 << 1) else False
-        autofill_new_correspondents = True if flags & (1 << 2) else False
-        id = Int.read(b)
-        
-        title = String.read(b)
-        
-        photo = TLObject.read(b) if flags & (1 << 3) else None
-        
-        return Folder(id=id, title=title, autofill_new_broadcasts=autofill_new_broadcasts, autofill_public_groups=autofill_public_groups, autofill_new_correspondents=autofill_new_correspondents, photo=photo)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.autofill_new_broadcasts else 0
-        flags |= (1 << 1) if self.autofill_public_groups else 0
-        flags |= (1 << 2) if self.autofill_new_correspondents else 0
-        flags |= (1 << 3) if self.photo is not None else 0
-        b.write(Int(flags))
-        
-        b.write(Int(self.id))
-        
-        b.write(String(self.title))
-        
-        if self.photo is not None:
-            b.write(self.photo.write())
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        photo_file_id: str,
+        id: str = None,
+        title: str = None,
+        description: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List["types.MessageEntity"] = None,
+        reply_markup: "types.InlineKeyboardMarkup" = None,
+        input_message_content: "types.InputMessageContent" = None
+    ):
+        super().__init__("photo", id, input_message_content, reply_markup)
+
+        self.photo_file_id = photo_file_id
+        self.title = title
+        self.description = description
+        self.caption = caption
+        self.parse_mode = parse_mode
+        self.caption_entities = caption_entities
+        self.reply_markup = reply_markup
+        self.input_message_content = input_message_content
+
+    async def write(self, client: "pyrogram.Client"):
+        message, entities = (await utils.parse_text_entities(
+            client, self.caption, self.parse_mode, self.caption_entities
+        )).values()
+
+        file_id = FileId.decode(self.photo_file_id)
+
+        return raw.types.InputBotInlineResultPhoto(
+            id=self.id,
+            type=self.type,
+            photo=raw.types.InputPhoto(
+                id=file_id.media_id,
+                access_hash=file_id.access_hash,
+                file_reference=file_id.file_reference,
+            ),
+            send_message=(
+                await self.input_message_content.write(client, self.reply_markup)
+                if self.input_message_content
+                else raw.types.InputBotInlineMessageMediaAuto(
+                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
+                    message=message,
+                    entities=entities
+                )
+            )
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_bot_inline_message_text.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_audio.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,89 +12,71 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import Optional, List, BinaryIO, Union
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+from .input_media import InputMedia
+from ..messages_and_media import MessageEntity
+from ... import enums
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
+class InputMediaAudio(InputMedia):
+    """An audio to be sent inside an album.
 
-class InputBotInlineMessageText(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.InputBotInlineMessage`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``3DCD7A87``
+    It is intended to be used with :meth:`~pyrogram.Client.send_media_group`.
 
     Parameters:
-        message (``str``):
-            N/A
-
-        no_webpage (``bool``, *optional*):
-            N/A
+        media (``str`` | ``BinaryIO``):
+            Audio to send.
+            Pass a file_id as string to send an audio that exists on the Telegram servers or
+            pass a file path as string to upload a new audio that exists on your local machine or
+            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
+            pass an HTTP URL as a string for Telegram to get an audio file from the Internet.
+
+        thumb (``str``, *optional*):
+            Thumbnail of the music file album cover.
+            The thumbnail should be in JPEG format and less than 200 KB in size.
+            A thumbnail's width and height should not exceed 320 pixels.
+            Thumbnails can't be reused and can be only uploaded as a new file.
+
+        caption (``str``, *optional*):
+            Caption of the audio to be sent, 0-1024 characters.
+            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
+
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
+
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
-        entities (List of :obj:`MessageEntity <pyrogram.raw.base.MessageEntity>`, *optional*):
-            N/A
+        duration (``int``, *optional*):
+            Duration of the audio in seconds
 
-        reply_markup (:obj:`ReplyMarkup <pyrogram.raw.base.ReplyMarkup>`, *optional*):
-            N/A
+        performer (``str``, *optional*):
+            Performer of the audio
 
+        title (``str``, *optional*):
+            Title of the audio
     """
 
-    __slots__: List[str] = ["message", "no_webpage", "entities", "reply_markup"]
-
-    ID = 0x3dcd7a87
-    QUALNAME = "types.InputBotInlineMessageText"
-
-    def __init__(self, *, message: str, no_webpage: Optional[bool] = None, entities: Optional[List["raw.base.MessageEntity"]] = None, reply_markup: "raw.base.ReplyMarkup" = None) -> None:
-        self.message = message  # string
-        self.no_webpage = no_webpage  # flags.0?true
-        self.entities = entities  # flags.1?Vector<MessageEntity>
-        self.reply_markup = reply_markup  # flags.2?ReplyMarkup
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "InputBotInlineMessageText":
-        
-        flags = Int.read(b)
-        
-        no_webpage = True if flags & (1 << 0) else False
-        message = String.read(b)
-        
-        entities = TLObject.read(b) if flags & (1 << 1) else []
-        
-        reply_markup = TLObject.read(b) if flags & (1 << 2) else None
-        
-        return InputBotInlineMessageText(message=message, no_webpage=no_webpage, entities=entities, reply_markup=reply_markup)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.no_webpage else 0
-        flags |= (1 << 1) if self.entities else 0
-        flags |= (1 << 2) if self.reply_markup is not None else 0
-        b.write(Int(flags))
-        
-        b.write(String(self.message))
-        
-        if self.entities is not None:
-            b.write(Vector(self.entities))
-        
-        if self.reply_markup is not None:
-            b.write(self.reply_markup.write())
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        media: Union[str, BinaryIO],
+        thumb: str = None,
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List[MessageEntity] = None,
+        duration: int = 0,
+        performer: str = "",
+        title: str = ""
+    ):
+        super().__init__(media, caption, parse_mode, caption_entities)
+
+        self.thumb = thumb
+        self.duration = duration
+        self.performer = performer
+        self.title = title
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_peer_photo_file_location.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_photo.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,77 +12,52 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import Optional, List, Union, BinaryIO
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+from .input_media import InputMedia
+from ..messages_and_media import MessageEntity
+from ... import enums
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
-
-class InputPeerPhotoFileLocation(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.InputFileLocation`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``37257E99``
+class InputMediaPhoto(InputMedia):
+    """A photo to be sent inside an album.
+    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
 
     Parameters:
-        peer (:obj:`InputPeer <pyrogram.raw.base.InputPeer>`):
-            N/A
+        media (``str`` | ``BinaryIO``):
+            Photo to send.
+            Pass a file_id as string to send a photo that exists on the Telegram servers or
+            pass a file path as string to upload a new photo that exists on your local machine or
+            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
+            pass an HTTP URL as a string for Telegram to get a photo from the Internet.
+
+        caption (``str``, *optional*):
+            Caption of the photo to be sent, 0-1024 characters.
+            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
+
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
 
-        photo_id (``int`` ``64-bit``):
-            N/A
-
-        big (``bool``, *optional*):
-            N/A
+        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+        has_spoiler (``bool``, *optional*):
+            Pass True if the photo needs to be covered with a spoiler animation.
     """
 
-    __slots__: List[str] = ["peer", "photo_id", "big"]
-
-    ID = 0x37257e99
-    QUALNAME = "types.InputPeerPhotoFileLocation"
+    def __init__(
+        self,
+        media: Union[str, BinaryIO],
+        caption: str = "",
+        parse_mode: Optional["enums.ParseMode"] = None,
+        caption_entities: List[MessageEntity] = None,
+        has_spoiler: bool = None
+    ):
+        super().__init__(media, caption, parse_mode, caption_entities)
 
-    def __init__(self, *, peer: "raw.base.InputPeer", photo_id: int, big: Optional[bool] = None) -> None:
-        self.peer = peer  # InputPeer
-        self.photo_id = photo_id  # long
-        self.big = big  # flags.0?true
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "InputPeerPhotoFileLocation":
-        
-        flags = Int.read(b)
-        
-        big = True if flags & (1 << 0) else False
-        peer = TLObject.read(b)
-        
-        photo_id = Long.read(b)
-        
-        return InputPeerPhotoFileLocation(peer=peer, photo_id=photo_id, big=big)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.big else 0
-        b.write(Int(flags))
-        
-        b.write(self.peer.write())
-        
-        b.write(Long(self.photo_id))
-        
-        return b.getvalue()
+        self.has_spoiler = has_spoiler
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/input_single_media.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,89 +12,57 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from typing import Optional, List
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
+import pyrogram
+from pyrogram import raw, types, utils, enums
+from .input_message_content import InputMessageContent
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
 
-
-class InputSingleMedia(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.InputSingleMedia`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``1CC6E91F``
+class InputTextMessageContent(InputMessageContent):
+    """Content of a text message to be sent as the result of an inline query.
 
     Parameters:
-        media (:obj:`InputMedia <pyrogram.raw.base.InputMedia>`):
-            N/A
+        message_text (``str``):
+            Text of the message to be sent, 1-4096 characters.
 
-        random_id (``int`` ``64-bit``):
-            N/A
+        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
+            By default, texts are parsed using both Markdown and HTML styles.
+            You can combine both syntaxes together.
 
-        message (``str``):
-            N/A
-
-        entities (List of :obj:`MessageEntity <pyrogram.raw.base.MessageEntity>`, *optional*):
-            N/A
+        entities (List of :obj:`~pyrogram.types.MessageEntity`):
+            List of special entities that appear in message text, which can be specified instead of *parse_mode*.
 
+        disable_web_page_preview (``bool``, *optional*):
+            Disables link previews for links in this message.
     """
 
-    __slots__: List[str] = ["media", "random_id", "message", "entities"]
-
-    ID = 0x1cc6e91f
-    QUALNAME = "types.InputSingleMedia"
-
-    def __init__(self, *, media: "raw.base.InputMedia", random_id: int, message: str, entities: Optional[List["raw.base.MessageEntity"]] = None) -> None:
-        self.media = media  # InputMedia
-        self.random_id = random_id  # long
-        self.message = message  # string
-        self.entities = entities  # flags.0?Vector<MessageEntity>
-
-    @staticmethod
-    def read(b: BytesIO, *args: Any) -> "InputSingleMedia":
-        
-        flags = Int.read(b)
-        
-        media = TLObject.read(b)
-        
-        random_id = Long.read(b)
-        
-        message = String.read(b)
-        
-        entities = TLObject.read(b) if flags & (1 << 0) else []
-        
-        return InputSingleMedia(media=media, random_id=random_id, message=message, entities=entities)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.entities else 0
-        b.write(Int(flags))
-        
-        b.write(self.media.write())
-        
-        b.write(Long(self.random_id))
-        
-        b.write(String(self.message))
-        
-        if self.entities is not None:
-            b.write(Vector(self.entities))
-        
-        return b.getvalue()
+    def __init__(
+        self,
+        message_text: str,
+        parse_mode: Optional["enums.ParseMode"] = None,
+        entities: List["types.MessageEntity"] = None,
+        disable_web_page_preview: bool = None
+    ):
+        super().__init__()
+
+        self.message_text = message_text
+        self.parse_mode = parse_mode
+        self.entities = entities
+        self.disable_web_page_preview = disable_web_page_preview
+
+    async def write(self, client: "pyrogram.Client", reply_markup):
+        message, entities = (await utils.parse_text_entities(
+            client, self.message_text, self.parse_mode, self.entities
+        )).values()
+
+        return raw.types.InputBotInlineMessageText(
+            no_webpage=self.disable_web_page_preview or None,
+            reply_markup=await reply_markup.write(client) if reply_markup else None,
+            message=message,
+            entities=entities
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/raw/types/keyboard_button_switch_inline.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,87 +12,84 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from io import BytesIO
+from pyrogram import raw, types
+from ..object import Object
 
-from pyrogram.raw.core.primitives import Int, Long, Int128, Int256, Bool, Bytes, String, Double, Vector
-from pyrogram.raw.core import TLObject
-from pyrogram import raw
-from typing import List, Optional, Any
 
-# # # # # # # # # # # # # # # # # # # # # # # #
-#               !!! WARNING !!!               #
-#          This is a generated file!          #
-# All changes made in this file will be lost! #
-# # # # # # # # # # # # # # # # # # # # # # # #
-
-
-class KeyboardButtonSwitchInline(TLObject):  # type: ignore
-    """Telegram API type.
-
-    Constructor of :obj:`~pyrogram.raw.base.KeyboardButton`.
-
-    Details:
-        - Layer: ``158``
-        - ID: ``93B9FBB5``
+class KeyboardButton(Object):
+    """One button of the reply keyboard.
+    For simple text buttons String can be used instead of this object to specify text of the button.
+    Optional fields are mutually exclusive.
 
     Parameters:
         text (``str``):
-            N/A
+            Text of the button. If none of the optional fields are used, it will be sent as a message when
+            the button is pressed.
 
-        query (``str``):
-            N/A
-
-        same_peer (``bool``, *optional*):
-            N/A
-
-        peer_types (List of :obj:`InlineQueryPeerType <pyrogram.raw.base.InlineQueryPeerType>`, *optional*):
-            N/A
+        request_contact (``bool``, *optional*):
+            If True, the user's phone number will be sent as a contact when the button is pressed.
+            Available in private chats only.
+
+        request_location (``bool``, *optional*):
+            If True, the user's current location will be sent when the button is pressed.
+            Available in private chats only.
+
+        web_app (:obj:`~pyrogram.types.WebAppInfo`, *optional*):
+            If specified, the described `Web App <https://core.telegram.org/bots/webapps>`_ will be launched when the
+            button is pressed. The Web App will be able to send a “web_app_data” service message. Available in private
+            chats only.
 
     """
 
-    __slots__: List[str] = ["text", "query", "same_peer", "peer_types"]
-
-    ID = 0x93b9fbb5
-    QUALNAME = "types.KeyboardButtonSwitchInline"
-
-    def __init__(self, *, text: str, query: str, same_peer: Optional[bool] = None, peer_types: Optional[List["raw.base.InlineQueryPeerType"]] = None) -> None:
-        self.text = text  # string
-        self.query = query  # string
-        self.same_peer = same_peer  # flags.0?true
-        self.peer_types = peer_types  # flags.1?Vector<InlineQueryPeerType>
+    def __init__(
+        self,
+        text: str,
+        request_contact: bool = None,
+        request_location: bool = None,
+        web_app: "types.WebAppInfo" = None
+    ):
+        super().__init__()
+
+        self.text = str(text)
+        self.request_contact = request_contact
+        self.request_location = request_location
+        self.web_app = web_app
 
     @staticmethod
-    def read(b: BytesIO, *args: Any) -> "KeyboardButtonSwitchInline":
-        
-        flags = Int.read(b)
-        
-        same_peer = True if flags & (1 << 0) else False
-        text = String.read(b)
-        
-        query = String.read(b)
-        
-        peer_types = TLObject.read(b) if flags & (1 << 1) else []
-        
-        return KeyboardButtonSwitchInline(text=text, query=query, same_peer=same_peer, peer_types=peer_types)
-
-    def write(self, *args) -> bytes:
-        b = BytesIO()
-        b.write(Int(self.ID, False))
-
-        flags = 0
-        flags |= (1 << 0) if self.same_peer else 0
-        flags |= (1 << 1) if self.peer_types else 0
-        b.write(Int(flags))
-        
-        b.write(String(self.text))
-        
-        b.write(String(self.query))
-        
-        if self.peer_types is not None:
-            b.write(Vector(self.peer_types))
-        
-        return b.getvalue()
+    def read(b):
+        if isinstance(b, raw.types.KeyboardButton):
+            return b.text
+
+        if isinstance(b, raw.types.KeyboardButtonRequestPhone):
+            return KeyboardButton(
+                text=b.text,
+                request_contact=True
+            )
+
+        if isinstance(b, raw.types.KeyboardButtonRequestGeoLocation):
+            return KeyboardButton(
+                text=b.text,
+                request_location=True
+            )
+
+        if isinstance(b, raw.types.KeyboardButtonSimpleWebView):
+            return KeyboardButton(
+                text=b.text,
+                web_app=types.WebAppInfo(
+                    url=b.url
+                )
+            )
+
+    def write(self):
+        if self.request_contact:
+            return raw.types.KeyboardButtonRequestPhone(text=self.text)
+        elif self.request_location:
+            return raw.types.KeyboardButtonRequestGeoLocation(text=self.text)
+        elif self.web_app:
+            return raw.types.KeyboardButtonSimpleWebView(text=self.text, url=self.web_app.url)
+        else:
+            return raw.types.KeyboardButton(text=self.text)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .auth import Auth
-from .session import Session
+from .data_center import DataCenter
+from .msg_factory import MsgFactory
+from .msg_id import MsgId
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/auth.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from .data_center import DataCenter
-from .msg_factory import MsgFactory
-from .msg_id import MsgId
+from ..object import Object
+
+
+class GeneralTopicUnhidden(Object):
+    """A service message about a general topic unhidden in the chat.
+
+    Currently holds no information.
+    """
+
+    def __init__(self):
+        super().__init__()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/data_center.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/internals/seq_no.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,23 +12,18 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from threading import Lock
+from ..object import Object
 
 
-class SeqNo:
-    def __init__(self):
-        self.content_related_messages_sent = 0
-        self.lock = Lock()
-
-    def __call__(self, is_content_related: bool) -> int:
-        with self.lock:
-            seq_no = (self.content_related_messages_sent * 2) + (1 if is_content_related else 0)
+class CallbackGame(Object):
+    """Placeholder, currently holds no information.
 
-            if is_content_related:
-                self.content_related_messages_sent += 1
+    Use BotFather to set up your game.
+    """
 
-            return seq_no
+    def __init__(self):
+        super().__init__()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/session/session.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/memory_storage.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/mongo_storage.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/sqlite_storage.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/storage/storage.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/sync.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/authorization/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/authorization/sent_code.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-dev-2.1.8.dev202305201740/tests/filters/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,21 +12,25 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import pyrogram
-from pyrogram import raw
-from .bot_command_scope import BotCommandScope
+class Client:
+    def __init__(self):
+        self.me = User("username")
 
+    async def get_me(self):
+        return self.me
 
-class BotCommandScopeAllGroupChats(BotCommandScope):
-    """Represents the scope of bot commands, covering all group and supergroup chats.
-    """
 
-    def __init__(self):
-        super().__init__("all_group_chats")
+class User:
+    def __init__(self, username: str = None):
+        self.username = username
+
 
-    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
-        return raw.types.BotCommandScopeChats()
+class Message:
+    def __init__(self, text: str = None, caption: str = None):
+        self.text = text
+        self.caption = caption
+        self.command = None
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,37 +12,35 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Union
-
-import pyrogram
 from pyrogram import raw
-from .bot_command_scope import BotCommandScope
+from ..object import Object
 
 
-class BotCommandScopeChatMember(BotCommandScope):
-    """Represents the scope of bot commands, covering a specific member of a group or supergroup chat.
+class PeerChannel(Object):
+    """A PeerChannel.
 
-    Parameters:
-        chat_id (``int`` | ``str``):
-            Unique identifier for the target chat or username of the target supergroup (in the format
-            @supergroupusername).
 
-        user_id (``int`` | ``str``):
-            Unique identifier of the target user.
+    Parameters:
+        channel_id (``Integer``):
+            Id of the channel.
     """
 
-    def __init__(self, chat_id: Union[int, str], user_id: Union[int, str]):
-        super().__init__("chat_member")
+    def __init__(
+        self, *,
+        channel_id: int
+    ):
+        super().__init__()
+
+        self.channel_id = channel_id
+
+    @staticmethod
+    def _parse(action: "raw.types.PeerChannel") -> "PeerChannel":
 
-        self.chat_id = chat_id
-        self.user_id = user_id
 
-    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
-        return raw.types.BotCommandScopePeerUser(
-            peer=await client.resolve_peer(self.chat_id),
-            user_id=await client.resolve_peer(self.user_id)
+        return PeerChannel(
+            channel_id=getattr(action,"channel_id", None)
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
 from pyrogram import raw
-from .bot_command_scope import BotCommandScope
+from .menu_button import MenuButton
 
 
-class BotCommandScopeDefault(BotCommandScope):
-    """Represents the default scope of bot commands.
-    Default commands are used if no commands with a narrower scope are specified for the user.
+class MenuButtonCommands(MenuButton):
+    """A menu button, which opens the bot's list of commands.
     """
 
     def __init__(self):
-        super().__init__("default")
+        super().__init__("commands")
 
-    async def write(self, client: "pyrogram.Client") -> "raw.base.BotCommandScope":
-        return raw.types.BotCommandScopeDefault()
+    async def write(self, client: "pyrogram.Client") -> "raw.types.BotMenuButtonCommands":
+        return raw.types.BotMenuButtonCommands()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from ..object import Object
 
 
-class CallbackGame(Object):
-    """Placeholder, currently holds no information.
+class ChatJoinedByRequest(Object):
+    """A service message about a user join request approved in the chat.
 
-    Use BotFather to set up your game.
+    Currently holds no information.
     """
 
     def __init__(self):
         super().__init__()
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/game.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,58 +13,87 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
-from pyrogram import raw, utils
+from pyrogram import raw
 from pyrogram import types
 from ..object import Object
 
 
-class GameHighScore(Object):
-    """One row of the high scores table for a game.
+class Game(Object):
+    """A game.
+    Use BotFather to create and edit games, their short names will act as unique identifiers.
 
     Parameters:
-        user (:obj:`~pyrogram.types.User`):
-            User.
+        id (``int``):
+            Unique identifier of the game.
 
-        score (``int``):
-            Score.
+        title (``str``):
+            Title of the game.
 
-        position (``int``, *optional*):
-            Position in high score table for the game.
+        short_name (``str``):
+            Unique short name of the game.
+
+        description (``str``):
+            Description of the game.
+
+        photo (:obj:`~pyrogram.types.Photo`):
+            Photo that will be displayed in the game message in chats.
+
+        animation (:obj:`~pyrogram.types.Animation`, *optional*):
+            Animation that will be displayed in the game message in chats.
+            Upload via BotFather.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
-        user: "types.User",
-        score: int,
-        position: int = None
+        id: int,
+        title: str,
+        short_name: str,
+        description: str,
+        photo: "types.Photo",
+        animation: "types.Animation" = None
     ):
         super().__init__(client)
 
-        self.user = user
-        self.score = score
-        self.position = position
-
-    @staticmethod
-    def _parse(client, game_high_score: raw.types.HighScore, users: dict) -> "GameHighScore":
-        users = {i.id: i for i in users}
-
-        return GameHighScore(
-            user=types.User._parse(client, users[game_high_score.user_id]),
-            score=game_high_score.score,
-            position=game_high_score.pos,
-            client=client
-        )
+        self.id = id
+        self.title = title
+        self.short_name = short_name
+        self.description = description
+        self.photo = photo
+        self.animation = animation
 
     @staticmethod
-    def _parse_action(client, service: raw.types.MessageService, users: dict):
-        return GameHighScore(
-            user=types.User._parse(client, users[utils.get_raw_peer_id(service.from_id or service.peer_id)]),
-            score=service.action.score,
+    def _parse(client, message: "raw.types.Message") -> "Game":
+        game: "raw.types.Game" = message.media.game
+        animation = None
+
+        if game.document:
+            attributes = {type(i): i for i in game.document.attributes}
+
+            file_name = getattr(
+                attributes.get(
+                    raw.types.DocumentAttributeFilename, None
+                ), "file_name", None
+            )
+
+            animation = types.Animation._parse(
+                client,
+                game.document,
+                attributes.get(raw.types.DocumentAttributeVideo, None),
+                file_name
+            )
+
+        return Game(
+            id=game.id,
+            title=game.title,
+            short_name=game.short_name,
+            description=game.description,
+            photo=types.Photo._parse(client, game.photo),
+            animation=animation,
             client=client
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,84 +12,79 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from pyrogram import raw, types
+from pyrogram import raw
+
 from ..object import Object
 
 
-class KeyboardButton(Object):
-    """One button of the reply keyboard.
-    For simple text buttons String can be used instead of this object to specify text of the button.
-    Optional fields are mutually exclusive.
+class LoginUrl(Object):
+    """Represents a parameter of the inline keyboard button used to automatically authorize a user.
+
+    Serves as a great replacement for the Telegram Login Widget when the user is coming from Telegram.
+    All the user needs to do is tap/click a button and confirm that they want to log in.
 
     Parameters:
-        text (``str``):
-            Text of the button. If none of the optional fields are used, it will be sent as a message when
-            the button is pressed.
-
-        request_contact (``bool``, *optional*):
-            If True, the user's phone number will be sent as a contact when the button is pressed.
-            Available in private chats only.
-
-        request_location (``bool``, *optional*):
-            If True, the user's current location will be sent when the button is pressed.
-            Available in private chats only.
-
-        web_app (:obj:`~pyrogram.types.WebAppInfo`, *optional*):
-            If specified, the described `Web App <https://core.telegram.org/bots/webapps>`_ will be launched when the
-            button is pressed. The Web App will be able to send a “web_app_data” service message. Available in private
-            chats only.
+        url (``str``):
+            An HTTP URL to be opened with user authorization data added to the query string when the button is pressed.
+            If the user refuses to provide authorization data, the original URL without information about the user will
+            be opened. The data added is the same as described in
+            `Receiving authorization data <https://core.telegram.org/widgets/login#receiving-authorization-data>`.
+
+            **NOTE**: You **must** always check the hash of the received data to verify the authentication and the
+            integrity of the data as described in
+            `Checking authorization <https://core.telegram.org/widgets/login#checking-authorization>`_.
+
+        forward_text (``str``, *optional*):
+            New text of the button in forwarded messages.
+
+        bot_username (``str``, *optional*):
+            Username of a bot, which will be used for user authorization.
+            See `Setting up a bot <https://core.telegram.org/widgets/login#setting-up-a-bot>`_ for more details.
+            If not specified, the current bot's username will be assumed. The url's domain must be the same as the
+            domain linked with the bot.
+            See `Linking your domain to the bot <https://core.telegram.org/widgets/login#linking-your-domain-to-the-bot>`_
+            for more details.
+
+        request_write_access (``str``, *optional*):
+            Pass True to request the permission for your bot to send messages to the user.
 
+        button_id (``int``):
+            Button identifier.
     """
 
     def __init__(
-        self,
-        text: str,
-        request_contact: bool = None,
-        request_location: bool = None,
-        web_app: "types.WebAppInfo" = None
+        self, *,
+        url: str,
+        forward_text: str = None,
+        bot_username: str = None,
+        request_write_access: str = None,
+        button_id: int = None
     ):
         super().__init__()
 
-        self.text = str(text)
-        self.request_contact = request_contact
-        self.request_location = request_location
-        self.web_app = web_app
+        self.url = url
+        self.forward_text = forward_text
+        self.bot_username = bot_username
+        self.request_write_access = request_write_access
+        self.button_id = button_id
 
     @staticmethod
-    def read(b):
-        if isinstance(b, raw.types.KeyboardButton):
-            return b.text
-
-        if isinstance(b, raw.types.KeyboardButtonRequestPhone):
-            return KeyboardButton(
-                text=b.text,
-                request_contact=True
-            )
-
-        if isinstance(b, raw.types.KeyboardButtonRequestGeoLocation):
-            return KeyboardButton(
-                text=b.text,
-                request_location=True
-            )
-
-        if isinstance(b, raw.types.KeyboardButtonSimpleWebView):
-            return KeyboardButton(
-                text=b.text,
-                web_app=types.WebAppInfo(
-                    url=b.url
-                )
-            )
-
-    def write(self):
-        if self.request_contact:
-            return raw.types.KeyboardButtonRequestPhone(text=self.text)
-        elif self.request_location:
-            return raw.types.KeyboardButtonRequestGeoLocation(text=self.text)
-        elif self.web_app:
-            return raw.types.KeyboardButtonSimpleWebView(text=self.text, url=self.web_app.url)
-        else:
-            return raw.types.KeyboardButton(text=self.text)
+    def read(b: "raw.types.KeyboardButtonUrlAuth") -> "LoginUrl":
+        return LoginUrl(
+            url=b.url,
+            forward_text=b.fwd_text,
+            button_id=b.button_id
+        )
+
+    def write(self, text: str, bot: "raw.types.InputUser"):
+        return raw.types.InputKeyboardButtonUrlAuth(
+            text=text,
+            url=self.url,
+            bot=bot,
+            fwd_text=self.forward_text,
+            request_write_access=self.request_write_access
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,35 @@
 
 import pyrogram
 from pyrogram import raw, types, utils, enums
 from .inline_query_result import InlineQueryResult
 from ...file_id import FileId
 
 
-class InlineQueryResultCachedAudio(InlineQueryResult):
-    """A link to an MP3 audio file stored on the Telegram servers
+class InlineQueryResultCachedVideo(InlineQueryResult):
+    """A link to a video file stored on the Telegram servers.
 
-    By default, this audio file will be sent by the user. Alternatively, you can use *input_message_content* to send a
-    message with the specified content instead of the audio.
+    By default, this video file will be sent by the user with an optional caption.
+    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
+    video.
 
     Parameters:
-        audio_file_id (``str``):
-            A valid file identifier for the audio file.
+        video_file_id (``str``):
+            A valid file identifier for the video file.
+
+        title (``str``):
+            Title for the result.
 
         id (``str``, *optional*):
             Unique identifier for this result, 1-64 bytes.
             Defaults to a randomly generated UUID4.
 
+        description (``str``, *optional*):
+            Short description of the result.
+
         caption (``str``, *optional*):
             Caption of the photo to be sent, 0-1024 characters.
 
         parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
 
@@ -53,41 +60,47 @@
 
         input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
             Content of the message to be sent instead of the photo.
     """
 
     def __init__(
         self,
-        audio_file_id: str,
+        video_file_id: str,
+        title: str,
         id: str = None,
+        description: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
         reply_markup: "types.InlineKeyboardMarkup" = None,
         input_message_content: "types.InputMessageContent" = None
     ):
-        super().__init__("audio", id, input_message_content, reply_markup)
+        super().__init__("video", id, input_message_content, reply_markup)
 
-        self.audio_file_id = audio_file_id
+        self.video_file_id = video_file_id
+        self.title = title
+        self.description = description
         self.caption = caption
         self.parse_mode = parse_mode
         self.caption_entities = caption_entities
         self.reply_markup = reply_markup
         self.input_message_content = input_message_content
 
     async def write(self, client: "pyrogram.Client"):
         message, entities = (await utils.parse_text_entities(
             client, self.caption, self.parse_mode, self.caption_entities
         )).values()
 
-        file_id = FileId.decode(self.audio_file_id)
+        file_id = FileId.decode(self.video_file_id)
 
         return raw.types.InputBotInlineResultDocument(
             id=self.id,
             type=self.type,
+            title=self.title,
+            description=self.description,
             document=raw.types.InputDocument(
                 id=file_id.media_id,
                 access_hash=file_id.access_hash,
                 file_reference=file_id.file_reference,
             ),
             send_message=(
                 await self.input_message_content.write(client, self.reply_markup)
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,92 +17,132 @@
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Optional, List
 
 import pyrogram
 from pyrogram import raw, types, utils, enums
 from .inline_query_result import InlineQueryResult
-from ...file_id import FileId
 
 
-class InlineQueryResultCachedPhoto(InlineQueryResult):
-    """A link to a photo stored on the Telegram servers.
+class InlineQueryResultVideo(InlineQueryResult):
+    """Link to a page containing an embedded video player or a video file.
 
-    By default, this photo will be sent by the user with an optional caption. Alternatively, you can use
-    *input_message_content* to send a message with the specified content instead of the photo.
+    By default, this video file will be sent by the user with an optional caption.
+    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
+    video.
 
     Parameters:
-        photo_file_id (``str``):
-            A valid file identifier of the photo.
+        video_url (``str``):
+            A valid URL for the embedded video player or video file.
+
+        thumb_url (``str``):
+            URL of the thumbnail (jpeg only) for the video.
+
+        title (``str``):
+            Title for the result.
 
         id (``str``, *optional*):
             Unique identifier for this result, 1-64 bytes.
             Defaults to a randomly generated UUID4.
 
-        title (``str``, *optional*):
-            Title for the result.
+        mime_type (``str``):
+            Mime type of the content of video url, "text/html" or "video/mp4".
+            Defaults to "video/mp4".
+
+        video_width (``int``):
+            Video width.
+
+        video_height (``int``):
+            Video height.
+
+        video_duration (``int``):
+            Video duration in seconds.
 
         description (``str``, *optional*):
             Short description of the result.
 
         caption (``str``, *optional*):
-            Caption of the photo to be sent, 0-1024 characters.
+            Caption of the video to be sent, 0-1024 characters.
 
         parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
 
         caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
             List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
         reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
-            An InlineKeyboardMarkup object.
+            Inline keyboard attached to the message
 
         input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
-            Content of the message to be sent instead of the photo.
+            Content of the message to be sent instead of the video. This field is required if InlineQueryResultVideo is
+            used to send an HTML-page as a result (e.g., a YouTube video).
     """
 
     def __init__(
         self,
-        photo_file_id: str,
+        video_url: str,
+        thumb_url: str,
+        title: str,
         id: str = None,
-        title: str = None,
+        mime_type: str = "video/mp4",
+        video_width: int = 0,
+        video_height: int = 0,
+        video_duration: int = 0,
         description: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
         reply_markup: "types.InlineKeyboardMarkup" = None,
         input_message_content: "types.InputMessageContent" = None
     ):
-        super().__init__("photo", id, input_message_content, reply_markup)
+        super().__init__("video", id, input_message_content, reply_markup)
 
-        self.photo_file_id = photo_file_id
+        self.video_url = video_url
+        self.thumb_url = thumb_url
         self.title = title
+        self.video_width = video_width
+        self.video_height = video_height
+        self.video_duration = video_duration
         self.description = description
         self.caption = caption
         self.parse_mode = parse_mode
         self.caption_entities = caption_entities
-        self.reply_markup = reply_markup
-        self.input_message_content = input_message_content
+        self.mime_type = mime_type
 
     async def write(self, client: "pyrogram.Client"):
+        video = raw.types.InputWebDocument(
+            url=self.video_url,
+            size=0,
+            mime_type=self.mime_type,
+            attributes=[raw.types.DocumentAttributeVideo(
+                duration=self.video_duration,
+                w=self.video_width,
+                h=self.video_height
+            )]
+        )
+
+        thumb = raw.types.InputWebDocument(
+            url=self.thumb_url,
+            size=0,
+            mime_type="image/jpeg",
+            attributes=[]
+        )
+
         message, entities = (await utils.parse_text_entities(
             client, self.caption, self.parse_mode, self.caption_entities
         )).values()
 
-        file_id = FileId.decode(self.photo_file_id)
-
-        return raw.types.InputBotInlineResultPhoto(
+        return raw.types.InputBotInlineResult(
             id=self.id,
             type=self.type,
-            photo=raw.types.InputPhoto(
-                id=file_id.media_id,
-                access_hash=file_id.access_hash,
-                file_reference=file_id.file_reference,
-            ),
+            title=self.title,
+            description=self.description,
+            thumb=thumb,
+            content=video,
             send_message=(
                 await self.input_message_content.write(client, self.reply_markup)
                 if self.input_message_content
                 else raw.types.InputBotInlineMessageMediaAuto(
                     reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
                     message=message,
                     entities=entities
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,64 +15,100 @@
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
 from pyrogram import raw, types
 from .inline_query_result import InlineQueryResult
-from ...file_id import FileId
 
 
-class InlineQueryResultCachedSticker(InlineQueryResult):
-    """A link to a sticker stored on the Telegram servers
+class InlineQueryResultContact(InlineQueryResult):
+    """Contact with a phone number
+    
+    By default, this contact will be sent by the user.
+    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
+    contact.
+    
+    Parameters:
+        phone_number (``str``):
+            Contact's phone number.
 
-    By default, this sticker will be sent by the user. Alternatively, you can use *input_message_content* to send a
-    message with the specified content instead of the sticker.
+        first_name (``str``):
+            Contact's first name.
 
-    Parameters:
-        sticker_file_id (``str``):
-            A valid file identifier of the sticker.
+        last_name (``str``, *optional*):
+            Contact's last name.
+
+        vcard (``str``, *optional*):
+            Additional data about the contact in the form of a `vCard <https://en.wikipedia.org/wiki/VCard>`_.
 
         id (``str``, *optional*):
             Unique identifier for this result, 1-64 bytes.
             Defaults to a randomly generated UUID4.
 
         reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
-            An InlineKeyboardMarkup object.
+            Inline keyboard attached to the message.
+            
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`, *optional*):
+            Content of the message to be sent instead of the contact.
+
+        thumb_url (``str``, *optional*):
+            Url of the thumbnail for the result.
 
-        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
-            Content of the message to be sent instead of the photo.
+        thumb_width (``int``, *optional*):
+            Thumbnail width.
+
+        thumb_height (``int``, *optional*):
+            Thumbnail height.
     """
 
     def __init__(
         self,
-        sticker_file_id: str,
+        phone_number: str,
+        first_name: str,
+        last_name: str = "",
+        vcard: str = "",
         id: str = None,
         reply_markup: "types.InlineKeyboardMarkup" = None,
-        input_message_content: "types.InputMessageContent" = None
+        input_message_content: "types.InputMessageContent" = None,
+        thumb_url: str = None,
+        thumb_width: int = 0,
+        thumb_height: int = 0
     ):
-        super().__init__("sticker", id, input_message_content, reply_markup)
+        super().__init__("contact", id, input_message_content, reply_markup)
 
-        self.sticker_file_id = sticker_file_id
-        self.reply_markup = reply_markup
-        self.input_message_content = input_message_content
+        self.phone_number = phone_number
+        self.first_name = first_name
+        self.last_name = last_name
+        self.vcard = vcard
+        self.thumb_url = thumb_url
+        self.thumb_width = thumb_width
+        self.thumb_height = thumb_height
 
     async def write(self, client: "pyrogram.Client"):
-        file_id = FileId.decode(self.sticker_file_id)
-
-        return raw.types.InputBotInlineResultDocument(
+        return raw.types.InputBotInlineResult(
             id=self.id,
             type=self.type,
-            document=raw.types.InputDocument(
-                id=file_id.media_id,
-                access_hash=file_id.access_hash,
-                file_reference=file_id.file_reference,
-            ),
+            title=self.first_name,
             send_message=(
                 await self.input_message_content.write(client, self.reply_markup)
                 if self.input_message_content
-                else raw.types.InputBotInlineMessageMediaAuto(
+                else raw.types.InputBotInlineMessageMediaContact(
+                    phone_number=self.phone_number,
+                    first_name=self.first_name,
+                    last_name=self.last_name,
+                    vcard=self.vcard,
                     reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
-                    message="",
                 )
-            )
+            ),
+            thumb=raw.types.InputWebDocument(
+                url=self.thumb_url,
+                size=0,
+                mime_type="image/jpg",
+                attributes=[
+                    raw.types.DocumentAttributeImageSize(
+                        w=self.thumb_width,
+                        h=self.thumb_height
+                    )
+                ]
+            ) if self.thumb_url else None
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/photo.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,103 +12,119 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List
+from datetime import datetime
+from typing import List
 
 import pyrogram
-from pyrogram import raw, types, utils, enums
-from .inline_query_result import InlineQueryResult
-from ...file_id import FileId
+from pyrogram import raw, utils
+from pyrogram import types
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
+from ..object import Object
 
 
-class InlineQueryResultCachedVideo(InlineQueryResult):
-    """A link to a video file stored on the Telegram servers.
-
-    By default, this video file will be sent by the user with an optional caption.
-    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
-    video.
+class Photo(Object):
+    """A Photo.
 
     Parameters:
-        video_file_id (``str``):
-            A valid file identifier for the video file.
-
-        title (``str``):
-            Title for the result.
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        id (``str``, *optional*):
-            Unique identifier for this result, 1-64 bytes.
-            Defaults to a randomly generated UUID4.
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-        description (``str``, *optional*):
-            Short description of the result.
+        width (``int``):
+            Photo width.
 
-        caption (``str``, *optional*):
-            Caption of the photo to be sent, 0-1024 characters.
+        height (``int``):
+            Photo height.
 
-        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
-            By default, texts are parsed using both Markdown and HTML styles.
-            You can combine both syntaxes together.
+        file_size (``int``):
+            File size.
 
-        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
-            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+        date (:py:obj:`~datetime.datetime`):
+            Date the photo was sent.
 
-        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
-            An InlineKeyboardMarkup object.
+        ttl_seconds (``int``, *optional*):
+            Time-to-live seconds, for secret photos.
 
-        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
-            Content of the message to be sent instead of the photo.
+        thumbs (List of :obj:`~pyrogram.types.Thumbnail`, *optional*):
+            Available thumbnails of this photo.
     """
 
     def __init__(
         self,
-        video_file_id: str,
-        title: str,
-        id: str = None,
-        description: str = None,
-        caption: str = "",
-        parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List["types.MessageEntity"] = None,
-        reply_markup: "types.InlineKeyboardMarkup" = None,
-        input_message_content: "types.InputMessageContent" = None
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        width: int,
+        height: int,
+        file_size: int,
+        date: datetime,
+        ttl_seconds: int = None,
+        thumbs: List["types.Thumbnail"] = None
     ):
-        super().__init__("video", id, input_message_content, reply_markup)
+        super().__init__(client)
 
-        self.video_file_id = video_file_id
-        self.title = title
-        self.description = description
-        self.caption = caption
-        self.parse_mode = parse_mode
-        self.caption_entities = caption_entities
-        self.reply_markup = reply_markup
-        self.input_message_content = input_message_content
-
-    async def write(self, client: "pyrogram.Client"):
-        message, entities = (await utils.parse_text_entities(
-            client, self.caption, self.parse_mode, self.caption_entities
-        )).values()
-
-        file_id = FileId.decode(self.video_file_id)
-
-        return raw.types.InputBotInlineResultDocument(
-            id=self.id,
-            type=self.type,
-            title=self.title,
-            description=self.description,
-            document=raw.types.InputDocument(
-                id=file_id.media_id,
-                access_hash=file_id.access_hash,
-                file_reference=file_id.file_reference,
-            ),
-            send_message=(
-                await self.input_message_content.write(client, self.reply_markup)
-                if self.input_message_content
-                else raw.types.InputBotInlineMessageMediaAuto(
-                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
-                    message=message,
-                    entities=entities
-                )
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.width = width
+        self.height = height
+        self.file_size = file_size
+        self.date = date
+        self.ttl_seconds = ttl_seconds
+        self.thumbs = thumbs
+
+    @staticmethod
+    def _parse(client, photo: "raw.types.Photo", ttl_seconds: int = None) -> "Photo":
+        if isinstance(photo, raw.types.Photo):
+            photos: List[raw.types.PhotoSize] = []
+
+            for p in photo.sizes:
+                if isinstance(p, raw.types.PhotoSize):
+                    photos.append(p)
+
+                if isinstance(p, raw.types.PhotoSizeProgressive):
+                    photos.append(
+                        raw.types.PhotoSize(
+                            type=p.type,
+                            w=p.w,
+                            h=p.h,
+                            size=max(p.sizes)
+                        )
+                    )
+
+            photos.sort(key=lambda p: p.size)
+
+            main = photos[-1]
+
+            return Photo(
+                file_id=FileId(
+                    file_type=FileType.PHOTO,
+                    dc_id=photo.dc_id,
+                    media_id=photo.id,
+                    access_hash=photo.access_hash,
+                    file_reference=photo.file_reference,
+                    thumbnail_source=ThumbnailSource.THUMBNAIL,
+                    thumbnail_file_type=FileType.PHOTO,
+                    thumbnail_size=main.type,
+                    volume_id=0,
+                    local_id=0
+                ).encode(),
+                file_unique_id=FileUniqueId(
+                    file_unique_type=FileUniqueType.DOCUMENT,
+                    media_id=photo.id
+                ).encode(),
+                width=main.w,
+                height=main.h,
+                file_size=main.size,
+                date=utils.timestamp_to_datetime(photo.date),
+                ttl_seconds=ttl_seconds,
+                thumbs=types.Thumbnail._parse(client, photo),
+                client=client
             )
-        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/audio.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,97 +12,110 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List
+from datetime import datetime
+from typing import List
 
 import pyrogram
-from pyrogram import raw, types, utils, enums
-from .inline_query_result import InlineQueryResult
-from ...file_id import FileId
+from pyrogram import raw, utils
+from pyrogram import types
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
+from ..object import Object
 
 
-class InlineQueryResultCachedVoice(InlineQueryResult):
-    """A link to a voice message stored on the Telegram servers.
-
-    By default, this voice message will be sent by the user.
-    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the voice
-    message.
+class Audio(Object):
+    """An audio file to be treated as music by the Telegram clients.
 
     Parameters:
-        voice_file_id (``str``):
-            A valid file identifier for the voice message.
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
+
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
+
+        duration (``int``):
+            Duration of the audio in seconds as defined by sender.
 
-        id (``str``, *optional*):
-            Unique identifier for this result, 1-64 bytes.
-            Defaults to a randomly generated UUID4.
+        performer (``str``, *optional*):
+            Performer of the audio as defined by sender or by audio tags.
 
         title (``str``, *optional*):
-            Title for the result.
+            Title of the audio as defined by sender or by audio tags.
 
-        caption (``str``, *optional*):
-            Caption of the photo to be sent, 0-1024 characters.
+        file_name (``str``, *optional*):
+            Audio file name.
 
-        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
-            By default, texts are parsed using both Markdown and HTML styles.
-            You can combine both syntaxes together.
+        mime_type (``str``, *optional*):
+            MIME type of the file as defined by sender.
 
-        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
-            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+        file_size (``int``, *optional*):
+            File size.
 
-        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
-            An InlineKeyboardMarkup object.
+        date (:py:obj:`~datetime.datetime`, *optional*):
+            Date the audio was originally sent.
 
-        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
-            Content of the message to be sent instead of the photo.
+        thumbs (List of :obj:`~pyrogram.types.Thumbnail`, *optional*):
+            Thumbnails of the music file album cover.
     """
 
     def __init__(
         self,
-        voice_file_id: str,
-        id: str = None,
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        duration: int,
+        performer: str = None,
         title: str = None,
-        caption: str = "",
-        parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List["types.MessageEntity"] = None,
-        reply_markup: "types.InlineKeyboardMarkup" = None,
-        input_message_content: "types.InputMessageContent" = None
+        file_name: str = None,
+        mime_type: str = None,
+        file_size: int = None,
+        date: datetime = None,
+        thumbs: List["types.Thumbnail"] = None
     ):
-        super().__init__("voice", id, input_message_content, reply_markup)
+        super().__init__(client)
 
-        self.voice_file_id = voice_file_id
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.duration = duration
+        self.performer = performer
         self.title = title
-        self.caption = caption
-        self.parse_mode = parse_mode
-        self.caption_entities = caption_entities
-        self.reply_markup = reply_markup
-        self.input_message_content = input_message_content
-
-    async def write(self, client: "pyrogram.Client"):
-        message, entities = (await utils.parse_text_entities(
-            client, self.caption, self.parse_mode, self.caption_entities
-        )).values()
-
-        file_id = FileId.decode(self.voice_file_id)
-
-        return raw.types.InputBotInlineResultDocument(
-            id=self.id,
-            type=self.type,
-            title=self.title,
-            document=raw.types.InputDocument(
-                id=file_id.media_id,
-                access_hash=file_id.access_hash,
-                file_reference=file_id.file_reference,
-            ),
-            send_message=(
-                await self.input_message_content.write(client, self.reply_markup)
-                if self.input_message_content
-                else raw.types.InputBotInlineMessageMediaAuto(
-                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
-                    message=message,
-                    entities=entities
-                )
-            )
+        self.file_name = file_name
+        self.mime_type = mime_type
+        self.file_size = file_size
+        self.date = date
+        self.thumbs = thumbs
+
+    @staticmethod
+    def _parse(
+        client,
+        audio: "raw.types.Document",
+        audio_attributes: "raw.types.DocumentAttributeAudio",
+        file_name: str
+    ) -> "Audio":
+        return Audio(
+            file_id=FileId(
+                file_type=FileType.AUDIO,
+                dc_id=audio.dc_id,
+                media_id=audio.id,
+                access_hash=audio.access_hash,
+                file_reference=audio.file_reference
+            ).encode(),
+            file_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=audio.id
+            ).encode(),
+            duration=audio_attributes.duration,
+            performer=audio_attributes.performer,
+            title=audio_attributes.title,
+            mime_type=audio.mime_type,
+            file_size=audio.size,
+            file_name=file_name,
+            date=utils.timestamp_to_datetime(audio.date),
+            thumbs=types.Thumbnail._parse(client, audio),
+            client=client
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,98 +17,115 @@
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 import pyrogram
 from pyrogram import raw, types
 from .inline_query_result import InlineQueryResult
 
 
-class InlineQueryResultContact(InlineQueryResult):
-    """Contact with a phone number
-    
-    By default, this contact will be sent by the user.
-    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
-    contact.
-    
+class InlineQueryResultVenue(InlineQueryResult):
+    """A venue.
+
+    By default, the venue will be sent by the user. Alternatively, you can use *input_message_content* to send a message
+    with the specified content instead of the venue.
+
     Parameters:
-        phone_number (``str``):
-            Contact's phone number.
+        title (``str``):
+            Title for the result.
 
-        first_name (``str``):
-            Contact's first name.
+        address (``str``):
+            Address of the venue.
 
-        last_name (``str``, *optional*):
-            Contact's last name.
+        latitude (``float``):
+            Location latitude in degrees.
 
-        vcard (``str``, *optional*):
-            Additional data about the contact in the form of a `vCard <https://en.wikipedia.org/wiki/VCard>`_.
+        longitude (``float``):
+            Location longitude in degrees.
 
         id (``str``, *optional*):
             Unique identifier for this result, 1-64 bytes.
             Defaults to a randomly generated UUID4.
 
+        foursquare_id (``str``, *optional*):
+            Foursquare identifier of the venue if known.
+
+        foursquare_type (``str``, *optional*):
+            Foursquare type of the venue, if known.
+
+        google_place_id (``str``, *optional*):
+            Google Places identifier of the venue.
+
+        google_place_type (``str``, *optional*):
+            Google Places type of the venue.
+
         reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
             Inline keyboard attached to the message.
-            
-        input_message_content (:obj:`~pyrogram.types.InputMessageContent`, *optional*):
-            Content of the message to be sent instead of the contact.
+
+        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
+            Content of the message to be sent instead of the file.
 
         thumb_url (``str``, *optional*):
             Url of the thumbnail for the result.
 
         thumb_width (``int``, *optional*):
             Thumbnail width.
 
         thumb_height (``int``, *optional*):
             Thumbnail height.
     """
 
     def __init__(
         self,
-        phone_number: str,
-        first_name: str,
-        last_name: str = "",
-        vcard: str = "",
+        title: str,
+        address: str,
+        latitude: float,
+        longitude: float,
         id: str = None,
+        foursquare_id: str = None,
+        foursquare_type: str = None,
+        google_place_id: str = None,
+        google_place_type: str = None,
         reply_markup: "types.InlineKeyboardMarkup" = None,
         input_message_content: "types.InputMessageContent" = None,
         thumb_url: str = None,
         thumb_width: int = 0,
         thumb_height: int = 0
     ):
-        super().__init__("contact", id, input_message_content, reply_markup)
+        super().__init__("venue", id, input_message_content, reply_markup)
 
-        self.phone_number = phone_number
-        self.first_name = first_name
-        self.last_name = last_name
-        self.vcard = vcard
+        self.title = title
+        self.address = address
+        self.latitude = latitude
+        self.longitude = longitude
+        self.foursquare_id = foursquare_id
+        self.foursquare_type = foursquare_type
+        self.google_place_id = google_place_id
+        self.google_place_type = google_place_type
         self.thumb_url = thumb_url
         self.thumb_width = thumb_width
         self.thumb_height = thumb_height
 
     async def write(self, client: "pyrogram.Client"):
         return raw.types.InputBotInlineResult(
             id=self.id,
             type=self.type,
-            title=self.first_name,
+            title=self.title,
             send_message=(
                 await self.input_message_content.write(client, self.reply_markup)
                 if self.input_message_content
-                else raw.types.InputBotInlineMessageMediaContact(
-                    phone_number=self.phone_number,
-                    first_name=self.first_name,
-                    last_name=self.last_name,
-                    vcard=self.vcard,
-                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
+                else raw.types.InputBotInlineMessageMediaVenue(
+                    geo_point=raw.types.InputGeoPoint(
+                        lat=self.latitude,
+                        long=self.longitude
+                    ),
+                    title=self.title,
+                    address=self.address,
+                    provider=(
+                        "foursquare" if self.foursquare_id or self.foursquare_type
+                        else "google" if self.google_place_id or self.google_place_type
+                        else ""
+                    ),
+                    venue_id=self.foursquare_id or self.google_place_id or "",
+                    venue_type=self.foursquare_type or self.google_place_type or "",
+                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None
                 )
-            ),
-            thumb=raw.types.InputWebDocument(
-                url=self.thumb_url,
-                size=0,
-                mime_type="image/jpg",
-                attributes=[
-                    raw.types.DocumentAttributeImageSize(
-                        w=self.thumb_width,
-                        h=self.thumb_height
-                    )
-                ]
-            ) if self.thumb_url else None
+            )
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,124 +19,126 @@
 from typing import Optional, List
 
 import pyrogram
 from pyrogram import raw, types, utils, enums
 from .inline_query_result import InlineQueryResult
 
 
-class InlineQueryResultDocument(InlineQueryResult):
-    """Link to a file.
+class InlineQueryResultPhoto(InlineQueryResult):
+    """Link to a photo.
 
-    By default, this file will be sent by the user with an optional caption.
-    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the file.
+    By default, this photo will be sent by the user with optional caption.
+    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
+    photo.
 
     Parameters:
-        document_url (``str``):
-            A valid URL for the file.
+        photo_url (``str``):
+            A valid URL of the photo.
+            Photo must be in jpeg format an must not exceed 5 MB.
 
-        title (``str``):
-            Title for the result.
+        thumb_url (``str``, *optional*):
+            URL of the thumbnail for the photo.
+            Defaults to the value passed in *photo_url*.
 
-        mime_type (``str``, *optional*):
-            Mime type of the content of the file, either “application/pdf” or “application/zip”.
-            Defaults to "application/zip".
+        photo_width (``int``, *optional*):
+            Width of the photo.
+
+        photo_height (``int``, *optional*):
+            Height of the photo
 
         id (``str``, *optional*):
             Unique identifier for this result, 1-64 bytes.
             Defaults to a randomly generated UUID4.
 
+        title (``str``, *optional*):
+            Title for the result.
+
+        description (``str``, *optional*):
+            Short description of the result.
+
         caption (``str``, *optional*):
-            Caption of the video to be sent, 0-1024 characters.
+            Caption of the photo to be sent, 0-1024 characters.
 
         parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
 
         caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
             List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
-        description (``str``, *optional*):
-            Short description of the result.
-
         reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
-            Inline keyboard attached to the message.
+            An InlineKeyboardMarkup object.
 
         input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
-            Content of the message to be sent instead of the file.
-
-        thumb_url (``str``, *optional*):
-            Url of the thumbnail for the result.
-
-        thumb_width (``int``, *optional*):
-            Thumbnail width.
-
-        thumb_height (``int``, *optional*):
-            Thumbnail height.
+            Content of the message to be sent instead of the photo.
     """
 
     def __init__(
         self,
-        document_url: str,
-        title: str,
-        mime_type: str = "application/zip",
+        photo_url: str,
+        thumb_url: str = None,
+        photo_width: int = 0,
+        photo_height: int = 0,
         id: str = None,
+        title: str = None,
+        description: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List["types.MessageEntity"] = None,
-        description: str = "",
         reply_markup: "types.InlineKeyboardMarkup" = None,
-        input_message_content: "types.InputMessageContent" = None,
-        thumb_url: str = None,
-        thumb_width: int = 0,
-        thumb_height: int = 0
+        input_message_content: "types.InputMessageContent" = None
     ):
-        super().__init__("file", id, input_message_content, reply_markup)
+        super().__init__("photo", id, input_message_content, reply_markup)
 
-        self.document_url = document_url
+        self.photo_url = photo_url
+        self.thumb_url = thumb_url
+        self.photo_width = photo_width
+        self.photo_height = photo_height
         self.title = title
-        self.mime_type = mime_type
+        self.description = description
         self.caption = caption
         self.parse_mode = parse_mode
         self.caption_entities = caption_entities
-        self.description = description
-        self.thumb_url = thumb_url
-        self.thumb_width = thumb_width
-        self.thumb_height = thumb_height
+        self.reply_markup = reply_markup
+        self.input_message_content = input_message_content
 
     async def write(self, client: "pyrogram.Client"):
-        document = raw.types.InputWebDocument(
-            url=self.document_url,
-            size=0,
-            mime_type=self.mime_type,
-            attributes=[]
-        )
-
-        thumb = raw.types.InputWebDocument(
-            url=self.thumb_url,
+        photo = raw.types.InputWebDocument(
+            url=self.photo_url,
             size=0,
             mime_type="image/jpeg",
             attributes=[
                 raw.types.DocumentAttributeImageSize(
-                    w=self.thumb_width,
-                    h=self.thumb_height
+                    w=self.photo_width,
+                    h=self.photo_height
                 )
             ]
-        ) if self.thumb_url else None
+        )
+
+        if self.thumb_url is None:
+            thumb = photo
+        else:
+            thumb = raw.types.InputWebDocument(
+                url=self.thumb_url,
+                size=0,
+                mime_type="image/jpeg",
+                attributes=[]
+            )
 
         message, entities = (await utils.parse_text_entities(
             client, self.caption, self.parse_mode, self.caption_entities
         )).values()
 
         return raw.types.InputBotInlineResult(
             id=self.id,
             type=self.type,
             title=self.title,
             description=self.description,
             thumb=thumb,
-            content=document,
+            content=photo,
             send_message=(
                 await self.input_message_content.write(client, self.reply_markup)
                 if self.input_message_content
                 else raw.types.InputBotInlineMessageMediaAuto(
                     reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
                     message=message,
                     entities=entities
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/video.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,136 +12,123 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List
+from datetime import datetime
+from typing import List
 
 import pyrogram
-from pyrogram import raw, types, utils, enums
-from .inline_query_result import InlineQueryResult
+from pyrogram import raw, utils
+from pyrogram import types
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
+from ..object import Object
 
 
-class InlineQueryResultPhoto(InlineQueryResult):
-    """Link to a photo.
-
-    By default, this photo will be sent by the user with optional caption.
-    Alternatively, you can use *input_message_content* to send a message with the specified content instead of the
-    photo.
+class Video(Object):
+    """A video file.
 
     Parameters:
-        photo_url (``str``):
-            A valid URL of the photo.
-            Photo must be in jpeg format an must not exceed 5 MB.
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        thumb_url (``str``, *optional*):
-            URL of the thumbnail for the photo.
-            Defaults to the value passed in *photo_url*.
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-        photo_width (``int``, *optional*):
-            Width of the photo.
+        width (``int``):
+            Video width as defined by sender.
 
-        photo_height (``int``, *optional*):
-            Height of the photo
+        height (``int``):
+            Video height as defined by sender.
 
-        id (``str``, *optional*):
-            Unique identifier for this result, 1-64 bytes.
-            Defaults to a randomly generated UUID4.
+        duration (``int``):
+            Duration of the video in seconds as defined by sender.
 
-        title (``str``, *optional*):
-            Title for the result.
+        file_name (``str``, *optional*):
+            Video file name.
 
-        description (``str``, *optional*):
-            Short description of the result.
+        mime_type (``str``, *optional*):
+            Mime type of a file as defined by sender.
 
-        caption (``str``, *optional*):
-            Caption of the photo to be sent, 0-1024 characters.
+        file_size (``int``, *optional*):
+            File size.
 
-        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
-            By default, texts are parsed using both Markdown and HTML styles.
-            You can combine both syntaxes together.
+        supports_streaming (``bool``, *optional*):
+            True, if the video was uploaded with streaming support.
 
-        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
-            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
+        ttl_seconds (``int``. *optional*):
+            Time-to-live seconds, for secret photos.
 
-        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
-            An InlineKeyboardMarkup object.
+        date (:py:obj:`~datetime.datetime`, *optional*):
+            Date the video was sent.
 
-        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
-            Content of the message to be sent instead of the photo.
+        thumbs (List of :obj:`~pyrogram.types.Thumbnail`, *optional*):
+            Video thumbnails.
     """
 
     def __init__(
         self,
-        photo_url: str,
-        thumb_url: str = None,
-        photo_width: int = 0,
-        photo_height: int = 0,
-        id: str = None,
-        title: str = None,
-        description: str = None,
-        caption: str = "",
-        parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List["types.MessageEntity"] = None,
-        reply_markup: "types.InlineKeyboardMarkup" = None,
-        input_message_content: "types.InputMessageContent" = None
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        width: int,
+        height: int,
+        duration: int,
+        file_name: str = None,
+        mime_type: str = None,
+        file_size: int = None,
+        supports_streaming: bool = None,
+        ttl_seconds: int = None,
+        date: datetime = None,
+        thumbs: List["types.Thumbnail"] = None
     ):
-        super().__init__("photo", id, input_message_content, reply_markup)
-
-        self.photo_url = photo_url
-        self.thumb_url = thumb_url
-        self.photo_width = photo_width
-        self.photo_height = photo_height
-        self.title = title
-        self.description = description
-        self.caption = caption
-        self.parse_mode = parse_mode
-        self.caption_entities = caption_entities
-        self.reply_markup = reply_markup
-        self.input_message_content = input_message_content
-
-    async def write(self, client: "pyrogram.Client"):
-        photo = raw.types.InputWebDocument(
-            url=self.photo_url,
-            size=0,
-            mime_type="image/jpeg",
-            attributes=[
-                raw.types.DocumentAttributeImageSize(
-                    w=self.photo_width,
-                    h=self.photo_height
-                )
-            ]
-        )
+        super().__init__(client)
 
-        if self.thumb_url is None:
-            thumb = photo
-        else:
-            thumb = raw.types.InputWebDocument(
-                url=self.thumb_url,
-                size=0,
-                mime_type="image/jpeg",
-                attributes=[]
-            )
-
-        message, entities = (await utils.parse_text_entities(
-            client, self.caption, self.parse_mode, self.caption_entities
-        )).values()
-
-        return raw.types.InputBotInlineResult(
-            id=self.id,
-            type=self.type,
-            title=self.title,
-            description=self.description,
-            thumb=thumb,
-            content=photo,
-            send_message=(
-                await self.input_message_content.write(client, self.reply_markup)
-                if self.input_message_content
-                else raw.types.InputBotInlineMessageMediaAuto(
-                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None,
-                    message=message,
-                    entities=entities
-                )
-            )
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
+        self.width = width
+        self.height = height
+        self.duration = duration
+        self.file_name = file_name
+        self.mime_type = mime_type
+        self.file_size = file_size
+        self.supports_streaming = supports_streaming
+        self.ttl_seconds = ttl_seconds
+        self.date = date
+        self.thumbs = thumbs
+
+    @staticmethod
+    def _parse(
+        client,
+        video: "raw.types.Document",
+        video_attributes: "raw.types.DocumentAttributeVideo",
+        file_name: str,
+        ttl_seconds: int = None
+    ) -> "Video":
+        return Video(
+            file_id=FileId(
+                file_type=FileType.VIDEO,
+                dc_id=video.dc_id,
+                media_id=video.id,
+                access_hash=video.access_hash,
+                file_reference=video.file_reference
+            ).encode(),
+            file_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=video.id
+            ).encode(),
+            width=video_attributes.w,
+            height=video_attributes.h,
+            duration=video_attributes.duration,
+            file_name=file_name,
+            mime_type=video.mime_type,
+            supports_streaming=video_attributes.supports_streaming,
+            file_size=video.size,
+            date=utils.timestamp_to_datetime(video.date),
+            ttl_seconds=ttl_seconds,
+            thumbs=types.Thumbnail._parse(client, video),
+            client=client
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,120 +12,128 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-import pyrogram
-from pyrogram import raw, types
-from .inline_query_result import InlineQueryResult
+from datetime import datetime
+from typing import Dict
 
+import pyrogram
+from pyrogram import raw, utils
+from pyrogram import types
+from ..object import Object
+from ..update import Update
 
-class InlineQueryResultVenue(InlineQueryResult):
-    """A venue.
 
-    By default, the venue will be sent by the user. Alternatively, you can use *input_message_content* to send a message
-    with the specified content instead of the venue.
+class ChatJoinRequest(Object, Update):
+    """Represents a join request sent to a chat.
 
     Parameters:
-        title (``str``):
-            Title for the result.
-
-        address (``str``):
-            Address of the venue.
-
-        latitude (``float``):
-            Location latitude in degrees.
-
-        longitude (``float``):
-            Location longitude in degrees.
-
-        id (``str``, *optional*):
-            Unique identifier for this result, 1-64 bytes.
-            Defaults to a randomly generated UUID4.
-
-        foursquare_id (``str``, *optional*):
-            Foursquare identifier of the venue if known.
-
-        foursquare_type (``str``, *optional*):
-            Foursquare type of the venue, if known.
+        chat (:obj:`~pyrogram.types.Chat`):
+            Chat to which the request was sent.
 
-        google_place_id (``str``, *optional*):
-            Google Places identifier of the venue.
+        from_user (:obj:`~pyrogram.types.User`):
+            User that sent the join request.
 
-        google_place_type (``str``, *optional*):
-            Google Places type of the venue.
+        date (:py:obj:`~datetime.datetime`):
+            Date the request was sent.
 
-        reply_markup (:obj:`~pyrogram.types.InlineKeyboardMarkup`, *optional*):
-            Inline keyboard attached to the message.
+        bio (``str``, *optional*):
+            Bio of the user.
 
-        input_message_content (:obj:`~pyrogram.types.InputMessageContent`):
-            Content of the message to be sent instead of the file.
-
-        thumb_url (``str``, *optional*):
-            Url of the thumbnail for the result.
-
-        thumb_width (``int``, *optional*):
-            Thumbnail width.
-
-        thumb_height (``int``, *optional*):
-            Thumbnail height.
+        invite_link (:obj:`~pyrogram.types.ChatInviteLink`, *optional*):
+            Chat invite link that was used by the user to send the join request.
     """
 
     def __init__(
         self,
-        title: str,
-        address: str,
-        latitude: float,
-        longitude: float,
-        id: str = None,
-        foursquare_id: str = None,
-        foursquare_type: str = None,
-        google_place_id: str = None,
-        google_place_type: str = None,
-        reply_markup: "types.InlineKeyboardMarkup" = None,
-        input_message_content: "types.InputMessageContent" = None,
-        thumb_url: str = None,
-        thumb_width: int = 0,
-        thumb_height: int = 0
+        *,
+        client: "pyrogram.Client" = None,
+        chat: "types.Chat",
+        from_user: "types.User",
+        date: datetime,
+        bio: str = None,
+        invite_link: "types.ChatInviteLink" = None
     ):
-        super().__init__("venue", id, input_message_content, reply_markup)
+        super().__init__(client)
+
+        self.chat = chat
+        self.from_user = from_user
+        self.date = date
+        self.bio = bio
+        self.invite_link = invite_link
+
+    @staticmethod
+    def _parse(
+        client: "pyrogram.Client",
+        update: "raw.types.UpdateBotChatInviteRequester",
+        users: Dict[int, "raw.types.User"],
+        chats: Dict[int, "raw.types.Chat"]
+    ) -> "ChatJoinRequest":
+        chat_id = utils.get_raw_peer_id(update.peer)
+
+        return ChatJoinRequest(
+            chat=types.Chat._parse_chat(client, chats[chat_id]),
+            from_user=types.User._parse(client, users[update.user_id]),
+            date=utils.timestamp_to_datetime(update.date),
+            bio=update.about,
+            invite_link=types.ChatInviteLink._parse(client, update.invite, users),
+            client=client
+        )
+
+    async def approve(self) -> bool:
+        """Bound method *approve* of :obj:`~pyrogram.types.ChatJoinRequest`.
+        
+        Use as a shortcut for:
+        
+        .. code-block:: python
+
+            await client.approve_chat_join_request(
+                chat_id=request.chat.id,
+                user_id=request.from_user.id
+            )
+            
+        Example:
+            .. code-block:: python
+
+                await request.approve()
+                
+        Returns:
+            ``bool``: True on success.
+        
+        Raises:
+            RPCError: In case of a Telegram RPC error.
+        """
+        return await self._client.approve_chat_join_request(
+            chat_id=self.chat.id,
+            user_id=self.from_user.id
+        )
 
-        self.title = title
-        self.address = address
-        self.latitude = latitude
-        self.longitude = longitude
-        self.foursquare_id = foursquare_id
-        self.foursquare_type = foursquare_type
-        self.google_place_id = google_place_id
-        self.google_place_type = google_place_type
-        self.thumb_url = thumb_url
-        self.thumb_width = thumb_width
-        self.thumb_height = thumb_height
-
-    async def write(self, client: "pyrogram.Client"):
-        return raw.types.InputBotInlineResult(
-            id=self.id,
-            type=self.type,
-            title=self.title,
-            send_message=(
-                await self.input_message_content.write(client, self.reply_markup)
-                if self.input_message_content
-                else raw.types.InputBotInlineMessageMediaVenue(
-                    geo_point=raw.types.InputGeoPoint(
-                        lat=self.latitude,
-                        long=self.longitude
-                    ),
-                    title=self.title,
-                    address=self.address,
-                    provider=(
-                        "foursquare" if self.foursquare_id or self.foursquare_type
-                        else "google" if self.google_place_id or self.google_place_type
-                        else ""
-                    ),
-                    venue_id=self.foursquare_id or self.google_place_id or "",
-                    venue_type=self.foursquare_type or self.google_place_type or "",
-                    reply_markup=await self.reply_markup.write(client) if self.reply_markup else None
-                )
+    async def decline(self) -> bool:
+        """Bound method *decline* of :obj:`~pyrogram.types.ChatJoinRequest`.
+        
+        Use as a shortcut for:
+        
+        .. code-block:: python
+
+            await client.decline_chat_join_request(
+                chat_id=request.chat.id,
+                user_id=request.from_user.id
             )
+            
+        Example:
+            .. code-block:: python
+
+                await request.decline()
+                
+        Returns:
+            ``bool``: True on success.
+        
+        Raises:
+            RPCError: In case of a Telegram RPC error.
+        """
+        return await self._client.decline_chat_join_request(
+            chat_id=self.chat.id,
+            user_id=self.from_user.id
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_media/input_media_video.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,71 +12,80 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List, BinaryIO, Union
+from typing import Optional, List, Union, BinaryIO
 
 from .input_media import InputMedia
 from ..messages_and_media import MessageEntity
 from ... import enums
 
 
-class InputMediaAudio(InputMedia):
-    """An audio to be sent inside an album.
-
-    It is intended to be used with :meth:`~pyrogram.Client.send_media_group`.
+class InputMediaVideo(InputMedia):
+    """A video to be sent inside an album.
+    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
 
     Parameters:
         media (``str`` | ``BinaryIO``):
-            Audio to send.
-            Pass a file_id as string to send an audio that exists on the Telegram servers or
-            pass a file path as string to upload a new audio that exists on your local machine or
+            Video to send.
+            Pass a file_id as string to send a video that exists on the Telegram servers or
+            pass a file path as string to upload a new video that exists on your local machine or
             pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get an audio file from the Internet.
+            pass an HTTP URL as a string for Telegram to get a video from the Internet.
 
-        thumb (``str``, *optional*):
-            Thumbnail of the music file album cover.
+        thumb (``str``):
+            Thumbnail of the video sent.
             The thumbnail should be in JPEG format and less than 200 KB in size.
             A thumbnail's width and height should not exceed 320 pixels.
             Thumbnails can't be reused and can be only uploaded as a new file.
 
         caption (``str``, *optional*):
-            Caption of the audio to be sent, 0-1024 characters.
+            Caption of the video to be sent, 0-1024 characters.
             If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
 
         parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
             By default, texts are parsed using both Markdown and HTML styles.
             You can combine both syntaxes together.
 
         caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
             List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
 
+        width (``int``, *optional*):
+            Video width.
+
+        height (``int``, *optional*):
+            Video height.
+
         duration (``int``, *optional*):
-            Duration of the audio in seconds
+            Video duration.
 
-        performer (``str``, *optional*):
-            Performer of the audio
+        supports_streaming (``bool``, *optional*):
+            Pass True, if the uploaded video is suitable for streaming.
 
-        title (``str``, *optional*):
-            Title of the audio
+        has_spoiler (``bool``, *optional*):
+            Pass True if the photo needs to be covered with a spoiler animation.
     """
 
     def __init__(
         self,
         media: Union[str, BinaryIO],
         thumb: str = None,
         caption: str = "",
         parse_mode: Optional["enums.ParseMode"] = None,
         caption_entities: List[MessageEntity] = None,
+        width: int = 0,
+        height: int = 0,
         duration: int = 0,
-        performer: str = "",
-        title: str = ""
+        supports_streaming: bool = True,
+        has_spoiler: bool = None,
     ):
         super().__init__(media, caption, parse_mode, caption_entities)
 
         self.thumb = thumb
+        self.width = width
+        self.height = height
         self.duration = duration
-        self.performer = performer
-        self.title = title
+        self.supports_streaming = supports_streaming
+        self.has_spoiler = has_spoiler
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_media/input_media_video.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,80 +12,100 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Optional, List, Union, BinaryIO
+from typing import List, Optional, Union
 
-from .input_media import InputMedia
-from ..messages_and_media import MessageEntity
-from ... import enums
+import pyrogram
+from pyrogram import raw
+from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
+from ..object import Object
 
 
-class InputMediaVideo(InputMedia):
-    """A video to be sent inside an album.
-    It is intended to be used with :obj:`~pyrogram.Client.send_media_group`.
+class Thumbnail(Object):
+    """One size of a photo or a file/sticker thumbnail.
 
     Parameters:
-        media (``str`` | ``BinaryIO``):
-            Video to send.
-            Pass a file_id as string to send a video that exists on the Telegram servers or
-            pass a file path as string to upload a new video that exists on your local machine or
-            pass a binary file-like object with its attribute “.name” set for in-memory uploads or
-            pass an HTTP URL as a string for Telegram to get a video from the Internet.
-
-        thumb (``str``):
-            Thumbnail of the video sent.
-            The thumbnail should be in JPEG format and less than 200 KB in size.
-            A thumbnail's width and height should not exceed 320 pixels.
-            Thumbnails can't be reused and can be only uploaded as a new file.
-
-        caption (``str``, *optional*):
-            Caption of the video to be sent, 0-1024 characters.
-            If not specified, the original caption is kept. Pass "" (empty string) to remove the caption.
-
-        parse_mode (:obj:`~pyrogram.enums.ParseMode`, *optional*):
-            By default, texts are parsed using both Markdown and HTML styles.
-            You can combine both syntaxes together.
-
-        caption_entities (List of :obj:`~pyrogram.types.MessageEntity`):
-            List of special entities that appear in the caption, which can be specified instead of *parse_mode*.
-
-        width (``int``, *optional*):
-            Video width.
-
-        height (``int``, *optional*):
-            Video height.
+        file_id (``str``):
+            Identifier for this file, which can be used to download or reuse the file.
 
-        duration (``int``, *optional*):
-            Video duration.
+        file_unique_id (``str``):
+            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
+            Can't be used to download or reuse the file.
 
-        supports_streaming (``bool``, *optional*):
-            Pass True, if the uploaded video is suitable for streaming.
+        width (``int``):
+            Photo width.
 
-        has_spoiler (``bool``, *optional*):
-            Pass True if the photo needs to be covered with a spoiler animation.
+        height (``int``):
+            Photo height.
+
+        file_size (``int``):
+            File size.
     """
 
     def __init__(
         self,
-        media: Union[str, BinaryIO],
-        thumb: str = None,
-        caption: str = "",
-        parse_mode: Optional["enums.ParseMode"] = None,
-        caption_entities: List[MessageEntity] = None,
-        width: int = 0,
-        height: int = 0,
-        duration: int = 0,
-        supports_streaming: bool = True,
-        has_spoiler: bool = None,
+        *,
+        client: "pyrogram.Client" = None,
+        file_id: str,
+        file_unique_id: str,
+        width: int,
+        height: int,
+        file_size: int
     ):
-        super().__init__(media, caption, parse_mode, caption_entities)
+        super().__init__(client)
 
-        self.thumb = thumb
+        self.file_id = file_id
+        self.file_unique_id = file_unique_id
         self.width = width
         self.height = height
-        self.duration = duration
-        self.supports_streaming = supports_streaming
-        self.has_spoiler = has_spoiler
+        self.file_size = file_size
+
+    @staticmethod
+    def _parse(client, media: Union["raw.types.Photo", "raw.types.Document"]) -> Optional[List["Thumbnail"]]:
+        if isinstance(media, raw.types.Photo):
+            raw_thumbs = [i for i in media.sizes if isinstance(i, raw.types.PhotoSize)]
+            raw_thumbs.sort(key=lambda p: p.size)
+            raw_thumbs = raw_thumbs[:-1]
+
+            file_type = FileType.PHOTO
+        elif isinstance(media, raw.types.Document):
+            raw_thumbs = media.thumbs
+            file_type = FileType.THUMBNAIL
+        else:
+            return
+
+        parsed_thumbs = []
+
+        for thumb in raw_thumbs:
+            if not isinstance(thumb, raw.types.PhotoSize):
+                continue
+
+            parsed_thumbs.append(
+                Thumbnail(
+                    file_id=FileId(
+                        file_type=file_type,
+                        dc_id=media.dc_id,
+                        media_id=media.id,
+                        access_hash=media.access_hash,
+                        file_reference=media.file_reference,
+                        thumbnail_file_type=file_type,
+                        thumbnail_source=ThumbnailSource.THUMBNAIL,
+                        thumbnail_size=thumb.type,
+                        volume_id=0,
+                        local_id=0
+                    ).encode(),
+                    file_unique_id=FileUniqueId(
+                        file_unique_type=FileUniqueType.DOCUMENT,
+                        media_id=media.id
+                    ).encode(),
+                    width=thumb.w,
+                    height=thumb.h,
+                    file_size=thumb.size,
+                    client=client
+                )
+            )
+
+        return parsed_thumbs or None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_message_content/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/list.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/animation.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/contact.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,60 +12,66 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
+from datetime import datetime
+from typing import Optional
+
 import pyrogram
 from pyrogram import raw
+from pyrogram import utils
 from ..object import Object
 
 
-class Contact(Object):
-    """A phone contact.
+class EmojiStatus(Object):
+    """A user emoji status.
 
     Parameters:
-        phone_number (``str``):
-            Contact's phone number.
-
-        first_name (``str``):
-            Contact's first name.
-
-        last_name (``str``, *optional*):
-            Contact's last name.
+        custom_emoji_id (``int``):
+            Custom emoji id.
 
-        user_id (``int``, *optional*):
-            Contact's user identifier in Telegram.
-
-        vcard (``str``, *optional*):
-            Additional data about the contact in the form of a vCard.
+        until_date (:py:obj:`~datetime.datetime`, *optional*):
+            Valid until date.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
-        phone_number: str,
-        first_name: str,
-        last_name: str = None,
-        user_id: int = None,
-        vcard: str = None
+        custom_emoji_id: int,
+        until_date: Optional[datetime] = None
     ):
         super().__init__(client)
 
-        self.phone_number = phone_number
-        self.first_name = first_name
-        self.last_name = last_name
-        self.user_id = user_id
-        self.vcard = vcard
+        self.custom_emoji_id = custom_emoji_id
+        self.until_date = until_date
 
     @staticmethod
-    def _parse(client: "pyrogram.Client", contact: "raw.types.MessageMediaContact") -> "Contact":
-        return Contact(
-            phone_number=contact.phone_number,
-            first_name=contact.first_name,
-            last_name=contact.last_name or None,
-            vcard=contact.vcard or None,
-            user_id=contact.user_id or None,
-            client=client
+    def _parse(client, emoji_status: "raw.base.EmojiStatus") -> Optional["EmojiStatus"]:
+        if isinstance(emoji_status, raw.types.EmojiStatus):
+            return EmojiStatus(
+                client=client,
+                custom_emoji_id=emoji_status.document_id
+            )
+
+        if isinstance(emoji_status, raw.types.EmojiStatusUntil):
+            return EmojiStatus(
+                client=client,
+                custom_emoji_id=emoji_status.document_id,
+                until_date=utils.timestamp_to_datetime(emoji_status.until)
+            )
+
+        return None
+
+    def write(self):
+        if self.until_date:
+            return raw.types.EmojiStatusUntil(
+                document_id=self.custom_emoji_id,
+                until=utils.datetime_to_timestamp(self.until_date)
+            )
+
+        return raw.types.EmojiStatus(
+            document_id=self.custom_emoji_id
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/message.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/poll.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,100 +12,96 @@
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import List, Optional, Union
+from typing import Union
 
 import pyrogram
 from pyrogram import raw
 from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType, ThumbnailSource
 from ..object import Object
 
 
-class Thumbnail(Object):
-    """One size of a photo or a file/sticker thumbnail.
+class ChatPhoto(Object):
+    """A chat photo.
 
     Parameters:
-        file_id (``str``):
-            Identifier for this file, which can be used to download or reuse the file.
-
-        file_unique_id (``str``):
-            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
-            Can't be used to download or reuse the file.
-
-        width (``int``):
-            Photo width.
-
-        height (``int``):
-            Photo height.
-
-        file_size (``int``):
-            File size.
+        small_file_id (``str``):
+            File identifier of small (160x160) chat photo.
+            This file_id can be used only for photo download and only for as long as the photo is not changed.
+
+        small_photo_unique_id (``str``):
+            Unique file identifier of small (160x160) chat photo, which is supposed to be the same over time and for
+            different accounts. Can't be used to download or reuse the file.
+
+        big_file_id (``str``):
+            File identifier of big (640x640) chat photo.
+            This file_id can be used only for photo download and only for as long as the photo is not changed.
+
+        big_photo_unique_id (``str``):
+            Unique file identifier of big (640x640) chat photo, which is supposed to be the same over time and for
+            different accounts. Can't be used to download or reuse the file.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
-        file_id: str,
-        file_unique_id: str,
-        width: int,
-        height: int,
-        file_size: int
+        small_file_id: str,
+        small_photo_unique_id: str,
+        big_file_id: str,
+        big_photo_unique_id: str
+
     ):
         super().__init__(client)
 
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.width = width
-        self.height = height
-        self.file_size = file_size
+        self.small_file_id = small_file_id
+        self.small_photo_unique_id = small_photo_unique_id
+        self.big_file_id = big_file_id
+        self.big_photo_unique_id = big_photo_unique_id
 
     @staticmethod
-    def _parse(client, media: Union["raw.types.Photo", "raw.types.Document"]) -> Optional[List["Thumbnail"]]:
-        if isinstance(media, raw.types.Photo):
-            raw_thumbs = [i for i in media.sizes if isinstance(i, raw.types.PhotoSize)]
-            raw_thumbs.sort(key=lambda p: p.size)
-            raw_thumbs = raw_thumbs[:-1]
-
-            file_type = FileType.PHOTO
-        elif isinstance(media, raw.types.Document):
-            raw_thumbs = media.thumbs
-            file_type = FileType.THUMBNAIL
-        else:
-            return
-
-        parsed_thumbs = []
-
-        for thumb in raw_thumbs:
-            if not isinstance(thumb, raw.types.PhotoSize):
-                continue
-
-            parsed_thumbs.append(
-                Thumbnail(
-                    file_id=FileId(
-                        file_type=file_type,
-                        dc_id=media.dc_id,
-                        media_id=media.id,
-                        access_hash=media.access_hash,
-                        file_reference=media.file_reference,
-                        thumbnail_file_type=file_type,
-                        thumbnail_source=ThumbnailSource.THUMBNAIL,
-                        thumbnail_size=thumb.type,
-                        volume_id=0,
-                        local_id=0
-                    ).encode(),
-                    file_unique_id=FileUniqueId(
-                        file_unique_type=FileUniqueType.DOCUMENT,
-                        media_id=media.id
-                    ).encode(),
-                    width=thumb.w,
-                    height=thumb.h,
-                    file_size=thumb.size,
-                    client=client
-                )
-            )
+    def _parse(
+        client,
+        chat_photo: Union["raw.types.UserProfilePhoto", "raw.types.ChatPhoto"],
+        peer_id: int,
+        peer_access_hash: int
+    ):
+        if not isinstance(chat_photo, (raw.types.UserProfilePhoto, raw.types.ChatPhoto)):
+            return None
 
-        return parsed_thumbs or None
+        return ChatPhoto(
+            small_file_id=FileId(
+                file_type=FileType.CHAT_PHOTO,
+                dc_id=chat_photo.dc_id,
+                media_id=chat_photo.photo_id,
+                access_hash=0,
+                volume_id=0,
+                thumbnail_source=ThumbnailSource.CHAT_PHOTO_SMALL,
+                local_id=0,
+                chat_id=peer_id,
+                chat_access_hash=peer_access_hash
+            ).encode(),
+            small_photo_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=chat_photo.photo_id
+            ).encode(),
+            big_file_id=FileId(
+                file_type=FileType.CHAT_PHOTO,
+                dc_id=chat_photo.dc_id,
+                media_id=chat_photo.photo_id,
+                access_hash=0,
+                volume_id=0,
+                thumbnail_source=ThumbnailSource.CHAT_PHOTO_BIG,
+                local_id=0,
+                chat_id=peer_id,
+                chat_access_hash=peer_access_hash
+            ).encode(),
+            big_photo_unique_id=FileUniqueId(
+                file_unique_type=FileUniqueType.DOCUMENT,
+                media_id=chat_photo.photo_id
+            ).encode(),
+            client=client
+        )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,96 +13,90 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
-from typing import List
+from typing import Dict, Union
 
 import pyrogram
 from pyrogram import raw, utils
 from pyrogram import types
-from pyrogram.file_id import FileId, FileType, FileUniqueId, FileUniqueType
 from ..object import Object
+from ..update import Update
 
 
-class VideoNote(Object):
-    """A video note.
+class ChatMemberUpdated(Object, Update):
+    """Represents changes in the status of a chat member.
 
     Parameters:
-        file_id (``str``):
-            Identifier for this file, which can be used to download or reuse the file.
+        chat (:obj:`~pyrogram.types.Chat`):
+            Chat the user belongs to.
 
-        file_unique_id (``str``):
-            Unique identifier for this file, which is supposed to be the same over time and for different accounts.
-            Can't be used to download or reuse the file.
+        from_user (:obj:`~pyrogram.types.User`):
+            Performer of the action, which resulted in the change.
 
-        length (``int``):
-            Video width and height as defined by sender.
+        date (:py:obj:`~datetime.datetime`):
+            Date the change was done.
 
-        duration (``int``):
-            Duration of the video in seconds as defined by sender.
+        old_chat_member (:obj:`~pyrogram.types.ChatMember`, *optional*):
+            Previous information about the chat member.
 
-        mime_type (``str``, *optional*):
-            MIME type of the file as defined by sender.
+        new_chat_member (:obj:`~pyrogram.types.ChatMember`, *optional*):
+            New information about the chat member.
 
-        file_size (``int``, *optional*):
-            File size.
-
-        date (:py:obj:`~datetime.datetime`, *optional*):
-            Date the video note was sent.
-
-        thumbs (List of :obj:`~pyrogram.types.Thumbnail`, *optional*):
-            Video thumbnails.
+        invite_link (:obj:`~pyrogram.types.ChatInviteLink`, *optional*):
+            Chat invite link, which was used by the user to join the chat; for joining by invite link events only.
     """
 
     def __init__(
         self,
         *,
         client: "pyrogram.Client" = None,
-        file_id: str,
-        file_unique_id: str,
-        length: int,
-        duration: int,
-        thumbs: List["types.Thumbnail"] = None,
-        mime_type: str = None,
-        file_size: int = None,
-        date: datetime = None
+        chat: "types.Chat",
+        from_user: "types.User",
+        date: datetime,
+        old_chat_member: "types.ChatMember",
+        new_chat_member: "types.ChatMember",
+        invite_link: "types.ChatInviteLink" = None,
     ):
         super().__init__(client)
 
-        self.file_id = file_id
-        self.file_unique_id = file_unique_id
-        self.mime_type = mime_type
-        self.file_size = file_size
+        self.chat = chat
+        self.from_user = from_user
         self.date = date
-        self.length = length
-        self.duration = duration
-        self.thumbs = thumbs
+        self.old_chat_member = old_chat_member
+        self.new_chat_member = new_chat_member
+        self.invite_link = invite_link
 
     @staticmethod
     def _parse(
-        client,
-        video_note: "raw.types.Document",
-        video_attributes: "raw.types.DocumentAttributeVideo"
-    ) -> "VideoNote":
-        return VideoNote(
-            file_id=FileId(
-                file_type=FileType.VIDEO_NOTE,
-                dc_id=video_note.dc_id,
-                media_id=video_note.id,
-                access_hash=video_note.access_hash,
-                file_reference=video_note.file_reference
-            ).encode(),
-            file_unique_id=FileUniqueId(
-                file_unique_type=FileUniqueType.DOCUMENT,
-                media_id=video_note.id
-            ).encode(),
-            length=video_attributes.w,
-            duration=video_attributes.duration,
-            file_size=video_note.size,
-            mime_type=video_note.mime_type,
-            date=utils.timestamp_to_datetime(video_note.date),
-            thumbs=types.Thumbnail._parse(client, video_note),
+        client: "pyrogram.Client",
+        update: Union["raw.types.UpdateChatParticipant", "raw.types.UpdateChannelParticipant"],
+        users: Dict[int, "raw.types.User"],
+        chats: Dict[int, "raw.types.Chat"]
+    ) -> "ChatMemberUpdated":
+        chat_id = getattr(update, "chat_id", None) or getattr(update, "channel_id")
+
+        old_chat_member = None
+        new_chat_member = None
+        invite_link = None
+
+        if update.prev_participant:
+            old_chat_member = types.ChatMember._parse(client, update.prev_participant, users, chats)
+
+        if update.new_participant:
+            new_chat_member = types.ChatMember._parse(client, update.new_participant, users, chats)
+
+        if update.invite:
+            invite_link = types.ChatInviteLink._parse(client, update.invite, users)
+
+        return ChatMemberUpdated(
+            chat=types.Chat._parse_chat(client, chats[chat_id]),
+            from_user=types.User._parse(client, users[update.actor_id]),
+            date=utils.timestamp_to_datetime(update.date),
+            old_chat_member=old_chat_member,
+            new_chat_member=new_chat_member,
+            invite_link=invite_link,
             client=client
         )
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/object.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-dev-2.1.8.dev202305201740/NOTICE`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,17 @@
-#  Pyrogram - Telegram MTProto API Client Library for Python
-#  Copyright (C) 2017-present Dan <https://github.com/delivrance>
-#
-#  This file is part of Pyrogram.
-#
-#  Pyrogram is free software: you can redistribute it and/or modify
-#  it under the terms of the GNU Lesser General Public License as published
-#  by the Free Software Foundation, either version 3 of the License, or
-#  (at your option) any later version.
-#
-#  Pyrogram is distributed in the hope that it will be useful,
-#  but WITHOUT ANY WARRANTY; without even the implied warranty of
-#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#  GNU Lesser General Public License for more details.
-#
-#  You should have received a copy of the GNU Lesser General Public License
-#  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
+Pyrogram - Telegram MTProto API Client Library for Python
+Copyright (C) 2017-present Dan <https://github.com/delivrance>
 
-from ..object import Object
+This file is part of Pyrogram.
 
+Pyrogram is free software: you can redistribute it and/or modify
+it under the terms of the GNU Lesser General Public License as published
+by the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
 
-class ChatJoinedByRequest(Object):
-    """A service message about a user join request approved in the chat.
+Pyrogram is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Lesser General Public License for more details.
 
-    Currently holds no information.
-    """
-
-    def __init__(self):
-        super().__init__()
+You should have received a copy of the GNU Lesser General Public License
+along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/types/user_and_chats/user.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/pyrogram/utils.py` & `PyroFork-dev-2.1.8.dev202305201740/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201733/PKG-INFO` & `PyroFork-dev-2.1.8.dev202305201740/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 Metadata-Version: 2.1
-Name: pyrofork-dev
-Version: 2.1.8.dev202305201733
+Name: PyroFork-dev
+Version: 2.1.8.dev202305201740
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
-License: LGPL-3.0-or-later
-Keywords: telegram,chat,messenger,mtproto,api,client,library,python
-Author: Dan
-Author-email: 14043624+delivrance@users.noreply.github.com
-Requires-Python: >=3.9,<4.0
+Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
+Author: wulan17
+Author-email: mayuri@mayuri.my.id
+License: LGPLv3
+Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
+Project-URL: Source, https://github.com/Mayuri-Chan/pyrofork
+Project-URL: Documentation, https://pyrofork.mayuri.my.id
+Keywords: telegram chat messenger mtproto api client library python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Natural Language :: English
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Internet
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: aiosqlite (<1.0.0)
-Requires-Dist: async-pymongo (==0.1.2)
-Requires-Dist: pyaes (==1.6.1)
-Requires-Dist: pymediainfo (==6.0.1)
-Requires-Dist: pymongo (==4.3.3)
-Requires-Dist: pysocks (==1.7.1)
-Project-URL: Documentation, https://pyrofork.mayuri.my.id
-Project-URL: Repository, https://github.com/Mayuri-Chan/pyrofork
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
+License-File: COPYING
+License-File: COPYING.lesser
+License-File: NOTICE
 
 <p align="center">
     <a href="https://github.com/Mayuri-Chan/pyrofork">
         <img src="https://docs.pyrogram.org/_static/pyrogram.png" alt="PyroFork" width="128">
     </a>
     <br>
     <b>Telegram MTProto API Framework for Python</b>
@@ -92,21 +90,12 @@
 
 ### Installing
 
 ``` bash
 pip3 install pyrofork
 ```
 
-### Install from source
-
-```bash
-git clone https://github.com/Mayuri-Chan/pyrofork.git -b master
-cd pyrofork
-make install
-```
-
 ### Resources
 
 - Check out the docs at https://pyrofork.mayuri.my.id to learn more about PyroFork, get started right
 away and discover more in-depth material for building your client applications.
 
-
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
-Metadata-Version: 2.1 Name: pyrofork-dev Version: 2.1.8.dev202305201733
+Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.1.8.dev202305201740
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
-License: LGPL-3.0-or-later Keywords:
-telegram,chat,messenger,mtproto,api,client,library,python Author: Dan Author-
-email: 14043624+delivrance@users.noreply.github.com Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: GNU Lesser General Public
-License v3 (LGPLv3) Classifier: License :: OSI Approved :: GNU Lesser General
-Public License v3 or later (LGPLv3+) Classifier: Natural Language :: English
+Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest Author:
+wulan17 Author-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker,
+https://github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://
+github.com/Mayuri-Chan/pyrofork Project-URL: Documentation, https://
+pyrofork.mayuri.my.id Keywords: telegram chat messenger mtproto api client
+library python Classifier: Development Status :: 4 - Beta Classifier: Intended
+Audience :: Developers Classifier: Natural Language :: English Classifier:
+License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: Implementation Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Programming
-Language :: Python :: Implementation :: PyPy Classifier: Topic ::
-Communications Classifier: Topic :: Communications :: Chat Classifier: Topic ::
-Internet Classifier: Topic :: Software Development :: Libraries Classifier:
-Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: aiosqlite (<1.0.0) Requires-Dist: async-pymongo (==0.1.2)
-Requires-Dist: pyaes (==1.6.1) Requires-Dist: pymediainfo (==6.0.1) Requires-
-Dist: pymongo (==4.3.3) Requires-Dist: pysocks (==1.7.1) Project-URL:
-Documentation, https://pyrofork.mayuri.my.id Project-URL: Repository, https://
-github.com/Mayuri-Chan/pyrofork Description-Content-Type: text/markdown
+Language :: Python :: Implementation :: PyPy Classifier: Topic :: Internet
+Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
+Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Classifier: Topic ::
+Software Development :: Libraries :: Application Frameworks Requires-Python:
+~=3.9 Description-Content-Type: text/markdown License-File: COPYING License-
+File: COPYING.lesser License-File: NOTICE
                                   [PyroFork]
                   Telegram MTProto API Framework for Python
                           Homepage â¢ Documentation
 ## PyroFork > Elegant, modern and asynchronous Telegram MTProto API framework
 in Python for users and bots ``` python from pyrogram import Client, filters
 app = Client("my_account") @app.on_message(filters.private) async def hello
 (client, message): await message.reply("Hello from Pyrogram!") app.run() ```
@@ -41,12 +39,10 @@
 usages. - **Elegant**: Low-level details are abstracted and re-presented in a
 more convenient way. - **Fast**: Boosted up by [TgCrypto](https://github.com/
 pyrogram/tgcrypto), a high-performance cryptography library written in C. -
 **Type-hinted**: Types and methods are all type-hinted, enabling excellent
 editor support. - **Async**: Fully asynchronous (also usable synchronously if
 wanted, for convenience). - **Powerful**: Full access to Telegram's API to
 execute any official client action and more. ### Installing ``` bash pip3
-install pyrofork ``` ### Install from source ```bash git clone https://
-github.com/Mayuri-Chan/pyrofork.git -b master cd pyrofork make install ``` ###
-Resources - Check out the docs at https://pyrofork.mayuri.my.id to learn more
-about PyroFork, get started right away and discover more in-depth material for
-building your client applications.
+install pyrofork ``` ### Resources - Check out the docs at https://
+pyrofork.mayuri.my.id to learn more about PyroFork, get started right away and
+discover more in-depth material for building your client applications.
```

