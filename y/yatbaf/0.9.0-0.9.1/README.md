# Comparing `tmp/yatbaf-0.9.0.tar.gz` & `tmp/yatbaf-0.9.1.tar.gz`

## Comparing `yatbaf-0.9.0.tar` & `yatbaf-0.9.1.tar`

### file list

```diff
@@ -1,352 +1,352 @@
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/__main__.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/abc.py
--rw-r--r--   0        0        0   186998 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/bot.py
--rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/di.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/dispatcher.py
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/enums.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/exceptions.py
--rw-r--r--   0        0        0    43574 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/handler.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/helpers.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/http.py
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/long_polling.py
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/middleware.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/py.typed
--rw-r--r--   0        0        0    28065 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/router.py
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/telegram.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/typing.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/utils.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/version.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/warnings.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/__init__.py
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/base.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/callback_data.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/chat_id.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/command.py
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/content_type.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/text_content.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/filters/user.py
--rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/__init__.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/abc.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/add_sticker_to_set.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/answer_callback_query.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/answer_inline_query.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/answer_pre_checkout_query.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/answer_shipping_query.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/answer_web_app_query.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/approve_chat_join_request.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/ban_chat_member.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/ban_chat_sender_chat.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/close.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/close_forum_topic.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/close_general_forum_topic.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/copy_message.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/copy_messages.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/create_chat_invite_link.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/create_forum_topic.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/create_invoice_link.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/create_new_sticker_set.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/decline_chat_join_request.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_chat_photo.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_chat_sticker_set.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_forum_topic.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_message.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_messages.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_my_commands.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_sticker_from_set.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_sticker_set.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/delete_webhook.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_chat_invite_link.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_forum_topic.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_general_forum_topic.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_message_caption.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_message_live_location.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_message_media.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_message_reply_markup.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/edit_message_text.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/export_chat_invite_link.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/forward_message.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/forward_messages.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_business_connection.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_chat.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_chat_administrators.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_chat_member.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_chat_member_count.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_chat_menu_button.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_custom_emoji_stickers.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_file.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_forum_topic_icon_stickers.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_game_high_scores.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_me.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_my_commands.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_my_default_administrator_rights.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_my_description.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_my_name.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_my_short_description.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_sticker_set.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_updates.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_user_chat_boosts.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_user_profile_photos.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/get_webhook_info.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/hide_general_forum_topic.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/leave_chat.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/log_out.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/pin_chat_message.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/promote_chat_member.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/reopen_forum_topic.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/reopen_general_forum_topic.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/replace_sticker_in_set.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/restrict_chat_member.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/revoke_chat_invite_link.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_animation.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_audio.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_chat_action.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_contact.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_dice.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_document.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_game.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_invoice.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_location.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_media_group.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_message.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_photo.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_poll.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_sticker.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_venue.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_video.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_video_note.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/send_voice.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_chat_administrator_custom_title.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_chat_description.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_chat_menu_button.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_chat_permissions.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_chat_photo.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_chat_sticker_set.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_chat_title.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_custom_emoji_sticker_set_thumbnail.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_game_score.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_message_reaction.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_my_commands.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_my_default_administrator_rights.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_my_description.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_my_name.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_my_short_description.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_passport_data_errors.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_sticker_emoji_list.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_sticker_keywords.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_sticker_mask_position.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_sticker_position_in_set.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_sticker_set_thumbnail.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_sticker_set_title.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/set_webhook.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/stop_message_live_location.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/stop_poll.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/unban_chat_member.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/unban_chat_sender_chat.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/unhide_general_forum_topic.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/unpin_all_chat_messages.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/unpin_all_forum_topic_messages.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/unpin_all_general_forum_topic_messages.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/unpin_chat_message.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/methods/upload_sticker_file.py
--rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/abc.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/animation.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/audio.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/birthdate.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/bot_command.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/bot_command_scope.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/bot_description.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/bot_name.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/bot_short_description.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/business_connection.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/business_intro.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/business_location.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/business_messages_deleted.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/business_opening_hours.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/business_opening_hours_interval.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/callback_game.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/callback_query.py
--rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_administrator_rights.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_boost.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_boost_added.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_boost_removed.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_boost_source.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_boost_updated.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_invite_link.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_join_request.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_location.py
--rw-r--r--   0        0        0     9053 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_member.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_permissions.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_photo.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chat_shared.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/chosen_inline_result.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/contact.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/dice.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/document.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/external_reply_info.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/file.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/force_reply.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/forum_topic.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/forum_topic_closed.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/forum_topic_created.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/forum_topic_edited.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/forum_topic_reopened.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/game.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/game_high_score.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/general_forum_topic_hidden.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/general_forum_topic_unhidden.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/giveaway.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/giveaway_completed.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/giveaway_created.py
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/giveaway_winners.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/inaccessible_message.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/inline_keyboard_button.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/inline_keyboard_markup.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/inline_query.py
--rw-r--r--   0        0        0    33883 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/inline_query_result.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_contact_message_content.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_invoce_message_content.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_location_message_content.py
--rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_media.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_message_content.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_sticker.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_text_message_content.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/input_venue_message_content.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/invoice.py
--rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/keyboard_button.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/labeled_price.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/link_preview_options.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/location.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/login_url.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/mask_position.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/maybe_inaccessible_message.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/menu_button.py
--rw-r--r--   0        0        0    55258 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/message.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/message_auto_delete_timer_changed.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/message_entity.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/message_id.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/message_origin.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/message_reaction_count_updated.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/message_reaction_updated.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/order_info.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/passport.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/passport_element_error.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/photo_size.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/poll.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/poll_answer.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/poll_option.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/pre_checkout_query.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/proximity_alert_triggered.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/reaction_count.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/reaction_type.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/reply_keyboard_markup.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/reply_keyboard_remove.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/reply_parameters.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/response_parameters.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/sent_web_app_message.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/shared_user.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/shipping_address.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/shipping_option.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/shipping_query.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/sticker.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/sticker_set.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/story.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/successful_payment.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/switch_inline_query_chosen_chat.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/text_quote.py
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/update.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/user.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/user_chat_boosts.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/user_profile_photos.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/users_shared.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/venue.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/video.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/video_chat_ended.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/video_chat_participants_invited.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/video_chat_scheduled.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/video_chat_started.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/video_note.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/voice.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/web_app_data.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/web_app_info.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/webhook_info.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yatbaf-0.9.0/src/yatbaf/types/write_access_allowed.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/api/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/api/conftest.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/api/test_methods.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/api/test_types.py
--rw-r--r--   0        0        0   555312 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/api/data/api.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/bot/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/bot/test_bot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/client/__init__.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/client/test_http.py
--rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/client/test_telegram.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/di/__init__.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/di/test_cleanup_group.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/di/test_dependency_batches.py
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/di/test_provide.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/di/test_resolve_dependencies.py
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/di/test_utils.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/dispatcher/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/dispatcher/test_dispatcher.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/dispatcher/test_guards.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/dispatcher/test_middleware.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/dispatcher/test_resolve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/__init__.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_chat.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_command.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_compat.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_content.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_logical.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_priority.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_text.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/filters/test_user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/__init__.py
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/test_dependencies.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/test_guards.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/test_handler.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/test_match.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/test_middleware.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/test_priority.py
--rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/handler/test_sorting.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/helpers/test_deeplink.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/helpers/test_markdown.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/helpers/test_parse_command_args.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/long_polling/__init__.py
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/long_polling/test_polling.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/methods/__init__.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/methods/test_attrs.py
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/methods/test_encode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/middleware/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/middleware/test_middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/__init__.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_add_guard.py
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_add_handler.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_add_middleware.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_add_router.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_filters.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_find_handler.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_guards.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_middleware.py
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_parse_handlers.py
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_resolve.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_router.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/router/test_sort_handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/types/__init__.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/types/test_attrs.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/types/test_bot_object.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/types/test_ctx.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/utils/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/utils/test_parse_command.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 yatbaf-0.9.0/tests/utils/test_wrap_middleware.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 yatbaf-0.9.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 yatbaf-0.9.0/LICENSE
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 yatbaf-0.9.0/README.md
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 yatbaf-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 yatbaf-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/__main__.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/abc.py
+-rw-r--r--   0        0        0   186998 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/bot.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/di.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/dispatcher.py
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/enums.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/exceptions.py
+-rw-r--r--   0        0        0    43574 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/handler.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/helpers.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/http.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/long_polling.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/middleware.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/py.typed
+-rw-r--r--   0        0        0    28065 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/router.py
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/telegram.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/typing.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/utils.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/version.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/warnings.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/__init__.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/base.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/callback_data.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/chat_id.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/command.py
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/content_type.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/text_content.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/filters/user.py
+-rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/__init__.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/abc.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/add_sticker_to_set.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/answer_callback_query.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/answer_inline_query.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/answer_pre_checkout_query.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/answer_shipping_query.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/answer_web_app_query.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/approve_chat_join_request.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/ban_chat_member.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/ban_chat_sender_chat.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/close.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/close_forum_topic.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/close_general_forum_topic.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/copy_message.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/copy_messages.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/create_chat_invite_link.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/create_forum_topic.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/create_invoice_link.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/create_new_sticker_set.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/decline_chat_join_request.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_chat_photo.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_chat_sticker_set.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_forum_topic.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_message.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_messages.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_my_commands.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_sticker_from_set.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_sticker_set.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/delete_webhook.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_chat_invite_link.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_forum_topic.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_general_forum_topic.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_message_caption.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_message_live_location.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_message_media.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_message_reply_markup.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/edit_message_text.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/export_chat_invite_link.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/forward_message.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/forward_messages.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_business_connection.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_chat.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_chat_administrators.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_chat_member.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_chat_member_count.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_chat_menu_button.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_custom_emoji_stickers.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_file.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_forum_topic_icon_stickers.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_game_high_scores.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_me.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_my_commands.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_my_default_administrator_rights.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_my_description.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_my_name.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_my_short_description.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_sticker_set.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_updates.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_user_chat_boosts.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_user_profile_photos.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/get_webhook_info.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/hide_general_forum_topic.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/leave_chat.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/log_out.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/pin_chat_message.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/promote_chat_member.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/reopen_forum_topic.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/reopen_general_forum_topic.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/replace_sticker_in_set.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/restrict_chat_member.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/revoke_chat_invite_link.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_animation.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_audio.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_chat_action.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_contact.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_dice.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_document.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_game.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_invoice.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_location.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_media_group.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_message.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_photo.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_poll.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_sticker.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_venue.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_video.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_video_note.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/send_voice.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_chat_administrator_custom_title.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_chat_description.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_chat_menu_button.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_chat_permissions.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_chat_photo.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_chat_sticker_set.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_chat_title.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_custom_emoji_sticker_set_thumbnail.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_game_score.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_message_reaction.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_my_commands.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_my_default_administrator_rights.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_my_description.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_my_name.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_my_short_description.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_passport_data_errors.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_sticker_emoji_list.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_sticker_keywords.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_sticker_mask_position.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_sticker_position_in_set.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_sticker_set_thumbnail.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_sticker_set_title.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/set_webhook.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/stop_message_live_location.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/stop_poll.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/unban_chat_member.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/unban_chat_sender_chat.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/unhide_general_forum_topic.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/unpin_all_chat_messages.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/unpin_all_forum_topic_messages.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/unpin_all_general_forum_topic_messages.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/unpin_chat_message.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/methods/upload_sticker_file.py
+-rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/abc.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/animation.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/audio.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/birthdate.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/bot_command.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/bot_command_scope.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/bot_description.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/bot_name.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/bot_short_description.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/business_connection.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/business_intro.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/business_location.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/business_messages_deleted.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/business_opening_hours.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/business_opening_hours_interval.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/callback_game.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/callback_query.py
+-rw-r--r--   0        0        0    21574 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat.py
+-rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_administrator_rights.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_boost.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_boost_added.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_boost_removed.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_boost_source.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_boost_updated.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_invite_link.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_join_request.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_location.py
+-rw-r--r--   0        0        0     9053 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_member.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_permissions.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_photo.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chat_shared.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/chosen_inline_result.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/contact.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/dice.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/document.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/external_reply_info.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/file.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/force_reply.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/forum_topic.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/forum_topic_closed.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/forum_topic_created.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/forum_topic_edited.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/forum_topic_reopened.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/game.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/game_high_score.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/general_forum_topic_hidden.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/general_forum_topic_unhidden.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/giveaway.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/giveaway_completed.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/giveaway_created.py
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/giveaway_winners.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/inaccessible_message.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/inline_keyboard_button.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/inline_keyboard_markup.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/inline_query.py
+-rw-r--r--   0        0        0    33883 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/inline_query_result.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_contact_message_content.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_invoce_message_content.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_location_message_content.py
+-rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_media.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_message_content.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_sticker.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_text_message_content.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/input_venue_message_content.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/invoice.py
+-rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/keyboard_button.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/labeled_price.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/link_preview_options.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/location.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/login_url.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/mask_position.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/maybe_inaccessible_message.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/menu_button.py
+-rw-r--r--   0        0        0    55258 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/message.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/message_auto_delete_timer_changed.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/message_entity.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/message_id.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/message_origin.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/message_reaction_count_updated.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/message_reaction_updated.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/order_info.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/passport.py
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/passport_element_error.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/photo_size.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/poll.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/poll_answer.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/poll_option.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/pre_checkout_query.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/proximity_alert_triggered.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/reaction_count.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/reaction_type.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/reply_keyboard_markup.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/reply_keyboard_remove.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/reply_parameters.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/response_parameters.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/sent_web_app_message.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/shared_user.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/shipping_address.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/shipping_option.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/shipping_query.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/sticker.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/sticker_set.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/story.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/successful_payment.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/switch_inline_query_chosen_chat.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/text_quote.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/update.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/user.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/user_chat_boosts.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/user_profile_photos.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/users_shared.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/venue.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/video.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/video_chat_ended.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/video_chat_participants_invited.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/video_chat_scheduled.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/video_chat_started.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/video_note.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/voice.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/web_app_data.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/web_app_info.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/webhook_info.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yatbaf-0.9.1/src/yatbaf/types/write_access_allowed.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/api/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/api/conftest.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/api/test_methods.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/api/test_types.py
+-rw-r--r--   0        0        0   555312 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/api/data/api.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/bot/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/bot/test_bot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/client/__init__.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/client/test_http.py
+-rw-r--r--   0        0        0     6991 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/client/test_telegram.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/di/__init__.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/di/test_cleanup_group.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/di/test_dependency_batches.py
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/di/test_provide.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/di/test_resolve_dependencies.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/di/test_utils.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/dispatcher/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/dispatcher/test_dispatcher.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/dispatcher/test_guards.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/dispatcher/test_middleware.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/dispatcher/test_resolve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/__init__.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_chat.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_command.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_compat.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_content.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_logical.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_priority.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_text.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/filters/test_user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/__init__.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/test_dependencies.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/test_guards.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/test_handler.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/test_match.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/test_middleware.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/test_priority.py
+-rw-r--r--   0        0        0     8634 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/handler/test_sorting.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/helpers/test_deeplink.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/helpers/test_markdown.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/helpers/test_parse_command_args.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/long_polling/__init__.py
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/long_polling/test_polling.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/methods/__init__.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/methods/test_attrs.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/methods/test_encode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/middleware/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/middleware/test_middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/__init__.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_add_guard.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_add_handler.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_add_middleware.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_add_router.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_filters.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_find_handler.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_guards.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_middleware.py
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_parse_handlers.py
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_resolve.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_router.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/router/test_sort_handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/types/__init__.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/types/test_attrs.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/types/test_bot_object.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/types/test_ctx.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/utils/test_parse_command.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 yatbaf-0.9.1/tests/utils/test_wrap_middleware.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 yatbaf-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 yatbaf-0.9.1/LICENSE
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 yatbaf-0.9.1/README.md
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 yatbaf-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 yatbaf-0.9.1/PKG-INFO
```

### Comparing `yatbaf-0.9.0/src/yatbaf/__init__.py` & `yatbaf-0.9.1/src/yatbaf/__init__.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/abc.py` & `yatbaf-0.9.1/src/yatbaf/abc.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/bot.py` & `yatbaf-0.9.1/src/yatbaf/bot.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/di.py` & `yatbaf-0.9.1/src/yatbaf/di.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     provider: Provide,
     dependencies: dict[str, Provide],
 ) -> None:
     if is_reserved_key(key):
         raise DependencyError(f"name {key!r} is reserved.")
 
     for k, v in dependencies.items():
-        if v == provider:
+        if v == provider and k != key:
             raise DependencyError(
                 f"Provider {key!r} is already registered as {k!r}! "
                 "Use the same name to override provider."
             )
 
 
 async def _resolve_dependency(
```

### Comparing `yatbaf-0.9.0/src/yatbaf/dispatcher.py` & `yatbaf-0.9.1/src/yatbaf/dispatcher.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/enums.py` & `yatbaf-0.9.1/src/yatbaf/enums.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/exceptions.py` & `yatbaf-0.9.1/src/yatbaf/exceptions.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/handler.py` & `yatbaf-0.9.1/src/yatbaf/handler.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/helpers.py` & `yatbaf-0.9.1/src/yatbaf/helpers.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/http.py` & `yatbaf-0.9.1/src/yatbaf/http.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/long_polling.py` & `yatbaf-0.9.1/src/yatbaf/long_polling.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/middleware.py` & `yatbaf-0.9.1/src/yatbaf/middleware.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/models.py` & `yatbaf-0.9.1/src/yatbaf/models.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/router.py` & `yatbaf-0.9.1/src/yatbaf/router.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/telegram.py` & `yatbaf-0.9.1/src/yatbaf/telegram.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/typing.py` & `yatbaf-0.9.1/src/yatbaf/typing.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/utils.py` & `yatbaf-0.9.1/src/yatbaf/utils.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/__init__.py` & `yatbaf-0.9.1/src/yatbaf/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/base.py` & `yatbaf-0.9.1/src/yatbaf/filters/base.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/callback_data.py` & `yatbaf-0.9.1/src/yatbaf/filters/callback_data.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/chat_id.py` & `yatbaf-0.9.1/src/yatbaf/filters/chat_id.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/command.py` & `yatbaf-0.9.1/src/yatbaf/filters/command.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/content_type.py` & `yatbaf-0.9.1/src/yatbaf/filters/content_type.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/text_content.py` & `yatbaf-0.9.1/src/yatbaf/filters/text_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/filters/user.py` & `yatbaf-0.9.1/src/yatbaf/filters/user.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/__init__.py` & `yatbaf-0.9.1/src/yatbaf/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/abc.py` & `yatbaf-0.9.1/src/yatbaf/methods/abc.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/answer_callback_query.py` & `yatbaf-0.9.1/src/yatbaf/methods/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/answer_inline_query.py` & `yatbaf-0.9.1/src/yatbaf/methods/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/copy_message.py` & `yatbaf-0.9.1/src/yatbaf/methods/copy_message.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/copy_messages.py` & `yatbaf-0.9.1/src/yatbaf/methods/copy_messages.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/create_chat_invite_link.py` & `yatbaf-0.9.1/src/yatbaf/methods/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/create_invoice_link.py` & `yatbaf-0.9.1/src/yatbaf/methods/create_invoice_link.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/create_new_sticker_set.py` & `yatbaf-0.9.1/src/yatbaf/methods/create_new_sticker_set.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/edit_chat_invite_link.py` & `yatbaf-0.9.1/src/yatbaf/methods/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/edit_message_caption.py` & `yatbaf-0.9.1/src/yatbaf/methods/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/edit_message_live_location.py` & `yatbaf-0.9.1/src/yatbaf/methods/edit_message_live_location.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/edit_message_media.py` & `yatbaf-0.9.1/src/yatbaf/methods/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/edit_message_reply_markup.py` & `yatbaf-0.9.1/src/yatbaf/methods/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/edit_message_text.py` & `yatbaf-0.9.1/src/yatbaf/methods/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/forward_message.py` & `yatbaf-0.9.1/src/yatbaf/methods/forward_message.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/forward_messages.py` & `yatbaf-0.9.1/src/yatbaf/methods/forward_messages.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/promote_chat_member.py` & `yatbaf-0.9.1/src/yatbaf/methods/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/restrict_chat_member.py` & `yatbaf-0.9.1/src/yatbaf/methods/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_animation.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_animation.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_audio.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_audio.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_contact.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_contact.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_dice.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_dice.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_document.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_document.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_game.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_game.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_invoice.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_invoice.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_location.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_location.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_media_group.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_media_group.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_message.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_message.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_photo.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_photo.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_poll.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_poll.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_sticker.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_sticker.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_venue.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_venue.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_video.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_video.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_video_note.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_video_note.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/send_voice.py` & `yatbaf-0.9.1/src/yatbaf/methods/send_voice.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/set_game_score.py` & `yatbaf-0.9.1/src/yatbaf/methods/set_game_score.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/set_sticker_set_thumbnail.py` & `yatbaf-0.9.1/src/yatbaf/methods/set_sticker_set_thumbnail.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/set_webhook.py` & `yatbaf-0.9.1/src/yatbaf/methods/set_webhook.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/stop_message_live_location.py` & `yatbaf-0.9.1/src/yatbaf/methods/stop_message_live_location.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/methods/upload_sticker_file.py` & `yatbaf-0.9.1/src/yatbaf/methods/upload_sticker_file.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/__init__.py` & `yatbaf-0.9.1/src/yatbaf/types/__init__.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/abc.py` & `yatbaf-0.9.1/src/yatbaf/types/abc.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/animation.py` & `yatbaf-0.9.1/src/yatbaf/types/animation.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/audio.py` & `yatbaf-0.9.1/src/yatbaf/types/audio.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/bot_command_scope.py` & `yatbaf-0.9.1/src/yatbaf/types/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/business_connection.py` & `yatbaf-0.9.1/src/yatbaf/types/business_connection.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/business_intro.py` & `yatbaf-0.9.1/src/yatbaf/types/business_intro.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/business_messages_deleted.py` & `yatbaf-0.9.1/src/yatbaf/types/business_messages_deleted.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/business_opening_hours.py` & `yatbaf-0.9.1/src/yatbaf/types/business_opening_hours.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/business_opening_hours_interval.py` & `yatbaf-0.9.1/src/yatbaf/types/business_opening_hours_interval.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/callback_query.py` & `yatbaf-0.9.1/src/yatbaf/types/callback_query.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat.py` & `yatbaf-0.9.1/src/yatbaf/types/chat.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_administrator_rights.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_administrator_rights.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_boost.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_boost.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_boost_removed.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_boost_removed.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_boost_source.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_boost_source.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_invite_link.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_join_request.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_location.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_location.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_member.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_member.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_permissions.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_photo.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_photo.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chat_shared.py` & `yatbaf-0.9.1/src/yatbaf/types/chat_shared.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/chosen_inline_result.py` & `yatbaf-0.9.1/src/yatbaf/types/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/contact.py` & `yatbaf-0.9.1/src/yatbaf/types/contact.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/dice.py` & `yatbaf-0.9.1/src/yatbaf/types/dice.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/document.py` & `yatbaf-0.9.1/src/yatbaf/types/document.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/external_reply_info.py` & `yatbaf-0.9.1/src/yatbaf/types/external_reply_info.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/file.py` & `yatbaf-0.9.1/src/yatbaf/types/file.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/force_reply.py` & `yatbaf-0.9.1/src/yatbaf/types/force_reply.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/forum_topic.py` & `yatbaf-0.9.1/src/yatbaf/types/forum_topic.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/forum_topic_created.py` & `yatbaf-0.9.1/src/yatbaf/types/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/forum_topic_edited.py` & `yatbaf-0.9.1/src/yatbaf/types/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/game.py` & `yatbaf-0.9.1/src/yatbaf/types/game.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/giveaway.py` & `yatbaf-0.9.1/src/yatbaf/types/giveaway.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/giveaway_completed.py` & `yatbaf-0.9.1/src/yatbaf/types/giveaway_completed.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/giveaway_winners.py` & `yatbaf-0.9.1/src/yatbaf/types/giveaway_winners.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/inaccessible_message.py` & `yatbaf-0.9.1/src/yatbaf/types/inaccessible_message.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/inline_keyboard_button.py` & `yatbaf-0.9.1/src/yatbaf/types/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/inline_query.py` & `yatbaf-0.9.1/src/yatbaf/types/inline_query.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/inline_query_result.py` & `yatbaf-0.9.1/src/yatbaf/types/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_contact_message_content.py` & `yatbaf-0.9.1/src/yatbaf/types/input_contact_message_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_invoce_message_content.py` & `yatbaf-0.9.1/src/yatbaf/types/input_invoce_message_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_location_message_content.py` & `yatbaf-0.9.1/src/yatbaf/types/input_location_message_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_media.py` & `yatbaf-0.9.1/src/yatbaf/types/input_media.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_message_content.py` & `yatbaf-0.9.1/src/yatbaf/types/input_message_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_sticker.py` & `yatbaf-0.9.1/src/yatbaf/types/input_sticker.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_text_message_content.py` & `yatbaf-0.9.1/src/yatbaf/types/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/input_venue_message_content.py` & `yatbaf-0.9.1/src/yatbaf/types/input_venue_message_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/invoice.py` & `yatbaf-0.9.1/src/yatbaf/types/invoice.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/keyboard_button.py` & `yatbaf-0.9.1/src/yatbaf/types/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/link_preview_options.py` & `yatbaf-0.9.1/src/yatbaf/types/link_preview_options.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/location.py` & `yatbaf-0.9.1/src/yatbaf/types/location.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/login_url.py` & `yatbaf-0.9.1/src/yatbaf/types/login_url.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/mask_position.py` & `yatbaf-0.9.1/src/yatbaf/types/mask_position.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/menu_button.py` & `yatbaf-0.9.1/src/yatbaf/types/menu_button.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/message.py` & `yatbaf-0.9.1/src/yatbaf/types/message.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/message_entity.py` & `yatbaf-0.9.1/src/yatbaf/types/message_entity.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/message_origin.py` & `yatbaf-0.9.1/src/yatbaf/types/message_origin.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/message_reaction_count_updated.py` & `yatbaf-0.9.1/src/yatbaf/types/message_reaction_count_updated.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/message_reaction_updated.py` & `yatbaf-0.9.1/src/yatbaf/types/message_reaction_updated.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/order_info.py` & `yatbaf-0.9.1/src/yatbaf/types/order_info.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/passport.py` & `yatbaf-0.9.1/src/yatbaf/types/passport.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/passport_element_error.py` & `yatbaf-0.9.1/src/yatbaf/types/passport_element_error.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/photo_size.py` & `yatbaf-0.9.1/src/yatbaf/types/photo_size.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/poll.py` & `yatbaf-0.9.1/src/yatbaf/types/poll.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/poll_answer.py` & `yatbaf-0.9.1/src/yatbaf/types/poll_answer.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/pre_checkout_query.py` & `yatbaf-0.9.1/src/yatbaf/types/pre_checkout_query.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/proximity_alert_triggered.py` & `yatbaf-0.9.1/src/yatbaf/types/proximity_alert_triggered.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/reaction_type.py` & `yatbaf-0.9.1/src/yatbaf/types/reaction_type.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/reply_keyboard_markup.py` & `yatbaf-0.9.1/src/yatbaf/types/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/reply_keyboard_remove.py` & `yatbaf-0.9.1/src/yatbaf/types/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/reply_parameters.py` & `yatbaf-0.9.1/src/yatbaf/types/reply_parameters.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/response_parameters.py` & `yatbaf-0.9.1/src/yatbaf/types/response_parameters.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/shared_user.py` & `yatbaf-0.9.1/src/yatbaf/types/shared_user.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/shipping_address.py` & `yatbaf-0.9.1/src/yatbaf/types/shipping_address.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/shipping_query.py` & `yatbaf-0.9.1/src/yatbaf/types/shipping_query.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/sticker.py` & `yatbaf-0.9.1/src/yatbaf/types/sticker.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/sticker_set.py` & `yatbaf-0.9.1/src/yatbaf/types/sticker_set.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/successful_payment.py` & `yatbaf-0.9.1/src/yatbaf/types/successful_payment.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/switch_inline_query_chosen_chat.py` & `yatbaf-0.9.1/src/yatbaf/types/switch_inline_query_chosen_chat.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/text_quote.py` & `yatbaf-0.9.1/src/yatbaf/types/text_quote.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/update.py` & `yatbaf-0.9.1/src/yatbaf/types/update.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/user.py` & `yatbaf-0.9.1/src/yatbaf/types/user.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/users_shared.py` & `yatbaf-0.9.1/src/yatbaf/types/users_shared.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/venue.py` & `yatbaf-0.9.1/src/yatbaf/types/venue.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/video.py` & `yatbaf-0.9.1/src/yatbaf/types/video.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/video_note.py` & `yatbaf-0.9.1/src/yatbaf/types/video_note.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/voice.py` & `yatbaf-0.9.1/src/yatbaf/types/voice.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/web_app_data.py` & `yatbaf-0.9.1/src/yatbaf/types/web_app_data.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/webhook_info.py` & `yatbaf-0.9.1/src/yatbaf/types/webhook_info.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/src/yatbaf/types/write_access_allowed.py` & `yatbaf-0.9.1/src/yatbaf/types/write_access_allowed.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/conftest.py` & `yatbaf-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/api/test_methods.py` & `yatbaf-0.9.1/tests/api/test_methods.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/api/test_types.py` & `yatbaf-0.9.1/tests/api/test_types.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/api/data/api.json` & `yatbaf-0.9.1/tests/api/data/api.json`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/bot/test_bot.py` & `yatbaf-0.9.1/tests/bot/test_bot.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/client/test_http.py` & `yatbaf-0.9.1/tests/client/test_http.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/client/test_telegram.py` & `yatbaf-0.9.1/tests/client/test_telegram.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/di/test_cleanup_group.py` & `yatbaf-0.9.1/tests/di/test_cleanup_group.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/di/test_dependency_batches.py` & `yatbaf-0.9.1/tests/di/test_dependency_batches.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/di/test_provide.py` & `yatbaf-0.9.1/tests/di/test_provide.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/di/test_resolve_dependencies.py` & `yatbaf-0.9.1/tests/di/test_resolve_dependencies.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/di/test_utils.py` & `yatbaf-0.9.1/tests/di/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,12 +87,17 @@
 
 def test_validate_provider_reserved_name():
     provider = Provide(async_fn)
     with pytest.raises(DependencyError):
         validate_provider("update", provider, {})
 
 
-def test_validate_provider_override():
+def test_validate_provider_diff_name():
     with pytest.raises(DependencyError):
         validate_provider(
             "data1", Provide(async_fn), {"data": Provide(async_fn)}
         )
+
+
+def test_validate_provider_override():
+    validate_provider("data", Provide(async_fn), {"data": Provide(async_fn)})
+    validate_provider("data", Provide(async_fn), {"data": Provide(async_gen)})
```

### Comparing `yatbaf-0.9.0/tests/dispatcher/test_guards.py` & `yatbaf-0.9.1/tests/dispatcher/test_guards.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/dispatcher/test_middleware.py` & `yatbaf-0.9.1/tests/dispatcher/test_middleware.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/dispatcher/test_resolve.py` & `yatbaf-0.9.1/tests/dispatcher/test_resolve.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_chat.py` & `yatbaf-0.9.1/tests/filters/test_chat.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_command.py` & `yatbaf-0.9.1/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_compat.py` & `yatbaf-0.9.1/tests/filters/test_compat.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_content.py` & `yatbaf-0.9.1/tests/filters/test_content.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_logical.py` & `yatbaf-0.9.1/tests/filters/test_logical.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_priority.py` & `yatbaf-0.9.1/tests/filters/test_priority.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_text.py` & `yatbaf-0.9.1/tests/filters/test_text.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/filters/test_user.py` & `yatbaf-0.9.1/tests/filters/test_user.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/handler/test_dependencies.py` & `yatbaf-0.9.1/tests/handler/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/handler/test_guards.py` & `yatbaf-0.9.1/tests/handler/test_guards.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/handler/test_handler.py` & `yatbaf-0.9.1/tests/handler/test_handler.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/handler/test_match.py` & `yatbaf-0.9.1/tests/handler/test_match.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/handler/test_middleware.py` & `yatbaf-0.9.1/tests/handler/test_middleware.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/handler/test_priority.py` & `yatbaf-0.9.1/tests/handler/test_priority.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/handler/test_sorting.py` & `yatbaf-0.9.1/tests/handler/test_sorting.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/helpers/test_deeplink.py` & `yatbaf-0.9.1/tests/helpers/test_deeplink.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/helpers/test_markdown.py` & `yatbaf-0.9.1/tests/helpers/test_markdown.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/long_polling/test_polling.py` & `yatbaf-0.9.1/tests/long_polling/test_polling.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/methods/test_attrs.py` & `yatbaf-0.9.1/tests/methods/test_attrs.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/methods/test_encode.py` & `yatbaf-0.9.1/tests/methods/test_encode.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/middleware/test_middleware.py` & `yatbaf-0.9.1/tests/middleware/test_middleware.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_add_guard.py` & `yatbaf-0.9.1/tests/router/test_add_guard.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_add_handler.py` & `yatbaf-0.9.1/tests/router/test_add_handler.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_add_middleware.py` & `yatbaf-0.9.1/tests/router/test_add_middleware.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_add_router.py` & `yatbaf-0.9.1/tests/router/test_add_router.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_filters.py` & `yatbaf-0.9.1/tests/router/test_filters.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_find_handler.py` & `yatbaf-0.9.1/tests/router/test_find_handler.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_guards.py` & `yatbaf-0.9.1/tests/router/test_guards.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_middleware.py` & `yatbaf-0.9.1/tests/router/test_middleware.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_parse_handlers.py` & `yatbaf-0.9.1/tests/router/test_parse_handlers.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_resolve.py` & `yatbaf-0.9.1/tests/router/test_resolve.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_router.py` & `yatbaf-0.9.1/tests/router/test_router.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/router/test_sort_handlers.py` & `yatbaf-0.9.1/tests/router/test_sort_handlers.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/types/test_attrs.py` & `yatbaf-0.9.1/tests/types/test_attrs.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/tests/utils/test_parse_command.py` & `yatbaf-0.9.1/tests/utils/test_parse_command.py`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/LICENSE` & `yatbaf-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/pyproject.toml` & `yatbaf-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yatbaf-0.9.0/PKG-INFO` & `yatbaf-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yatbaf
-Version: 0.9.0
+Version: 0.9.1
 Summary: Telegram Bot framework
 Project-URL: Source, https://codeberg.org/maraudeur/yatbaf
 Author-email: Maraudeur <maraudeur1@protonmail.ch>
 License:  The MIT License (MIT)
         
          Copyright (c) 2023 Maraudeur
```

