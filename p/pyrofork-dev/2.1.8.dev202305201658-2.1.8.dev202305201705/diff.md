# Comparing `tmp/pyrofork_dev-2.1.8.dev202305201658.tar.gz` & `tmp/pyrofork_dev-2.1.8.dev202305201705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrofork_dev-2.1.8.dev202305201658.tar", max compression
+gzip compressed data, was "pyrofork_dev-2.1.8.dev202305201705.tar", max compression
```

## Comparing `pyrofork_dev-2.1.8.dev202305201658.tar` & `pyrofork_dev-2.1.8.dev202305201705.tar`

### file list

```diff
@@ -1,1684 +1,1684 @@
--rw-r--r--   0        0        0     2155 2023-05-20 16:58:30.749641 pyrofork_dev-2.1.8.dev202305201658/README.md
--rw-r--r--   0        0        0     1931 2023-05-20 16:59:12.489930 pyrofork_dev-2.1.8.dev202305201658/pyproject.toml
--rw-r--r--   0        0        0     1446 2023-05-20 16:58:43.825726 pyrofork_dev-2.1.8.dev202305201658/pyrogram/__init__.py
--rw-r--r--   0        0        0    40792 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/client.py
--rw-r--r--   0        0        0      854 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/__init__.py
--rw-r--r--   0        0        0     2830 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/connection.py
--rw-r--r--   0        0        0      838 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/__init__.py
--rw-r--r--   0        0        0     1044 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0        0        0     4100 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0        0        0     1768 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0        0        0     2830 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0        0        0     1906 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0        0        0     1511 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0        0        0     2453 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
--rw-r--r--   0        0        0      818 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/__init__.py
--rw-r--r--   0        0        0     4013 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/aes.py
--rw-r--r--   0        0        0     4767 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/mtproto.py
--rw-r--r--   0        0        0     2446 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/prime.py
--rw-r--r--   0        0        0    13437 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/rsa.py
--rw-r--r--   0        0        0    10085 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/dispatcher.py
--rw-r--r--   0        0        0   208021 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/emoji.py
--rw-r--r--   0        0        0     1736 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/__init__.py
--rw-r--r--   0        0        0     1002 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/auto_name.py
--rw-r--r--   0        0        0     2307 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_action.py
--rw-r--r--   0        0        0     4520 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_event_action.py
--rw-r--r--   0        0        0     1265 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_member_status.py
--rw-r--r--   0        0        0     1446 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0        0        0     1238 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_type.py
--rw-r--r--   0        0        0     2464 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/message_entity_type.py
--rw-r--r--   0        0        0     1599 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/message_media_type.py
--rw-r--r--   0        0        0     2468 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/message_service_type.py
--rw-r--r--   0        0        0     2406 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/messages_filter.py
--rw-r--r--   0        0        0     1521 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/next_code_type.py
--rw-r--r--   0        0        0     1188 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/parse_mode.py
--rw-r--r--   0        0        0     1047 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/poll_type.py
--rw-r--r--   0        0        0     1723 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/sent_code_type.py
--rw-r--r--   0        0        0     1299 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/user_status.py
--rw-r--r--   0        0        0     2489 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/__init__.py
--rw-r--r--   0        0        0     1066 2023-05-20 16:59:12.477930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/__init__.py
--rw-r--r--   0        0        0    25520 2023-05-20 16:59:12.481931 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/all.py
--rw-r--r--   0        0        0    64535 2023-05-20 16:59:12.481931 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/bad_request_400.py
--rw-r--r--   0        0        0     1941 2023-05-20 16:59:12.477930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/flood_420.py
--rw-r--r--   0        0        0     6046 2023-05-20 16:59:12.477930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/forbidden_403.py
--rw-r--r--   0        0        0    10644 2023-05-20 16:59:12.477930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/internal_server_error_500.py
--rw-r--r--   0        0        0     3580 2023-05-20 16:59:12.477930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/not_acceptable_406.py
--rw-r--r--   0        0        0     1952 2023-05-20 16:59:12.473930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/see_other_303.py
--rw-r--r--   0        0        0     1351 2023-05-20 16:59:12.473930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/service_unavailable_503.py
--rw-r--r--   0        0        0     2672 2023-05-20 16:59:12.477930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/unauthorized_401.py
--rw-r--r--   0        0        0     3315 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/rpc_error.py
--rw-r--r--   0        0        0    15154 2023-05-20 16:58:30.753641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/file_id.py
--rw-r--r--   0        0        0    24836 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/filters.py
--rw-r--r--   0        0        0     1475 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0        0        0     2011 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0        0        0     2046 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0        0        0     2101 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0        0        0     2543 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0        0        0     1702 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0        0        0     1979 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0        0        0     1550 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/handler.py
--rw-r--r--   0        0        0     1984 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0        0        0     1935 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/message_handler.py
--rw-r--r--   0        0        0     1914 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/poll_handler.py
--rw-r--r--   0        0        0     2942 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0        0        0     1989 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/user_status_handler.py
--rw-r--r--   0        0        0     1365 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/__init__.py
--rw-r--r--   0        0        0      988 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0        0        0     3133 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0        0        0     4560 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0        0        0     8164 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/save_file.py
--rw-r--r--   0        0        0     1655 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/__init__.py
--rw-r--r--   0        0        0     1468 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0        0        0     1942 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/check_password.py
--rw-r--r--   0        0        0     1749 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/connect.py
--rw-r--r--   0        0        0     1504 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0        0        0     1307 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0        0        0     1664 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/initialize.py
--rw-r--r--   0        0        0     1626 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/log_out.py
--rw-r--r--   0        0        0     1831 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0        0        0     2150 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0        0        0     2786 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/send_code.py
--rw-r--r--   0        0        0     1473 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0        0        0     3085 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0        0        0     2723 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0        0        0     2355 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0        0        0     1859 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/terminate.py
--rw-r--r--   0        0        0     2041 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/__init__.py
--rw-r--r--   0        0        0     3311 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0        0        0     4990 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0        0        0     1989 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0        0        0     2360 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0        0        0     2573 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0        0        0     2051 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0        0        0     2319 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0        0        0     2798 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0        0        0     3365 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0        0        0     2847 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0        0        0     4191 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/send_game.py
--rw-r--r--   0        0        0     2886 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0        0        0     2710 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0        0        0     3186 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0        0        0     2048 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0        0        0     3946 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_game_score.py
--rw-r--r--   0        0        0     4299 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/__init__.py
--rw-r--r--   0        0        0     3364 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0        0        0     2216 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0        0        0     4620 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0        0        0     1848 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0        0        0     1711 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0        0        0     1817 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0        0        0     2333 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0        0        0     2281 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_group.py
--rw-r--r--   0        0        0     1955 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0        0        0     1585 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0        0        0     2307 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0        0        0     1943 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0        0        0     1603 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0        0        0     1969 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0        0        0     2177 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0        0        0     1830 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0        0        0     3282 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0        0        0     4032 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0        0        0     3338 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0        0        0     5282 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0        0        0     2264 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0        0        0     1723 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0        0        0     3360 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0        0        0     2096 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0        0        0     2285 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0        0        0     3145 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0        0        0     2401 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0        0        0     2136 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0        0        0     1715 2023-05-20 16:58:30.757641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0        0        0     2694 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0        0        0     2605 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0        0        0     1528 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0        0        0     3157 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0        0        0     3925 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0        0        0     1853 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0        0        0     1734 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0        0        0     4381 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0        0        0     3136 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0        0        0     2247 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0        0        0     3484 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0        0        0     4601 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0        0        0     1727 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0        0        0     2572 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0        0        0     2296 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0        0        0     1982 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0        0        0     2083 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0        0        0     2230 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0        0        0     2305 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0        0        0     1724 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0        0        0     2139 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unpin_chat_message.py
--rw-r--r--   0        0        0     1154 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0        0        0     2566 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0        0        0     2448 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0        0        0     1605 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0        0        0     1422 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0        0        0     1934 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/import_contacts.py
--rw-r--r--   0        0        0     1624 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0        0        0     2169 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0        0        0     2190 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0        0        0     2217 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0        0        0     2183 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0        0        0     1553 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0        0        0     2172 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0        0        0     2167 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0        0        0     2138 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0        0        0     2120 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0        0        0     1818 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0        0        0     2154 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_user_status.py
--rw-r--r--   0        0        0     2435 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0        0        0     1894 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0        0        0     1924 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0        0        0     3369 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0        0        0     1895 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0        0        0     1925 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0        0        0     2031 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0        0        0     1751 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0        0        0     3533 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0        0        0     2582 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0        0        0     3566 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0        0        0     2335 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0        0        0     1997 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0        0        0     1925 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0        0        0     2928 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0        0        0     1929 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0        0        0     2947 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0        0        0     2329 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     3921 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/__init__.py
--rw-r--r--   0        0        0     5963 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0        0        0     5423 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0        0        0     3148 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0        0        0     7530 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/download_media.py
--rw-r--r--   0        0        0     2271 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0        0        0    10375 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0        0        0     2464 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0        0        0     3115 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0        0        0     2978 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0        0        0    13022 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0        0        0     2976 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0        0        0     3906 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0        0        0     4824 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0        0        0     4501 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0        0        0     2389 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0        0        0     1980 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0     2229 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0        0        0     2808 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0        0        0     1950 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0        0        0     2946 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0        0        0     4741 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0        0        0     2175 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0        0        0     2527 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0        0        0     2124 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0        0        0     4160 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_global.py
--rw-r--r--   0        0        0     2156 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0        0        0     5349 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0        0        0     3203 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0        0        0    12828 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0        0        0    11362 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0        0        0     5723 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0        0        0     3076 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0        0        0     5111 2023-05-20 16:58:30.761641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0        0        0     5085 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0        0        0    10712 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_document.py
--rw-r--r--   0        0        0     4820 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_location.py
--rw-r--r--   0        0        0    20821 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0        0        0     7509 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_message.py
--rw-r--r--   0        0        0     9682 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0        0        0     8315 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0        0        0     2361 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0        0        0     8582 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0        0        0     5641 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0        0        0    12198 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_video.py
--rw-r--r--   0        0        0     9556 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0        0        0     9672 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0        0        0     2819 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0        0        0     3937 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0        0        0     2504 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/vote_poll.py
--rw-r--r--   0        0        0     1088 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/__init__.py
--rw-r--r--   0        0        0     2797 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0        0        0     3006 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0        0        0     2143 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/remove_cloud_password.py
--rw-r--r--   0        0        0     1049 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0        0        0     2819 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0        0        0     4292 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0        0        0     1752 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/get_sticker_set.py
--rw-r--r--   0        0        0     1659 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/__init__.py
--rw-r--r--   0        0        0     1771 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/block_user.py
--rw-r--r--   0        0        0     2237 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0        0        0     4421 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0        0        0     2509 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0        0        0     2359 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0        0        0     1664 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0        0        0     1565 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_me.py
--rw-r--r--   0        0        0     2562 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_users.py
--rw-r--r--   0        0        0     1882 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0        0        0     2718 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0        0        0     1876 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/set_username.py
--rw-r--r--   0        0        0     1781 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0        0        0     2376 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/update_profile.py
--rw-r--r--   0        0        0     1253 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0        0        0     2346 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0        0        0     2232 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/compose.py
--rw-r--r--   0        0        0     1557 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0        0        0     2750 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/idle.py
--rw-r--r--   0        0        0     2210 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0        0        0     2294 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/restart.py
--rw-r--r--   0        0        0     2857 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/run.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/start.py
--rw-r--r--   0        0        0     2117 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/stop.py
--rw-r--r--   0        0        0     1724 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0        0        0    61915 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/mime_types.py
--rw-r--r--   0        0        0      846 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/__init__.py
--rw-r--r--   0        0        0     8681 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/html.py
--rw-r--r--   0        0        0     5770 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/markdown.py
--rw-r--r--   0        0        0     2077 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/parser.py
--rw-r--r--   0        0        0     1545 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/utils.py
--rw-r--r--   0        0        0        0 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/py.typed
--rw-r--r--   0        0        0     1040 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/__init__.py
--rw-r--r--   0        0        0   105239 2023-05-20 16:59:12.449930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/all.py
--rw-r--r--   0        0        0    14050 2023-05-20 16:59:12.429930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/__init__.py
--rw-r--r--   0        0        0     1934 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/access_point_rule.py
--rw-r--r--   0        0        0     2134 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/account_days_ttl.py
--rw-r--r--   0        0        0     2158 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/app_web_view_result.py
--rw-r--r--   0        0        0     1922 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bot.py
--rw-r--r--   0        0        0     1947 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bot_icon.py
--rw-r--r--   0        0        0     1978 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bot_icon_color.py
--rw-r--r--   0        0        0     2215 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bots.py
--rw-r--r--   0        0        0     2157 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bots_bot.py
--rw-r--r--   0        0        0     2256 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_peer_type.py
--rw-r--r--   0        0        0     2126 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/authorization.py
--rw-r--r--   0        0        0     1964 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/auto_download_settings.py
--rw-r--r--   0        0        0     1946 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/auto_save_exception.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/auto_save_settings.py
--rw-r--r--   0        0        0     1945 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/available_reaction.py
--rw-r--r--   0        0        0     2004 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bad_msg_notification.py
--rw-r--r--   0        0        0     1935 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bank_card_open_url.py
--rw-r--r--   0        0        0     2124 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/base_theme.py
--rw-r--r--   0        0        0     1941 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bind_auth_key_inner.py
--rw-r--r--   0        0        0     1939 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_app.py
--rw-r--r--   0        0        0     2107 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_command.py
--rw-r--r--   0        0        0     2363 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_command_scope.py
--rw-r--r--   0        0        0     1885 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_info.py
--rw-r--r--   0        0        0     2336 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_inline_message.py
--rw-r--r--   0        0        0     2000 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_inline_result.py
--rw-r--r--   0        0        0     2261 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_menu_button.py
--rw-r--r--   0        0        0     2099 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/cdn_config.py
--rw-r--r--   0        0        0     1916 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/cdn_public_key.py
--rw-r--r--   0        0        0     1965 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_admin_log_event.py
--rw-r--r--   0        0        0     6564 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_admin_log_event_action.py
--rw-r--r--   0        0        0     2008 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_admin_log_events_filter.py
--rw-r--r--   0        0        0     1999 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_location.py
--rw-r--r--   0        0        0     2048 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_messages_filter.py
--rw-r--r--   0        0        0     2309 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_participant.py
--rw-r--r--   0        0        0     2524 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_participants_filter.py
--rw-r--r--   0        0        0     2057 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat.py
--rw-r--r--   0        0        0     1934 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_admin_rights.py
--rw-r--r--   0        0        0     1965 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_admin_with_invites.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_banned_rights.py
--rw-r--r--   0        0        0     1939 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_full.py
--rw-r--r--   0        0        0     2225 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_invite.py
--rw-r--r--   0        0        0     1952 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_invite_importer.py
--rw-r--r--   0        0        0     2113 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_onlines.py
--rw-r--r--   0        0        0     2068 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_participant.py
--rw-r--r--   0        0        0     2015 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_participants.py
--rw-r--r--   0        0        0     1951 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_photo.py
--rw-r--r--   0        0        0     2046 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_reactions.py
--rw-r--r--   0        0        0     1947 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/client_dh_inner_data.py
--rw-r--r--   0        0        0     1915 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/code_settings.py
--rw-r--r--   0        0        0     2077 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/config.py
--rw-r--r--   0        0        0     1884 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/contact.py
--rw-r--r--   0        0        0     2126 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/contact_status.py
--rw-r--r--   0        0        0     2131 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/data_json.py
--rw-r--r--   0        0        0     1891 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dc_option.py
--rw-r--r--   0        0        0     2160 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/default_history_ttl.py
--rw-r--r--   0        0        0     2267 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/destroy_auth_key_res.py
--rw-r--r--   0        0        0     2205 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/destroy_session_res.py
--rw-r--r--   0        0        0     1928 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog.py
--rw-r--r--   0        0        0     2254 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog_filter.py
--rw-r--r--   0        0        0     2189 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog_filter_suggested.py
--rw-r--r--   0        0        0     2175 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog_peer.py
--rw-r--r--   0        0        0     2266 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/document.py
--rw-r--r--   0        0        0     2487 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/document_attribute.py
--rw-r--r--   0        0        0     1975 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/draft_message.py
--rw-r--r--   0        0        0     2094 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/email_verification.py
--rw-r--r--   0        0        0     2133 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/email_verify_purpose.py
--rw-r--r--   0        0        0     1903 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_group.py
--rw-r--r--   0        0        0     1979 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_keyword.py
--rw-r--r--   0        0        0     2241 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_keywords_difference.py
--rw-r--r--   0        0        0     2140 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_language.py
--rw-r--r--   0        0        0     2271 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_list.py
--rw-r--r--   0        0        0     2024 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_status.py
--rw-r--r--   0        0        0     2096 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_url.py
--rw-r--r--   0        0        0     2436 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/encrypted_chat.py
--rw-r--r--   0        0        0     2196 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/encrypted_file.py
--rw-r--r--   0        0        0     2011 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/encrypted_message.py
--rw-r--r--   0        0        0     1872 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/error.py
--rw-r--r--   0        0        0     2244 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_chat_invite.py
--rw-r--r--   0        0        0     2189 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_chatlist_invite.py
--rw-r--r--   0        0        0     2176 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_contact_token.py
--rw-r--r--   0        0        0     2169 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_message_link.py
--rw-r--r--   0        0        0     2168 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/file_hash.py
--rw-r--r--   0        0        0     1878 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/folder.py
--rw-r--r--   0        0        0     1903 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/folder_peer.py
--rw-r--r--   0        0        0     1963 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/forum_topic.py
--rw-r--r--   0        0        0     1866 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/game.py
--rw-r--r--   0        0        0     1943 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/geo_point.py
--rw-r--r--   0        0        0     2233 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/global_privacy_settings.py
--rw-r--r--   0        0        0     1959 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call.py
--rw-r--r--   0        0        0     1964 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_participant.py
--rw-r--r--   0        0        0     1995 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_participant_video.py
--rw-r--r--   0        0        0     2063 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_participant_video_source_group.py
--rw-r--r--   0        0        0     1977 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_stream_channel.py
--rw-r--r--   0        0        0     1897 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/high_score.py
--rw-r--r--   0        0        0     1891 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/http_wait.py
--rw-r--r--   0        0        0     1933 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/imported_contact.py
--rw-r--r--   0        0        0     1947 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/inline_bot_switch_pm.py
--rw-r--r--   0        0        0     1941 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/inline_bot_web_view.py
--rw-r--r--   0        0        0     2351 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/inline_query_peer_type.py
--rw-r--r--   0        0        0     1922 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_app_event.py
--rw-r--r--   0        0        0     1980 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_app.py
--rw-r--r--   0        0        0     2492 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_inline_message.py
--rw-r--r--   0        0        0     2060 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_inline_message_id.py
--rw-r--r--   0        0        0     2195 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_inline_result.py
--rw-r--r--   0        0        0     2046 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_channel.py
--rw-r--r--   0        0        0     2061 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_chat_photo.py
--rw-r--r--   0        0        0     1945 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_chatlist.py
--rw-r--r--   0        0        0     2043 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_check_password_srp.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_client_proxy.py
--rw-r--r--   0        0        0     1925 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_contact.py
--rw-r--r--   0        0        0     2002 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_dialog_peer.py
--rw-r--r--   0        0        0     1983 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_document.py
--rw-r--r--   0        0        0     1952 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_encrypted_chat.py
--rw-r--r--   0        0        0     2184 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_encrypted_file.py
--rw-r--r--   0        0        0     1947 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_file.py
--rw-r--r--   0        0        0     2601 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_file_location.py
--rw-r--r--   0        0        0     1934 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_folder_peer.py
--rw-r--r--   0        0        0     1963 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_game.py
--rw-r--r--   0        0        0     1984 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_geo_point.py
--rw-r--r--   0        0        0     1928 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_group_call.py
--rw-r--r--   0        0        0     1987 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_invoice.py
--rw-r--r--   0        0        0     2779 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_media.py
--rw-r--r--   0        0        0     2119 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_message.py
--rw-r--r--   0        0        0     2183 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_notify_peer.py
--rw-r--r--   0        0        0     2240 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_payment_credentials.py
--rw-r--r--   0        0        0     2270 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_peer.py
--rw-r--r--   0        0        0     1983 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_peer_notify_settings.py
--rw-r--r--   0        0        0     1928 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_phone_call.py
--rw-r--r--   0        0        0     1959 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_photo.py
--rw-r--r--   0        0        0     2571 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_privacy_key.py
--rw-r--r--   0        0        0     2588 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_privacy_rule.py
--rw-r--r--   0        0        0     2006 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_secure_file.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_secure_value.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_single_media.py
--rw-r--r--   0        0        0     2695 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_sticker_set.py
--rw-r--r--   0        0        0     1959 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_sticker_set_item.py
--rw-r--r--   0        0        0     2048 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_stickered_media.py
--rw-r--r--   0        0        0     2095 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_store_payment_purpose.py
--rw-r--r--   0        0        0     1957 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_theme.py
--rw-r--r--   0        0        0     1952 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_theme_settings.py
--rw-r--r--   0        0        0     2067 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_user.py
--rw-r--r--   0        0        0     2055 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_wall_paper.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_web_document.py
--rw-r--r--   0        0        0     2142 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_web_file_location.py
--rw-r--r--   0        0        0     1884 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/invoice.py
--rw-r--r--   0        0        0     1929 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/ip_port.py
--rw-r--r--   0        0        0     1934 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/json_object_value.py
--rw-r--r--   0        0        0     2115 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/json_value.py
--rw-r--r--   0        0        0     3020 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/keyboard_button.py
--rw-r--r--   0        0        0     1946 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/keyboard_button_row.py
--rw-r--r--   0        0        0     1915 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/labeled_price.py
--rw-r--r--   0        0        0     2193 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/lang_pack_difference.py
--rw-r--r--   0        0        0     2180 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/lang_pack_language.py
--rw-r--r--   0        0        0     2273 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/lang_pack_string.py
--rw-r--r--   0        0        0     1903 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/mask_coords.py
--rw-r--r--   0        0        0     1987 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message.py
--rw-r--r--   0        0        0     4917 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_action.py
--rw-r--r--   0        0        0     3249 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_entity.py
--rw-r--r--   0        0        0     2044 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_extended_media.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_fwd_header.py
--rw-r--r--   0        0        0     2000 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_interaction_counters.py
--rw-r--r--   0        0        0     2945 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_media.py
--rw-r--r--   0        0        0     1958 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_peer_reaction.py
--rw-r--r--   0        0        0     2123 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_range.py
--rw-r--r--   0        0        0     1939 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_reactions.py
--rw-r--r--   0        0        0     1927 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_replies.py
--rw-r--r--   0        0        0     1952 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_reply_header.py
--rw-r--r--   0        0        0     2083 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_user_vote.py
--rw-r--r--   0        0        0     1915 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_views.py
--rw-r--r--   0        0        0     3181 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/messages_filter.py
--rw-r--r--   0        0        0     1996 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msg_detailed_info.py
--rw-r--r--   0        0        0     1972 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msg_resend_req.py
--rw-r--r--   0        0        0     1885 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_ack.py
--rw-r--r--   0        0        0     1910 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_all_info.py
--rw-r--r--   0        0        0     1922 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_state_info.py
--rw-r--r--   0        0        0     1916 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_state_req.py
--rw-r--r--   0        0        0     2099 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/nearest_dc.py
--rw-r--r--   0        0        0     1917 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/new_session.py
--rw-r--r--   0        0        0     2171 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/notification_sound.py
--rw-r--r--   0        0        0     2112 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/notify_peer.py
--rw-r--r--   0        0        0     1866 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/null.py
--rw-r--r--   0        0        0     1866 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page.py
--rw-r--r--   0        0        0     3535 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_block.py
--rw-r--r--   0        0        0     1909 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_caption.py
--rw-r--r--   0        0        0     1986 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_list_item.py
--rw-r--r--   0        0        0     2043 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_list_ordered_item.py
--rw-r--r--   0        0        0     1952 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_related_article.py
--rw-r--r--   0        0        0     1922 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_table_cell.py
--rw-r--r--   0        0        0     1916 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_table_row.py
--rw-r--r--   0        0        0     2104 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/password_kdf_algo.py
--rw-r--r--   0        0        0     1921 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_charge.py
--rw-r--r--   0        0        0     1946 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_form_method.py
--rw-r--r--   0        0        0     1964 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_requested_info.py
--rw-r--r--   0        0        0     1990 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_saved_credentials.py
--rw-r--r--   0        0        0     2185 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer.py
--rw-r--r--   0        0        0     1909 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_blocked.py
--rw-r--r--   0        0        0     1965 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_located.py
--rw-r--r--   0        0        0     2162 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_notify_settings.py
--rw-r--r--   0        0        0     1915 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_settings.py
--rw-r--r--   0        0        0     2189 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_call.py
--rw-r--r--   0        0        0     2237 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_call_discard_reason.py
--rw-r--r--   0        0        0     1946 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_call_protocol.py
--rw-r--r--   0        0        0     2001 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_connection.py
--rw-r--r--   0        0        0     1918 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/photo.py
--rw-r--r--   0        0        0     2181 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/photo_size.py
--rw-r--r--   0        0        0     1866 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll.py
--rw-r--r--   0        0        0     1903 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll_answer.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll_answer_voters.py
--rw-r--r--   0        0        0     1909 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll_results.py
--rw-r--r--   0        0        0     2088 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/pong.py
--rw-r--r--   0        0        0     1927 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/popular_contact.py
--rw-r--r--   0        0        0     1909 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/post_address.py
--rw-r--r--   0        0        0     2076 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/pq_inner_data.py
--rw-r--r--   0        0        0     1946 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/premium_gift_option.py
--rw-r--r--   0        0        0     1994 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/premium_subscription_option.py
--rw-r--r--   0        0        0     2460 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/privacy_key.py
--rw-r--r--   0        0        0     2487 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/privacy_rule.py
--rw-r--r--   0        0        0     2015 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/reaction.py
--rw-r--r--   0        0        0     1921 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/reaction_count.py
--rw-r--r--   0        0        0     2178 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/read_participant_date.py
--rw-r--r--   0        0        0     2180 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/received_notify_message.py
--rw-r--r--   0        0        0     2169 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/recent_me_url.py
--rw-r--r--   0        0        0     2115 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/reply_markup.py
--rw-r--r--   0        0        0     2640 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/report_reason.py
--rw-r--r--   0        0        0     2079 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/request_peer_type.py
--rw-r--r--   0        0        0     2087 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/res_pq.py
--rw-r--r--   0        0        0     1945 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/restriction_reason.py
--rw-r--r--   0        0        0     2572 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rich_text.py
--rw-r--r--   0        0        0     2255 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rpc_drop_answer.py
--rw-r--r--   0        0        0     1891 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rpc_error.py
--rw-r--r--   0        0        0     1897 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rpc_result.py
--rw-r--r--   0        0        0     2127 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/saved_contact.py
--rw-r--r--   0        0        0     2007 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/search_results_calendar_period.py
--rw-r--r--   0        0        0     1968 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/search_results_position.py
--rw-r--r--   0        0        0     2000 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_credentials_encrypted.py
--rw-r--r--   0        0        0     1903 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_data.py
--rw-r--r--   0        0        0     1959 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_file.py
--rw-r--r--   0        0        0     2184 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_password_kdf_algo.py
--rw-r--r--   0        0        0     1994 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_plain_data.py
--rw-r--r--   0        0        0     2024 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_required_type.py
--rw-r--r--   0        0        0     1964 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_secret_settings.py
--rw-r--r--   0        0        0     2192 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value.py
--rw-r--r--   0        0        0     2537 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value_error.py
--rw-r--r--   0        0        0     1934 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value_hash.py
--rw-r--r--   0        0        0     2918 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value_type.py
--rw-r--r--   0        0        0     1904 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/send_as_peer.py
--rw-r--r--   0        0        0     3337 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/send_message_action.py
--rw-r--r--   0        0        0     1947 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/server_dh_inner_data.py
--rw-r--r--   0        0        0     2190 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/server_dh_params.py
--rw-r--r--   0        0        0     2243 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/set_client_dh_params_answer.py
--rw-r--r--   0        0        0     1927 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/shipping_option.py
--rw-r--r--   0        0        0     2179 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/simple_web_view_result.py
--rw-r--r--   0        0        0     1939 2023-05-20 16:59:12.193928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sponsored_message.py
--rw-r--r--   0        0        0     1966 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_abs_value_and_prev.py
--rw-r--r--   0        0        0     1953 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_date_range_days.py
--rw-r--r--   0        0        0     2219 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_graph.py
--rw-r--r--   0        0        0     1953 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_group_top_admin.py
--rw-r--r--   0        0        0     1965 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_group_top_inviter.py
--rw-r--r--   0        0        0     1959 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_group_top_poster.py
--rw-r--r--   0        0        0     1946 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_percent_value.py
--rw-r--r--   0        0        0     1891 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_url.py
--rw-r--r--   0        0        0     1927 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_keyword.py
--rw-r--r--   0        0        0     1909 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_pack.py
--rw-r--r--   0        0        0     1903 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_set.py
--rw-r--r--   0        0        0     2359 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_set_covered.py
--rw-r--r--   0        0        0     1940 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/text_with_entities.py
--rw-r--r--   0        0        0     2138 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/theme.py
--rw-r--r--   0        0        0     1921 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/theme_settings.py
--rw-r--r--   0        0        0     1885 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/top_peer.py
--rw-r--r--   0        0        0     2476 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/top_peer_category.py
--rw-r--r--   0        0        0     1965 2023-05-20 16:59:12.173928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/top_peer_category_peers.py
--rw-r--r--   0        0        0     9329 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/update.py
--rw-r--r--   0        0        0     5681 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/updates_t.py
--rw-r--r--   0        0        0     2313 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/url_auth_result.py
--rw-r--r--   0        0        0     2251 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user.py
--rw-r--r--   0        0        0     1891 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user_full.py
--rw-r--r--   0        0        0     2008 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user_profile_photo.py
--rw-r--r--   0        0        0     2215 2023-05-20 16:59:12.161928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user_status.py
--rw-r--r--   0        0        0     1890 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/username.py
--rw-r--r--   0        0        0     2032 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/video_size.py
--rw-r--r--   0        0        0     2234 2023-05-20 16:59:12.165928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/wall_paper.py
--rw-r--r--   0        0        0     1946 2023-05-20 16:59:12.185928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/wall_paper_settings.py
--rw-r--r--   0        0        0     1939 2023-05-20 16:59:12.181928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_authorization.py
--rw-r--r--   0        0        0     1971 2023-05-20 16:59:12.177928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_document.py
--rw-r--r--   0        0        0     2253 2023-05-20 16:59:12.169928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_page.py
--rw-r--r--   0        0        0     1950 2023-05-20 16:59:12.189928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_page_attribute.py
--rw-r--r--   0        0        0     2171 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_view_message_sent.py
--rw-r--r--   0        0        0     2136 2023-05-20 16:59:12.197928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_view_result.py
--rw-r--r--   0        0        0     1312 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/__init__.py
--rw-r--r--   0        0        0     1692 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/future_salt.py
--rw-r--r--   0        0        0     1891 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/future_salts.py
--rw-r--r--   0        0        0     1814 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0        0        0     1048 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/list.py
--rw-r--r--   0        0        0     1851 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/message.py
--rw-r--r--   0        0        0     1614 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/msg_container.py
--rw-r--r--   0        0        0     1012 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0        0        0     1497 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0        0        0     1759 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0        0        0     1193 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0        0        0     1358 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0        0        0     1194 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0        0        0     2022 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0        0        0     2495 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/tl_object.py
--rw-r--r--   0        0        0     1998 2023-05-20 16:59:12.441930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/__init__.py
--rw-r--r--   0        0        0     2010 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/destroy_auth_key.py
--rw-r--r--   0        0        0     2211 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/destroy_session.py
--rw-r--r--   0        0        0     2133 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/get_future_salts.py
--rw-r--r--   0        0        0     4863 2023-05-20 16:59:12.361930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/init_connection.py
--rw-r--r--   0        0        0     2397 2023-05-20 16:59:12.361930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_after_msg.py
--rw-r--r--   0        0        0     2450 2023-05-20 16:59:12.361930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_after_msgs.py
--rw-r--r--   0        0        0     2389 2023-05-20 16:59:12.361930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_with_layer.py
--rw-r--r--   0        0        0     2492 2023-05-20 16:59:12.361930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_with_messages_range.py
--rw-r--r--   0        0        0     2445 2023-05-20 16:59:12.361930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_with_takeout.py
--rw-r--r--   0        0        0     2209 2023-05-20 16:59:12.361930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_without_updates.py
--rw-r--r--   0        0        0     2118 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/ping.py
--rw-r--r--   0        0        0     2477 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/ping_delay_disconnect.py
--rw-r--r--   0        0        0     3390 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/req_dh_params.py
--rw-r--r--   0        0        0     2113 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/req_pq.py
--rw-r--r--   0        0        0     2133 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/req_pq_multi.py
--rw-r--r--   0        0        0     2199 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/rpc_drop_answer.py
--rw-r--r--   0        0        0     2750 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/set_client_dh_params.py
--rw-r--r--   0        0        0    56200 2023-05-20 16:59:12.437930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/access_point_rule.py
--rw-r--r--   0        0        0     2329 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/account_days_ttl.py
--rw-r--r--   0        0        0     2345 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/app_web_view_result_url.py
--rw-r--r--   0        0        0     4075 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bot.py
--rw-r--r--   0        0        0     2923 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bot_icon.py
--rw-r--r--   0        0        0     2362 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bot_icon_color.py
--rw-r--r--   0        0        0     2886 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bots.py
--rw-r--r--   0        0        0     2675 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bots_bot.py
--rw-r--r--   0        0        0     2234 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bots_not_modified.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_bot_pm.py
--rw-r--r--   0        0        0     2036 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_broadcast.py
--rw-r--r--   0        0        0     2014 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_chat.py
--rw-r--r--   0        0        0     2008 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_pm.py
--rw-r--r--   0        0        0     2036 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_same_bot_pm.py
--rw-r--r--   0        0        0     6710 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/authorization.py
--rw-r--r--   0        0        0     4611 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/auto_download_settings.py
--rw-r--r--   0        0        0     2492 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/auto_save_exception.py
--rw-r--r--   0        0        0     2962 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/auto_save_settings.py
--rw-r--r--   0        0        0     5709 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/available_reaction.py
--rw-r--r--   0        0        0     2718 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bad_msg_notification.py
--rw-r--r--   0        0        0     2991 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bad_server_salt.py
--rw-r--r--   0        0        0     2307 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bank_card_open_url.py
--rw-r--r--   0        0        0     1979 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_arctic.py
--rw-r--r--   0        0        0     1983 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_classic.py
--rw-r--r--   0        0        0     1967 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_day.py
--rw-r--r--   0        0        0     1975 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_night.py
--rw-r--r--   0        0        0     1979 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_tinted.py
--rw-r--r--   0        0        0     3288 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bind_auth_key_inner.py
--rw-r--r--   0        0        0     3944 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_app.py
--rw-r--r--   0        0        0     1984 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_app_not_modified.py
--rw-r--r--   0        0        0     2584 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command.py
--rw-r--r--   0        0        0     2025 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_chat_admins.py
--rw-r--r--   0        0        0     2005 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_chats.py
--rw-r--r--   0        0        0     2013 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_default.py
--rw-r--r--   0        0        0     2204 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_peer.py
--rw-r--r--   0        0        0     2228 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_peer_admins.py
--rw-r--r--   0        0        0     2495 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_peer_user.py
--rw-r--r--   0        0        0     2005 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_users.py
--rw-r--r--   0        0        0     4814 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_info.py
--rw-r--r--   0        0        0     4328 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_media_result.py
--rw-r--r--   0        0        0     3220 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_auto.py
--rw-r--r--   0        0        0     3471 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_contact.py
--rw-r--r--   0        0        0     4119 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_geo.py
--rw-r--r--   0        0        0     4576 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_invoice.py
--rw-r--r--   0        0        0     3871 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_venue.py
--rw-r--r--   0        0        0     3494 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_text.py
--rw-r--r--   0        0        0     4665 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_result.py
--rw-r--r--   0        0        0     2502 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_menu_button.py
--rw-r--r--   0        0        0     2212 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_menu_button_commands.py
--rw-r--r--   0        0        0     2208 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_menu_button_default.py
--rw-r--r--   0        0        0     2456 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/cdn_config.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/cdn_public_key.py
--rw-r--r--   0        0        0    12591 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel.py
--rw-r--r--   0        0        0     2887 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event.py
--rw-r--r--   0        0        0     2514 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_about.py
--rw-r--r--   0        0        0     2720 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_available_reactions.py
--rw-r--r--   0        0        0     2538 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_history_ttl.py
--rw-r--r--   0        0        0     2542 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_linked_chat.py
--rw-r--r--   0        0        0     2694 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_location.py
--rw-r--r--   0        0        0     2604 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_photo.py
--rw-r--r--   0        0        0     2794 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_sticker_set.py
--rw-r--r--   0        0        0     2514 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_title.py
--rw-r--r--   0        0        0     2526 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_username.py
--rw-r--r--   0        0        0     2610 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_usernames.py
--rw-r--r--   0        0        0     2300 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_create_topic.py
--rw-r--r--   0        0        0     2868 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_default_banned_rights.py
--rw-r--r--   0        0        0     2314 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_delete_message.py
--rw-r--r--   0        0        0     2300 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_delete_topic.py
--rw-r--r--   0        0        0     2327 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_discard_group_call.py
--rw-r--r--   0        0        0     2656 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_edit_message.py
--rw-r--r--   0        0        0     2636 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_edit_topic.py
--rw-r--r--   0        0        0     2377 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_delete.py
--rw-r--r--   0        0        0     2754 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_edit.py
--rw-r--r--   0        0        0     2377 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_revoke.py
--rw-r--r--   0        0        0     2410 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_invite.py
--rw-r--r--   0        0        0     2100 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_join.py
--rw-r--r--   0        0        0     2746 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_invite.py
--rw-r--r--   0        0        0     2650 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_request.py
--rw-r--r--   0        0        0     2104 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_leave.py
--rw-r--r--   0        0        0     2410 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_mute.py
--rw-r--r--   0        0        0     2860 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_admin.py
--rw-r--r--   0        0        0     2852 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_ban.py
--rw-r--r--   0        0        0     2418 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_unmute.py
--rw-r--r--   0        0        0     2418 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_volume.py
--rw-r--r--   0        0        0     3005 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_pin_topic.py
--rw-r--r--   0        0        0     2306 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_send_message.py
--rw-r--r--   0        0        0     2319 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_start_group_call.py
--rw-r--r--   0        0        0     2294 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_stop_poll.py
--rw-r--r--   0        0        0     2279 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_anti_spam.py
--rw-r--r--   0        0        0     2265 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_forum.py
--rw-r--r--   0        0        0     2320 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_group_call_setting.py
--rw-r--r--   0        0        0     2275 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_invites.py
--rw-r--r--   0        0        0     2287 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_no_forwards.py
--rw-r--r--   0        0        0     2311 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_pre_history_hidden.py
--rw-r--r--   0        0        0     2287 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_signatures.py
--rw-r--r--   0        0        0     2530 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_slow_mode.py
--rw-r--r--   0        0        0     2310 2023-05-20 16:59:12.313929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_update_pinned.py
--rw-r--r--   0        0        0     6648 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_events_filter.py
--rw-r--r--   0        0        0     3591 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_forbidden.py
--rw-r--r--   0        0        0    21188 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_full.py
--rw-r--r--   0        0        0     2445 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_location.py
--rw-r--r--   0        0        0     2005 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_location_empty.py
--rw-r--r--   0        0        0     2699 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_messages_filter.py
--rw-r--r--   0        0        0     2035 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_messages_filter_empty.py
--rw-r--r--   0        0        0     2365 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant.py
--rw-r--r--   0        0        0     4333 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_admin.py
--rw-r--r--   0        0        0     3281 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_banned.py
--rw-r--r--   0        0        0     2936 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_creator.py
--rw-r--r--   0        0        0     2199 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_left.py
--rw-r--r--   0        0        0     2977 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_self.py
--rw-r--r--   0        0        0     2035 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_admins.py
--rw-r--r--   0        0        0     2150 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_banned.py
--rw-r--r--   0        0        0     2027 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_bots.py
--rw-r--r--   0        0        0     2158 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_contacts.py
--rw-r--r--   0        0        0     2150 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_kicked.py
--rw-r--r--   0        0        0     2762 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_mentions.py
--rw-r--r--   0        0        0     2035 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_recent.py
--rw-r--r--   0        0        0     2148 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_search.py
--rw-r--r--   0        0        0     6664 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat.py
--rw-r--r--   0        0        0     5640 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_admin_rights.py
--rw-r--r--   0        0        0     2809 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_admin_with_invites.py
--rw-r--r--   0        0        0     8389 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_banned_rights.py
--rw-r--r--   0        0        0     2079 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_empty.py
--rw-r--r--   0        0        0     2293 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_forbidden.py
--rw-r--r--   0        0        0     9951 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_full.py
--rw-r--r--   0        0        0     5192 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite.py
--rw-r--r--   0        0        0     2379 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_already.py
--rw-r--r--   0        0        0     6062 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_exported.py
--rw-r--r--   0        0        0     3786 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_importer.py
--rw-r--r--   0        0        0     2585 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_peek.py
--rw-r--r--   0        0        0     2249 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_public_join_requests.py
--rw-r--r--   0        0        0     2339 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_onlines.py
--rw-r--r--   0        0        0     2598 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participant.py
--rw-r--r--   0        0        0     2618 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participant_admin.py
--rw-r--r--   0        0        0     2187 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participant_creator.py
--rw-r--r--   0        0        0     2750 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participants.py
--rw-r--r--   0        0        0     2804 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participants_forbidden.py
--rw-r--r--   0        0        0     3122 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_photo.py
--rw-r--r--   0        0        0     1975 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_photo_empty.py
--rw-r--r--   0        0        0     2297 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_reactions_all.py
--rw-r--r--   0        0        0     1991 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_reactions_none.py
--rw-r--r--   0        0        0     2257 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_reactions_some.py
--rw-r--r--   0        0        0     2842 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/client_dh_inner_data.py
--rw-r--r--   0        0        0     4902 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/code_settings.py
--rw-r--r--   0        0        0    19235 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/config.py
--rw-r--r--   0        0        0     2322 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/contact.py
--rw-r--r--   0        0        0     2625 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/contact_status.py
--rw-r--r--   0        0        0     2331 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/data_json.py
--rw-r--r--   0        0        0     4562 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dc_option.py
--rw-r--r--   0        0        0     2370 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/default_history_ttl.py
--rw-r--r--   0        0        0     2197 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_auth_key_fail.py
--rw-r--r--   0        0        0     2197 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_auth_key_none.py
--rw-r--r--   0        0        0     2189 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_auth_key_ok.py
--rw-r--r--   0        0        0     2398 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_session_none.py
--rw-r--r--   0        0        0     2390 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_session_ok.py
--rw-r--r--   0        0        0     2906 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dh_gen_fail.py
--rw-r--r--   0        0        0     2898 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dh_gen_ok.py
--rw-r--r--   0        0        0     2910 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dh_gen_retry.py
--rw-r--r--   0        0        0     6524 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog.py
--rw-r--r--   0        0        0     6358 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter.py
--rw-r--r--   0        0        0     4000 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter_chatlist.py
--rw-r--r--   0        0        0     2207 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter_default.py
--rw-r--r--   0        0        0     2718 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter_suggested.py
--rw-r--r--   0        0        0     4534 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_folder.py
--rw-r--r--   0        0        0     2356 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_peer.py
--rw-r--r--   0        0        0     2386 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_peer_folder.py
--rw-r--r--   0        0        0     5113 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document.py
--rw-r--r--   0        0        0     2027 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_animated.py
--rw-r--r--   0        0        0     3632 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_audio.py
--rw-r--r--   0        0        0     3079 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_custom_emoji.py
--rw-r--r--   0        0        0     2214 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_filename.py
--rw-r--r--   0        0        0     2039 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_has_stickers.py
--rw-r--r--   0        0        0     2312 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_image_size.py
--rw-r--r--   0        0        0     3253 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_sticker.py
--rw-r--r--   0        0        0     3253 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_video.py
--rw-r--r--   0        0        0     2422 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_empty.py
--rw-r--r--   0        0        0     3616 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/draft_message.py
--rw-r--r--   0        0        0     2333 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/draft_message_empty.py
--rw-r--r--   0        0        0     2166 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verification_apple.py
--rw-r--r--   0        0        0     2153 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verification_code.py
--rw-r--r--   0        0        0     2170 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verification_google.py
--rw-r--r--   0        0        0     2044 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verify_purpose_login_change.py
--rw-r--r--   0        0        0     2542 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verify_purpose_login_setup.py
--rw-r--r--   0        0        0     2032 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verify_purpose_passport.py
--rw-r--r--   0        0        0     2660 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_group.py
--rw-r--r--   0        0        0     2413 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_keyword.py
--rw-r--r--   0        0        0     2441 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_keyword_deleted.py
--rw-r--r--   0        0        0     3271 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_keywords_difference.py
--rw-r--r--   0        0        0     2380 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_language.py
--rw-r--r--   0        0        0     2706 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_list.py
--rw-r--r--   0        0        0     2306 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_list_not_modified.py
--rw-r--r--   0        0        0     2175 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_status.py
--rw-r--r--   0        0        0     1985 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_status_empty.py
--rw-r--r--   0        0        0     2395 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_status_until.py
--rw-r--r--   0        0        0     2287 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_url.py
--rw-r--r--   0        0        0     3831 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat.py
--rw-r--r--   0        0        0     2770 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_discarded.py
--rw-r--r--   0        0        0     2370 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_empty.py
--rw-r--r--   0        0        0     3974 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_requested.py
--rw-r--r--   0        0        0     3340 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_waiting.py
--rw-r--r--   0        0        0     3257 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_file.py
--rw-r--r--   0        0        0     2207 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_file_empty.py
--rw-r--r--   0        0        0     3056 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_message.py
--rw-r--r--   0        0        0     2818 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_message_service.py
--rw-r--r--   0        0        0     2268 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/error.py
--rw-r--r--   0        0        0     2876 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/exported_chatlist_invite.py
--rw-r--r--   0        0        0     2572 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/exported_contact_token.py
--rw-r--r--   0        0        0     2546 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/exported_message_link.py
--rw-r--r--   0        0        0     2781 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/file_hash.py
--rw-r--r--   0        0        0     3983 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/folder.py
--rw-r--r--   0        0        0     2379 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/folder_peer.py
--rw-r--r--   0        0        0     7364 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/forum_topic.py
--rw-r--r--   0        0        0     2112 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/forum_topic_deleted.py
--rw-r--r--   0        0        0     3740 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/game.py
--rw-r--r--   0        0        0     3070 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/geo_point.py
--rw-r--r--   0        0        0     1970 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/geo_point_empty.py
--rw-r--r--   0        0        0     2977 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/global_privacy_settings.py
--rw-r--r--   0        0        0     8290 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call.py
--rw-r--r--   0        0        0     2604 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_discarded.py
--rw-r--r--   0        0        0     8200 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_participant.py
--rw-r--r--   0        0        0     3410 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_participant_video.py
--rw-r--r--   0        0        0     2535 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_participant_video_source_group.py
--rw-r--r--   0        0        0     2702 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_stream_channel.py
--rw-r--r--   0        0        0     2511 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/high_score.py
--rw-r--r--   0        0        0     2611 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/http_wait.py
--rw-r--r--   0        0        0     2398 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/imported_contact.py
--rw-r--r--   0        0        0     2389 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_bot_switch_pm.py
--rw-r--r--   0        0        0     2312 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_bot_web_view.py
--rw-r--r--   0        0        0     2023 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_bot_pm.py
--rw-r--r--   0        0        0     2041 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_broadcast.py
--rw-r--r--   0        0        0     2021 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_chat.py
--rw-r--r--   0        0        0     2041 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_megagroup.py
--rw-r--r--   0        0        0     2013 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_pm.py
--rw-r--r--   0        0        0     2041 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_same_bot_pm.py
--rw-r--r--   0        0        0     2765 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_app_event.py
--rw-r--r--   0        0        0     2359 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_app_id.py
--rw-r--r--   0        0        0     2465 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_app_short_name.py
--rw-r--r--   0        0        0     2528 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_game.py
--rw-r--r--   0        0        0     2611 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_id.py
--rw-r--r--   0        0        0     2846 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_id64.py
--rw-r--r--   0        0        0     3245 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_auto.py
--rw-r--r--   0        0        0     3496 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_contact.py
--rw-r--r--   0        0        0     4220 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_geo.py
--rw-r--r--   0        0        0     4490 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_invoice.py
--rw-r--r--   0        0        0     3970 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_venue.py
--rw-r--r--   0        0        0     3519 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_text.py
--rw-r--r--   0        0        0     4750 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result.py
--rw-r--r--   0        0        0     3846 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result_document.py
--rw-r--r--   0        0        0     2763 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result_game.py
--rw-r--r--   0        0        0     2976 2023-05-20 16:59:12.289929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result_photo.py
--rw-r--r--   0        0        0     2428 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_channel.py
--rw-r--r--   0        0        0     1990 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_channel_empty.py
--rw-r--r--   0        0        0     2674 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_channel_from_message.py
--rw-r--r--   0        0        0     2169 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chat_photo.py
--rw-r--r--   0        0        0     2000 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chat_photo_empty.py
--rw-r--r--   0        0        0     3852 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chat_uploaded_photo.py
--rw-r--r--   0        0        0     2212 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chatlist_dialog_filter.py
--rw-r--r--   0        0        0     2023 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_check_password_empty.py
--rw-r--r--   0        0        0     2515 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_check_password_srp.py
--rw-r--r--   0        0        0     2350 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_client_proxy.py
--rw-r--r--   0        0        0     2188 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_dialog_peer.py
--rw-r--r--   0        0        0     2198 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_dialog_peer_folder.py
--rw-r--r--   0        0        0     2641 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_document.py
--rw-r--r--   0        0        0     1995 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_document_empty.py
--rw-r--r--   0        0        0     2936 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_document_file_location.py
--rw-r--r--   0        0        0     2428 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_chat.py
--rw-r--r--   0        0        0     2386 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file.py
--rw-r--r--   0        0        0     2663 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_big_uploaded.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_empty.py
--rw-r--r--   0        0        0     2417 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_location.py
--rw-r--r--   0        0        0     2912 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_uploaded.py
--rw-r--r--   0        0        0     2734 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_file.py
--rw-r--r--   0        0        0     2485 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_file_big.py
--rw-r--r--   0        0        0     2906 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_file_location.py
--rw-r--r--   0        0        0     2424 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_folder_peer.py
--rw-r--r--   0        0        0     2347 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_game_id.py
--rw-r--r--   0        0        0     2455 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_game_short_name.py
--rw-r--r--   0        0        0     2838 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_geo_point.py
--rw-r--r--   0        0        0     1995 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_geo_point_empty.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_group_call.py
--rw-r--r--   0        0        0     3582 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_group_call_stream.py
--rw-r--r--   0        0        0     2410 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_invoice_message.py
--rw-r--r--   0        0        0     2128 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_invoice_slug.py
--rw-r--r--   0        0        0     3407 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_keyboard_button_url_auth.py
--rw-r--r--   0        0        0     2463 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_keyboard_button_user_profile.py
--rw-r--r--   0        0        0     2877 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_contact.py
--rw-r--r--   0        0        0     2154 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_dice.py
--rw-r--r--   0        0        0     3281 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_document.py
--rw-r--r--   0        0        0     2891 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_document_external.py
--rw-r--r--   0        0        0     1980 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_empty.py
--rw-r--r--   0        0        0     2161 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_game.py
--rw-r--r--   0        0        0     3929 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_geo_live.py
--rw-r--r--   0        0        0     2256 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_geo_point.py
--rw-r--r--   0        0        0     4853 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_invoice.py
--rw-r--r--   0        0        0     2903 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_photo.py
--rw-r--r--   0        0        0     2879 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_photo_external.py
--rw-r--r--   0        0        0     3669 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_poll.py
--rw-r--r--   0        0        0     5063 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_uploaded_document.py
--rw-r--r--   0        0        0     3430 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_uploaded_photo.py
--rw-r--r--   0        0        0     3351 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_venue.py
--rw-r--r--   0        0        0     2378 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_callback_query.py
--rw-r--r--   0        0        0     2687 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_entity_mention_name.py
--rw-r--r--   0        0        0     2104 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_id.py
--rw-r--r--   0        0        0     1994 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_pinned.py
--rw-r--r--   0        0        0     2124 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_reply_to.py
--rw-r--r--   0        0        0     2040 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_chat_photos.py
--rw-r--r--   0        0        0     2032 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_contacts.py
--rw-r--r--   0        0        0     2032 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_document.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_empty.py
--rw-r--r--   0        0        0     2012 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_geo.py
--rw-r--r--   0        0        0     2012 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_gif.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_music.py
--rw-r--r--   0        0        0     2040 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_my_mentions.py
--rw-r--r--   0        0        0     2296 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_phone_calls.py
--rw-r--r--   0        0        0     2040 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_photo_video.py
--rw-r--r--   0        0        0     2024 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_photos.py
--rw-r--r--   0        0        0     2024 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_pinned.py
--rw-r--r--   0        0        0     2040 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_round_video.py
--rw-r--r--   0        0        0     2040 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_round_voice.py
--rw-r--r--   0        0        0     2012 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_url.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_video.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_voice.py
--rw-r--r--   0        0        0     2009 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_broadcasts.py
--rw-r--r--   0        0        0     1989 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_chats.py
--rw-r--r--   0        0        0     2457 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_forum_topic.py
--rw-r--r--   0        0        0     2188 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_peer.py
--rw-r--r--   0        0        0     1989 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_users.py
--rw-r--r--   0        0        0     2509 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials.py
--rw-r--r--   0        0        0     2326 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials_apple_pay.py
--rw-r--r--   0        0        0     2341 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials_google_pay.py
--rw-r--r--   0        0        0     2431 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials_saved.py
--rw-r--r--   0        0        0     2441 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_channel.py
--rw-r--r--   0        0        0     2687 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_channel_from_message.py
--rw-r--r--   0        0        0     2145 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_chat.py
--rw-r--r--   0        0        0     1975 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_empty.py
--rw-r--r--   0        0        0     3679 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_notify_settings.py
--rw-r--r--   0        0        0     2740 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_photo_file_location.py
--rw-r--r--   0        0        0     1971 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_self.py
--rw-r--r--   0        0        0     2402 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_user.py
--rw-r--r--   0        0        0     2648 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_user_from_message.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_phone_call.py
--rw-r--r--   0        0        0     2857 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_phone_contact.py
--rw-r--r--   0        0        0     2626 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo.py
--rw-r--r--   0        0        0     1980 2023-05-20 16:59:12.213929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo_empty.py
--rw-r--r--   0        0        0     2924 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo_file_location.py
--rw-r--r--   0        0        0     3383 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo_legacy_file_location.py
--rw-r--r--   0        0        0     2033 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_added_by_phone.py
--rw-r--r--   0        0        0     2025 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_chat_invite.py
--rw-r--r--   0        0        0     2017 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_forwards.py
--rw-r--r--   0        0        0     2021 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_phone_call.py
--rw-r--r--   0        0        0     2027 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_phone_number.py
--rw-r--r--   0        0        0     2017 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_phone_p2_p.py
--rw-r--r--   0        0        0     2033 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_profile_photo.py
--rw-r--r--   0        0        0     2045 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_status_timestamp.py
--rw-r--r--   0        0        0     2037 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_voice_messages.py
--rw-r--r--   0        0        0     2026 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_all.py
--rw-r--r--   0        0        0     2274 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_chat_participants.py
--rw-r--r--   0        0        0     2044 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_contacts.py
--rw-r--r--   0        0        0     2268 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_users.py
--rw-r--r--   0        0        0     2038 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_all.py
--rw-r--r--   0        0        0     2286 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_chat_participants.py
--rw-r--r--   0        0        0     2056 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_contacts.py
--rw-r--r--   0        0        0     2280 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_users.py
--rw-r--r--   0        0        0     2030 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_child_abuse.py
--rw-r--r--   0        0        0     2026 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_copyright.py
--rw-r--r--   0        0        0     2006 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_fake.py
--rw-r--r--   0        0        0     2042 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_geo_irrelevant.py
--rw-r--r--   0        0        0     2036 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_illegal_drugs.py
--rw-r--r--   0        0        0     2010 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_other.py
--rw-r--r--   0        0        0     2050 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_personal_details.py
--rw-r--r--   0        0        0     2034 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_pornography.py
--rw-r--r--   0        0        0     2006 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_spam.py
--rw-r--r--   0        0        0     2022 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_violence.py
--rw-r--r--   0        0        0     2371 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_file.py
--rw-r--r--   0        0        0     2405 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_file_location.py
--rw-r--r--   0        0        0     3050 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_file_uploaded.py
--rw-r--r--   0        0        0     5597 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_value.py
--rw-r--r--   0        0        0     3187 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_single_media.py
--rw-r--r--   0        0        0     2035 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_animated_emoji.py
--rw-r--r--   0        0        0     2075 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_animated_emoji_animations.py
--rw-r--r--   0        0        0     2179 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_dice.py
--rw-r--r--   0        0        0     2065 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_emoji_default_statuses.py
--rw-r--r--   0        0        0     2073 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_emoji_default_topic_icons.py
--rw-r--r--   0        0        0     2071 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_emoji_generic_animations.py
--rw-r--r--   0        0        0     2005 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_empty.py
--rw-r--r--   0        0        0     2379 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_id.py
--rw-r--r--   0        0        0     3374 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_item.py
--rw-r--r--   0        0        0     2033 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_premium_gifts.py
--rw-r--r--   0        0        0     2217 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_short_name.py
--rw-r--r--   0        0        0     2560 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_thumb.py
--rw-r--r--   0        0        0     2236 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_stickered_media_document.py
--rw-r--r--   0        0        0     2214 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_stickered_media_photo.py
--rw-r--r--   0        0        0     2713 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_store_payment_gift_premium.py
--rw-r--r--   0        0        0     2610 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_store_payment_premium_subscription.py
--rw-r--r--   0        0        0     2023 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_takeout_file_location.py
--rw-r--r--   0        0        0     2346 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_theme.py
--rw-r--r--   0        0        0     5043 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_theme_settings.py
--rw-r--r--   0        0        0     2118 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_theme_slug.py
--rw-r--r--   0        0        0     2386 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user.py
--rw-r--r--   0        0        0     1975 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user_empty.py
--rw-r--r--   0        0        0     2632 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user_from_message.py
--rw-r--r--   0        0        0     1971 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user_self.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_wall_paper.py
--rw-r--r--   0        0        0     2133 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_wall_paper_no_file.py
--rw-r--r--   0        0        0     2138 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_wall_paper_slug.py
--rw-r--r--   0        0        0     2906 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_document.py
--rw-r--r--   0        0        0     3532 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_file_audio_album_thumb_location.py
--rw-r--r--   0        0        0     3282 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_file_geo_point_location.py
--rw-r--r--   0        0        0     2400 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_file_location.py
--rw-r--r--   0        0        0     6967 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/invoice.py
--rw-r--r--   0        0        0     2275 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/ip_port.py
--rw-r--r--   0        0        0     2507 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/ip_port_secret.py
--rw-r--r--   0        0        0     2189 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_array.py
--rw-r--r--   0        0        0     2098 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_bool.py
--rw-r--r--   0        0        0     1951 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_null.py
--rw-r--r--   0        0        0     2125 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_number.py
--rw-r--r--   0        0        0     2217 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_object.py
--rw-r--r--   0        0        0     2377 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_object_value.py
--rw-r--r--   0        0        0     2110 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_string.py
--rw-r--r--   0        0        0     2122 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button.py
--rw-r--r--   0        0        0     2134 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_buy.py
--rw-r--r--   0        0        0     2746 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_callback.py
--rw-r--r--   0        0        0     2138 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_game.py
--rw-r--r--   0        0        0     2194 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_geo_location.py
--rw-r--r--   0        0        0     2719 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_peer.py
--rw-r--r--   0        0        0     2170 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_phone.py
--rw-r--r--   0        0        0     2550 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_poll.py
--rw-r--r--   0        0        0     2267 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_row.py
--rw-r--r--   0        0        0     2354 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_simple_web_view.py
--rw-r--r--   0        0        0     3225 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_switch_inline.py
--rw-r--r--   0        0        0     2314 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_url.py
--rw-r--r--   0        0        0     2998 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_url_auth.py
--rw-r--r--   0        0        0     2387 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_user_profile.py
--rw-r--r--   0        0        0     2330 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_web_view.py
--rw-r--r--   0        0        0     2333 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/labeled_price.py
--rw-r--r--   0        0        0     3227 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_difference.py
--rw-r--r--   0        0        0     5222 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_language.py
--rw-r--r--   0        0        0     2514 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_string.py
--rw-r--r--   0        0        0     2344 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_string_deleted.py
--rw-r--r--   0        0        0     4665 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_string_pluralized.py
--rw-r--r--   0        0        0     2635 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/mask_coords.py
--rw-r--r--   0        0        0    12715 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message.py
--rw-r--r--   0        0        0     3061 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_bot_allowed.py
--rw-r--r--   0        0        0     2178 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_channel_create.py
--rw-r--r--   0        0        0     2419 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_channel_migrate_from.py
--rw-r--r--   0        0        0     2215 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_add_user.py
--rw-r--r--   0        0        0     2409 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_create.py
--rw-r--r--   0        0        0     2035 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_delete_photo.py
--rw-r--r--   0        0        0     2205 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_delete_user.py
--rw-r--r--   0        0        0     2223 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_edit_photo.py
--rw-r--r--   0        0        0     2178 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_edit_title.py
--rw-r--r--   0        0        0     2238 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_joined_by_link.py
--rw-r--r--   0        0        0     2051 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_joined_by_request.py
--rw-r--r--   0        0        0     2228 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_migrate_to.py
--rw-r--r--   0        0        0     2027 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_contact_sign_up.py
--rw-r--r--   0        0        0     2192 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_custom_action.py
--rw-r--r--   0        0        0     1995 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_empty.py
--rw-r--r--   0        0        0     2385 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_game_score.py
--rw-r--r--   0        0        0     2727 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_geo_proximity_reached.py
--rw-r--r--   0        0        0     3574 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_gift_premium.py
--rw-r--r--   0        0        0     2668 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_group_call.py
--rw-r--r--   0        0        0     2542 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_group_call_scheduled.py
--rw-r--r--   0        0        0     2023 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_history_clear.py
--rw-r--r--   0        0        0     2509 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_invite_to_group_call.py
--rw-r--r--   0        0        0     3599 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_payment_sent.py
--rw-r--r--   0        0        0     4621 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_payment_sent_me.py
--rw-r--r--   0        0        0     3345 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_phone_call.py
--rw-r--r--   0        0        0     2015 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_pin_message.py
--rw-r--r--   0        0        0     2446 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_requested_peer.py
--rw-r--r--   0        0        0     2035 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_screenshot_taken.py
--rw-r--r--   0        0        0     2297 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_secure_values_sent.py
--rw-r--r--   0        0        0     2679 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_secure_values_sent_me.py
--rw-r--r--   0        0        0     2201 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_chat_theme.py
--rw-r--r--   0        0        0     2287 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_chat_wall_paper.py
--rw-r--r--   0        0        0     2729 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_messages_ttl.py
--rw-r--r--   0        0        0     2303 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_same_chat_wall_paper.py
--rw-r--r--   0        0        0     2247 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_suggest_profile_photo.py
--rw-r--r--   0        0        0     2905 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_topic_create.py
--rw-r--r--   0        0        0     3532 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_topic_edit.py
--rw-r--r--   0        0        0     2177 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_web_view_data_sent.py
--rw-r--r--   0        0        0     2374 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_web_view_data_sent_me.py
--rw-r--r--   0        0        0     2552 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_empty.py
--rw-r--r--   0        0        0     2378 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_bank_card.py
--rw-r--r--   0        0        0     2384 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_blockquote.py
--rw-r--r--   0        0        0     2362 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_bold.py
--rw-r--r--   0        0        0     2386 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_bot_command.py
--rw-r--r--   0        0        0     2374 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_cashtag.py
--rw-r--r--   0        0        0     2362 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_code.py
--rw-r--r--   0        0        0     2647 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_custom_emoji.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_email.py
--rw-r--r--   0        0        0     2374 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_hashtag.py
--rw-r--r--   0        0        0     2370 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_italic.py
--rw-r--r--   0        0        0     2374 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_mention.py
--rw-r--r--   0        0        0     2611 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_mention_name.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_phone.py
--rw-r--r--   0        0        0     2583 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_pre.py
--rw-r--r--   0        0        0     2374 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_spoiler.py
--rw-r--r--   0        0        0     2370 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_strike.py
--rw-r--r--   0        0        0     2554 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_text_url.py
--rw-r--r--   0        0        0     2382 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_underline.py
--rw-r--r--   0        0        0     2374 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_unknown.py
--rw-r--r--   0        0        0     2358 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_url.py
--rw-r--r--   0        0        0     2234 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_extended_media.py
--rw-r--r--   0        0        0     3529 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_extended_media_preview.py
--rw-r--r--   0        0        0     5501 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_fwd_header.py
--rw-r--r--   0        0        0     2629 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_interaction_counters.py
--rw-r--r--   0        0        0     3393 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_contact.py
--rw-r--r--   0        0        0     2649 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_dice.py
--rw-r--r--   0        0        0     3702 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_document.py
--rw-r--r--   0        0        0     2275 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_empty.py
--rw-r--r--   0        0        0     2454 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_game.py
--rw-r--r--   0        0        0     2457 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_geo.py
--rw-r--r--   0        0        0     3725 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_geo_live.py
--rw-r--r--   0        0        0     5586 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_invoice.py
--rw-r--r--   0        0        0     3360 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_photo.py
--rw-r--r--   0        0        0     2739 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_poll.py
--rw-r--r--   0        0        0     2299 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_unsupported.py
--rw-r--r--   0        0        0     3572 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_venue.py
--rw-r--r--   0        0        0     2505 2023-05-20 16:59:12.225929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_web_page.py
--rw-r--r--   0        0        0     3222 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_peer_reaction.py
--rw-r--r--   0        0        0     2546 2023-05-20 16:59:12.285929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_range.py
--rw-r--r--   0        0        0     3439 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_reactions.py
--rw-r--r--   0        0        0     4451 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_replies.py
--rw-r--r--   0        0        0     3938 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_reply_header.py
--rw-r--r--   0        0        0     5782 2023-05-20 16:59:12.221929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_service.py
--rw-r--r--   0        0        0     2558 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_user_vote.py
--rw-r--r--   0        0        0     2394 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_user_vote_input_option.py
--rw-r--r--   0        0        0     2639 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_user_vote_multiple.py
--rw-r--r--   0        0        0     3169 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_views.py
--rw-r--r--   0        0        0     2834 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_detailed_info.py
--rw-r--r--   0        0        0     2634 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_new_detailed_info.py
--rw-r--r--   0        0        0     2196 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_resend_ans_req.py
--rw-r--r--   0        0        0     2184 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_resend_req.py
--rw-r--r--   0        0        0     2159 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_ack.py
--rw-r--r--   0        0        0     2368 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_all_info.py
--rw-r--r--   0        0        0     2365 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_state_info.py
--rw-r--r--   0        0        0     2184 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_state_req.py
--rw-r--r--   0        0        0     2788 2023-05-20 16:59:12.261929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/nearest_dc.py
--rw-r--r--   0        0        0     2703 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/new_session_created.py
--rw-r--r--   0        0        0     2023 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_default.py
--rw-r--r--   0        0        0     2355 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_local.py
--rw-r--r--   0        0        0     2011 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_none.py
--rw-r--r--   0        0        0     2156 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_ringtone.py
--rw-r--r--   0        0        0     1984 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_broadcasts.py
--rw-r--r--   0        0        0     1964 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_chats.py
--rw-r--r--   0        0        0     2412 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_forum_topic.py
--rw-r--r--   0        0        0     2143 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_peer.py
--rw-r--r--   0        0        0     1964 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_users.py
--rw-r--r--   0        0        0     1930 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/null.py
--rw-r--r--   0        0        0     4034 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page.py
--rw-r--r--   0        0        0     2121 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_anchor.py
--rw-r--r--   0        0        0     2443 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_audio.py
--rw-r--r--   0        0        0     2493 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_author_date.py
--rw-r--r--   0        0        0     2467 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_blockquote.py
--rw-r--r--   0        0        0     2193 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_channel.py
--rw-r--r--   0        0        0     2502 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_collage.py
--rw-r--r--   0        0        0     2187 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_cover.py
--rw-r--r--   0        0        0     2766 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_details.py
--rw-r--r--   0        0        0     1983 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_divider.py
--rw-r--r--   0        0        0     4659 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_embed.py
--rw-r--r--   0        0        0     3638 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_embed_post.py
--rw-r--r--   0        0        0     2178 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_footer.py
--rw-r--r--   0        0        0     2178 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_header.py
--rw-r--r--   0        0        0     2178 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_kicker.py
--rw-r--r--   0        0        0     2217 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_list.py
--rw-r--r--   0        0        0     2961 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_map.py
--rw-r--r--   0        0        0     2273 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_ordered_list.py
--rw-r--r--   0        0        0     2190 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_paragraph.py
--rw-r--r--   0        0        0     3234 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_photo.py
--rw-r--r--   0        0        0     2427 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_preformatted.py
--rw-r--r--   0        0        0     2463 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_pullquote.py
--rw-r--r--   0        0        0     2567 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_related_articles.py
--rw-r--r--   0        0        0     2508 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_slideshow.py
--rw-r--r--   0        0        0     2190 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_subheader.py
--rw-r--r--   0        0        0     2186 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_subtitle.py
--rw-r--r--   0        0        0     3055 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_table.py
--rw-r--r--   0        0        0     2174 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_title.py
--rw-r--r--   0        0        0     1999 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_unsupported.py
--rw-r--r--   0        0        0     3004 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_video.py
--rw-r--r--   0        0        0     2428 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_caption.py
--rw-r--r--   0        0        0     2237 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_item_blocks.py
--rw-r--r--   0        0        0     2185 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_item_text.py
--rw-r--r--   0        0        0     2452 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_ordered_item_blocks.py
--rw-r--r--   0        0        0     2400 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_ordered_item_text.py
--rw-r--r--   0        0        0     4412 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_related_article.py
--rw-r--r--   0        0        0     4643 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_table_cell.py
--rw-r--r--   0        0        0     2220 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_table_row.py
--rw-r--r--   0        0        0     2863 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/password_kdf_algo_sha256_sha256_pbkdf2_hmacsha512iter100000_sha256_mod_pow.py
--rw-r--r--   0        0        0     2013 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/password_kdf_algo_unknown.py
--rw-r--r--   0        0        0     2414 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_charge.py
--rw-r--r--   0        0        0     2326 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_form_method.py
--rw-r--r--   0        0        0     3602 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_requested_info.py
--rw-r--r--   0        0        0     2363 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_saved_credentials_card.py
--rw-r--r--   0        0        0     2366 2023-05-20 16:59:12.341930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_blocked.py
--rw-r--r--   0        0        0     2380 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_channel.py
--rw-r--r--   0        0        0     2341 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_chat.py
--rw-r--r--   0        0        0     2593 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_located.py
--rw-r--r--   0        0        0     4953 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_notify_settings.py
--rw-r--r--   0        0        0     2152 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_self_located.py
--rw-r--r--   0        0        0     6386 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_settings.py
--rw-r--r--   0        0        0     2341 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_user.py
--rw-r--r--   0        0        0     5084 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call.py
--rw-r--r--   0        0        0     3871 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_accepted.py
--rw-r--r--   0        0        0     2036 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_busy.py
--rw-r--r--   0        0        0     2060 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_disconnect.py
--rw-r--r--   0        0        0     2044 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_hangup.py
--rw-r--r--   0        0        0     2044 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_missed.py
--rw-r--r--   0        0        0     3877 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discarded.py
--rw-r--r--   0        0        0     2104 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_empty.py
--rw-r--r--   0        0        0     3390 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_protocol.py
--rw-r--r--   0        0        0     3920 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_requested.py
--rw-r--r--   0        0        0     4119 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_waiting.py
--rw-r--r--   0        0        0     3167 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_connection.py
--rw-r--r--   0        0        0     3664 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_connection_webrtc.py
--rw-r--r--   0        0        0     4128 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo.py
--rw-r--r--   0        0        0     2646 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_cached_size.py
--rw-r--r--   0        0        0     2084 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_empty.py
--rw-r--r--   0        0        0     2312 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_path_size.py
--rw-r--r--   0        0        0     2616 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_size.py
--rw-r--r--   0        0        0     2115 2023-05-20 16:59:12.229929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_size_empty.py
--rw-r--r--   0        0        0     2709 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_size_progressive.py
--rw-r--r--   0        0        0     2328 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_stripped_size.py
--rw-r--r--   0        0        0     4634 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll.py
--rw-r--r--   0        0        0     2310 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll_answer.py
--rw-r--r--   0        0        0     2930 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll_answer_voters.py
--rw-r--r--   0        0        0     4558 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll_results.py
--rw-r--r--   0        0        0     2537 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pong.py
--rw-r--r--   0        0        0     2408 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/popular_contact.py
--rw-r--r--   0        0        0     3322 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/post_address.py
--rw-r--r--   0        0        0     3145 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data.py
--rw-r--r--   0        0        0     3326 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data_dc.py
--rw-r--r--   0        0        0     3406 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data_temp.py
--rw-r--r--   0        0        0     3587 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data_temp_dc.py
--rw-r--r--   0        0        0     3297 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/premium_gift_option.py
--rw-r--r--   0        0        0     4408 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/premium_subscription_option.py
--rw-r--r--   0        0        0     2008 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_added_by_phone.py
--rw-r--r--   0        0        0     2000 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_chat_invite.py
--rw-r--r--   0        0        0     1992 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_forwards.py
--rw-r--r--   0        0        0     1996 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_phone_call.py
--rw-r--r--   0        0        0     2004 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_phone_number.py
--rw-r--r--   0        0        0     1992 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_phone_p2_p.py
--rw-r--r--   0        0        0     2008 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_profile_photo.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_status_timestamp.py
--rw-r--r--   0        0        0     2010 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_voice_messages.py
--rw-r--r--   0        0        0     2001 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_all.py
--rw-r--r--   0        0        0     2249 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_chat_participants.py
--rw-r--r--   0        0        0     2021 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_contacts.py
--rw-r--r--   0        0        0     2205 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_users.py
--rw-r--r--   0        0        0     2013 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_all.py
--rw-r--r--   0        0        0     2261 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_chat_participants.py
--rw-r--r--   0        0        0     2033 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_contacts.py
--rw-r--r--   0        0        0     2217 2023-05-20 16:59:12.269929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_users.py
--rw-r--r--   0        0        0     2888 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_count.py
--rw-r--r--   0        0        0     2204 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_custom_emoji.py
--rw-r--r--   0        0        0     2148 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_emoji.py
--rw-r--r--   0        0        0     1970 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_empty.py
--rw-r--r--   0        0        0     2589 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/read_participant_date.py
--rw-r--r--   0        0        0     2550 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/received_notify_message.py
--rw-r--r--   0        0        0     2335 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_chat.py
--rw-r--r--   0        0        0     2455 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_chat_invite.py
--rw-r--r--   0        0        0     2411 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_sticker_set.py
--rw-r--r--   0        0        0     2126 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_unknown.py
--rw-r--r--   0        0        0     2335 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_user.py
--rw-r--r--   0        0        0     2246 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_inline_markup.py
--rw-r--r--   0        0        0     3010 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_keyboard_force_reply.py
--rw-r--r--   0        0        0     2272 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_keyboard_hide.py
--rw-r--r--   0        0        0     3850 2023-05-20 16:59:12.281929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_keyboard_markup.py
--rw-r--r--   0        0        0     3842 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/request_peer_type_broadcast.py
--rw-r--r--   0        0        0     4511 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/request_peer_type_chat.py
--rw-r--r--   0        0        0     2699 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/request_peer_type_user.py
--rw-r--r--   0        0        0     3224 2023-05-20 16:59:12.201928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/res_pq.py
--rw-r--r--   0        0        0     2569 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/restriction_reason.py
--rw-r--r--   0        0        0     2758 2023-05-20 16:59:12.209928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_answer_dropped.py
--rw-r--r--   0        0        0     2212 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_answer_dropped_running.py
--rw-r--r--   0        0        0     2184 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_answer_unknown.py
--rw-r--r--   0        0        0     2418 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_error.py
--rw-r--r--   0        0        0     2403 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_result.py
--rw-r--r--   0        0        0     3010 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/saved_phone_contact.py
--rw-r--r--   0        0        0     2573 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/search_result_position.py
--rw-r--r--   0        0        0     2879 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/search_results_calendar_period.py
--rw-r--r--   0        0        0     2581 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_credentials_encrypted.py
--rw-r--r--   0        0        0     2546 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_data.py
--rw-r--r--   0        0        0     3374 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_file.py
--rw-r--r--   0        0        0     1980 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_file_empty.py
--rw-r--r--   0        0        0     2262 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_password_kdf_algo_pbkdf2_hmacsha512iter100000.py
--rw-r--r--   0        0        0     2182 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_password_kdf_algo_sha512.py
--rw-r--r--   0        0        0     2039 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_password_kdf_algo_unknown.py
--rw-r--r--   0        0        0     2140 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_plain_email.py
--rw-r--r--   0        0        0     2140 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_plain_phone.py
--rw-r--r--   0        0        0     3307 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_required_type.py
--rw-r--r--   0        0        0     2288 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_required_type_one_of.py
--rw-r--r--   0        0        0     2897 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_secret_settings.py
--rw-r--r--   0        0        0     5944 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value.py
--rw-r--r--   0        0        0     2596 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error.py
--rw-r--r--   0        0        0     2855 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_data.py
--rw-r--r--   0        0        0     2657 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_file.py
--rw-r--r--   0        0        0     2701 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_files.py
--rw-r--r--   0        0        0     2673 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_front_side.py
--rw-r--r--   0        0        0     2685 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_reverse_side.py
--rw-r--r--   0        0        0     2665 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_selfie.py
--rw-r--r--   0        0        0     2701 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_translation_file.py
--rw-r--r--   0        0        0     2745 2023-05-20 16:59:12.325929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_translation_files.py
--rw-r--r--   0        0        0     2402 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_hash.py
--rw-r--r--   0        0        0     2013 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_address.py
--rw-r--r--   0        0        0     2037 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_bank_statement.py
--rw-r--r--   0        0        0     2035 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_driver_license.py
--rw-r--r--   0        0        0     2005 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_email.py
--rw-r--r--   0        0        0     2033 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_identity_card.py
--rw-r--r--   0        0        0     2049 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_internal_passport.py
--rw-r--r--   0        0        0     2017 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_passport.py
--rw-r--r--   0        0        0     2065 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_passport_registration.py
--rw-r--r--   0        0        0     2045 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_personal_details.py
--rw-r--r--   0        0        0     2005 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_phone.py
--rw-r--r--   0        0        0     2045 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_rental_agreement.py
--rw-r--r--   0        0        0     2069 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_temporary_registration.py
--rw-r--r--   0        0        0     2029 2023-05-20 16:59:12.321929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_utility_bill.py
--rw-r--r--   0        0        0     2536 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_as_peer.py
--rw-r--r--   0        0        0     2019 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_cancel_action.py
--rw-r--r--   0        0        0     2047 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_choose_contact_action.py
--rw-r--r--   0        0        0     2047 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_choose_sticker_action.py
--rw-r--r--   0        0        0     2731 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_emoji_interaction.py
--rw-r--r--   0        0        0     2229 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_emoji_interaction_seen.py
--rw-r--r--   0        0        0     2027 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_game_play_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_geo_location_action.py
--rw-r--r--   0        0        0     2227 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_history_import_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_record_audio_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_record_round_action.py
--rw-r--r--   0        0        0     2039 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_record_video_action.py
--rw-r--r--   0        0        0     2019 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_typing_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_audio_action.py
--rw-r--r--   0        0        0     2231 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_document_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_photo_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_round_action.py
--rw-r--r--   0        0        0     2219 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_video_action.py
--rw-r--r--   0        0        0     3256 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/server_dh_inner_data.py
--rw-r--r--   0        0        0     2918 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/server_dh_params_fail.py
--rw-r--r--   0        0        0     2917 2023-05-20 16:59:12.205928 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/server_dh_params_ok.py
--rw-r--r--   0        0        0     2604 2023-05-20 16:59:12.309929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/shipping_option.py
--rw-r--r--   0        0        0     2363 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/simple_web_view_result_url.py
--rw-r--r--   0        0        0     2027 2023-05-20 16:59:12.265929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/speaking_in_group_call_action.py
--rw-r--r--   0        0        0     6685 2023-05-20 16:59:12.345929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sponsored_message.py
--rw-r--r--   0        0        0     2434 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_abs_value_and_prev.py
--rw-r--r--   0        0        0     2407 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_date_range_days.py
--rw-r--r--   0        0        0     2817 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_graph.py
--rw-r--r--   0        0        0     2335 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_graph_async.py
--rw-r--r--   0        0        0     2335 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_graph_error.py
--rw-r--r--   0        0        0     2810 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_group_top_admin.py
--rw-r--r--   0        0        0     2438 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_group_top_inviter.py
--rw-r--r--   0        0        0     2642 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_group_top_poster.py
--rw-r--r--   0        0        0     2365 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_percent_value.py
--rw-r--r--   0        0        0     2083 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_url.py
--rw-r--r--   0        0        0     2446 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_keyword.py
--rw-r--r--   0        0        0     2422 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_pack.py
--rw-r--r--   0        0        0     7071 2023-05-20 16:59:12.277929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set.py
--rw-r--r--   0        0        0     2660 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_covered.py
--rw-r--r--   0        0        0     3351 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_full_covered.py
--rw-r--r--   0        0        0     2711 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_multi_covered.py
--rw-r--r--   0        0        0     2413 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_no_covered.py
--rw-r--r--   0        0        0     2346 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_anchor.py
--rw-r--r--   0        0        0     2149 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_bold.py
--rw-r--r--   0        0        0     2188 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_concat.py
--rw-r--r--   0        0        0     2351 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_email.py
--rw-r--r--   0        0        0     1954 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_empty.py
--rw-r--r--   0        0        0     2153 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_fixed.py
--rw-r--r--   0        0        0     2490 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_image.py
--rw-r--r--   0        0        0     2157 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_italic.py
--rw-r--r--   0        0        0     2155 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_marked.py
--rw-r--r--   0        0        0     2351 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_phone.py
--rw-r--r--   0        0        0     2096 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_plain.py
--rw-r--r--   0        0        0     2157 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_strike.py
--rw-r--r--   0        0        0     2169 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_subscript.py
--rw-r--r--   0        0        0     2177 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_superscript.py
--rw-r--r--   0        0        0     2169 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_underline.py
--rw-r--r--   0        0        0     2573 2023-05-20 16:59:12.301929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_url.py
--rw-r--r--   0        0        0     2456 2023-05-20 16:59:12.357930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_with_entities.py
--rw-r--r--   0        0        0     5594 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/theme.py
--rw-r--r--   0        0        0     4409 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/theme_settings.py
--rw-r--r--   0        0        0     2350 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer.py
--rw-r--r--   0        0        0     2025 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_bots_inline.py
--rw-r--r--   0        0        0     2009 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_bots_pm.py
--rw-r--r--   0        0        0     2017 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_channels.py
--rw-r--r--   0        0        0     2039 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_correspondents.py
--rw-r--r--   0        0        0     2033 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_forward_chats.py
--rw-r--r--   0        0        0     2033 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_forward_users.py
--rw-r--r--   0        0        0     2009 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_groups.py
--rw-r--r--   0        0        0     2746 2023-05-20 16:59:12.297929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_peers.py
--rw-r--r--   0        0        0     2025 2023-05-20 16:59:12.293929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_phone_calls.py
--rw-r--r--   0        0        0     1996 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_attach_menu_bots.py
--rw-r--r--   0        0        0     2004 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_auto_save_settings.py
--rw-r--r--   0        0        0     3975 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_callback_query.py
--rw-r--r--   0        0        0     3307 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_chat_invite_requester.py
--rw-r--r--   0        0        0     2691 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_commands.py
--rw-r--r--   0        0        0     3736 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_inline_query.py
--rw-r--r--   0        0        0     3449 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_inline_send.py
--rw-r--r--   0        0        0     2441 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_menu_button.py
--rw-r--r--   0        0        0     4117 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_precheckout_query.py
--rw-r--r--   0        0        0     2991 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_shipping_query.py
--rw-r--r--   0        0        0     2739 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_stopped.py
--rw-r--r--   0        0        0     2195 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_webhook_json.py
--rw-r--r--   0        0        0     2663 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_webhook_json_query.py
--rw-r--r--   0        0        0     2169 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel.py
--rw-r--r--   0        0        0     2536 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_available_messages.py
--rw-r--r--   0        0        0     2629 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_message_forwards.py
--rw-r--r--   0        0        0     2590 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_message_views.py
--rw-r--r--   0        0        0     4986 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_participant.py
--rw-r--r--   0        0        0     2743 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_pinned_topic.py
--rw-r--r--   0        0        0     2653 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_pinned_topics.py
--rw-r--r--   0        0        0     2972 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_read_messages_contents.py
--rw-r--r--   0        0        0     2576 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_too_long.py
--rw-r--r--   0        0        0     3222 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_user_typing.py
--rw-r--r--   0        0        0     2884 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_web_page.py
--rw-r--r--   0        0        0     2130 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat.py
--rw-r--r--   0        0        0     2864 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_default_banned_rights.py
--rw-r--r--   0        0        0     4611 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant.py
--rw-r--r--   0        0        0     3064 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant_add.py
--rw-r--r--   0        0        0     2854 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant_admin.py
--rw-r--r--   0        0        0     2637 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant_delete.py
--rw-r--r--   0        0        0     2305 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participants.py
--rw-r--r--   0        0        0     2727 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_user_typing.py
--rw-r--r--   0        0        0     1964 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_config.py
--rw-r--r--   0        0        0     1992 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_contacts_reset.py
--rw-r--r--   0        0        0     2251 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dc_options.py
--rw-r--r--   0        0        0     2910 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_delete_channel_messages.py
--rw-r--r--   0        0        0     2634 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_delete_messages.py
--rw-r--r--   0        0        0     2482 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_delete_scheduled_messages.py
--rw-r--r--   0        0        0     2596 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_filter.py
--rw-r--r--   0        0        0     2201 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_filter_order.py
--rw-r--r--   0        0        0     1992 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_filters.py
--rw-r--r--   0        0        0     2898 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_pinned.py
--rw-r--r--   0        0        0     2514 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_unread_mark.py
--rw-r--r--   0        0        0     2898 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_draft_message.py
--rw-r--r--   0        0        0     2652 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_edit_channel_message.py
--rw-r--r--   0        0        0     2624 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_edit_message.py
--rw-r--r--   0        0        0     2187 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_encrypted_chat_typing.py
--rw-r--r--   0        0        0     2613 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_encrypted_messages_read.py
--rw-r--r--   0        0        0     2390 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_encryption.py
--rw-r--r--   0        0        0     1992 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_faved_stickers.py
--rw-r--r--   0        0        0     2703 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_folder_peers.py
--rw-r--r--   0        0        0     2384 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_geo_live_viewed.py
--rw-r--r--   0        0        0     2400 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_call.py
--rw-r--r--   0        0        0     2588 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_call_connection.py
--rw-r--r--   0        0        0     2853 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_call_participants.py
--rw-r--r--   0        0        0     2222 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_invite_privacy_forbidden.py
--rw-r--r--   0        0        0     3884 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_inline_bot_callback_query.py
--rw-r--r--   0        0        0     2265 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_lang_pack.py
--rw-r--r--   0        0        0     2187 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_lang_pack_too_long.py
--rw-r--r--   0        0        0     1980 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_login_token.py
--rw-r--r--   0        0        0     2796 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_extended_media.py
--rw-r--r--   0        0        0     2341 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_id.py
--rw-r--r--   0        0        0     2871 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_poll.py
--rw-r--r--   0        0        0     2834 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_poll_vote.py
--rw-r--r--   0        0        0     3175 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_reactions.py
--rw-r--r--   0        0        0     2769 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_move_sticker_set_to_top.py
--rw-r--r--   0        0        0     2648 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_channel_message.py
--rw-r--r--   0        0        0     2456 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_encrypted_message.py
--rw-r--r--   0        0        0     2620 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_message.py
--rw-r--r--   0        0        0     2238 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_scheduled_message.py
--rw-r--r--   0        0        0     2289 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_sticker_set.py
--rw-r--r--   0        0        0     2588 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_notify_settings.py
--rw-r--r--   0        0        0     2406 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_blocked.py
--rw-r--r--   0        0        0     2635 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_history_ttl.py
--rw-r--r--   0        0        0     2226 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_located.py
--rw-r--r--   0        0        0     2469 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_settings.py
--rw-r--r--   0        0        0     2849 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pending_join_requests.py
--rw-r--r--   0        0        0     2233 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_phone_call.py
--rw-r--r--   0        0        0     2446 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_phone_call_signaling_data.py
--rw-r--r--   0        0        0     3213 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pinned_channel_messages.py
--rw-r--r--   0        0        0     2826 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pinned_dialogs.py
--rw-r--r--   0        0        0     3167 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pinned_messages.py
--rw-r--r--   0        0        0     2455 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_privacy.py
--rw-r--r--   0        0        0     1980 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pts_changed.py
--rw-r--r--   0        0        0     3680 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_discussion_inbox.py
--rw-r--r--   0        0        0     2748 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_discussion_outbox.py
--rw-r--r--   0        0        0     3358 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_inbox.py
--rw-r--r--   0        0        0     2418 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_outbox.py
--rw-r--r--   0        0        0     2040 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_featured_emoji_stickers.py
--rw-r--r--   0        0        0     2020 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_featured_stickers.py
--rw-r--r--   0        0        0     3576 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_history_inbox.py
--rw-r--r--   0        0        0     2818 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_history_outbox.py
--rw-r--r--   0        0        0     2658 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_messages_contents.py
--rw-r--r--   0        0        0     2016 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_recent_emoji_statuses.py
--rw-r--r--   0        0        0     2000 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_recent_reactions.py
--rw-r--r--   0        0        0     1996 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_recent_stickers.py
--rw-r--r--   0        0        0     1976 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_saved_gifs.py
--rw-r--r--   0        0        0     1996 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_saved_ringtones.py
--rw-r--r--   0        0        0     3674 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_service_notification.py
--rw-r--r--   0        0        0     5802 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short.py
--rw-r--r--   0        0        0    10243 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short_chat_message.py
--rw-r--r--   0        0        0    10006 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short_message.py
--rw-r--r--   0        0        0     7778 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short_sent_message.py
--rw-r--r--   0        0        0     2489 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_sticker_sets.py
--rw-r--r--   0        0        0     2750 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_sticker_sets_order.py
--rw-r--r--   0        0        0     2156 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_theme.py
--rw-r--r--   0        0        0     3195 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_transcribed_audio.py
--rw-r--r--   0        0        0     2130 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user.py
--rw-r--r--   0        0        0     2504 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_emoji_status.py
--rw-r--r--   0        0        0     2936 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_name.py
--rw-r--r--   0        0        0     2346 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_phone.py
--rw-r--r--   0        0        0     2426 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_status.py
--rw-r--r--   0        0        0     2454 2023-05-20 16:59:12.241929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_typing.py
--rw-r--r--   0        0        0     2608 2023-05-20 16:59:12.249929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_web_page.py
--rw-r--r--   0        0        0     2191 2023-05-20 16:59:12.253929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_web_view_result_sent.py
--rw-r--r--   0        0        0     6789 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/updates_combined.py
--rw-r--r--   0        0        0     6521 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/updates_t.py
--rw-r--r--   0        0        0     5414 2023-05-20 16:59:12.257929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/updates_too_long.py
--rw-r--r--   0        0        0     2383 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/url_auth_result_accepted.py
--rw-r--r--   0        0        0     2246 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/url_auth_result_default.py
--rw-r--r--   0        0        0     3056 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/url_auth_result_request.py
--rw-r--r--   0        0        0    13966 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user.py
--rw-r--r--   0        0        0     2419 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_empty.py
--rw-r--r--   0        0        0    12871 2023-05-20 16:59:12.237929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_full.py
--rw-r--r--   0        0        0     3433 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_profile_photo.py
--rw-r--r--   0        0        0     2010 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_profile_photo_empty.py
--rw-r--r--   0        0        0     1978 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_empty.py
--rw-r--r--   0        0        0     1996 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_last_month.py
--rw-r--r--   0        0        0     1990 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_last_week.py
--rw-r--r--   0        0        0     2182 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_offline.py
--rw-r--r--   0        0        0     2155 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_online.py
--rw-r--r--   0        0        0     1992 2023-05-20 16:59:12.217929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_recently.py
--rw-r--r--   0        0        0     2707 2023-05-20 16:59:12.353930 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/username.py
--rw-r--r--   0        0        0     3129 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/video_size.py
--rw-r--r--   0        0        0     2530 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/video_size_emoji_markup.py
--rw-r--r--   0        0        0     2882 2023-05-20 16:59:12.337929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/video_size_sticker_markup.py
--rw-r--r--   0        0        0     4657 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/wall_paper.py
--rw-r--r--   0        0        0     3419 2023-05-20 16:59:12.233929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/wall_paper_no_file.py
--rw-r--r--   0        0        0     5408 2023-05-20 16:59:12.329929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/wall_paper_settings.py
--rw-r--r--   0        0        0     3892 2023-05-20 16:59:12.317929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_authorization.py
--rw-r--r--   0        0        0     3138 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_document.py
--rw-r--r--   0        0        0     2909 2023-05-20 16:59:12.305929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_document_no_proxy.py
--rw-r--r--   0        0        0     8698 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page.py
--rw-r--r--   0        0        0     2943 2023-05-20 16:59:12.333929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_attribute_theme.py
--rw-r--r--   0        0        0     2297 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_empty.py
--rw-r--r--   0        0        0     2678 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_not_modified.py
--rw-r--r--   0        0        0     2496 2023-05-20 16:59:12.273929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_pending.py
--rw-r--r--   0        0        0     2694 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_view_message_sent.py
--rw-r--r--   0        0        0     2555 2023-05-20 16:59:12.349929 pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_view_result_url.py
--rw-r--r--   0        0        0      871 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/__init__.py
--rw-r--r--   0        0        0    10513 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/auth.py
--rw-r--r--   0        0        0      917 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/__init__.py
--rw-r--r--   0        0        0     2452 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/data_center.py
--rw-r--r--   0        0        0     1374 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0        0        0     1587 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/msg_id.py
--rw-r--r--   0        0        0     1257 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/seq_no.py
--rw-r--r--   0        0        0    12440 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/session.py
--rw-r--r--   0        0        0      968 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/file_storage.py
--rw-r--r--   0        0        0     2741 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/memory_storage.py
--rw-r--r--   0        0        0     5428 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/mongo_storage.py
--rw-r--r--   0        0        0     6382 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0        0        0     2781 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/storage.py
--rw-r--r--   0        0        0     3739 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/sync.py
--rw-r--r--   0        0        0     1109 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/__init__.py
--rw-r--r--   0        0        0      938 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/authorization/__init__.py
--rw-r--r--   0        0        0     2288 2023-05-20 16:58:30.765641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0        0        0     1930 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/authorization/terms_of_service.py
--rw-r--r--   0        0        0     2830 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0        0        0     2788 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0        0        0     1293 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0        0        0     1258 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0        0        0     1249 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0        0        0     1562 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0        0        0     1639 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0        0        0     1817 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0        0        0     1308 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0        0        0     1029 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0        0        0    12797 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0        0        0     2383 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0        0        0     2216 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0        0        0     8120 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0        0        0     2460 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0        0        0     3514 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0        0        0     3712 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0        0        0     1603 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0        0        0     1209 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0        0        0     1212 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0        0        0     1809 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0        0        0     4575 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0        0        0     2339 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1564 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0        0        0     1313 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/web_app_info.py
--rw-r--r--   0        0        0     2755 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0        0        0     3662 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0        0        0     7298 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0        0        0     2411 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0        0        0     5782 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0        0        0     3304 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0        0        0     4505 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0        0        0     4245 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0        0        0     4029 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0        0        0     4388 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0        0        0     4312 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0        0        0     3031 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0        0        0     4394 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0        0        0     4202 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0        0        0     4132 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0        0        0     5240 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0        0        0     4619 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0        0        0     5261 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0        0        0     4754 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0        0        0     5474 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0        0        0     4360 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_voice.py
--rw-r--r--   0        0        0     1314 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/__init__.py
--rw-r--r--   0        0        0     1638 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media.py
--rw-r--r--   0        0        0     3428 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0        0        0     3282 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0        0        0     2771 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0        0        0     2685 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0        0        0     3620 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0        0        0     1737 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_phone_contact.py
--rw-r--r--   0        0        0     1006 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0        0        0     1413 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0        0        0     2638 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0        0        0     1093 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/list.py
--rw-r--r--   0        0        0     1885 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0        0        0     4044 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0        0        0     4069 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0        0        0     2207 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0        0        0     1587 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0        0        0     3409 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0        0        0     3044 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0        0        0     1660 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0        0        0   153174 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0        0        0     4352 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0        0        0     1800 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0        0        0     4309 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0        0        0     8016 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0        0        0     1532 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0        0        0     2617 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0        0        0     6909 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0        0        0     2765 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0        0        0     1431 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0        0        0     3755 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0        0        0     2291 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0        0        0     4389 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0        0        0     3601 2023-05-20 16:58:30.769641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0        0        0     3204 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0        0        0     1565 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0        0        0     6351 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0        0        0     3862 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/object.py
--rw-r--r--   0        0        0     1030 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/update.py
--rw-r--r--   0        0        0     3063 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0        0        0    33966 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0        0        0     2236 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0        0        0    22023 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0        0        0     5514 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0        0        0     4579 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0        0        0     4245 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0        0        0     1054 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0        0        0     2564 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0        0        0     9444 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0        0        0     3674 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0        0        0     4718 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0        0        0     3967 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0        0        0     2592 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0        0        0     5300 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0        0        0     2356 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0        0        0     2682 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0        0        0     2422 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0        0        0     4970 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0        0        0     1043 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0        0        0     1850 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0        0        0     1861 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0        0        0     1047 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0        0        0     1047 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0        0        0     1051 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     1951 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0        0        0     1329 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0        0        0     1293 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0        0        0     1663 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0        0        0    13658 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0        0        0     1691 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0        0        0     1346 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0        0        0     1610 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0        0        0     1531 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0        0        0     1043 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0        0        0    10911 2023-05-20 16:58:30.773641 pyrofork_dev-2.1.8.dev202305201658/pyrogram/utils.py
--rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 pyrofork_dev-2.1.8.dev202305201658/PKG-INFO
+-rw-r--r--   0        0        0     2155 2023-05-20 17:04:54.294236 pyrofork_dev-2.1.8.dev202305201705/README.md
+-rw-r--r--   0        0        0     1931 2023-05-20 17:05:48.442349 pyrofork_dev-2.1.8.dev202305201705/pyproject.toml
+-rw-r--r--   0        0        0     1446 2023-05-20 17:05:06.846305 pyrofork_dev-2.1.8.dev202305201705/pyrogram/__init__.py
+-rw-r--r--   0        0        0    40792 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/client.py
+-rw-r--r--   0        0        0      854 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/__init__.py
+-rw-r--r--   0        0        0     2830 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/connection.py
+-rw-r--r--   0        0        0      838 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/__init__.py
+-rw-r--r--   0        0        0     1044 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0        0        0     4100 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0        0        0     1768 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0        0        0     2830 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0        0        0     1906 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0        0        0     1511 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0        0        0     2453 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+-rw-r--r--   0        0        0      818 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/__init__.py
+-rw-r--r--   0        0        0     4013 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/aes.py
+-rw-r--r--   0        0        0     4767 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/mtproto.py
+-rw-r--r--   0        0        0     2446 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/prime.py
+-rw-r--r--   0        0        0    13437 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/rsa.py
+-rw-r--r--   0        0        0    10085 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/dispatcher.py
+-rw-r--r--   0        0        0   208021 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/emoji.py
+-rw-r--r--   0        0        0     1736 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/__init__.py
+-rw-r--r--   0        0        0     1002 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/auto_name.py
+-rw-r--r--   0        0        0     2307 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_action.py
+-rw-r--r--   0        0        0     4520 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0        0        0     1265 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0        0        0     1446 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0        0        0     1238 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_type.py
+-rw-r--r--   0        0        0     2464 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0        0        0     1599 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/message_media_type.py
+-rw-r--r--   0        0        0     2468 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/message_service_type.py
+-rw-r--r--   0        0        0     2406 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/messages_filter.py
+-rw-r--r--   0        0        0     1521 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/next_code_type.py
+-rw-r--r--   0        0        0     1188 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/parse_mode.py
+-rw-r--r--   0        0        0     1047 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/poll_type.py
+-rw-r--r--   0        0        0     1723 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0        0        0     1299 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/user_status.py
+-rw-r--r--   0        0        0     2489 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/__init__.py
+-rw-r--r--   0        0        0     1066 2023-05-20 17:05:48.434349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/__init__.py
+-rw-r--r--   0        0        0    25520 2023-05-20 17:05:48.438349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/all.py
+-rw-r--r--   0        0        0    64535 2023-05-20 17:05:48.438349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/bad_request_400.py
+-rw-r--r--   0        0        0     1941 2023-05-20 17:05:48.430349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/flood_420.py
+-rw-r--r--   0        0        0     6046 2023-05-20 17:05:48.430349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/forbidden_403.py
+-rw-r--r--   0        0        0    10644 2023-05-20 17:05:48.430349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/internal_server_error_500.py
+-rw-r--r--   0        0        0     3580 2023-05-20 17:05:48.434349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/not_acceptable_406.py
+-rw-r--r--   0        0        0     1952 2023-05-20 17:05:48.430349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/see_other_303.py
+-rw-r--r--   0        0        0     1351 2023-05-20 17:05:48.430349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/service_unavailable_503.py
+-rw-r--r--   0        0        0     2672 2023-05-20 17:05:48.434349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/unauthorized_401.py
+-rw-r--r--   0        0        0     3315 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/rpc_error.py
+-rw-r--r--   0        0        0    15154 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/file_id.py
+-rw-r--r--   0        0        0    24836 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/filters.py
+-rw-r--r--   0        0        0     1475 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0        0        0     2011 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0        0        0     2046 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0        0        0     2101 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0        0        0     2543 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0        0        0     1702 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0        0        0     1979 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0        0        0     1550 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/handler.py
+-rw-r--r--   0        0        0     1984 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0        0        0     1935 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/message_handler.py
+-rw-r--r--   0        0        0     1914 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0        0        0     2942 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0        0        0     1989 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/user_status_handler.py
+-rw-r--r--   0        0        0     1365 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/__init__.py
+-rw-r--r--   0        0        0      988 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0        0        0     3133 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0        0        0     4560 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0        0        0     8164 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/save_file.py
+-rw-r--r--   0        0        0     1655 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0        0        0     1468 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0        0        0     1942 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0        0        0     1749 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/connect.py
+-rw-r--r--   0        0        0     1504 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0        0        0     1307 2023-05-20 17:04:54.298236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0        0        0     1664 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0        0        0     1626 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0        0        0     1831 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0        0        0     2150 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0        0        0     2786 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0        0        0     1473 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0        0        0     3085 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0        0        0     2723 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0        0        0     2355 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0        0        0     1859 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/terminate.py
+-rw-r--r--   0        0        0     2041 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0        0        0     3311 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0        0        0     4990 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0        0        0     1989 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0        0        0     2360 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0        0        0     2573 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0        0        0     2051 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0        0        0     2319 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0        0        0     2798 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0        0        0     3365 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0        0        0     2847 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0        0        0     4191 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0        0        0     2886 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0        0        0     2710 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0        0        0     3186 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0        0        0     2048 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0        0        0     3946 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_game_score.py
+-rw-r--r--   0        0        0     4299 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0        0        0     3364 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0        0        0     2216 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0        0        0     4620 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0        0        0     1848 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0        0        0     1711 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0        0        0     1817 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0        0        0     2333 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0        0        0     2281 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0        0        0     1955 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0        0        0     1585 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0        0        0     2307 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0        0        0     1943 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0        0        0     1603 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0        0        0     1969 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0        0        0     2177 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0        0        0     1830 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0        0        0     3282 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0        0        0     4032 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0        0        0     3338 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0        0        0     5282 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0        0        0     2264 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0        0        0     1723 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0        0        0     3360 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0        0        0     2096 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0        0        0     2285 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0        0        0     3145 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0        0        0     2401 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0        0        0     2136 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0        0        0     1715 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0        0        0     2694 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0        0        0     2605 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0        0        0     1528 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0        0        0     3157 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0        0        0     3925 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0        0        0     1853 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0        0        0     1734 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0        0        0     4381 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0        0        0     3136 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0        0        0     2247 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0        0        0     3484 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0        0        0     4601 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0        0        0     1727 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0        0        0     2572 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0        0        0     2296 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0        0        0     1982 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0        0        0     2083 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0        0        0     2230 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0        0        0     2305 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0        0        0     1724 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0     2139 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unpin_chat_message.py
+-rw-r--r--   0        0        0     1154 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0        0        0     2566 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0        0        0     2448 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0        0        0     1605 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0        0        0     1422 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0        0        0     1934 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/import_contacts.py
+-rw-r--r--   0        0        0     1624 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0        0        0     2169 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0        0        0     2190 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0        0        0     2217 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0        0        0     2183 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0        0        0     1553 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0        0        0     2172 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0        0        0     2167 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0        0        0     2138 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0        0        0     2120 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0        0        0     1818 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0        0        0     2154 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_user_status.py
+-rw-r--r--   0        0        0     2435 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0        0        0     1894 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1924 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0        0        0     3369 2023-05-20 17:04:54.302236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0        0        0     1895 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0        0        0     1925 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0        0        0     2031 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     1751 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0        0        0     3533 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0        0        0     2582 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0        0        0     3566 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0        0        0     2335 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0        0        0     1997 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0        0        0     1925 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0        0        0     2928 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0        0        0     1929 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0        0        0     2947 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0        0        0     2329 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     3921 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0        0        0     5963 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0        0        0     5423 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0        0        0     3148 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0        0        0     7530 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0        0        0     2271 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0        0        0    10375 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0        0        0     2464 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0        0        0     3115 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0        0        0     2978 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0        0        0    13022 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0        0        0     2976 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0        0        0     3906 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0        0        0     4824 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0        0        0     4501 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0        0        0     2389 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0        0        0     1980 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0     2229 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0        0        0     2808 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0        0        0     1950 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0        0        0     2946 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0        0        0     4741 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0        0        0     2175 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0        0        0     2527 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0        0        0     2124 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0        0        0     4160 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0        0        0     2156 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0        0        0     5349 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0        0        0     3203 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0        0        0    12828 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0        0        0    11362 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0        0        0     5723 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0        0        0     3076 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0        0        0     5111 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0        0        0     5085 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0        0        0    10712 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0        0        0     4820 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0        0        0    20821 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0        0        0     7509 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0        0        0     9682 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0        0        0     8315 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0        0        0     2361 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0        0        0     8582 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0        0        0     5641 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0        0        0    12198 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0        0        0     9556 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0        0        0     9672 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0        0        0     2819 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0        0        0     3937 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0        0        0     2504 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/vote_poll.py
+-rw-r--r--   0        0        0     1088 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/__init__.py
+-rw-r--r--   0        0        0     2797 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0        0        0     3006 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0        0        0     2143 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/remove_cloud_password.py
+-rw-r--r--   0        0        0     1049 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0        0        0     2819 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0        0        0     4292 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0        0        0     1752 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/get_sticker_set.py
+-rw-r--r--   0        0        0     1659 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/__init__.py
+-rw-r--r--   0        0        0     1771 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/block_user.py
+-rw-r--r--   0        0        0     2237 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0        0        0     4421 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0        0        0     2509 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0        0        0     2359 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0        0        0     1664 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0        0        0     1565 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_me.py
+-rw-r--r--   0        0        0     2562 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_users.py
+-rw-r--r--   0        0        0     1882 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0        0        0     2718 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0        0        0     1876 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/set_username.py
+-rw-r--r--   0        0        0     1781 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0        0        0     2376 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/update_profile.py
+-rw-r--r--   0        0        0     1253 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0        0        0     2346 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0        0        0     2232 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0        0        0     1557 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0        0        0     2750 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0        0        0     2210 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0        0        0     2294 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0        0        0     2857 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/run.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/start.py
+-rw-r--r--   0        0        0     2117 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0        0        0     1724 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0        0        0    61915 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/mime_types.py
+-rw-r--r--   0        0        0      846 2023-05-20 17:04:54.306236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/__init__.py
+-rw-r--r--   0        0        0     8681 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/html.py
+-rw-r--r--   0        0        0     5770 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/markdown.py
+-rw-r--r--   0        0        0     2077 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/parser.py
+-rw-r--r--   0        0        0     1545 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/utils.py
+-rw-r--r--   0        0        0        0 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/py.typed
+-rw-r--r--   0        0        0     1040 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/__init__.py
+-rw-r--r--   0        0        0   105239 2023-05-20 17:05:48.398348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/all.py
+-rw-r--r--   0        0        0    14050 2023-05-20 17:05:48.378348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/__init__.py
+-rw-r--r--   0        0        0     1934 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/access_point_rule.py
+-rw-r--r--   0        0        0     2134 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/account_days_ttl.py
+-rw-r--r--   0        0        0     2158 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/app_web_view_result.py
+-rw-r--r--   0        0        0     1922 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bot.py
+-rw-r--r--   0        0        0     1947 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bot_icon.py
+-rw-r--r--   0        0        0     1978 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bot_icon_color.py
+-rw-r--r--   0        0        0     2215 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bots.py
+-rw-r--r--   0        0        0     2157 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bots_bot.py
+-rw-r--r--   0        0        0     2256 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_peer_type.py
+-rw-r--r--   0        0        0     2126 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/authorization.py
+-rw-r--r--   0        0        0     1964 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/auto_download_settings.py
+-rw-r--r--   0        0        0     1946 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/auto_save_exception.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/auto_save_settings.py
+-rw-r--r--   0        0        0     1945 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/available_reaction.py
+-rw-r--r--   0        0        0     2004 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bad_msg_notification.py
+-rw-r--r--   0        0        0     1935 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bank_card_open_url.py
+-rw-r--r--   0        0        0     2124 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/base_theme.py
+-rw-r--r--   0        0        0     1941 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bind_auth_key_inner.py
+-rw-r--r--   0        0        0     1939 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_app.py
+-rw-r--r--   0        0        0     2107 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_command.py
+-rw-r--r--   0        0        0     2363 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_command_scope.py
+-rw-r--r--   0        0        0     1885 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_info.py
+-rw-r--r--   0        0        0     2336 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_inline_message.py
+-rw-r--r--   0        0        0     2000 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_inline_result.py
+-rw-r--r--   0        0        0     2261 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_menu_button.py
+-rw-r--r--   0        0        0     2099 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/cdn_config.py
+-rw-r--r--   0        0        0     1916 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/cdn_public_key.py
+-rw-r--r--   0        0        0     1965 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_admin_log_event.py
+-rw-r--r--   0        0        0     6564 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_admin_log_event_action.py
+-rw-r--r--   0        0        0     2008 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_admin_log_events_filter.py
+-rw-r--r--   0        0        0     1999 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_location.py
+-rw-r--r--   0        0        0     2048 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_messages_filter.py
+-rw-r--r--   0        0        0     2309 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_participant.py
+-rw-r--r--   0        0        0     2524 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_participants_filter.py
+-rw-r--r--   0        0        0     2057 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat.py
+-rw-r--r--   0        0        0     1934 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_admin_rights.py
+-rw-r--r--   0        0        0     1965 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_admin_with_invites.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_banned_rights.py
+-rw-r--r--   0        0        0     1939 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_full.py
+-rw-r--r--   0        0        0     2225 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_invite.py
+-rw-r--r--   0        0        0     1952 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_invite_importer.py
+-rw-r--r--   0        0        0     2113 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_onlines.py
+-rw-r--r--   0        0        0     2068 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_participant.py
+-rw-r--r--   0        0        0     2015 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_participants.py
+-rw-r--r--   0        0        0     1951 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_photo.py
+-rw-r--r--   0        0        0     2046 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_reactions.py
+-rw-r--r--   0        0        0     1947 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/client_dh_inner_data.py
+-rw-r--r--   0        0        0     1915 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/code_settings.py
+-rw-r--r--   0        0        0     2077 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/config.py
+-rw-r--r--   0        0        0     1884 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/contact.py
+-rw-r--r--   0        0        0     2126 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/contact_status.py
+-rw-r--r--   0        0        0     2131 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/data_json.py
+-rw-r--r--   0        0        0     1891 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dc_option.py
+-rw-r--r--   0        0        0     2160 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/default_history_ttl.py
+-rw-r--r--   0        0        0     2267 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/destroy_auth_key_res.py
+-rw-r--r--   0        0        0     2205 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/destroy_session_res.py
+-rw-r--r--   0        0        0     1928 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog.py
+-rw-r--r--   0        0        0     2254 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog_filter.py
+-rw-r--r--   0        0        0     2189 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog_filter_suggested.py
+-rw-r--r--   0        0        0     2175 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog_peer.py
+-rw-r--r--   0        0        0     2266 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/document.py
+-rw-r--r--   0        0        0     2487 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/document_attribute.py
+-rw-r--r--   0        0        0     1975 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/draft_message.py
+-rw-r--r--   0        0        0     2094 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/email_verification.py
+-rw-r--r--   0        0        0     2133 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/email_verify_purpose.py
+-rw-r--r--   0        0        0     1903 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_group.py
+-rw-r--r--   0        0        0     1979 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_keyword.py
+-rw-r--r--   0        0        0     2241 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_keywords_difference.py
+-rw-r--r--   0        0        0     2140 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_language.py
+-rw-r--r--   0        0        0     2271 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_list.py
+-rw-r--r--   0        0        0     2024 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_status.py
+-rw-r--r--   0        0        0     2096 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_url.py
+-rw-r--r--   0        0        0     2436 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/encrypted_chat.py
+-rw-r--r--   0        0        0     2196 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/encrypted_file.py
+-rw-r--r--   0        0        0     2011 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/encrypted_message.py
+-rw-r--r--   0        0        0     1872 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/error.py
+-rw-r--r--   0        0        0     2244 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_chat_invite.py
+-rw-r--r--   0        0        0     2189 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_chatlist_invite.py
+-rw-r--r--   0        0        0     2176 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_contact_token.py
+-rw-r--r--   0        0        0     2169 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_message_link.py
+-rw-r--r--   0        0        0     2168 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/file_hash.py
+-rw-r--r--   0        0        0     1878 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/folder.py
+-rw-r--r--   0        0        0     1903 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/folder_peer.py
+-rw-r--r--   0        0        0     1963 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/forum_topic.py
+-rw-r--r--   0        0        0     1866 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/game.py
+-rw-r--r--   0        0        0     1943 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/geo_point.py
+-rw-r--r--   0        0        0     2233 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/global_privacy_settings.py
+-rw-r--r--   0        0        0     1959 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call.py
+-rw-r--r--   0        0        0     1964 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_participant.py
+-rw-r--r--   0        0        0     1995 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_participant_video.py
+-rw-r--r--   0        0        0     2063 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_participant_video_source_group.py
+-rw-r--r--   0        0        0     1977 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_stream_channel.py
+-rw-r--r--   0        0        0     1897 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/high_score.py
+-rw-r--r--   0        0        0     1891 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/http_wait.py
+-rw-r--r--   0        0        0     1933 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/imported_contact.py
+-rw-r--r--   0        0        0     1947 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/inline_bot_switch_pm.py
+-rw-r--r--   0        0        0     1941 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/inline_bot_web_view.py
+-rw-r--r--   0        0        0     2351 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/inline_query_peer_type.py
+-rw-r--r--   0        0        0     1922 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_app_event.py
+-rw-r--r--   0        0        0     1980 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_app.py
+-rw-r--r--   0        0        0     2492 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_inline_message.py
+-rw-r--r--   0        0        0     2060 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_inline_message_id.py
+-rw-r--r--   0        0        0     2195 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_inline_result.py
+-rw-r--r--   0        0        0     2046 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_channel.py
+-rw-r--r--   0        0        0     2061 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_chat_photo.py
+-rw-r--r--   0        0        0     1945 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_chatlist.py
+-rw-r--r--   0        0        0     2043 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_check_password_srp.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_client_proxy.py
+-rw-r--r--   0        0        0     1925 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_contact.py
+-rw-r--r--   0        0        0     2002 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_dialog_peer.py
+-rw-r--r--   0        0        0     1983 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_document.py
+-rw-r--r--   0        0        0     1952 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_encrypted_chat.py
+-rw-r--r--   0        0        0     2184 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_encrypted_file.py
+-rw-r--r--   0        0        0     1947 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_file.py
+-rw-r--r--   0        0        0     2601 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_file_location.py
+-rw-r--r--   0        0        0     1934 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_folder_peer.py
+-rw-r--r--   0        0        0     1963 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_game.py
+-rw-r--r--   0        0        0     1984 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_geo_point.py
+-rw-r--r--   0        0        0     1928 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_group_call.py
+-rw-r--r--   0        0        0     1987 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_invoice.py
+-rw-r--r--   0        0        0     2779 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_media.py
+-rw-r--r--   0        0        0     2119 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_message.py
+-rw-r--r--   0        0        0     2183 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_notify_peer.py
+-rw-r--r--   0        0        0     2240 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_payment_credentials.py
+-rw-r--r--   0        0        0     2270 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_peer.py
+-rw-r--r--   0        0        0     1983 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_peer_notify_settings.py
+-rw-r--r--   0        0        0     1928 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_phone_call.py
+-rw-r--r--   0        0        0     1959 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_photo.py
+-rw-r--r--   0        0        0     2571 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_privacy_key.py
+-rw-r--r--   0        0        0     2588 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_privacy_rule.py
+-rw-r--r--   0        0        0     2006 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_secure_file.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_secure_value.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_single_media.py
+-rw-r--r--   0        0        0     2695 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_sticker_set.py
+-rw-r--r--   0        0        0     1959 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_sticker_set_item.py
+-rw-r--r--   0        0        0     2048 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_stickered_media.py
+-rw-r--r--   0        0        0     2095 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_store_payment_purpose.py
+-rw-r--r--   0        0        0     1957 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_theme.py
+-rw-r--r--   0        0        0     1952 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_theme_settings.py
+-rw-r--r--   0        0        0     2067 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_user.py
+-rw-r--r--   0        0        0     2055 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_wall_paper.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_web_document.py
+-rw-r--r--   0        0        0     2142 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_web_file_location.py
+-rw-r--r--   0        0        0     1884 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/invoice.py
+-rw-r--r--   0        0        0     1929 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/ip_port.py
+-rw-r--r--   0        0        0     1934 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/json_object_value.py
+-rw-r--r--   0        0        0     2115 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/json_value.py
+-rw-r--r--   0        0        0     3020 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/keyboard_button.py
+-rw-r--r--   0        0        0     1946 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/keyboard_button_row.py
+-rw-r--r--   0        0        0     1915 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/labeled_price.py
+-rw-r--r--   0        0        0     2193 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/lang_pack_difference.py
+-rw-r--r--   0        0        0     2180 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/lang_pack_language.py
+-rw-r--r--   0        0        0     2273 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/lang_pack_string.py
+-rw-r--r--   0        0        0     1903 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/mask_coords.py
+-rw-r--r--   0        0        0     1987 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message.py
+-rw-r--r--   0        0        0     4917 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_action.py
+-rw-r--r--   0        0        0     3249 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_entity.py
+-rw-r--r--   0        0        0     2044 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_extended_media.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_fwd_header.py
+-rw-r--r--   0        0        0     2000 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_interaction_counters.py
+-rw-r--r--   0        0        0     2945 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_media.py
+-rw-r--r--   0        0        0     1958 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_peer_reaction.py
+-rw-r--r--   0        0        0     2123 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_range.py
+-rw-r--r--   0        0        0     1939 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_reactions.py
+-rw-r--r--   0        0        0     1927 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_replies.py
+-rw-r--r--   0        0        0     1952 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_reply_header.py
+-rw-r--r--   0        0        0     2083 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_user_vote.py
+-rw-r--r--   0        0        0     1915 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_views.py
+-rw-r--r--   0        0        0     3181 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/messages_filter.py
+-rw-r--r--   0        0        0     1996 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msg_detailed_info.py
+-rw-r--r--   0        0        0     1972 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msg_resend_req.py
+-rw-r--r--   0        0        0     1885 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_ack.py
+-rw-r--r--   0        0        0     1910 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_all_info.py
+-rw-r--r--   0        0        0     1922 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_state_info.py
+-rw-r--r--   0        0        0     1916 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_state_req.py
+-rw-r--r--   0        0        0     2099 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/nearest_dc.py
+-rw-r--r--   0        0        0     1917 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/new_session.py
+-rw-r--r--   0        0        0     2171 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/notification_sound.py
+-rw-r--r--   0        0        0     2112 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/notify_peer.py
+-rw-r--r--   0        0        0     1866 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/null.py
+-rw-r--r--   0        0        0     1866 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page.py
+-rw-r--r--   0        0        0     3535 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_block.py
+-rw-r--r--   0        0        0     1909 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_caption.py
+-rw-r--r--   0        0        0     1986 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_list_item.py
+-rw-r--r--   0        0        0     2043 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_list_ordered_item.py
+-rw-r--r--   0        0        0     1952 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_related_article.py
+-rw-r--r--   0        0        0     1922 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_table_cell.py
+-rw-r--r--   0        0        0     1916 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_table_row.py
+-rw-r--r--   0        0        0     2104 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/password_kdf_algo.py
+-rw-r--r--   0        0        0     1921 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_charge.py
+-rw-r--r--   0        0        0     1946 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_form_method.py
+-rw-r--r--   0        0        0     1964 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_requested_info.py
+-rw-r--r--   0        0        0     1990 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_saved_credentials.py
+-rw-r--r--   0        0        0     2185 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer.py
+-rw-r--r--   0        0        0     1909 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_blocked.py
+-rw-r--r--   0        0        0     1965 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_located.py
+-rw-r--r--   0        0        0     2162 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_notify_settings.py
+-rw-r--r--   0        0        0     1915 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_settings.py
+-rw-r--r--   0        0        0     2189 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_call.py
+-rw-r--r--   0        0        0     2237 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_call_discard_reason.py
+-rw-r--r--   0        0        0     1946 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_call_protocol.py
+-rw-r--r--   0        0        0     2001 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_connection.py
+-rw-r--r--   0        0        0     1918 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/photo.py
+-rw-r--r--   0        0        0     2181 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/photo_size.py
+-rw-r--r--   0        0        0     1866 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll.py
+-rw-r--r--   0        0        0     1903 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll_answer.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll_answer_voters.py
+-rw-r--r--   0        0        0     1909 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll_results.py
+-rw-r--r--   0        0        0     2088 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/pong.py
+-rw-r--r--   0        0        0     1927 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/popular_contact.py
+-rw-r--r--   0        0        0     1909 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/post_address.py
+-rw-r--r--   0        0        0     2076 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/pq_inner_data.py
+-rw-r--r--   0        0        0     1946 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/premium_gift_option.py
+-rw-r--r--   0        0        0     1994 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/premium_subscription_option.py
+-rw-r--r--   0        0        0     2460 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/privacy_key.py
+-rw-r--r--   0        0        0     2487 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/privacy_rule.py
+-rw-r--r--   0        0        0     2015 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/reaction.py
+-rw-r--r--   0        0        0     1921 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/reaction_count.py
+-rw-r--r--   0        0        0     2178 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/read_participant_date.py
+-rw-r--r--   0        0        0     2180 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/received_notify_message.py
+-rw-r--r--   0        0        0     2169 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/recent_me_url.py
+-rw-r--r--   0        0        0     2115 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/reply_markup.py
+-rw-r--r--   0        0        0     2640 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/report_reason.py
+-rw-r--r--   0        0        0     2079 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/request_peer_type.py
+-rw-r--r--   0        0        0     2087 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/res_pq.py
+-rw-r--r--   0        0        0     1945 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/restriction_reason.py
+-rw-r--r--   0        0        0     2572 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rich_text.py
+-rw-r--r--   0        0        0     2255 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rpc_drop_answer.py
+-rw-r--r--   0        0        0     1891 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rpc_error.py
+-rw-r--r--   0        0        0     1897 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rpc_result.py
+-rw-r--r--   0        0        0     2127 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/saved_contact.py
+-rw-r--r--   0        0        0     2007 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/search_results_calendar_period.py
+-rw-r--r--   0        0        0     1968 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/search_results_position.py
+-rw-r--r--   0        0        0     2000 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_credentials_encrypted.py
+-rw-r--r--   0        0        0     1903 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_data.py
+-rw-r--r--   0        0        0     1959 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_file.py
+-rw-r--r--   0        0        0     2184 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_password_kdf_algo.py
+-rw-r--r--   0        0        0     1994 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_plain_data.py
+-rw-r--r--   0        0        0     2024 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_required_type.py
+-rw-r--r--   0        0        0     1964 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_secret_settings.py
+-rw-r--r--   0        0        0     2192 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value.py
+-rw-r--r--   0        0        0     2537 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value_error.py
+-rw-r--r--   0        0        0     1934 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value_hash.py
+-rw-r--r--   0        0        0     2918 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value_type.py
+-rw-r--r--   0        0        0     1904 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/send_as_peer.py
+-rw-r--r--   0        0        0     3337 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/send_message_action.py
+-rw-r--r--   0        0        0     1947 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/server_dh_inner_data.py
+-rw-r--r--   0        0        0     2190 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/server_dh_params.py
+-rw-r--r--   0        0        0     2243 2023-05-20 17:05:48.114348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/set_client_dh_params_answer.py
+-rw-r--r--   0        0        0     1927 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/shipping_option.py
+-rw-r--r--   0        0        0     2179 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/simple_web_view_result.py
+-rw-r--r--   0        0        0     1939 2023-05-20 17:05:48.150348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sponsored_message.py
+-rw-r--r--   0        0        0     1966 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_abs_value_and_prev.py
+-rw-r--r--   0        0        0     1953 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_date_range_days.py
+-rw-r--r--   0        0        0     2219 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_graph.py
+-rw-r--r--   0        0        0     1953 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_group_top_admin.py
+-rw-r--r--   0        0        0     1965 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_group_top_inviter.py
+-rw-r--r--   0        0        0     1959 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_group_top_poster.py
+-rw-r--r--   0        0        0     1946 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_percent_value.py
+-rw-r--r--   0        0        0     1891 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_url.py
+-rw-r--r--   0        0        0     1927 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_keyword.py
+-rw-r--r--   0        0        0     1909 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_pack.py
+-rw-r--r--   0        0        0     1903 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_set.py
+-rw-r--r--   0        0        0     2359 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_set_covered.py
+-rw-r--r--   0        0        0     1940 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/text_with_entities.py
+-rw-r--r--   0        0        0     2138 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/theme.py
+-rw-r--r--   0        0        0     1921 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/theme_settings.py
+-rw-r--r--   0        0        0     1885 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/top_peer.py
+-rw-r--r--   0        0        0     2476 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/top_peer_category.py
+-rw-r--r--   0        0        0     1965 2023-05-20 17:05:48.130348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/top_peer_category_peers.py
+-rw-r--r--   0        0        0     9329 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/update.py
+-rw-r--r--   0        0        0     5681 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/updates_t.py
+-rw-r--r--   0        0        0     2313 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/url_auth_result.py
+-rw-r--r--   0        0        0     2251 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user.py
+-rw-r--r--   0        0        0     1891 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user_full.py
+-rw-r--r--   0        0        0     2008 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user_profile_photo.py
+-rw-r--r--   0        0        0     2215 2023-05-20 17:05:48.118348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user_status.py
+-rw-r--r--   0        0        0     1890 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/username.py
+-rw-r--r--   0        0        0     2032 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/video_size.py
+-rw-r--r--   0        0        0     2234 2023-05-20 17:05:48.122348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/wall_paper.py
+-rw-r--r--   0        0        0     1946 2023-05-20 17:05:48.142348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/wall_paper_settings.py
+-rw-r--r--   0        0        0     1939 2023-05-20 17:05:48.138348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_authorization.py
+-rw-r--r--   0        0        0     1971 2023-05-20 17:05:48.134348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_document.py
+-rw-r--r--   0        0        0     2253 2023-05-20 17:05:48.126348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_page.py
+-rw-r--r--   0        0        0     1950 2023-05-20 17:05:48.146348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_page_attribute.py
+-rw-r--r--   0        0        0     2171 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_view_message_sent.py
+-rw-r--r--   0        0        0     2136 2023-05-20 17:05:48.154348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_view_result.py
+-rw-r--r--   0        0        0     1312 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/__init__.py
+-rw-r--r--   0        0        0     1692 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0        0        0     1891 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0        0        0     1814 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0        0        0     1048 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/list.py
+-rw-r--r--   0        0        0     1851 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/message.py
+-rw-r--r--   0        0        0     1614 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/msg_container.py
+-rw-r--r--   0        0        0     1012 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0        0        0     1497 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0        0        0     1759 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0        0        0     1193 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0        0        0     1358 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0        0        0     1194 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0        0        0     2022 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0        0        0     2495 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/tl_object.py
+-rw-r--r--   0        0        0     1998 2023-05-20 17:05:48.394348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/__init__.py
+-rw-r--r--   0        0        0     2010 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/destroy_auth_key.py
+-rw-r--r--   0        0        0     2211 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/destroy_session.py
+-rw-r--r--   0        0        0     2133 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/get_future_salts.py
+-rw-r--r--   0        0        0     4863 2023-05-20 17:05:48.314348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/init_connection.py
+-rw-r--r--   0        0        0     2397 2023-05-20 17:05:48.314348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_after_msg.py
+-rw-r--r--   0        0        0     2450 2023-05-20 17:05:48.314348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_after_msgs.py
+-rw-r--r--   0        0        0     2389 2023-05-20 17:05:48.314348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_with_layer.py
+-rw-r--r--   0        0        0     2492 2023-05-20 17:05:48.314348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_with_messages_range.py
+-rw-r--r--   0        0        0     2445 2023-05-20 17:05:48.314348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_with_takeout.py
+-rw-r--r--   0        0        0     2209 2023-05-20 17:05:48.314348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_without_updates.py
+-rw-r--r--   0        0        0     2118 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/ping.py
+-rw-r--r--   0        0        0     2477 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/ping_delay_disconnect.py
+-rw-r--r--   0        0        0     3390 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/req_dh_params.py
+-rw-r--r--   0        0        0     2113 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/req_pq.py
+-rw-r--r--   0        0        0     2133 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/req_pq_multi.py
+-rw-r--r--   0        0        0     2199 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/rpc_drop_answer.py
+-rw-r--r--   0        0        0     2750 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/set_client_dh_params.py
+-rw-r--r--   0        0        0    56200 2023-05-20 17:05:48.390349 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/access_point_rule.py
+-rw-r--r--   0        0        0     2329 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/account_days_ttl.py
+-rw-r--r--   0        0        0     2345 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/app_web_view_result_url.py
+-rw-r--r--   0        0        0     4075 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bot.py
+-rw-r--r--   0        0        0     2923 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bot_icon.py
+-rw-r--r--   0        0        0     2362 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bot_icon_color.py
+-rw-r--r--   0        0        0     2886 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bots.py
+-rw-r--r--   0        0        0     2675 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bots_bot.py
+-rw-r--r--   0        0        0     2234 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bots_not_modified.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_bot_pm.py
+-rw-r--r--   0        0        0     2036 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_broadcast.py
+-rw-r--r--   0        0        0     2014 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_chat.py
+-rw-r--r--   0        0        0     2008 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_pm.py
+-rw-r--r--   0        0        0     2036 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_same_bot_pm.py
+-rw-r--r--   0        0        0     6710 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/authorization.py
+-rw-r--r--   0        0        0     4611 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/auto_download_settings.py
+-rw-r--r--   0        0        0     2492 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/auto_save_exception.py
+-rw-r--r--   0        0        0     2962 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/auto_save_settings.py
+-rw-r--r--   0        0        0     5709 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/available_reaction.py
+-rw-r--r--   0        0        0     2718 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bad_msg_notification.py
+-rw-r--r--   0        0        0     2991 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bad_server_salt.py
+-rw-r--r--   0        0        0     2307 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bank_card_open_url.py
+-rw-r--r--   0        0        0     1979 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_arctic.py
+-rw-r--r--   0        0        0     1983 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_classic.py
+-rw-r--r--   0        0        0     1967 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_day.py
+-rw-r--r--   0        0        0     1975 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_night.py
+-rw-r--r--   0        0        0     1979 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_tinted.py
+-rw-r--r--   0        0        0     3288 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bind_auth_key_inner.py
+-rw-r--r--   0        0        0     3944 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_app.py
+-rw-r--r--   0        0        0     1984 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_app_not_modified.py
+-rw-r--r--   0        0        0     2584 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command.py
+-rw-r--r--   0        0        0     2025 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_chat_admins.py
+-rw-r--r--   0        0        0     2005 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_chats.py
+-rw-r--r--   0        0        0     2013 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_default.py
+-rw-r--r--   0        0        0     2204 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_peer.py
+-rw-r--r--   0        0        0     2228 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_peer_admins.py
+-rw-r--r--   0        0        0     2495 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_peer_user.py
+-rw-r--r--   0        0        0     2005 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_users.py
+-rw-r--r--   0        0        0     4814 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_info.py
+-rw-r--r--   0        0        0     4328 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_media_result.py
+-rw-r--r--   0        0        0     3220 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_auto.py
+-rw-r--r--   0        0        0     3471 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_contact.py
+-rw-r--r--   0        0        0     4119 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_geo.py
+-rw-r--r--   0        0        0     4576 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_invoice.py
+-rw-r--r--   0        0        0     3871 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_venue.py
+-rw-r--r--   0        0        0     3494 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_text.py
+-rw-r--r--   0        0        0     4665 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_result.py
+-rw-r--r--   0        0        0     2502 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_menu_button.py
+-rw-r--r--   0        0        0     2212 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_menu_button_commands.py
+-rw-r--r--   0        0        0     2208 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_menu_button_default.py
+-rw-r--r--   0        0        0     2456 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/cdn_config.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/cdn_public_key.py
+-rw-r--r--   0        0        0    12591 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel.py
+-rw-r--r--   0        0        0     2887 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event.py
+-rw-r--r--   0        0        0     2514 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_about.py
+-rw-r--r--   0        0        0     2720 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_available_reactions.py
+-rw-r--r--   0        0        0     2538 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_history_ttl.py
+-rw-r--r--   0        0        0     2542 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_linked_chat.py
+-rw-r--r--   0        0        0     2694 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_location.py
+-rw-r--r--   0        0        0     2604 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_photo.py
+-rw-r--r--   0        0        0     2794 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_sticker_set.py
+-rw-r--r--   0        0        0     2514 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_title.py
+-rw-r--r--   0        0        0     2526 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_username.py
+-rw-r--r--   0        0        0     2610 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_usernames.py
+-rw-r--r--   0        0        0     2300 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_create_topic.py
+-rw-r--r--   0        0        0     2868 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_default_banned_rights.py
+-rw-r--r--   0        0        0     2314 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_delete_message.py
+-rw-r--r--   0        0        0     2300 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_delete_topic.py
+-rw-r--r--   0        0        0     2327 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_discard_group_call.py
+-rw-r--r--   0        0        0     2656 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_edit_message.py
+-rw-r--r--   0        0        0     2636 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_edit_topic.py
+-rw-r--r--   0        0        0     2377 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_delete.py
+-rw-r--r--   0        0        0     2754 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_edit.py
+-rw-r--r--   0        0        0     2377 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_revoke.py
+-rw-r--r--   0        0        0     2410 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_invite.py
+-rw-r--r--   0        0        0     2100 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_join.py
+-rw-r--r--   0        0        0     2746 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_invite.py
+-rw-r--r--   0        0        0     2650 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_request.py
+-rw-r--r--   0        0        0     2104 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_leave.py
+-rw-r--r--   0        0        0     2410 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_mute.py
+-rw-r--r--   0        0        0     2860 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_admin.py
+-rw-r--r--   0        0        0     2852 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_ban.py
+-rw-r--r--   0        0        0     2418 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_unmute.py
+-rw-r--r--   0        0        0     2418 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_volume.py
+-rw-r--r--   0        0        0     3005 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_pin_topic.py
+-rw-r--r--   0        0        0     2306 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_send_message.py
+-rw-r--r--   0        0        0     2319 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_start_group_call.py
+-rw-r--r--   0        0        0     2294 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_stop_poll.py
+-rw-r--r--   0        0        0     2279 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_anti_spam.py
+-rw-r--r--   0        0        0     2265 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_forum.py
+-rw-r--r--   0        0        0     2320 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_group_call_setting.py
+-rw-r--r--   0        0        0     2275 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_invites.py
+-rw-r--r--   0        0        0     2287 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_no_forwards.py
+-rw-r--r--   0        0        0     2311 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_pre_history_hidden.py
+-rw-r--r--   0        0        0     2287 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_signatures.py
+-rw-r--r--   0        0        0     2530 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_slow_mode.py
+-rw-r--r--   0        0        0     2310 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_update_pinned.py
+-rw-r--r--   0        0        0     6648 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_events_filter.py
+-rw-r--r--   0        0        0     3591 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_forbidden.py
+-rw-r--r--   0        0        0    21188 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_full.py
+-rw-r--r--   0        0        0     2445 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_location.py
+-rw-r--r--   0        0        0     2005 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_location_empty.py
+-rw-r--r--   0        0        0     2699 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_messages_filter.py
+-rw-r--r--   0        0        0     2035 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_messages_filter_empty.py
+-rw-r--r--   0        0        0     2365 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant.py
+-rw-r--r--   0        0        0     4333 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_admin.py
+-rw-r--r--   0        0        0     3281 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_banned.py
+-rw-r--r--   0        0        0     2936 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_creator.py
+-rw-r--r--   0        0        0     2199 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_left.py
+-rw-r--r--   0        0        0     2977 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_self.py
+-rw-r--r--   0        0        0     2035 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_admins.py
+-rw-r--r--   0        0        0     2150 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_banned.py
+-rw-r--r--   0        0        0     2027 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_bots.py
+-rw-r--r--   0        0        0     2158 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_contacts.py
+-rw-r--r--   0        0        0     2150 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_kicked.py
+-rw-r--r--   0        0        0     2762 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_mentions.py
+-rw-r--r--   0        0        0     2035 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_recent.py
+-rw-r--r--   0        0        0     2148 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_search.py
+-rw-r--r--   0        0        0     6664 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat.py
+-rw-r--r--   0        0        0     5640 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_admin_rights.py
+-rw-r--r--   0        0        0     2809 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_admin_with_invites.py
+-rw-r--r--   0        0        0     8389 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_banned_rights.py
+-rw-r--r--   0        0        0     2079 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_empty.py
+-rw-r--r--   0        0        0     2293 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_forbidden.py
+-rw-r--r--   0        0        0     9951 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_full.py
+-rw-r--r--   0        0        0     5192 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite.py
+-rw-r--r--   0        0        0     2379 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_already.py
+-rw-r--r--   0        0        0     6062 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_exported.py
+-rw-r--r--   0        0        0     3786 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_importer.py
+-rw-r--r--   0        0        0     2585 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_peek.py
+-rw-r--r--   0        0        0     2249 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_public_join_requests.py
+-rw-r--r--   0        0        0     2339 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_onlines.py
+-rw-r--r--   0        0        0     2598 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participant.py
+-rw-r--r--   0        0        0     2618 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participant_admin.py
+-rw-r--r--   0        0        0     2187 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participant_creator.py
+-rw-r--r--   0        0        0     2750 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participants.py
+-rw-r--r--   0        0        0     2804 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participants_forbidden.py
+-rw-r--r--   0        0        0     3122 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_photo.py
+-rw-r--r--   0        0        0     1975 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_photo_empty.py
+-rw-r--r--   0        0        0     2297 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_reactions_all.py
+-rw-r--r--   0        0        0     1991 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_reactions_none.py
+-rw-r--r--   0        0        0     2257 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_reactions_some.py
+-rw-r--r--   0        0        0     2842 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/client_dh_inner_data.py
+-rw-r--r--   0        0        0     4902 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/code_settings.py
+-rw-r--r--   0        0        0    19235 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/config.py
+-rw-r--r--   0        0        0     2322 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/contact.py
+-rw-r--r--   0        0        0     2625 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/contact_status.py
+-rw-r--r--   0        0        0     2331 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/data_json.py
+-rw-r--r--   0        0        0     4562 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dc_option.py
+-rw-r--r--   0        0        0     2370 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/default_history_ttl.py
+-rw-r--r--   0        0        0     2197 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_auth_key_fail.py
+-rw-r--r--   0        0        0     2197 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_auth_key_none.py
+-rw-r--r--   0        0        0     2189 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_auth_key_ok.py
+-rw-r--r--   0        0        0     2398 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_session_none.py
+-rw-r--r--   0        0        0     2390 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_session_ok.py
+-rw-r--r--   0        0        0     2906 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dh_gen_fail.py
+-rw-r--r--   0        0        0     2898 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dh_gen_ok.py
+-rw-r--r--   0        0        0     2910 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dh_gen_retry.py
+-rw-r--r--   0        0        0     6524 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog.py
+-rw-r--r--   0        0        0     6358 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter.py
+-rw-r--r--   0        0        0     4000 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter_chatlist.py
+-rw-r--r--   0        0        0     2207 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter_default.py
+-rw-r--r--   0        0        0     2718 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter_suggested.py
+-rw-r--r--   0        0        0     4534 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_folder.py
+-rw-r--r--   0        0        0     2356 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_peer.py
+-rw-r--r--   0        0        0     2386 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_peer_folder.py
+-rw-r--r--   0        0        0     5113 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document.py
+-rw-r--r--   0        0        0     2027 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_animated.py
+-rw-r--r--   0        0        0     3632 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_audio.py
+-rw-r--r--   0        0        0     3079 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_custom_emoji.py
+-rw-r--r--   0        0        0     2214 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_filename.py
+-rw-r--r--   0        0        0     2039 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_has_stickers.py
+-rw-r--r--   0        0        0     2312 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_image_size.py
+-rw-r--r--   0        0        0     3253 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_sticker.py
+-rw-r--r--   0        0        0     3253 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_video.py
+-rw-r--r--   0        0        0     2422 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_empty.py
+-rw-r--r--   0        0        0     3616 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/draft_message.py
+-rw-r--r--   0        0        0     2333 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/draft_message_empty.py
+-rw-r--r--   0        0        0     2166 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verification_apple.py
+-rw-r--r--   0        0        0     2153 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verification_code.py
+-rw-r--r--   0        0        0     2170 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verification_google.py
+-rw-r--r--   0        0        0     2044 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verify_purpose_login_change.py
+-rw-r--r--   0        0        0     2542 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verify_purpose_login_setup.py
+-rw-r--r--   0        0        0     2032 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verify_purpose_passport.py
+-rw-r--r--   0        0        0     2660 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_group.py
+-rw-r--r--   0        0        0     2413 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_keyword.py
+-rw-r--r--   0        0        0     2441 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_keyword_deleted.py
+-rw-r--r--   0        0        0     3271 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_keywords_difference.py
+-rw-r--r--   0        0        0     2380 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_language.py
+-rw-r--r--   0        0        0     2706 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_list.py
+-rw-r--r--   0        0        0     2306 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_list_not_modified.py
+-rw-r--r--   0        0        0     2175 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_status.py
+-rw-r--r--   0        0        0     1985 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_status_empty.py
+-rw-r--r--   0        0        0     2395 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_status_until.py
+-rw-r--r--   0        0        0     2287 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_url.py
+-rw-r--r--   0        0        0     3831 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat.py
+-rw-r--r--   0        0        0     2770 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_discarded.py
+-rw-r--r--   0        0        0     2370 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_empty.py
+-rw-r--r--   0        0        0     3974 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_requested.py
+-rw-r--r--   0        0        0     3340 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_waiting.py
+-rw-r--r--   0        0        0     3257 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_file.py
+-rw-r--r--   0        0        0     2207 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_file_empty.py
+-rw-r--r--   0        0        0     3056 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_message.py
+-rw-r--r--   0        0        0     2818 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_message_service.py
+-rw-r--r--   0        0        0     2268 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/error.py
+-rw-r--r--   0        0        0     2876 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/exported_chatlist_invite.py
+-rw-r--r--   0        0        0     2572 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/exported_contact_token.py
+-rw-r--r--   0        0        0     2546 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/exported_message_link.py
+-rw-r--r--   0        0        0     2781 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/file_hash.py
+-rw-r--r--   0        0        0     3983 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/folder.py
+-rw-r--r--   0        0        0     2379 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/folder_peer.py
+-rw-r--r--   0        0        0     7364 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/forum_topic.py
+-rw-r--r--   0        0        0     2112 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/forum_topic_deleted.py
+-rw-r--r--   0        0        0     3740 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/game.py
+-rw-r--r--   0        0        0     3070 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/geo_point.py
+-rw-r--r--   0        0        0     1970 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/geo_point_empty.py
+-rw-r--r--   0        0        0     2977 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/global_privacy_settings.py
+-rw-r--r--   0        0        0     8290 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call.py
+-rw-r--r--   0        0        0     2604 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_discarded.py
+-rw-r--r--   0        0        0     8200 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_participant.py
+-rw-r--r--   0        0        0     3410 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_participant_video.py
+-rw-r--r--   0        0        0     2535 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_participant_video_source_group.py
+-rw-r--r--   0        0        0     2702 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_stream_channel.py
+-rw-r--r--   0        0        0     2511 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/high_score.py
+-rw-r--r--   0        0        0     2611 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/http_wait.py
+-rw-r--r--   0        0        0     2398 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/imported_contact.py
+-rw-r--r--   0        0        0     2389 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_bot_switch_pm.py
+-rw-r--r--   0        0        0     2312 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_bot_web_view.py
+-rw-r--r--   0        0        0     2023 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_bot_pm.py
+-rw-r--r--   0        0        0     2041 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_broadcast.py
+-rw-r--r--   0        0        0     2021 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_chat.py
+-rw-r--r--   0        0        0     2041 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_megagroup.py
+-rw-r--r--   0        0        0     2013 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_pm.py
+-rw-r--r--   0        0        0     2041 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_same_bot_pm.py
+-rw-r--r--   0        0        0     2765 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_app_event.py
+-rw-r--r--   0        0        0     2359 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_app_id.py
+-rw-r--r--   0        0        0     2465 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_app_short_name.py
+-rw-r--r--   0        0        0     2528 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_game.py
+-rw-r--r--   0        0        0     2611 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_id.py
+-rw-r--r--   0        0        0     2846 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_id64.py
+-rw-r--r--   0        0        0     3245 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_auto.py
+-rw-r--r--   0        0        0     3496 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_contact.py
+-rw-r--r--   0        0        0     4220 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_geo.py
+-rw-r--r--   0        0        0     4490 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_invoice.py
+-rw-r--r--   0        0        0     3970 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_venue.py
+-rw-r--r--   0        0        0     3519 2023-05-20 17:05:48.238348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_text.py
+-rw-r--r--   0        0        0     4750 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result.py
+-rw-r--r--   0        0        0     3846 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result_document.py
+-rw-r--r--   0        0        0     2763 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result_game.py
+-rw-r--r--   0        0        0     2976 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result_photo.py
+-rw-r--r--   0        0        0     2428 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_channel.py
+-rw-r--r--   0        0        0     1990 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_channel_empty.py
+-rw-r--r--   0        0        0     2674 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_channel_from_message.py
+-rw-r--r--   0        0        0     2169 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chat_photo.py
+-rw-r--r--   0        0        0     2000 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chat_photo_empty.py
+-rw-r--r--   0        0        0     3852 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chat_uploaded_photo.py
+-rw-r--r--   0        0        0     2212 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chatlist_dialog_filter.py
+-rw-r--r--   0        0        0     2023 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_check_password_empty.py
+-rw-r--r--   0        0        0     2515 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_check_password_srp.py
+-rw-r--r--   0        0        0     2350 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_client_proxy.py
+-rw-r--r--   0        0        0     2188 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_dialog_peer.py
+-rw-r--r--   0        0        0     2198 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_dialog_peer_folder.py
+-rw-r--r--   0        0        0     2641 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_document.py
+-rw-r--r--   0        0        0     1995 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_document_empty.py
+-rw-r--r--   0        0        0     2936 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_document_file_location.py
+-rw-r--r--   0        0        0     2428 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_chat.py
+-rw-r--r--   0        0        0     2386 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file.py
+-rw-r--r--   0        0        0     2663 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_big_uploaded.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_empty.py
+-rw-r--r--   0        0        0     2417 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_location.py
+-rw-r--r--   0        0        0     2912 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_uploaded.py
+-rw-r--r--   0        0        0     2734 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_file.py
+-rw-r--r--   0        0        0     2485 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_file_big.py
+-rw-r--r--   0        0        0     2906 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_file_location.py
+-rw-r--r--   0        0        0     2424 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_folder_peer.py
+-rw-r--r--   0        0        0     2347 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_game_id.py
+-rw-r--r--   0        0        0     2455 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_game_short_name.py
+-rw-r--r--   0        0        0     2838 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_geo_point.py
+-rw-r--r--   0        0        0     1995 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_geo_point_empty.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_group_call.py
+-rw-r--r--   0        0        0     3582 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_group_call_stream.py
+-rw-r--r--   0        0        0     2410 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_invoice_message.py
+-rw-r--r--   0        0        0     2128 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_invoice_slug.py
+-rw-r--r--   0        0        0     3407 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_keyboard_button_url_auth.py
+-rw-r--r--   0        0        0     2463 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_keyboard_button_user_profile.py
+-rw-r--r--   0        0        0     2877 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_contact.py
+-rw-r--r--   0        0        0     2154 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_dice.py
+-rw-r--r--   0        0        0     3281 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_document.py
+-rw-r--r--   0        0        0     2891 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_document_external.py
+-rw-r--r--   0        0        0     1980 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_empty.py
+-rw-r--r--   0        0        0     2161 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_game.py
+-rw-r--r--   0        0        0     3929 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_geo_live.py
+-rw-r--r--   0        0        0     2256 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_geo_point.py
+-rw-r--r--   0        0        0     4853 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_invoice.py
+-rw-r--r--   0        0        0     2903 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_photo.py
+-rw-r--r--   0        0        0     2879 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_photo_external.py
+-rw-r--r--   0        0        0     3669 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_poll.py
+-rw-r--r--   0        0        0     5063 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_uploaded_document.py
+-rw-r--r--   0        0        0     3430 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_uploaded_photo.py
+-rw-r--r--   0        0        0     3351 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_venue.py
+-rw-r--r--   0        0        0     2378 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_callback_query.py
+-rw-r--r--   0        0        0     2687 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_entity_mention_name.py
+-rw-r--r--   0        0        0     2104 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_id.py
+-rw-r--r--   0        0        0     1994 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_pinned.py
+-rw-r--r--   0        0        0     2124 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_reply_to.py
+-rw-r--r--   0        0        0     2040 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_chat_photos.py
+-rw-r--r--   0        0        0     2032 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_contacts.py
+-rw-r--r--   0        0        0     2032 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_document.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_empty.py
+-rw-r--r--   0        0        0     2012 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_geo.py
+-rw-r--r--   0        0        0     2012 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_gif.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_music.py
+-rw-r--r--   0        0        0     2040 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_my_mentions.py
+-rw-r--r--   0        0        0     2296 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_phone_calls.py
+-rw-r--r--   0        0        0     2040 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_photo_video.py
+-rw-r--r--   0        0        0     2024 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_photos.py
+-rw-r--r--   0        0        0     2024 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_pinned.py
+-rw-r--r--   0        0        0     2040 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_round_video.py
+-rw-r--r--   0        0        0     2040 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_round_voice.py
+-rw-r--r--   0        0        0     2012 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_url.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_video.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_voice.py
+-rw-r--r--   0        0        0     2009 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_broadcasts.py
+-rw-r--r--   0        0        0     1989 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_chats.py
+-rw-r--r--   0        0        0     2457 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_forum_topic.py
+-rw-r--r--   0        0        0     2188 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_peer.py
+-rw-r--r--   0        0        0     1989 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_users.py
+-rw-r--r--   0        0        0     2509 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials.py
+-rw-r--r--   0        0        0     2326 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials_apple_pay.py
+-rw-r--r--   0        0        0     2341 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials_google_pay.py
+-rw-r--r--   0        0        0     2431 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials_saved.py
+-rw-r--r--   0        0        0     2441 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_channel.py
+-rw-r--r--   0        0        0     2687 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_channel_from_message.py
+-rw-r--r--   0        0        0     2145 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_chat.py
+-rw-r--r--   0        0        0     1975 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_empty.py
+-rw-r--r--   0        0        0     3679 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_notify_settings.py
+-rw-r--r--   0        0        0     2740 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_photo_file_location.py
+-rw-r--r--   0        0        0     1971 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_self.py
+-rw-r--r--   0        0        0     2402 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_user.py
+-rw-r--r--   0        0        0     2648 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_user_from_message.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_phone_call.py
+-rw-r--r--   0        0        0     2857 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_phone_contact.py
+-rw-r--r--   0        0        0     2626 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo.py
+-rw-r--r--   0        0        0     1980 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo_empty.py
+-rw-r--r--   0        0        0     2924 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo_file_location.py
+-rw-r--r--   0        0        0     3383 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo_legacy_file_location.py
+-rw-r--r--   0        0        0     2033 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_added_by_phone.py
+-rw-r--r--   0        0        0     2025 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_chat_invite.py
+-rw-r--r--   0        0        0     2017 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_forwards.py
+-rw-r--r--   0        0        0     2021 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_phone_call.py
+-rw-r--r--   0        0        0     2027 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_phone_number.py
+-rw-r--r--   0        0        0     2017 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_phone_p2_p.py
+-rw-r--r--   0        0        0     2033 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_profile_photo.py
+-rw-r--r--   0        0        0     2045 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_status_timestamp.py
+-rw-r--r--   0        0        0     2037 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_voice_messages.py
+-rw-r--r--   0        0        0     2026 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_all.py
+-rw-r--r--   0        0        0     2274 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_chat_participants.py
+-rw-r--r--   0        0        0     2044 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_contacts.py
+-rw-r--r--   0        0        0     2268 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_users.py
+-rw-r--r--   0        0        0     2038 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_all.py
+-rw-r--r--   0        0        0     2286 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_chat_participants.py
+-rw-r--r--   0        0        0     2056 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_contacts.py
+-rw-r--r--   0        0        0     2280 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_users.py
+-rw-r--r--   0        0        0     2030 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_child_abuse.py
+-rw-r--r--   0        0        0     2026 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_copyright.py
+-rw-r--r--   0        0        0     2006 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_fake.py
+-rw-r--r--   0        0        0     2042 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_geo_irrelevant.py
+-rw-r--r--   0        0        0     2036 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_illegal_drugs.py
+-rw-r--r--   0        0        0     2010 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_other.py
+-rw-r--r--   0        0        0     2050 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_personal_details.py
+-rw-r--r--   0        0        0     2034 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_pornography.py
+-rw-r--r--   0        0        0     2006 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_spam.py
+-rw-r--r--   0        0        0     2022 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_violence.py
+-rw-r--r--   0        0        0     2371 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_file.py
+-rw-r--r--   0        0        0     2405 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_file_location.py
+-rw-r--r--   0        0        0     3050 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_file_uploaded.py
+-rw-r--r--   0        0        0     5597 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_value.py
+-rw-r--r--   0        0        0     3187 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_single_media.py
+-rw-r--r--   0        0        0     2035 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_animated_emoji.py
+-rw-r--r--   0        0        0     2075 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_animated_emoji_animations.py
+-rw-r--r--   0        0        0     2179 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_dice.py
+-rw-r--r--   0        0        0     2065 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_emoji_default_statuses.py
+-rw-r--r--   0        0        0     2073 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_emoji_default_topic_icons.py
+-rw-r--r--   0        0        0     2071 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_emoji_generic_animations.py
+-rw-r--r--   0        0        0     2005 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_empty.py
+-rw-r--r--   0        0        0     2379 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_id.py
+-rw-r--r--   0        0        0     3374 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_item.py
+-rw-r--r--   0        0        0     2033 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_premium_gifts.py
+-rw-r--r--   0        0        0     2217 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_short_name.py
+-rw-r--r--   0        0        0     2560 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_thumb.py
+-rw-r--r--   0        0        0     2236 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_stickered_media_document.py
+-rw-r--r--   0        0        0     2214 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_stickered_media_photo.py
+-rw-r--r--   0        0        0     2713 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_store_payment_gift_premium.py
+-rw-r--r--   0        0        0     2610 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_store_payment_premium_subscription.py
+-rw-r--r--   0        0        0     2023 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_takeout_file_location.py
+-rw-r--r--   0        0        0     2346 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_theme.py
+-rw-r--r--   0        0        0     5043 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_theme_settings.py
+-rw-r--r--   0        0        0     2118 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_theme_slug.py
+-rw-r--r--   0        0        0     2386 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user.py
+-rw-r--r--   0        0        0     1975 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user_empty.py
+-rw-r--r--   0        0        0     2632 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user_from_message.py
+-rw-r--r--   0        0        0     1971 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user_self.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_wall_paper.py
+-rw-r--r--   0        0        0     2133 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_wall_paper_no_file.py
+-rw-r--r--   0        0        0     2138 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_wall_paper_slug.py
+-rw-r--r--   0        0        0     2906 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_document.py
+-rw-r--r--   0        0        0     3532 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_file_audio_album_thumb_location.py
+-rw-r--r--   0        0        0     3282 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_file_geo_point_location.py
+-rw-r--r--   0        0        0     2400 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_file_location.py
+-rw-r--r--   0        0        0     6967 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/invoice.py
+-rw-r--r--   0        0        0     2275 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/ip_port.py
+-rw-r--r--   0        0        0     2507 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/ip_port_secret.py
+-rw-r--r--   0        0        0     2189 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_array.py
+-rw-r--r--   0        0        0     2098 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_bool.py
+-rw-r--r--   0        0        0     1951 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_null.py
+-rw-r--r--   0        0        0     2125 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_number.py
+-rw-r--r--   0        0        0     2217 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_object.py
+-rw-r--r--   0        0        0     2377 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_object_value.py
+-rw-r--r--   0        0        0     2110 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_string.py
+-rw-r--r--   0        0        0     2122 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button.py
+-rw-r--r--   0        0        0     2134 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_buy.py
+-rw-r--r--   0        0        0     2746 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_callback.py
+-rw-r--r--   0        0        0     2138 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_game.py
+-rw-r--r--   0        0        0     2194 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_geo_location.py
+-rw-r--r--   0        0        0     2719 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_peer.py
+-rw-r--r--   0        0        0     2170 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_phone.py
+-rw-r--r--   0        0        0     2550 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_poll.py
+-rw-r--r--   0        0        0     2267 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_row.py
+-rw-r--r--   0        0        0     2354 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_simple_web_view.py
+-rw-r--r--   0        0        0     3225 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_switch_inline.py
+-rw-r--r--   0        0        0     2314 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_url.py
+-rw-r--r--   0        0        0     2998 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_url_auth.py
+-rw-r--r--   0        0        0     2387 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_user_profile.py
+-rw-r--r--   0        0        0     2330 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_web_view.py
+-rw-r--r--   0        0        0     2333 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/labeled_price.py
+-rw-r--r--   0        0        0     3227 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_difference.py
+-rw-r--r--   0        0        0     5222 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_language.py
+-rw-r--r--   0        0        0     2514 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_string.py
+-rw-r--r--   0        0        0     2344 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_string_deleted.py
+-rw-r--r--   0        0        0     4665 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_string_pluralized.py
+-rw-r--r--   0        0        0     2635 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/mask_coords.py
+-rw-r--r--   0        0        0    12715 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message.py
+-rw-r--r--   0        0        0     3061 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_bot_allowed.py
+-rw-r--r--   0        0        0     2178 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_channel_create.py
+-rw-r--r--   0        0        0     2419 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_channel_migrate_from.py
+-rw-r--r--   0        0        0     2215 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_add_user.py
+-rw-r--r--   0        0        0     2409 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_create.py
+-rw-r--r--   0        0        0     2035 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_delete_photo.py
+-rw-r--r--   0        0        0     2205 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_delete_user.py
+-rw-r--r--   0        0        0     2223 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_edit_photo.py
+-rw-r--r--   0        0        0     2178 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_edit_title.py
+-rw-r--r--   0        0        0     2238 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_joined_by_link.py
+-rw-r--r--   0        0        0     2051 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_joined_by_request.py
+-rw-r--r--   0        0        0     2228 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_migrate_to.py
+-rw-r--r--   0        0        0     2027 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_contact_sign_up.py
+-rw-r--r--   0        0        0     2192 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_custom_action.py
+-rw-r--r--   0        0        0     1995 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_empty.py
+-rw-r--r--   0        0        0     2385 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_game_score.py
+-rw-r--r--   0        0        0     2727 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_geo_proximity_reached.py
+-rw-r--r--   0        0        0     3574 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_gift_premium.py
+-rw-r--r--   0        0        0     2668 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_group_call.py
+-rw-r--r--   0        0        0     2542 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_group_call_scheduled.py
+-rw-r--r--   0        0        0     2023 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_history_clear.py
+-rw-r--r--   0        0        0     2509 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_invite_to_group_call.py
+-rw-r--r--   0        0        0     3599 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_payment_sent.py
+-rw-r--r--   0        0        0     4621 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_payment_sent_me.py
+-rw-r--r--   0        0        0     3345 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_phone_call.py
+-rw-r--r--   0        0        0     2015 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_pin_message.py
+-rw-r--r--   0        0        0     2446 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_requested_peer.py
+-rw-r--r--   0        0        0     2035 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_screenshot_taken.py
+-rw-r--r--   0        0        0     2297 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_secure_values_sent.py
+-rw-r--r--   0        0        0     2679 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_secure_values_sent_me.py
+-rw-r--r--   0        0        0     2201 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_chat_theme.py
+-rw-r--r--   0        0        0     2287 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_chat_wall_paper.py
+-rw-r--r--   0        0        0     2729 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_messages_ttl.py
+-rw-r--r--   0        0        0     2303 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_same_chat_wall_paper.py
+-rw-r--r--   0        0        0     2247 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_suggest_profile_photo.py
+-rw-r--r--   0        0        0     2905 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_topic_create.py
+-rw-r--r--   0        0        0     3532 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_topic_edit.py
+-rw-r--r--   0        0        0     2177 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_web_view_data_sent.py
+-rw-r--r--   0        0        0     2374 2023-05-20 17:05:48.182348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_web_view_data_sent_me.py
+-rw-r--r--   0        0        0     2552 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_empty.py
+-rw-r--r--   0        0        0     2378 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_bank_card.py
+-rw-r--r--   0        0        0     2384 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_blockquote.py
+-rw-r--r--   0        0        0     2362 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_bold.py
+-rw-r--r--   0        0        0     2386 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_bot_command.py
+-rw-r--r--   0        0        0     2374 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_cashtag.py
+-rw-r--r--   0        0        0     2362 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_code.py
+-rw-r--r--   0        0        0     2647 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_custom_emoji.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_email.py
+-rw-r--r--   0        0        0     2374 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_hashtag.py
+-rw-r--r--   0        0        0     2370 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_italic.py
+-rw-r--r--   0        0        0     2374 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_mention.py
+-rw-r--r--   0        0        0     2611 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_mention_name.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_phone.py
+-rw-r--r--   0        0        0     2583 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_pre.py
+-rw-r--r--   0        0        0     2374 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_spoiler.py
+-rw-r--r--   0        0        0     2370 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_strike.py
+-rw-r--r--   0        0        0     2554 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_text_url.py
+-rw-r--r--   0        0        0     2382 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_underline.py
+-rw-r--r--   0        0        0     2374 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_unknown.py
+-rw-r--r--   0        0        0     2358 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_url.py
+-rw-r--r--   0        0        0     2234 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_extended_media.py
+-rw-r--r--   0        0        0     3529 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_extended_media_preview.py
+-rw-r--r--   0        0        0     5501 2023-05-20 17:05:48.242348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_fwd_header.py
+-rw-r--r--   0        0        0     2629 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_interaction_counters.py
+-rw-r--r--   0        0        0     3393 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_contact.py
+-rw-r--r--   0        0        0     2649 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_dice.py
+-rw-r--r--   0        0        0     3702 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_document.py
+-rw-r--r--   0        0        0     2275 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_empty.py
+-rw-r--r--   0        0        0     2454 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_game.py
+-rw-r--r--   0        0        0     2457 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_geo.py
+-rw-r--r--   0        0        0     3725 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_geo_live.py
+-rw-r--r--   0        0        0     5586 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_invoice.py
+-rw-r--r--   0        0        0     3360 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_photo.py
+-rw-r--r--   0        0        0     2739 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_poll.py
+-rw-r--r--   0        0        0     2299 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_unsupported.py
+-rw-r--r--   0        0        0     3572 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_venue.py
+-rw-r--r--   0        0        0     2505 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_web_page.py
+-rw-r--r--   0        0        0     3222 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_peer_reaction.py
+-rw-r--r--   0        0        0     2546 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_range.py
+-rw-r--r--   0        0        0     3439 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_reactions.py
+-rw-r--r--   0        0        0     4451 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_replies.py
+-rw-r--r--   0        0        0     3938 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_reply_header.py
+-rw-r--r--   0        0        0     5782 2023-05-20 17:05:48.178348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_service.py
+-rw-r--r--   0        0        0     2558 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_user_vote.py
+-rw-r--r--   0        0        0     2394 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_user_vote_input_option.py
+-rw-r--r--   0        0        0     2639 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_user_vote_multiple.py
+-rw-r--r--   0        0        0     3169 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_views.py
+-rw-r--r--   0        0        0     2834 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_detailed_info.py
+-rw-r--r--   0        0        0     2634 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_new_detailed_info.py
+-rw-r--r--   0        0        0     2196 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_resend_ans_req.py
+-rw-r--r--   0        0        0     2184 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_resend_req.py
+-rw-r--r--   0        0        0     2159 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_ack.py
+-rw-r--r--   0        0        0     2368 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_all_info.py
+-rw-r--r--   0        0        0     2365 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_state_info.py
+-rw-r--r--   0        0        0     2184 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_state_req.py
+-rw-r--r--   0        0        0     2788 2023-05-20 17:05:48.214348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/nearest_dc.py
+-rw-r--r--   0        0        0     2703 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/new_session_created.py
+-rw-r--r--   0        0        0     2023 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_default.py
+-rw-r--r--   0        0        0     2355 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_local.py
+-rw-r--r--   0        0        0     2011 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_none.py
+-rw-r--r--   0        0        0     2156 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_ringtone.py
+-rw-r--r--   0        0        0     1984 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_broadcasts.py
+-rw-r--r--   0        0        0     1964 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_chats.py
+-rw-r--r--   0        0        0     2412 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_forum_topic.py
+-rw-r--r--   0        0        0     2143 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_peer.py
+-rw-r--r--   0        0        0     1964 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_users.py
+-rw-r--r--   0        0        0     1930 2023-05-20 17:05:48.166348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/null.py
+-rw-r--r--   0        0        0     4034 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page.py
+-rw-r--r--   0        0        0     2121 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_anchor.py
+-rw-r--r--   0        0        0     2443 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_audio.py
+-rw-r--r--   0        0        0     2493 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_author_date.py
+-rw-r--r--   0        0        0     2467 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_blockquote.py
+-rw-r--r--   0        0        0     2193 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_channel.py
+-rw-r--r--   0        0        0     2502 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_collage.py
+-rw-r--r--   0        0        0     2187 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_cover.py
+-rw-r--r--   0        0        0     2766 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_details.py
+-rw-r--r--   0        0        0     1983 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_divider.py
+-rw-r--r--   0        0        0     4659 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_embed.py
+-rw-r--r--   0        0        0     3638 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_embed_post.py
+-rw-r--r--   0        0        0     2178 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_footer.py
+-rw-r--r--   0        0        0     2178 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_header.py
+-rw-r--r--   0        0        0     2178 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_kicker.py
+-rw-r--r--   0        0        0     2217 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_list.py
+-rw-r--r--   0        0        0     2961 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_map.py
+-rw-r--r--   0        0        0     2273 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_ordered_list.py
+-rw-r--r--   0        0        0     2190 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_paragraph.py
+-rw-r--r--   0        0        0     3234 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_photo.py
+-rw-r--r--   0        0        0     2427 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_preformatted.py
+-rw-r--r--   0        0        0     2463 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_pullquote.py
+-rw-r--r--   0        0        0     2567 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_related_articles.py
+-rw-r--r--   0        0        0     2508 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_slideshow.py
+-rw-r--r--   0        0        0     2190 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_subheader.py
+-rw-r--r--   0        0        0     2186 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_subtitle.py
+-rw-r--r--   0        0        0     3055 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_table.py
+-rw-r--r--   0        0        0     2174 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_title.py
+-rw-r--r--   0        0        0     1999 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_unsupported.py
+-rw-r--r--   0        0        0     3004 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_video.py
+-rw-r--r--   0        0        0     2428 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_caption.py
+-rw-r--r--   0        0        0     2237 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_item_blocks.py
+-rw-r--r--   0        0        0     2185 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_item_text.py
+-rw-r--r--   0        0        0     2452 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_ordered_item_blocks.py
+-rw-r--r--   0        0        0     2400 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_ordered_item_text.py
+-rw-r--r--   0        0        0     4412 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_related_article.py
+-rw-r--r--   0        0        0     4643 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_table_cell.py
+-rw-r--r--   0        0        0     2220 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_table_row.py
+-rw-r--r--   0        0        0     2863 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/password_kdf_algo_sha256_sha256_pbkdf2_hmacsha512iter100000_sha256_mod_pow.py
+-rw-r--r--   0        0        0     2013 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/password_kdf_algo_unknown.py
+-rw-r--r--   0        0        0     2414 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_charge.py
+-rw-r--r--   0        0        0     2326 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_form_method.py
+-rw-r--r--   0        0        0     3602 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_requested_info.py
+-rw-r--r--   0        0        0     2363 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_saved_credentials_card.py
+-rw-r--r--   0        0        0     2366 2023-05-20 17:05:48.294348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_blocked.py
+-rw-r--r--   0        0        0     2380 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_channel.py
+-rw-r--r--   0        0        0     2341 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_chat.py
+-rw-r--r--   0        0        0     2593 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_located.py
+-rw-r--r--   0        0        0     4953 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_notify_settings.py
+-rw-r--r--   0        0        0     2152 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_self_located.py
+-rw-r--r--   0        0        0     6386 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_settings.py
+-rw-r--r--   0        0        0     2341 2023-05-20 17:05:48.170348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_user.py
+-rw-r--r--   0        0        0     5084 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call.py
+-rw-r--r--   0        0        0     3871 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_accepted.py
+-rw-r--r--   0        0        0     2036 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_busy.py
+-rw-r--r--   0        0        0     2060 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_disconnect.py
+-rw-r--r--   0        0        0     2044 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_hangup.py
+-rw-r--r--   0        0        0     2044 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_missed.py
+-rw-r--r--   0        0        0     3877 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discarded.py
+-rw-r--r--   0        0        0     2104 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_empty.py
+-rw-r--r--   0        0        0     3390 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_protocol.py
+-rw-r--r--   0        0        0     3920 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_requested.py
+-rw-r--r--   0        0        0     4119 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_waiting.py
+-rw-r--r--   0        0        0     3167 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_connection.py
+-rw-r--r--   0        0        0     3664 2023-05-20 17:05:48.262348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_connection_webrtc.py
+-rw-r--r--   0        0        0     4128 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo.py
+-rw-r--r--   0        0        0     2646 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_cached_size.py
+-rw-r--r--   0        0        0     2084 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_empty.py
+-rw-r--r--   0        0        0     2312 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_path_size.py
+-rw-r--r--   0        0        0     2616 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_size.py
+-rw-r--r--   0        0        0     2115 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_size_empty.py
+-rw-r--r--   0        0        0     2709 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_size_progressive.py
+-rw-r--r--   0        0        0     2328 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_stripped_size.py
+-rw-r--r--   0        0        0     4634 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll.py
+-rw-r--r--   0        0        0     2310 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll_answer.py
+-rw-r--r--   0        0        0     2930 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll_answer_voters.py
+-rw-r--r--   0        0        0     4558 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll_results.py
+-rw-r--r--   0        0        0     2537 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pong.py
+-rw-r--r--   0        0        0     2408 2023-05-20 17:05:48.266348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/popular_contact.py
+-rw-r--r--   0        0        0     3322 2023-05-20 17:05:48.254348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/post_address.py
+-rw-r--r--   0        0        0     3145 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data.py
+-rw-r--r--   0        0        0     3326 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data_dc.py
+-rw-r--r--   0        0        0     3406 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data_temp.py
+-rw-r--r--   0        0        0     3587 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data_temp_dc.py
+-rw-r--r--   0        0        0     3297 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/premium_gift_option.py
+-rw-r--r--   0        0        0     4408 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/premium_subscription_option.py
+-rw-r--r--   0        0        0     2008 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_added_by_phone.py
+-rw-r--r--   0        0        0     2000 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_chat_invite.py
+-rw-r--r--   0        0        0     1992 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_forwards.py
+-rw-r--r--   0        0        0     1996 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_phone_call.py
+-rw-r--r--   0        0        0     2004 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_phone_number.py
+-rw-r--r--   0        0        0     1992 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_phone_p2_p.py
+-rw-r--r--   0        0        0     2008 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_profile_photo.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_status_timestamp.py
+-rw-r--r--   0        0        0     2010 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_voice_messages.py
+-rw-r--r--   0        0        0     2001 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_all.py
+-rw-r--r--   0        0        0     2249 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_chat_participants.py
+-rw-r--r--   0        0        0     2021 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_contacts.py
+-rw-r--r--   0        0        0     2205 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_users.py
+-rw-r--r--   0        0        0     2013 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_all.py
+-rw-r--r--   0        0        0     2261 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_chat_participants.py
+-rw-r--r--   0        0        0     2033 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_contacts.py
+-rw-r--r--   0        0        0     2217 2023-05-20 17:05:48.222348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_users.py
+-rw-r--r--   0        0        0     2888 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_count.py
+-rw-r--r--   0        0        0     2204 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_custom_emoji.py
+-rw-r--r--   0        0        0     2148 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_emoji.py
+-rw-r--r--   0        0        0     1970 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_empty.py
+-rw-r--r--   0        0        0     2589 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/read_participant_date.py
+-rw-r--r--   0        0        0     2550 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/received_notify_message.py
+-rw-r--r--   0        0        0     2335 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_chat.py
+-rw-r--r--   0        0        0     2455 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_chat_invite.py
+-rw-r--r--   0        0        0     2411 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_sticker_set.py
+-rw-r--r--   0        0        0     2126 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_unknown.py
+-rw-r--r--   0        0        0     2335 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_user.py
+-rw-r--r--   0        0        0     2246 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_inline_markup.py
+-rw-r--r--   0        0        0     3010 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_keyboard_force_reply.py
+-rw-r--r--   0        0        0     2272 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_keyboard_hide.py
+-rw-r--r--   0        0        0     3850 2023-05-20 17:05:48.234348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     3842 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/request_peer_type_broadcast.py
+-rw-r--r--   0        0        0     4511 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/request_peer_type_chat.py
+-rw-r--r--   0        0        0     2699 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/request_peer_type_user.py
+-rw-r--r--   0        0        0     3224 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/res_pq.py
+-rw-r--r--   0        0        0     2569 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/restriction_reason.py
+-rw-r--r--   0        0        0     2758 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_answer_dropped.py
+-rw-r--r--   0        0        0     2212 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_answer_dropped_running.py
+-rw-r--r--   0        0        0     2184 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_answer_unknown.py
+-rw-r--r--   0        0        0     2418 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_error.py
+-rw-r--r--   0        0        0     2403 2023-05-20 17:05:48.162348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_result.py
+-rw-r--r--   0        0        0     3010 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/saved_phone_contact.py
+-rw-r--r--   0        0        0     2573 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/search_result_position.py
+-rw-r--r--   0        0        0     2879 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/search_results_calendar_period.py
+-rw-r--r--   0        0        0     2581 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_credentials_encrypted.py
+-rw-r--r--   0        0        0     2546 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_data.py
+-rw-r--r--   0        0        0     3374 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_file.py
+-rw-r--r--   0        0        0     1980 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_file_empty.py
+-rw-r--r--   0        0        0     2262 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_password_kdf_algo_pbkdf2_hmacsha512iter100000.py
+-rw-r--r--   0        0        0     2182 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_password_kdf_algo_sha512.py
+-rw-r--r--   0        0        0     2039 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_password_kdf_algo_unknown.py
+-rw-r--r--   0        0        0     2140 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_plain_email.py
+-rw-r--r--   0        0        0     2140 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_plain_phone.py
+-rw-r--r--   0        0        0     3307 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_required_type.py
+-rw-r--r--   0        0        0     2288 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_required_type_one_of.py
+-rw-r--r--   0        0        0     2897 2023-05-20 17:05:48.278348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_secret_settings.py
+-rw-r--r--   0        0        0     5944 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value.py
+-rw-r--r--   0        0        0     2596 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error.py
+-rw-r--r--   0        0        0     2855 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_data.py
+-rw-r--r--   0        0        0     2657 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_file.py
+-rw-r--r--   0        0        0     2701 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_files.py
+-rw-r--r--   0        0        0     2673 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_front_side.py
+-rw-r--r--   0        0        0     2685 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_reverse_side.py
+-rw-r--r--   0        0        0     2665 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_selfie.py
+-rw-r--r--   0        0        0     2701 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_translation_file.py
+-rw-r--r--   0        0        0     2745 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_translation_files.py
+-rw-r--r--   0        0        0     2402 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_hash.py
+-rw-r--r--   0        0        0     2013 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_address.py
+-rw-r--r--   0        0        0     2037 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_bank_statement.py
+-rw-r--r--   0        0        0     2035 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_driver_license.py
+-rw-r--r--   0        0        0     2005 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_email.py
+-rw-r--r--   0        0        0     2033 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_identity_card.py
+-rw-r--r--   0        0        0     2049 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_internal_passport.py
+-rw-r--r--   0        0        0     2017 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_passport.py
+-rw-r--r--   0        0        0     2065 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_passport_registration.py
+-rw-r--r--   0        0        0     2045 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_personal_details.py
+-rw-r--r--   0        0        0     2005 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_phone.py
+-rw-r--r--   0        0        0     2045 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_rental_agreement.py
+-rw-r--r--   0        0        0     2069 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_temporary_registration.py
+-rw-r--r--   0        0        0     2029 2023-05-20 17:05:48.274348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_utility_bill.py
+-rw-r--r--   0        0        0     2536 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_as_peer.py
+-rw-r--r--   0        0        0     2019 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_cancel_action.py
+-rw-r--r--   0        0        0     2047 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_choose_contact_action.py
+-rw-r--r--   0        0        0     2047 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_choose_sticker_action.py
+-rw-r--r--   0        0        0     2731 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_emoji_interaction.py
+-rw-r--r--   0        0        0     2229 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_emoji_interaction_seen.py
+-rw-r--r--   0        0        0     2027 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_game_play_action.py
+-rw-r--r--   0        0        0     2039 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_geo_location_action.py
+-rw-r--r--   0        0        0     2227 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_history_import_action.py
+-rw-r--r--   0        0        0     2039 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_record_audio_action.py
+-rw-r--r--   0        0        0     2039 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_record_round_action.py
+-rw-r--r--   0        0        0     2039 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_record_video_action.py
+-rw-r--r--   0        0        0     2019 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_typing_action.py
+-rw-r--r--   0        0        0     2219 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_audio_action.py
+-rw-r--r--   0        0        0     2231 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_document_action.py
+-rw-r--r--   0        0        0     2219 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_photo_action.py
+-rw-r--r--   0        0        0     2219 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_round_action.py
+-rw-r--r--   0        0        0     2219 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_video_action.py
+-rw-r--r--   0        0        0     3256 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/server_dh_inner_data.py
+-rw-r--r--   0        0        0     2918 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/server_dh_params_fail.py
+-rw-r--r--   0        0        0     2917 2023-05-20 17:05:48.158348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/server_dh_params_ok.py
+-rw-r--r--   0        0        0     2604 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/shipping_option.py
+-rw-r--r--   0        0        0     2363 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/simple_web_view_result_url.py
+-rw-r--r--   0        0        0     2027 2023-05-20 17:05:48.218348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/speaking_in_group_call_action.py
+-rw-r--r--   0        0        0     6685 2023-05-20 17:05:48.298348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sponsored_message.py
+-rw-r--r--   0        0        0     2434 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_abs_value_and_prev.py
+-rw-r--r--   0        0        0     2407 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_date_range_days.py
+-rw-r--r--   0        0        0     2817 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_graph.py
+-rw-r--r--   0        0        0     2335 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_graph_async.py
+-rw-r--r--   0        0        0     2335 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_graph_error.py
+-rw-r--r--   0        0        0     2810 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_group_top_admin.py
+-rw-r--r--   0        0        0     2438 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_group_top_inviter.py
+-rw-r--r--   0        0        0     2642 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_group_top_poster.py
+-rw-r--r--   0        0        0     2365 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_percent_value.py
+-rw-r--r--   0        0        0     2083 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_url.py
+-rw-r--r--   0        0        0     2446 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_keyword.py
+-rw-r--r--   0        0        0     2422 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_pack.py
+-rw-r--r--   0        0        0     7071 2023-05-20 17:05:48.230348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set.py
+-rw-r--r--   0        0        0     2660 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_covered.py
+-rw-r--r--   0        0        0     3351 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_full_covered.py
+-rw-r--r--   0        0        0     2711 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_multi_covered.py
+-rw-r--r--   0        0        0     2413 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_no_covered.py
+-rw-r--r--   0        0        0     2346 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_anchor.py
+-rw-r--r--   0        0        0     2149 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_bold.py
+-rw-r--r--   0        0        0     2188 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_concat.py
+-rw-r--r--   0        0        0     2351 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_email.py
+-rw-r--r--   0        0        0     1954 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_empty.py
+-rw-r--r--   0        0        0     2153 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_fixed.py
+-rw-r--r--   0        0        0     2490 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_image.py
+-rw-r--r--   0        0        0     2157 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_italic.py
+-rw-r--r--   0        0        0     2155 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_marked.py
+-rw-r--r--   0        0        0     2351 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_phone.py
+-rw-r--r--   0        0        0     2096 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_plain.py
+-rw-r--r--   0        0        0     2157 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_strike.py
+-rw-r--r--   0        0        0     2169 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_subscript.py
+-rw-r--r--   0        0        0     2177 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_superscript.py
+-rw-r--r--   0        0        0     2169 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_underline.py
+-rw-r--r--   0        0        0     2573 2023-05-20 17:05:48.250348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_url.py
+-rw-r--r--   0        0        0     2456 2023-05-20 17:05:48.310348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_with_entities.py
+-rw-r--r--   0        0        0     5594 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/theme.py
+-rw-r--r--   0        0        0     4409 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/theme_settings.py
+-rw-r--r--   0        0        0     2350 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer.py
+-rw-r--r--   0        0        0     2025 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_bots_inline.py
+-rw-r--r--   0        0        0     2009 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_bots_pm.py
+-rw-r--r--   0        0        0     2017 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_channels.py
+-rw-r--r--   0        0        0     2039 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_correspondents.py
+-rw-r--r--   0        0        0     2033 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_forward_chats.py
+-rw-r--r--   0        0        0     2033 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_forward_users.py
+-rw-r--r--   0        0        0     2009 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_groups.py
+-rw-r--r--   0        0        0     2746 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_peers.py
+-rw-r--r--   0        0        0     2025 2023-05-20 17:05:48.246348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_phone_calls.py
+-rw-r--r--   0        0        0     1996 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_attach_menu_bots.py
+-rw-r--r--   0        0        0     2004 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_auto_save_settings.py
+-rw-r--r--   0        0        0     3975 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_callback_query.py
+-rw-r--r--   0        0        0     3307 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_chat_invite_requester.py
+-rw-r--r--   0        0        0     2691 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_commands.py
+-rw-r--r--   0        0        0     3736 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_inline_query.py
+-rw-r--r--   0        0        0     3449 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_inline_send.py
+-rw-r--r--   0        0        0     2441 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_menu_button.py
+-rw-r--r--   0        0        0     4117 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_precheckout_query.py
+-rw-r--r--   0        0        0     2991 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_shipping_query.py
+-rw-r--r--   0        0        0     2739 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_stopped.py
+-rw-r--r--   0        0        0     2195 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_webhook_json.py
+-rw-r--r--   0        0        0     2663 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_webhook_json_query.py
+-rw-r--r--   0        0        0     2169 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel.py
+-rw-r--r--   0        0        0     2536 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_available_messages.py
+-rw-r--r--   0        0        0     2629 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_message_forwards.py
+-rw-r--r--   0        0        0     2590 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_message_views.py
+-rw-r--r--   0        0        0     4986 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_participant.py
+-rw-r--r--   0        0        0     2743 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_pinned_topic.py
+-rw-r--r--   0        0        0     2653 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_pinned_topics.py
+-rw-r--r--   0        0        0     2972 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_read_messages_contents.py
+-rw-r--r--   0        0        0     2576 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_too_long.py
+-rw-r--r--   0        0        0     3222 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_user_typing.py
+-rw-r--r--   0        0        0     2884 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_web_page.py
+-rw-r--r--   0        0        0     2130 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat.py
+-rw-r--r--   0        0        0     2864 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_default_banned_rights.py
+-rw-r--r--   0        0        0     4611 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant.py
+-rw-r--r--   0        0        0     3064 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant_add.py
+-rw-r--r--   0        0        0     2854 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant_admin.py
+-rw-r--r--   0        0        0     2637 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant_delete.py
+-rw-r--r--   0        0        0     2305 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participants.py
+-rw-r--r--   0        0        0     2727 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_user_typing.py
+-rw-r--r--   0        0        0     1964 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_config.py
+-rw-r--r--   0        0        0     1992 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_contacts_reset.py
+-rw-r--r--   0        0        0     2251 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dc_options.py
+-rw-r--r--   0        0        0     2910 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_delete_channel_messages.py
+-rw-r--r--   0        0        0     2634 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_delete_messages.py
+-rw-r--r--   0        0        0     2482 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_delete_scheduled_messages.py
+-rw-r--r--   0        0        0     2596 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_filter.py
+-rw-r--r--   0        0        0     2201 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_filter_order.py
+-rw-r--r--   0        0        0     1992 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_filters.py
+-rw-r--r--   0        0        0     2898 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_pinned.py
+-rw-r--r--   0        0        0     2514 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_unread_mark.py
+-rw-r--r--   0        0        0     2898 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_draft_message.py
+-rw-r--r--   0        0        0     2652 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_edit_channel_message.py
+-rw-r--r--   0        0        0     2624 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_edit_message.py
+-rw-r--r--   0        0        0     2187 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_encrypted_chat_typing.py
+-rw-r--r--   0        0        0     2613 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_encrypted_messages_read.py
+-rw-r--r--   0        0        0     2390 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_encryption.py
+-rw-r--r--   0        0        0     1992 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_faved_stickers.py
+-rw-r--r--   0        0        0     2703 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_folder_peers.py
+-rw-r--r--   0        0        0     2384 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_geo_live_viewed.py
+-rw-r--r--   0        0        0     2400 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_call.py
+-rw-r--r--   0        0        0     2588 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_call_connection.py
+-rw-r--r--   0        0        0     2853 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_call_participants.py
+-rw-r--r--   0        0        0     2222 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_invite_privacy_forbidden.py
+-rw-r--r--   0        0        0     3884 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_inline_bot_callback_query.py
+-rw-r--r--   0        0        0     2265 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_lang_pack.py
+-rw-r--r--   0        0        0     2187 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_lang_pack_too_long.py
+-rw-r--r--   0        0        0     1980 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_login_token.py
+-rw-r--r--   0        0        0     2796 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_extended_media.py
+-rw-r--r--   0        0        0     2341 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_id.py
+-rw-r--r--   0        0        0     2871 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_poll.py
+-rw-r--r--   0        0        0     2834 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_poll_vote.py
+-rw-r--r--   0        0        0     3175 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_reactions.py
+-rw-r--r--   0        0        0     2769 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_move_sticker_set_to_top.py
+-rw-r--r--   0        0        0     2648 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_channel_message.py
+-rw-r--r--   0        0        0     2456 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_encrypted_message.py
+-rw-r--r--   0        0        0     2620 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_message.py
+-rw-r--r--   0        0        0     2238 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_scheduled_message.py
+-rw-r--r--   0        0        0     2289 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_sticker_set.py
+-rw-r--r--   0        0        0     2588 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_notify_settings.py
+-rw-r--r--   0        0        0     2406 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_blocked.py
+-rw-r--r--   0        0        0     2635 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_history_ttl.py
+-rw-r--r--   0        0        0     2226 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_located.py
+-rw-r--r--   0        0        0     2469 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_settings.py
+-rw-r--r--   0        0        0     2849 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pending_join_requests.py
+-rw-r--r--   0        0        0     2233 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_phone_call.py
+-rw-r--r--   0        0        0     2446 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_phone_call_signaling_data.py
+-rw-r--r--   0        0        0     3213 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pinned_channel_messages.py
+-rw-r--r--   0        0        0     2826 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pinned_dialogs.py
+-rw-r--r--   0        0        0     3167 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pinned_messages.py
+-rw-r--r--   0        0        0     2455 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_privacy.py
+-rw-r--r--   0        0        0     1980 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pts_changed.py
+-rw-r--r--   0        0        0     3680 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_discussion_inbox.py
+-rw-r--r--   0        0        0     2748 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_discussion_outbox.py
+-rw-r--r--   0        0        0     3358 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_inbox.py
+-rw-r--r--   0        0        0     2418 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_outbox.py
+-rw-r--r--   0        0        0     2040 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_featured_emoji_stickers.py
+-rw-r--r--   0        0        0     2020 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_featured_stickers.py
+-rw-r--r--   0        0        0     3576 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_history_inbox.py
+-rw-r--r--   0        0        0     2818 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_history_outbox.py
+-rw-r--r--   0        0        0     2658 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_messages_contents.py
+-rw-r--r--   0        0        0     2016 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_recent_emoji_statuses.py
+-rw-r--r--   0        0        0     2000 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_recent_reactions.py
+-rw-r--r--   0        0        0     1996 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_recent_stickers.py
+-rw-r--r--   0        0        0     1976 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_saved_gifs.py
+-rw-r--r--   0        0        0     1996 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_saved_ringtones.py
+-rw-r--r--   0        0        0     3674 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_service_notification.py
+-rw-r--r--   0        0        0     5802 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short.py
+-rw-r--r--   0        0        0    10243 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short_chat_message.py
+-rw-r--r--   0        0        0    10006 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short_message.py
+-rw-r--r--   0        0        0     7778 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short_sent_message.py
+-rw-r--r--   0        0        0     2489 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_sticker_sets.py
+-rw-r--r--   0        0        0     2750 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_sticker_sets_order.py
+-rw-r--r--   0        0        0     2156 2023-05-20 17:05:48.202348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_theme.py
+-rw-r--r--   0        0        0     3195 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_transcribed_audio.py
+-rw-r--r--   0        0        0     2130 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user.py
+-rw-r--r--   0        0        0     2504 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_emoji_status.py
+-rw-r--r--   0        0        0     2936 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_name.py
+-rw-r--r--   0        0        0     2346 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_phone.py
+-rw-r--r--   0        0        0     2426 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_status.py
+-rw-r--r--   0        0        0     2454 2023-05-20 17:05:48.194348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_typing.py
+-rw-r--r--   0        0        0     2608 2023-05-20 17:05:48.198348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_web_page.py
+-rw-r--r--   0        0        0     2191 2023-05-20 17:05:48.206348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_web_view_result_sent.py
+-rw-r--r--   0        0        0     6789 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/updates_combined.py
+-rw-r--r--   0        0        0     6521 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/updates_t.py
+-rw-r--r--   0        0        0     5414 2023-05-20 17:05:48.210348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/updates_too_long.py
+-rw-r--r--   0        0        0     2383 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/url_auth_result_accepted.py
+-rw-r--r--   0        0        0     2246 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/url_auth_result_default.py
+-rw-r--r--   0        0        0     3056 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/url_auth_result_request.py
+-rw-r--r--   0        0        0    13966 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user.py
+-rw-r--r--   0        0        0     2419 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_empty.py
+-rw-r--r--   0        0        0    12871 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_full.py
+-rw-r--r--   0        0        0     3433 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_profile_photo.py
+-rw-r--r--   0        0        0     2010 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_profile_photo_empty.py
+-rw-r--r--   0        0        0     1978 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_empty.py
+-rw-r--r--   0        0        0     1996 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_last_month.py
+-rw-r--r--   0        0        0     1990 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_last_week.py
+-rw-r--r--   0        0        0     2182 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_offline.py
+-rw-r--r--   0        0        0     2155 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_online.py
+-rw-r--r--   0        0        0     1992 2023-05-20 17:05:48.174348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_recently.py
+-rw-r--r--   0        0        0     2707 2023-05-20 17:05:48.306348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/username.py
+-rw-r--r--   0        0        0     3129 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/video_size.py
+-rw-r--r--   0        0        0     2530 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/video_size_emoji_markup.py
+-rw-r--r--   0        0        0     2882 2023-05-20 17:05:48.290348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/video_size_sticker_markup.py
+-rw-r--r--   0        0        0     4657 2023-05-20 17:05:48.186348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/wall_paper.py
+-rw-r--r--   0        0        0     3419 2023-05-20 17:05:48.190348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/wall_paper_no_file.py
+-rw-r--r--   0        0        0     5408 2023-05-20 17:05:48.282348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/wall_paper_settings.py
+-rw-r--r--   0        0        0     3892 2023-05-20 17:05:48.270348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_authorization.py
+-rw-r--r--   0        0        0     3138 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_document.py
+-rw-r--r--   0        0        0     2909 2023-05-20 17:05:48.258348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_document_no_proxy.py
+-rw-r--r--   0        0        0     8698 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page.py
+-rw-r--r--   0        0        0     2943 2023-05-20 17:05:48.286348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_attribute_theme.py
+-rw-r--r--   0        0        0     2297 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_empty.py
+-rw-r--r--   0        0        0     2678 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_not_modified.py
+-rw-r--r--   0        0        0     2496 2023-05-20 17:05:48.226348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_pending.py
+-rw-r--r--   0        0        0     2694 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_view_message_sent.py
+-rw-r--r--   0        0        0     2555 2023-05-20 17:05:48.302348 pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_view_result_url.py
+-rw-r--r--   0        0        0      871 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/__init__.py
+-rw-r--r--   0        0        0    10513 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/auth.py
+-rw-r--r--   0        0        0      917 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/__init__.py
+-rw-r--r--   0        0        0     2452 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/data_center.py
+-rw-r--r--   0        0        0     1374 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0        0        0     1587 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0        0        0     1257 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0        0        0    12440 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/session.py
+-rw-r--r--   0        0        0      968 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/file_storage.py
+-rw-r--r--   0        0        0     2741 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/memory_storage.py
+-rw-r--r--   0        0        0     5428 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/mongo_storage.py
+-rw-r--r--   0        0        0     6382 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0        0        0     2781 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/storage.py
+-rw-r--r--   0        0        0     3739 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/sync.py
+-rw-r--r--   0        0        0     1109 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/__init__.py
+-rw-r--r--   0        0        0      938 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0        0        0     2288 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0        0        0     1930 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/authorization/terms_of_service.py
+-rw-r--r--   0        0        0     2830 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0        0        0     2788 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0        0        0     1293 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0        0        0     1258 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0        0        0     1249 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0        0        0     1562 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0        0        0     1639 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0        0        0     1817 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0        0        0     1308 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0        0        0     1029 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0        0        0    12797 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0        0        0     2383 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0        0        0     2216 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0        0        0     8120 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0        0        0     2460 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0        0        0     3514 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0        0        0     3712 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0        0        0     1603 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0        0        0     1209 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0        0        0     1212 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0        0        0     1809 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0        0        0     4575 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     2339 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1564 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0        0        0     1313 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/web_app_info.py
+-rw-r--r--   0        0        0     2755 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0        0        0     3662 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0        0        0     7298 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0        0        0     2411 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0        0        0     5782 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0        0        0     3304 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0        0        0     4505 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0        0        0     4245 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0        0        0     4029 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0        0        0     4388 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0        0        0     4312 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0        0        0     3031 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0        0        0     4394 2023-05-20 17:04:54.310236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0        0        0     4202 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0        0        0     4132 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0        0        0     5240 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0        0        0     4619 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0        0        0     5261 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0        0        0     4754 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0        0        0     5474 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0        0        0     4360 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_voice.py
+-rw-r--r--   0        0        0     1314 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0        0        0     1638 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0        0        0     3428 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0        0        0     3282 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0        0        0     2771 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0        0        0     2685 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0        0        0     3620 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0        0        0     1737 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_phone_contact.py
+-rw-r--r--   0        0        0     1006 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0        0        0     1413 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0        0        0     2638 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0        0        0     1093 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/list.py
+-rw-r--r--   0        0        0     1885 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0        0        0     4044 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0        0        0     4069 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0        0        0     2207 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0        0        0     1587 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0        0        0     3409 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0        0        0     3044 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0        0        0     1660 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0        0        0   153174 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0        0        0     4352 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0        0        0     1800 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0        0        0     4309 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0        0        0     8016 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0        0        0     1532 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0        0        0     2617 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0        0        0     6909 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0        0        0     2765 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0        0        0     1431 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0        0        0     3755 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0        0        0     2291 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0        0        0     4389 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0        0        0     3601 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0        0        0     3204 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0        0        0     1565 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0        0        0     6351 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0        0        0     3862 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/object.py
+-rw-r--r--   0        0        0     1030 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/update.py
+-rw-r--r--   0        0        0     3063 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0        0        0    33966 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0        0        0     2236 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0        0        0    22023 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0        0        0     5514 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0        0        0     4579 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0        0        0     4245 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0        0        0     1054 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0        0        0     2564 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0        0        0     9444 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0        0        0     3674 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0        0        0     4718 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0        0        0     3967 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0        0        0     2592 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0        0        0     5300 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0        0        0     2356 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0        0        0     2682 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0        0        0     2422 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0        0        0     4970 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0        0        0     1043 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0        0        0     1850 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0        0        0     1861 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0        0        0     1047 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1047 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0     1051 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     1951 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0        0        0     1329 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0        0        0     1293 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0        0        0     1663 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0        0        0    13658 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0        0        0     1691 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0        0        0     1346 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0        0        0     1610 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0        0        0     1531 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0        0        0     1043 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0        0        0    10911 2023-05-20 17:04:54.314236 pyrofork_dev-2.1.8.dev202305201705/pyrogram/utils.py
+-rw-r--r--   0        0        0     4064 1970-01-01 00:00:00.000000 pyrofork_dev-2.1.8.dev202305201705/PKG-INFO
```

### Comparing `pyrofork_dev-2.1.8.dev202305201658/README.md` & `pyrofork_dev-2.1.8.dev202305201705/README.md`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyproject.toml` & `pyrofork_dev-2.1.8.dev202305201705/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrofork-dev"
-version = "2.1.8.dev202305201658"
+version = "2.1.8.dev202305201705"
 description = "Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots"
 license = "LGPL-3.0-or-later"
 authors = [
     "Dan <14043624+delivrance@users.noreply.github.com>",
     "wulan17 <wulan17@nusantararom.org>"
 ]
 readme = "README.md"
```

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork-dev"
-__version__ = "2.1.8.dev202305201658"
+__version__ = "2.1.8.dev202305201705"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2017-present Dan <https://github.com/delivrance>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/client.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/connection.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_abridged.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_full.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/aes.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/mtproto.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/prime.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/crypto/rsa.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/dispatcher.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/emoji.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/auto_name.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_event_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_member_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_members_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/chat_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/message_entity_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/message_media_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/message_service_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/messages_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/next_code_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/parse_mode.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/poll_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/sent_code_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/enums/user_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/all.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/all.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/bad_request_400.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/bad_request_400.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/flood_420.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/flood_420.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/forbidden_403.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/forbidden_403.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/internal_server_error_500.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/internal_server_error_500.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/not_acceptable_406.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/not_acceptable_406.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/see_other_303.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/see_other_303.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/service_unavailable_503.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/service_unavailable_503.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/exceptions/unauthorized_401.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/exceptions/unauthorized_401.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/errors/rpc_error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/file_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/filters.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/callback_query_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/chat_join_request_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/chat_member_updated_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/chosen_inline_result_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/deleted_messages_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/disconnect_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/edited_message_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/inline_query_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/message_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/poll_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/raw_update_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/handlers/user_status_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/invoke.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/resolve_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/advanced/save_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/accept_terms_of_service.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/check_password.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/connect.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/disconnect.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/get_password_hint.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/initialize.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/log_out.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/recover_password.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/resend_code.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/send_code.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/send_recovery_code.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/sign_in.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/sign_in_bot.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/sign_up.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/auth/terminate.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/answer_callback_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/answer_inline_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/answer_web_app_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/delete_bot_commands.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_bot_commands.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_bot_default_privileges.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_chat_menu_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_game_high_scores.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/get_inline_bot_results.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/request_callback_answer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/send_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/send_inline_bot_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_bot_commands.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_bot_default_privileges.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_chat_menu_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/bots/set_game_score.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/add_chat_members.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/archive_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/ban_chat_member.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/close_forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/close_general_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/create_supergroup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_chat_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_supergroup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/delete_user_history.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/edit_forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/edit_general_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_event_log.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_member.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_members.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_members_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_chat_online_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_dialogs.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_dialogs_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_forum_topics.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_forum_topics_by_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_nearby_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/get_send_as_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/hide_general_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/join_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/leave_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/mark_chat_unread.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/pin_chat_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/promote_chat_member.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/reopen_forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/reopen_general_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/restrict_chat_member.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_administrator_title.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_description.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_permissions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_protected_content.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_title.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_chat_username.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_send_as_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/set_slow_mode.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unarchive_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unban_chat_member.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unhide_general_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unpin_all_chat_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/chats/unpin_chat_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/add_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/delete_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/get_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/get_contacts_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/contacts/import_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_callback_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_chat_join_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_chat_member_updated.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_chosen_inline_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_deleted_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_disconnect.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_edited_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_inline_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_raw_update.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/decorators/on_user_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/approve_chat_join_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/create_chat_invite_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/decline_chat_join_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/export_chat_invite_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_invite_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/get_chat_join_requests.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/copy_media_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/copy_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/delete_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/download_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_caption.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_reply_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_inline_text.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_caption.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_reply_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/edit_message_text.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/forward_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_chat_history.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_chat_history_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_discussion_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_discussion_replies.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_discussion_replies_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_media_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/get_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/inline_session.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/read_chat_history.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/retract_vote.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_global.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_global_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/search_messages_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_animation.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_cached_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_chat_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_dice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_media_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_reaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_sticker.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_venue.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_video_note.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/send_voice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/stop_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/stream_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/messages/vote_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/change_cloud_password.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/enable_cloud_password.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/password/remove_cloud_password.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/add_sticker_to_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/create_sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/stickers/get_sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/block_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/delete_profile_photos.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_chat_photos.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_chat_photos_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_common_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_default_emoji_statuses.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_me.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/get_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/set_emoji_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/set_profile_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/set_username.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/unblock_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/users/update_profile.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/add_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/compose.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/export_session_string.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/idle.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/remove_handler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/restart.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/run.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/start.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/stop.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/methods/utilities/stop_transmission.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/mime_types.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/html.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/markdown.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/parser.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/parser/utils.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/all.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/all.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/access_point_rule.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/access_point_rule.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/account_days_ttl.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/account_days_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/app_web_view_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/app_web_view_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bot.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bot.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bot_icon.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bot_icon.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bot_icon_color.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bot_icon_color.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bots.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bots.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_bots_bot.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_bots_bot.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/attach_menu_peer_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/attach_menu_peer_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/authorization.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/authorization.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/auto_download_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/auto_download_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/auto_save_exception.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/auto_save_exception.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/auto_save_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/auto_save_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/available_reaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/available_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bad_msg_notification.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bad_msg_notification.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bank_card_open_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bank_card_open_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/base_theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/base_theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bind_auth_key_inner.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bind_auth_key_inner.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_app.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_app.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_command.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_command_scope.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_inline_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_inline_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_inline_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/bot_menu_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/bot_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/cdn_config.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/cdn_config.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/cdn_public_key.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/cdn_public_key.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_admin_log_event.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_admin_log_event.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_admin_log_event_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_admin_log_event_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_admin_log_events_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_admin_log_events_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_messages_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/channel_participants_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/channel_participants_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_admin_rights.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_admin_rights.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_admin_with_invites.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_admin_with_invites.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_banned_rights.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_banned_rights.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_full.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_full.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_invite_importer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_invite_importer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_onlines.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_onlines.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/chat_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/client_dh_inner_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/client_dh_inner_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/code_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/code_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/config.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/config.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/contact_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/contact_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/data_json.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/data_json.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dc_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dc_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/default_history_ttl.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/default_history_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/destroy_auth_key_res.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/destroy_auth_key_res.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/destroy_session_res.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/destroy_session_res.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog_filter_suggested.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog_filter_suggested.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/dialog_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/dialog_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/document_attribute.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/document_attribute.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/draft_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/draft_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/email_verification.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/email_verification.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/email_verify_purpose.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/email_verify_purpose.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_keyword.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_keyword.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_keywords_difference.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_keywords_difference.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_language.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_language.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_list.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/emoji_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/emoji_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/encrypted_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/encrypted_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/encrypted_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/encrypted_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/encrypted_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/encrypted_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_chat_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_chat_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_chatlist_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_chatlist_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_contact_token.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_contact_token.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/exported_message_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/exported_message_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/file_hash.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/file_hash.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/folder.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/folder.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/folder_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/folder_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/geo_point.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/geo_point.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/global_privacy_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/global_privacy_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_participant_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_participant_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_participant_video_source_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_participant_video_source_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/group_call_stream_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/group_call_stream_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/high_score.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/high_score.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/http_wait.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/http_wait.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/imported_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/imported_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/inline_bot_switch_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/inline_bot_switch_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/inline_bot_web_view.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/inline_bot_web_view.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/inline_query_peer_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/inline_query_peer_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_app_event.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_app_event.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_app.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_app.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_inline_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_inline_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_inline_message_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_inline_message_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_bot_inline_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_bot_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_chat_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_chatlist.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_chatlist.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_check_password_srp.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_check_password_srp.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_client_proxy.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_client_proxy.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_dialog_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_dialog_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_encrypted_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_encrypted_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_encrypted_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_encrypted_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_folder_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_folder_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_geo_point.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_geo_point.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_invoice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_invoice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_notify_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_notify_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_payment_credentials.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_payment_credentials.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_peer_notify_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_peer_notify_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_privacy_key.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_privacy_key.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_privacy_rule.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_privacy_rule.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_secure_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_secure_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_secure_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_secure_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_single_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_single_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_sticker_set_item.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_sticker_set_item.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_stickered_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_stickered_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_store_payment_purpose.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_store_payment_purpose.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_theme_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_theme_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_wall_paper.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_wall_paper.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_web_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_web_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/input_web_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/input_web_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/invoice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/invoice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/ip_port.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/ip_port.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/json_object_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/json_object_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/json_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/json_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/keyboard_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/keyboard_button_row.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/keyboard_button_row.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/labeled_price.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/labeled_price.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/lang_pack_difference.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/lang_pack_difference.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/lang_pack_language.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/lang_pack_language.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/lang_pack_string.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/lang_pack_string.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/mask_coords.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/mask_coords.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_entity.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_extended_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_extended_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_fwd_header.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_fwd_header.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_interaction_counters.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_interaction_counters.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_peer_reaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_peer_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_range.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_range.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_replies.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_replies.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_reply_header.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_reply_header.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_user_vote.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_user_vote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/message_views.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/message_views.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/messages_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msg_detailed_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msg_detailed_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msg_resend_req.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msg_resend_req.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_ack.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_ack.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_all_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_all_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_state_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_state_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/msgs_state_req.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/msgs_state_req.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/nearest_dc.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/nearest_dc.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/new_session.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/new_session.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/notification_sound.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/notification_sound.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/notify_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/notify_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/null.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/null.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_block.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_block.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_caption.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_caption.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_list_item.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_list_item.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_list_ordered_item.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_list_ordered_item.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_related_article.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_related_article.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_table_cell.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_table_cell.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/page_table_row.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/page_table_row.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/password_kdf_algo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/password_kdf_algo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_charge.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_charge.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_form_method.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_form_method.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_requested_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_requested_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/payment_saved_credentials.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/payment_saved_credentials.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_blocked.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_blocked.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_located.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_located.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_notify_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_notify_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/peer_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/peer_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_call_discard_reason.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_call_discard_reason.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_call_protocol.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_call_protocol.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/phone_connection.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/phone_connection.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/photo_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/photo_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll_answer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll_answer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll_answer_voters.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll_answer_voters.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/poll_results.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/poll_results.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/pong.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/pong.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/popular_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/popular_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/post_address.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/post_address.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/pq_inner_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/pq_inner_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/premium_gift_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/premium_gift_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/premium_subscription_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/premium_subscription_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/privacy_key.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/privacy_key.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/privacy_rule.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/privacy_rule.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/reaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/reaction_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/reaction_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/read_participant_date.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/read_participant_date.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/received_notify_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/received_notify_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/recent_me_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/recent_me_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/reply_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/reply_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/report_reason.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/report_reason.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/request_peer_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/request_peer_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/res_pq.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/res_pq.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/restriction_reason.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/restriction_reason.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rich_text.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rich_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rpc_drop_answer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rpc_drop_answer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rpc_error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/rpc_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/rpc_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/saved_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/saved_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/search_results_calendar_period.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/search_results_calendar_period.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/search_results_position.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/search_results_position.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_credentials_encrypted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_credentials_encrypted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_password_kdf_algo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_password_kdf_algo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_plain_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_plain_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_required_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_required_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_secret_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_secret_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value_error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value_error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value_hash.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value_hash.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/secure_value_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/secure_value_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/send_as_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/send_as_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/send_message_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/send_message_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/server_dh_inner_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/server_dh_inner_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/server_dh_params.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/server_dh_params.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/set_client_dh_params_answer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/set_client_dh_params_answer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/shipping_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/shipping_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/simple_web_view_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/simple_web_view_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sponsored_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sponsored_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_abs_value_and_prev.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_abs_value_and_prev.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_date_range_days.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_date_range_days.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_graph.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_graph.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_group_top_admin.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_group_top_admin.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_group_top_inviter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_group_top_inviter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_group_top_poster.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_group_top_poster.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_percent_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_percent_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/stats_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/stats_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_keyword.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_keyword.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_pack.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/sticker_set_covered.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/sticker_set_covered.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/text_with_entities.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/text_with_entities.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/theme_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/theme_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/top_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/top_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/top_peer_category.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/top_peer_category.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/top_peer_category_peers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/top_peer_category_peers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/update.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/update.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/updates_t.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/updates_t.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/url_auth_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/url_auth_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user_full.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user_full.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user_profile_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/user_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/user_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/username.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/video_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/video_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/wall_paper.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/wall_paper.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/wall_paper_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/wall_paper_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_authorization.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_authorization.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_page_attribute.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_page_attribute.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_view_message_sent.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_view_message_sent.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/base/web_view_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/base/web_view_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/future_salt.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/future_salts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/gzip_packed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/list.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/msg_container.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/bool.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/bytes.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/double.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/int.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/string.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/primitives/vector.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/core/tl_object.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/destroy_auth_key.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/destroy_auth_key.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/destroy_session.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/destroy_session.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/get_future_salts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/get_future_salts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/init_connection.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/init_connection.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_after_msg.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_after_msg.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_after_msgs.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_after_msgs.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_with_layer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_with_layer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_with_messages_range.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_with_messages_range.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_with_takeout.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_with_takeout.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/invoke_without_updates.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/invoke_without_updates.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/ping.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/ping.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/ping_delay_disconnect.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/ping_delay_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/req_dh_params.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/req_dh_params.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/req_pq.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/req_pq.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/req_pq_multi.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/req_pq_multi.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/rpc_drop_answer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/rpc_drop_answer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/functions/set_client_dh_params.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/functions/set_client_dh_params.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/access_point_rule.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/access_point_rule.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/account_days_ttl.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/account_days_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/app_web_view_result_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/app_web_view_result_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bot.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bot.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bot_icon.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bot_icon.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bot_icon_color.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bot_icon_color.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bots.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bots.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bots_bot.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bots_bot.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_bots_not_modified.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_bots_not_modified.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_bot_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_bot_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_broadcast.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_broadcast.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/attach_menu_peer_type_same_bot_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/attach_menu_peer_type_same_bot_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/authorization.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/authorization.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/auto_download_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/auto_download_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/auto_save_exception.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/auto_save_exception.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/auto_save_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/auto_save_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/available_reaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/available_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bad_msg_notification.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bad_msg_notification.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bad_server_salt.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bad_server_salt.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bank_card_open_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bank_card_open_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_arctic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_arctic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_classic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_classic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_day.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_day.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_night.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_night.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/base_theme_tinted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/base_theme_tinted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bind_auth_key_inner.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bind_auth_key_inner.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_app.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_app.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_app_not_modified.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_app_not_modified.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_chat_admins.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_chat_admins.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_default.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_peer_admins.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_peer_admins.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_peer_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_peer_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_command_scope_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_command_scope_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_media_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_media_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_auto.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_auto.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_geo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_geo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_invoice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_invoice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_media_venue.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_media_venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_message_text.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_inline_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_menu_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_menu_button_commands.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/bot_menu_button_default.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/bot_menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/cdn_config.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/cdn_config.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/cdn_public_key.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/cdn_public_key.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_about.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_about.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_available_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_available_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_history_ttl.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_history_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_linked_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_linked_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_title.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_title.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_username.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_change_usernames.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_change_usernames.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_create_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_create_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_default_banned_rights.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_default_banned_rights.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_delete_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_delete_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_delete_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_delete_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_discard_group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_discard_group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_edit_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_edit_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_edit_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_edit_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_delete.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_delete.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_edit.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_edit.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_revoke.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_exported_invite_revoke.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_join.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_join.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_join_by_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_leave.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_leave.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_mute.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_mute.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_admin.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_admin.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_ban.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_toggle_ban.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_unmute.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_unmute.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_participant_volume.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_participant_volume.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_pin_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_pin_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_send_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_send_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_start_group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_start_group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_stop_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_stop_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_anti_spam.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_anti_spam.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_forum.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_forum.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_group_call_setting.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_group_call_setting.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_invites.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_invites.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_no_forwards.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_no_forwards.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_pre_history_hidden.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_pre_history_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_signatures.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_signatures.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_toggle_slow_mode.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_toggle_slow_mode.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_event_action_update_pinned.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_event_action_update_pinned.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_admin_log_events_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_admin_log_events_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_forbidden.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_forbidden.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_full.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_full.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_location_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_location_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_messages_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_messages_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_messages_filter_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_messages_filter_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_admin.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_admin.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_banned.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_banned.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_creator.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_creator.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_left.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_left.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participant_self.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participant_self.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_admins.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_admins.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_banned.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_banned.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_bots.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_bots.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_kicked.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_kicked.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_mentions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_mentions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_recent.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_recent.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/channel_participants_search.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/channel_participants_search.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_admin_rights.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_admin_rights.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_admin_with_invites.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_admin_with_invites.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_banned_rights.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_banned_rights.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_forbidden.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_forbidden.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_full.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_full.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_already.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_already.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_exported.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_exported.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_importer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_importer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_peek.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_peek.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_invite_public_join_requests.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_invite_public_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_onlines.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_onlines.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participant_admin.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participant_admin.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participant_creator.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participant_creator.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_participants_forbidden.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_participants_forbidden.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_photo_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_photo_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_reactions_all.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_reactions_all.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_reactions_none.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_reactions_none.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/chat_reactions_some.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/chat_reactions_some.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/client_dh_inner_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/client_dh_inner_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/code_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/code_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/config.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/config.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/contact_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/contact_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/data_json.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/data_json.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dc_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dc_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/default_history_ttl.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/default_history_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_auth_key_fail.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_auth_key_fail.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_auth_key_none.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_auth_key_none.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_auth_key_ok.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_auth_key_ok.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_session_none.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_session_none.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/destroy_session_ok.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/destroy_session_ok.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dh_gen_fail.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dh_gen_fail.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dh_gen_ok.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dh_gen_ok.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dh_gen_retry.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dh_gen_retry.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter_chatlist.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter_chatlist.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter_default.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter_default.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_filter_suggested.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_filter_suggested.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_folder.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_folder.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/dialog_peer_folder.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/dialog_peer_folder.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_animated.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_animated.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_custom_emoji.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_custom_emoji.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_filename.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_filename.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_has_stickers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_has_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_image_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_image_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_sticker.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_attribute_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_attribute_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/document_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/document_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/draft_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/draft_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/draft_message_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/draft_message_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verification_apple.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verification_apple.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verification_code.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verification_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verification_google.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verification_google.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verify_purpose_login_change.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verify_purpose_login_change.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verify_purpose_login_setup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verify_purpose_login_setup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/email_verify_purpose_passport.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/email_verify_purpose_passport.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_keyword.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_keyword.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_keyword_deleted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_keyword_deleted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_keywords_difference.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_keywords_difference.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_language.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_language.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_list.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_list_not_modified.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_list_not_modified.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_status_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_status_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_status_until.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_status_until.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/emoji_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/emoji_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_discarded.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_discarded.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_requested.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_requested.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_chat_waiting.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_chat_waiting.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_file_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_file_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/encrypted_message_service.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/encrypted_message_service.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/exported_chatlist_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/exported_chatlist_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/exported_contact_token.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/exported_contact_token.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/exported_message_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/exported_message_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/file_hash.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/file_hash.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/folder.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/folder.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/folder_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/folder_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/forum_topic_deleted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/forum_topic_deleted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/geo_point.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/geo_point.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/geo_point_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/geo_point_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/global_privacy_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/global_privacy_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_discarded.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_discarded.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_participant_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_participant_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_participant_video_source_group.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_participant_video_source_group.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/group_call_stream_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/group_call_stream_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/high_score.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/high_score.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/http_wait.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/http_wait.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/imported_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/imported_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_bot_switch_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_bot_switch_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_bot_web_view.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_bot_web_view.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_bot_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_bot_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_broadcast.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_broadcast.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_megagroup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_megagroup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/inline_query_peer_type_same_bot_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/inline_query_peer_type_same_bot_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_app_event.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_app_event.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_app_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_app_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_app_short_name.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_app_short_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_id64.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_id64.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_auto.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_auto.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_geo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_geo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_invoice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_invoice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_media_venue.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_media_venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_message_text.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_message_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_bot_inline_result_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_bot_inline_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_channel_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_channel_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_channel_from_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_channel_from_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chat_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chat_photo_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chat_photo_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chat_uploaded_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chat_uploaded_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_chatlist_dialog_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_chatlist_dialog_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_check_password_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_check_password_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_check_password_srp.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_check_password_srp.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_client_proxy.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_client_proxy.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_dialog_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_dialog_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_dialog_peer_folder.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_dialog_peer_folder.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_document_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_document_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_document_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_document_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_big_uploaded.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_big_uploaded.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_encrypted_file_uploaded.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_encrypted_file_uploaded.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_file_big.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_file_big.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_folder_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_folder_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_game_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_game_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_game_short_name.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_game_short_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_geo_point.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_geo_point.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_geo_point_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_geo_point_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_group_call_stream.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_group_call_stream.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_invoice_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_invoice_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_invoice_slug.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_invoice_slug.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_keyboard_button_url_auth.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_keyboard_button_url_auth.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_keyboard_button_user_profile.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_keyboard_button_user_profile.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_dice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_dice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_document_external.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_document_external.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_geo_live.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_geo_live.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_geo_point.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_geo_point.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_invoice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_invoice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_photo_external.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_photo_external.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_uploaded_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_uploaded_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_uploaded_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_uploaded_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_media_venue.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_media_venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_callback_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_entity_mention_name.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_entity_mention_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_pinned.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_pinned.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_message_reply_to.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_message_reply_to.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_chat_photos.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_chat_photos.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_geo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_geo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_gif.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_gif.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_music.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_music.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_my_mentions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_my_mentions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_phone_calls.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_phone_calls.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_photo_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_photo_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_photos.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_photos.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_pinned.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_pinned.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_round_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_round_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_round_voice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_round_voice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_messages_filter_voice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_messages_filter_voice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_broadcasts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_broadcasts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_notify_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_notify_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials_apple_pay.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials_apple_pay.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials_google_pay.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials_google_pay.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_payment_credentials_saved.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_payment_credentials_saved.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_channel_from_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_channel_from_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_notify_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_notify_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_photo_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_photo_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_self.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_self.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_peer_user_from_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_peer_user_from_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_phone_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_photo_legacy_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_photo_legacy_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_added_by_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_added_by_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_chat_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_chat_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_forwards.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_forwards.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_phone_number.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_phone_number.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_phone_p2_p.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_phone_p2_p.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_profile_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_status_timestamp.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_status_timestamp.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_key_voice_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_key_voice_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_all.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_all.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_chat_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_chat_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_allow_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_allow_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_all.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_all.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_chat_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_chat_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_privacy_value_disallow_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_privacy_value_disallow_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_child_abuse.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_child_abuse.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_copyright.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_copyright.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_fake.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_fake.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_geo_irrelevant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_geo_irrelevant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_illegal_drugs.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_illegal_drugs.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_other.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_other.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_personal_details.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_personal_details.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_pornography.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_pornography.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_spam.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_spam.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_report_reason_violence.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_report_reason_violence.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_file_uploaded.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_file_uploaded.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_secure_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_secure_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_single_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_single_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_animated_emoji.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_animated_emoji.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_animated_emoji_animations.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_animated_emoji_animations.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_dice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_dice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_emoji_default_statuses.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_emoji_default_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_emoji_default_topic_icons.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_emoji_default_topic_icons.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_emoji_generic_animations.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_emoji_generic_animations.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_item.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_item.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_premium_gifts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_premium_gifts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_short_name.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_short_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_sticker_set_thumb.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_sticker_set_thumb.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_stickered_media_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_stickered_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_stickered_media_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_stickered_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_store_payment_gift_premium.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_store_payment_gift_premium.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_store_payment_premium_subscription.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_store_payment_premium_subscription.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_takeout_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_takeout_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_theme_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_theme_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_theme_slug.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_theme_slug.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user_from_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user_from_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_user_self.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_user_self.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_wall_paper.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_wall_paper.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_wall_paper_no_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_wall_paper_no_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_wall_paper_slug.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_wall_paper_slug.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_file_audio_album_thumb_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_file_audio_album_thumb_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_file_geo_point_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_file_geo_point_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/input_web_file_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/input_web_file_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/invoice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/invoice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/ip_port.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/ip_port.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/ip_port_secret.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/ip_port_secret.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_array.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_array.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_bool.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_bool.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_null.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_null.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_number.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_number.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_object.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_object.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_object_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_object_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/json_string.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/json_string.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_buy.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_buy.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_callback.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_callback.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_geo_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_geo_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_request_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_request_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_row.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_row.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_simple_web_view.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_simple_web_view.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_switch_inline.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_switch_inline.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_url_auth.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_url_auth.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_user_profile.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_user_profile.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/keyboard_button_web_view.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/keyboard_button_web_view.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/labeled_price.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/labeled_price.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_difference.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_difference.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_language.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_language.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_string.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_string.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_string_deleted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_string_deleted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/lang_pack_string_pluralized.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/lang_pack_string_pluralized.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/mask_coords.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/mask_coords.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_bot_allowed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_bot_allowed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_channel_create.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_channel_create.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_channel_migrate_from.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_channel_migrate_from.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_add_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_add_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_create.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_create.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_delete_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_delete_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_delete_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_delete_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_edit_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_edit_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_edit_title.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_edit_title.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_joined_by_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_joined_by_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_joined_by_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_chat_migrate_to.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_chat_migrate_to.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_contact_sign_up.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_contact_sign_up.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_custom_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_custom_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_game_score.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_game_score.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_geo_proximity_reached.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_geo_proximity_reached.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_gift_premium.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_gift_premium.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_group_call_scheduled.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_group_call_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_history_clear.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_history_clear.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_invite_to_group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_invite_to_group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_payment_sent.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_payment_sent.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_payment_sent_me.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_payment_sent_me.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_pin_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_pin_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_requested_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_requested_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_screenshot_taken.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_screenshot_taken.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_secure_values_sent.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_secure_values_sent.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_secure_values_sent_me.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_secure_values_sent_me.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_chat_theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_chat_theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_chat_wall_paper.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_chat_wall_paper.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_messages_ttl.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_messages_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_set_same_chat_wall_paper.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_set_same_chat_wall_paper.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_suggest_profile_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_suggest_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_topic_create.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_topic_create.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_topic_edit.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_topic_edit.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_web_view_data_sent.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_web_view_data_sent.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_action_web_view_data_sent_me.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_action_web_view_data_sent_me.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_bank_card.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_bank_card.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_blockquote.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_blockquote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_bold.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_bold.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_bot_command.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_cashtag.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_cashtag.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_code.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_custom_emoji.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_custom_emoji.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_email.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_email.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_hashtag.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_hashtag.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_italic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_italic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_mention.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_mention.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_mention_name.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_mention_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_pre.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_pre.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_spoiler.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_spoiler.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_strike.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_strike.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_text_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_text_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_underline.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_underline.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_unknown.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_unknown.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_entity_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_entity_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_extended_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_extended_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_extended_media_preview.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_extended_media_preview.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_fwd_header.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_fwd_header.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_interaction_counters.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_interaction_counters.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_dice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_dice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_geo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_geo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_geo_live.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_geo_live.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_invoice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_invoice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_unsupported.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_unsupported.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_venue.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_media_web_page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_media_web_page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_peer_reaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_peer_reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_range.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_range.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_replies.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_replies.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_reply_header.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_reply_header.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_service.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_service.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_user_vote.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_user_vote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_user_vote_input_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_user_vote_input_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_user_vote_multiple.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_user_vote_multiple.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/message_views.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/message_views.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_detailed_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_detailed_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_new_detailed_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_new_detailed_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_resend_ans_req.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_resend_ans_req.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msg_resend_req.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msg_resend_req.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_ack.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_ack.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_all_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_all_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_state_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_state_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/msgs_state_req.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/msgs_state_req.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/nearest_dc.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/nearest_dc.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/new_session_created.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/new_session_created.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_default.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_default.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_local.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_local.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_none.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_none.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notification_sound_ringtone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notification_sound_ringtone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_broadcasts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_broadcasts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/notify_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/notify_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/null.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/null.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_anchor.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_anchor.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_author_date.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_author_date.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_blockquote.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_blockquote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_collage.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_collage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_cover.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_cover.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_details.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_details.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_divider.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_divider.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_embed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_embed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_embed_post.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_embed_post.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_footer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_footer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_header.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_header.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_kicker.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_kicker.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_list.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_map.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_map.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_ordered_list.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_ordered_list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_paragraph.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_paragraph.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_preformatted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_preformatted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_pullquote.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_pullquote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_related_articles.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_related_articles.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_slideshow.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_slideshow.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_subheader.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_subheader.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_subtitle.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_subtitle.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_table.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_table.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_title.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_title.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_unsupported.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_unsupported.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_block_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_block_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_caption.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_caption.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_item_blocks.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_item_blocks.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_item_text.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_item_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_ordered_item_blocks.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_ordered_item_blocks.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_list_ordered_item_text.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_list_ordered_item_text.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_related_article.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_related_article.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_table_cell.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_table_cell.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/page_table_row.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/page_table_row.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/password_kdf_algo_sha256_sha256_pbkdf2_hmacsha512iter100000_sha256_mod_pow.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/password_kdf_algo_sha256_sha256_pbkdf2_hmacsha512iter100000_sha256_mod_pow.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/password_kdf_algo_unknown.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/password_kdf_algo_unknown.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_charge.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_charge.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_form_method.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_form_method.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_requested_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_requested_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/payment_saved_credentials_card.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/payment_saved_credentials_card.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_blocked.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_blocked.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_located.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_located.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_notify_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_notify_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_self_located.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_self_located.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/peer_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/peer_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_accepted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_accepted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_busy.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_busy.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_disconnect.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_disconnect.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_hangup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_hangup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discard_reason_missed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discard_reason_missed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_discarded.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_discarded.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_protocol.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_protocol.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_requested.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_requested.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_call_waiting.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_call_waiting.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_connection.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_connection.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/phone_connection_webrtc.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/phone_connection_webrtc.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_cached_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_cached_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_path_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_path_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_size_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_size_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_size_progressive.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_size_progressive.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/photo_stripped_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/photo_stripped_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll_answer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll_answer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll_answer_voters.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll_answer_voters.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/poll_results.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/poll_results.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pong.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pong.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/popular_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/popular_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/post_address.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/post_address.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data_dc.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data_dc.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data_temp.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data_temp.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/pq_inner_data_temp_dc.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/pq_inner_data_temp_dc.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/premium_gift_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/premium_gift_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/premium_subscription_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/premium_subscription_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_added_by_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_added_by_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_chat_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_chat_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_forwards.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_forwards.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_phone_number.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_phone_number.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_phone_p2_p.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_phone_p2_p.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_profile_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_status_timestamp.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_status_timestamp.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_key_voice_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_key_voice_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_all.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_all.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_chat_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_chat_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_allow_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_allow_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_all.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_all.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_chat_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_chat_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_contacts.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_contacts.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/privacy_value_disallow_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/privacy_value_disallow_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_count.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_count.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_custom_emoji.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_custom_emoji.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_emoji.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_emoji.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reaction_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reaction_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/read_participant_date.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/read_participant_date.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/received_notify_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/received_notify_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_chat_invite.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_chat_invite.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_unknown.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_unknown.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/recent_me_url_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/recent_me_url_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_inline_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_inline_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_keyboard_force_reply.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_keyboard_force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_keyboard_hide.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_keyboard_hide.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/reply_keyboard_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/request_peer_type_broadcast.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/request_peer_type_broadcast.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/request_peer_type_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/request_peer_type_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/request_peer_type_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/request_peer_type_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/res_pq.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/res_pq.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/restriction_reason.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/restriction_reason.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_answer_dropped.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_answer_dropped.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_answer_dropped_running.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_answer_dropped_running.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_answer_unknown.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_answer_unknown.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/rpc_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/rpc_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/saved_phone_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/saved_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/search_result_position.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/search_result_position.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/search_results_calendar_period.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/search_results_calendar_period.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_credentials_encrypted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_credentials_encrypted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_file_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_file_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_password_kdf_algo_pbkdf2_hmacsha512iter100000.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_password_kdf_algo_pbkdf2_hmacsha512iter100000.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_password_kdf_algo_sha512.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_password_kdf_algo_sha512.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_password_kdf_algo_unknown.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_password_kdf_algo_unknown.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_plain_email.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_plain_email.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_plain_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_plain_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_required_type.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_required_type.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_required_type_one_of.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_required_type_one_of.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_secret_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_secret_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_files.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_files.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_front_side.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_front_side.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_reverse_side.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_reverse_side.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_selfie.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_selfie.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_translation_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_translation_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_error_translation_files.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_error_translation_files.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_hash.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_hash.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_address.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_address.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_bank_statement.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_bank_statement.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_driver_license.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_driver_license.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_email.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_email.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_identity_card.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_identity_card.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_internal_passport.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_internal_passport.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_passport.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_passport.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_passport_registration.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_passport_registration.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_personal_details.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_personal_details.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_rental_agreement.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_rental_agreement.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_temporary_registration.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_temporary_registration.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/secure_value_type_utility_bill.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/secure_value_type_utility_bill.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_as_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_as_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_cancel_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_cancel_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_choose_contact_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_choose_contact_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_choose_sticker_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_choose_sticker_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_emoji_interaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_emoji_interaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_emoji_interaction_seen.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_emoji_interaction_seen.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_game_play_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_game_play_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_geo_location_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_geo_location_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_history_import_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_history_import_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_record_audio_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_record_audio_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_record_round_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_record_round_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_record_video_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_record_video_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_typing_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_typing_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_audio_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_audio_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_document_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_document_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_photo_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_photo_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_round_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_round_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/send_message_upload_video_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/send_message_upload_video_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/server_dh_inner_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/server_dh_inner_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/server_dh_params_fail.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/server_dh_params_fail.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/server_dh_params_ok.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/server_dh_params_ok.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/shipping_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/shipping_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/simple_web_view_result_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/simple_web_view_result_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/speaking_in_group_call_action.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/speaking_in_group_call_action.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sponsored_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sponsored_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_abs_value_and_prev.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_abs_value_and_prev.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_date_range_days.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_date_range_days.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_graph.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_graph.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_graph_async.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_graph_async.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_graph_error.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_graph_error.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_group_top_admin.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_group_top_admin.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_group_top_inviter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_group_top_inviter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_group_top_poster.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_group_top_poster.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_percent_value.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_percent_value.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/stats_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/stats_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_keyword.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_keyword.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_pack.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_covered.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_covered.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_full_covered.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_full_covered.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_multi_covered.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_multi_covered.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/sticker_set_no_covered.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/sticker_set_no_covered.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_anchor.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_anchor.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_bold.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_bold.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_concat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_concat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_email.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_email.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_fixed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_fixed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_image.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_image.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_italic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_italic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_marked.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_marked.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_plain.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_plain.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_strike.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_strike.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_subscript.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_subscript.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_superscript.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_superscript.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_underline.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_underline.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/text_with_entities.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/text_with_entities.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/theme_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/theme_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_bots_inline.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_bots_inline.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_bots_pm.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_bots_pm.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_channels.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_channels.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_correspondents.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_correspondents.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_forward_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_forward_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_forward_users.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_forward_users.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_groups.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_groups.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_peers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_peers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/top_peer_category_phone_calls.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/top_peer_category_phone_calls.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_attach_menu_bots.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_attach_menu_bots.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_auto_save_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_auto_save_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_callback_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_chat_invite_requester.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_chat_invite_requester.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_commands.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_inline_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_inline_send.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_inline_send.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_menu_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_precheckout_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_precheckout_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_shipping_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_shipping_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_stopped.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_stopped.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_webhook_json.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_webhook_json.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_bot_webhook_json_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_bot_webhook_json_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_available_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_available_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_message_forwards.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_message_forwards.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_message_views.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_message_views.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_pinned_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_pinned_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_pinned_topics.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_pinned_topics.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_read_messages_contents.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_read_messages_contents.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_too_long.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_too_long.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_user_typing.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_user_typing.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_channel_web_page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_channel_web_page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_default_banned_rights.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_default_banned_rights.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant_add.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant_add.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant_admin.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant_admin.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participant_delete.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participant_delete.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_chat_user_typing.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_chat_user_typing.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_config.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_config.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_contacts_reset.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_contacts_reset.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dc_options.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dc_options.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_delete_channel_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_delete_channel_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_delete_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_delete_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_delete_scheduled_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_delete_scheduled_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_filter_order.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_filter_order.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_filters.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_filters.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_pinned.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_pinned.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_dialog_unread_mark.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_dialog_unread_mark.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_draft_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_draft_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_edit_channel_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_edit_channel_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_edit_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_edit_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_encrypted_chat_typing.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_encrypted_chat_typing.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_encrypted_messages_read.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_encrypted_messages_read.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_encryption.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_encryption.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_faved_stickers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_faved_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_folder_peers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_folder_peers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_geo_live_viewed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_geo_live_viewed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_call_connection.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_call_connection.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_call_participants.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_call_participants.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_group_invite_privacy_forbidden.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_group_invite_privacy_forbidden.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_inline_bot_callback_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_inline_bot_callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_lang_pack.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_lang_pack.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_lang_pack_too_long.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_lang_pack_too_long.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_login_token.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_login_token.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_extended_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_extended_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_poll_vote.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_poll_vote.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_message_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_move_sticker_set_to_top.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_move_sticker_set_to_top.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_channel_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_channel_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_encrypted_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_encrypted_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_scheduled_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_scheduled_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_new_sticker_set.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_new_sticker_set.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_notify_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_notify_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_blocked.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_blocked.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_history_ttl.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_history_ttl.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_located.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_located.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_peer_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_peer_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pending_join_requests.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pending_join_requests.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_phone_call.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_phone_call.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_phone_call_signaling_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_phone_call_signaling_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pinned_channel_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pinned_channel_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pinned_dialogs.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pinned_dialogs.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pinned_messages.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pinned_messages.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_privacy.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_privacy.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_pts_changed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_pts_changed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_discussion_inbox.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_discussion_inbox.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_discussion_outbox.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_discussion_outbox.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_inbox.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_inbox.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_channel_outbox.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_channel_outbox.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_featured_emoji_stickers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_featured_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_featured_stickers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_featured_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_history_inbox.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_history_inbox.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_history_outbox.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_history_outbox.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_read_messages_contents.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_read_messages_contents.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_recent_emoji_statuses.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_recent_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_recent_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_recent_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_recent_stickers.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_recent_stickers.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_saved_gifs.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_saved_gifs.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_saved_ringtones.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_saved_ringtones.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_service_notification.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_service_notification.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short_chat_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short_chat_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_short_sent_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_short_sent_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_sticker_sets.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_sticker_sets.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_sticker_sets_order.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_sticker_sets_order.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_transcribed_audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_transcribed_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_emoji_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_name.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_name.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_phone.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_phone.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_user_typing.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_user_typing.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_web_page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_web_page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/update_web_view_result_sent.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/update_web_view_result_sent.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/updates_combined.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/updates_combined.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/updates_t.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/updates_t.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/updates_too_long.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/updates_too_long.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/url_auth_result_accepted.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/url_auth_result_accepted.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/url_auth_result_default.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/url_auth_result_default.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/url_auth_result_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/url_auth_result_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_full.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_full.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_profile_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_profile_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_profile_photo_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_profile_photo_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_last_month.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_last_month.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_last_week.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_last_week.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_offline.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_offline.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_online.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_online.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/user_status_recently.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/user_status_recently.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/username.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/video_size.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/video_size.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/video_size_emoji_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/video_size_emoji_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/video_size_sticker_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/video_size_sticker_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/wall_paper.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/wall_paper.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/wall_paper_no_file.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/wall_paper_no_file.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/wall_paper_settings.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/wall_paper_settings.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_authorization.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_authorization.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_document_no_proxy.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_document_no_proxy.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_attribute_theme.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_attribute_theme.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_empty.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_empty.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_not_modified.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_not_modified.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_page_pending.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_page_pending.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_view_message_sent.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_view_message_sent.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/raw/types/web_view_result_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/raw/types/web_view_result_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/auth.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/data_center.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/msg_factory.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/msg_id.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/internals/seq_no.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/session/session.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/file_storage.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/memory_storage.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/mongo_storage.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/sqlite_storage.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/storage/storage.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/sync.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/authorization/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/authorization/sent_code.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/authorization/terms_of_service.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/callback_game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/callback_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/force_reply.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/game_high_score.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/login_url.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/bots_and_keyboards/web_app_info.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/chosen_inline_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_animation.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_article.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_venue.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/inline_mode/inline_query_result_voice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_animation.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_media_video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_media/input_phone_contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_message_content/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_message_content/input_message_content.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/input_message_content/input_text_message_content.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/list.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/animation.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/audio.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/contact.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/dice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/document.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/game.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/location.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/message.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/message_entity.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/message_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/poll.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/poll_option.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/reaction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/sticker.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/stickerset.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/thumbnail.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/venue.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/video.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/video_note.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/voice.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/web_app_data.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/messages_and_media/web_page.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/object.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/update.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/__init__.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_event.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_event_filter.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_invite_link.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_join_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_joiner.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_member.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_member_updated.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_permissions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_photo.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_preview.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_privileges.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/chat_reactions.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/dialog.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/emoji_status.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_closed.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_created.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_edited.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/invite_link_importer.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/peer_channel.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/peer_user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/restriction.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/user.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/username.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_ended.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/types/user_and_chats/video_chat_started.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/pyrogram/utils.py` & `pyrofork_dev-2.1.8.dev202305201705/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `pyrofork_dev-2.1.8.dev202305201658/PKG-INFO` & `pyrofork_dev-2.1.8.dev202305201705/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrofork-dev
-Version: 2.1.8.dev202305201658
+Version: 2.1.8.dev202305201705
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 License: LGPL-3.0-or-later
 Keywords: telegram,chat,messenger,mtproto,api,client,library,python
 Author: Dan
 Author-email: 14043624+delivrance@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyrofork-dev Version: 2.1.8.dev202305201658
+Metadata-Version: 2.1 Name: pyrofork-dev Version: 2.1.8.dev202305201705
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
 License: LGPL-3.0-or-later Keywords:
 telegram,chat,messenger,mtproto,api,client,library,python Author: Dan Author-
 email: 14043624+delivrance@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: GNU Lesser General Public
```

