# Comparing `tmp/teams_ai-1.0.1.tar.gz` & `tmp/teams_ai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teams_ai-1.0.1.tar", max compression
+gzip compressed data, was "teams_ai-1.1.0.tar", max compression
```

## Comparing `teams_ai-1.0.1.tar` & `teams_ai-1.1.0.tar`

### file list

```diff
@@ -1,169 +1,191 @@
--rw-r--r--   0        0        0     1093 2024-02-28 17:27:33.896122 teams_ai-1.0.1/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-01 19:58:49.301616 teams_ai-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      913 2024-02-28 17:27:33.903101 teams_ai-1.0.1/README.md
--rw-r--r--   0        0        0      644 2024-02-28 17:27:33.921639 teams_ai-1.0.1/teams/__init__.py
--rw-r--r--   0        0        0      963 2024-02-28 17:27:33.922639 teams_ai-1.0.1/teams/activity_type.py
--rw-r--r--   0        0        0      386 2024-04-01 15:45:21.915342 teams_ai-1.0.1/teams/adaptive_cards/__init__.py
--rw-r--r--   0        0        0    10814 2024-04-01 15:45:21.926346 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards.py
--rw-r--r--   0        0        0      471 2024-02-28 17:27:33.941901 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards_options.py
--rw-r--r--   0        0        0      252 2024-02-28 17:27:33.941901 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards_search_params.py
--rw-r--r--   0        0        0      344 2024-03-26 18:27:31.042285 teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards_search_result.py
--rw-r--r--   0        0        0      183 2024-02-28 17:27:33.942826 teams_ai-1.0.1/teams/ai/__init__.py
--rw-r--r--   0        0        0      321 2024-02-28 17:27:33.943872 teams_ai-1.0.1/teams/ai/actions/__init__.py
--rw-r--r--   0        0        0     1001 2024-02-28 17:27:33.950724 teams_ai-1.0.1/teams/ai/actions/action_entry.py
--rw-r--r--   0        0        0      641 2024-02-28 17:27:33.950724 teams_ai-1.0.1/teams/ai/actions/action_turn_context.py
--rw-r--r--   0        0        0      502 2024-04-01 15:45:21.927348 teams_ai-1.0.1/teams/ai/actions/action_types.py
--rw-r--r--   0        0        0     9105 2024-04-01 15:45:21.935879 teams_ai-1.0.1/teams/ai/ai.py
--rw-r--r--   0        0        0      903 2024-04-01 15:45:21.942863 teams_ai-1.0.1/teams/ai/ai_options.py
--rw-r--r--   0        0        0      425 2024-02-28 17:27:33.959629 teams_ai-1.0.1/teams/ai/augmentations/__init__.py
--rw-r--r--   0        0        0     1635 2024-03-04 19:10:38.243854 teams_ai-1.0.1/teams/ai/augmentations/augmentation.py
--rw-r--r--   0        0        0     2554 2024-03-04 19:10:38.249089 teams_ai-1.0.1/teams/ai/augmentations/default_augmentation.py
--rw-r--r--   0        0        0     9793 2024-03-27 21:04:22.729223 teams_ai-1.0.1/teams/ai/augmentations/monologue_augmentation.py
--rw-r--r--   0        0        0     7071 2024-03-04 19:10:38.262051 teams_ai-1.0.1/teams/ai/augmentations/sequence_augmentation.py
--rw-r--r--   0        0        0      196 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/clients/__init__.py
--rw-r--r--   0        0        0     7230 2024-03-04 19:10:38.267267 teams_ai-1.0.1/teams/ai/clients/llm_client.py
--rw-r--r--   0        0        0      224 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/data_sources/__init__.py
--rw-r--r--   0        0        0     1360 2024-03-04 19:10:38.273303 teams_ai-1.0.1/teams/ai/data_sources/data_source.py
--rw-r--r--   0        0        0     2500 2024-03-04 19:10:38.279346 teams_ai-1.0.1/teams/ai/data_sources/text_data_source.py
--rw-r--r--   0        0        0      625 2024-04-01 15:45:21.948864 teams_ai-1.0.1/teams/ai/embeddings/__init__.py
--rw-r--r--   0        0        0     4409 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings.py
--rw-r--r--   0        0        0     1048 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings_options.py
--rw-r--r--   0        0        0      894 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/embeddings_model.py
--rw-r--r--   0        0        0      802 2024-02-28 17:27:33.962205 teams_ai-1.0.1/teams/ai/embeddings/embeddings_response.py
--rw-r--r--   0        0        0     3803 2024-02-28 17:27:33.968740 teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings.py
--rw-r--r--   0        0        0      991 2024-02-28 17:27:33.968740 teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings_options.py
--rw-r--r--   0        0        0      562 2024-02-28 17:27:33.968740 teams_ai-1.0.1/teams/ai/models/__init__.py
--rw-r--r--   0        0        0      729 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/models/chat_completion_action.py
--rw-r--r--   0        0        0     7123 2024-03-04 19:10:38.285350 teams_ai-1.0.1/teams/ai/models/openai_model.py
--rw-r--r--   0        0        0     1302 2024-03-04 19:10:38.291151 teams_ai-1.0.1/teams/ai/models/prompt_completion_model.py
--rw-r--r--   0        0        0      909 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/models/prompt_response.py
--rw-r--r--   0        0        0      557 2024-03-05 21:42:08.164469 teams_ai-1.0.1/teams/ai/moderators/__init__.py
--rw-r--r--   0        0        0     7695 2024-03-26 18:27:31.059067 teams_ai-1.0.1/teams/ai/moderators/azure_content_safety_moderator.py
--rw-r--r--   0        0        0      656 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/moderators/default_moderator.py
--rw-r--r--   0        0        0     1589 2024-03-04 19:10:38.297196 teams_ai-1.0.1/teams/ai/moderators/moderator.py
--rw-r--r--   0        0        0     4332 2024-03-05 21:41:32.156765 teams_ai-1.0.1/teams/ai/moderators/openai_moderator.py
--rw-r--r--   0        0        0      654 2024-04-01 15:45:21.950878 teams_ai-1.0.1/teams/ai/planners/__init__.py
--rw-r--r--   0        0        0     6127 2024-04-01 15:45:21.959862 teams_ai-1.0.1/teams/ai/planners/action_planner.py
--rw-r--r--   0        0        0    14445 2024-04-01 15:45:21.966864 teams_ai-1.0.1/teams/ai/planners/assistants_planner.py
--rw-r--r--   0        0        0     2085 2024-02-29 18:07:09.525392 teams_ai-1.0.1/teams/ai/planners/plan.py
--rw-r--r--   0        0        0     1065 2024-04-01 15:45:21.968867 teams_ai-1.0.1/teams/ai/planners/planner.py
--rw-r--r--   0        0        0     1476 2024-02-28 17:27:33.969778 teams_ai-1.0.1/teams/ai/prompts/__init__.py
--rw-r--r--   0        0        0      846 2024-02-28 17:27:33.975341 teams_ai-1.0.1/teams/ai/prompts/assistant_message.py
--rw-r--r--   0        0        0     1066 2024-02-28 17:27:33.975782 teams_ai-1.0.1/teams/ai/prompts/augmentation_config.py
--rw-r--r--   0        0        0     3285 2024-02-28 17:27:33.976301 teams_ai-1.0.1/teams/ai/prompts/completion_config.py
--rw-r--r--   0        0        0      428 2024-02-28 17:27:33.976301 teams_ai-1.0.1/teams/ai/prompts/function_call.py
--rw-r--r--   0        0        0     2992 2024-03-04 19:10:38.315390 teams_ai-1.0.1/teams/ai/prompts/function_call_message.py
--rw-r--r--   0        0        0     3137 2024-03-04 19:10:38.321390 teams_ai-1.0.1/teams/ai/prompts/function_response_message.py
--rw-r--r--   0        0        0     1511 2024-02-28 17:27:33.977950 teams_ai-1.0.1/teams/ai/prompts/message.py
--rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.978714 teams_ai-1.0.1/teams/ai/prompts/prompt.py
--rw-r--r--   0        0        0     2493 2024-03-04 19:10:38.326426 teams_ai-1.0.1/teams/ai/prompts/prompt_functions.py
--rw-r--r--   0        0        0    14657 2024-03-27 21:04:22.780312 teams_ai-1.0.1/teams/ai/prompts/prompt_manager.py
--rw-r--r--   0        0        0     1571 2024-02-28 17:27:33.986946 teams_ai-1.0.1/teams/ai/prompts/prompt_manager_options.py
--rw-r--r--   0        0        0      478 2024-02-28 17:27:33.986946 teams_ai-1.0.1/teams/ai/prompts/prompt_section_layout.py
--rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.988031 teams_ai-1.0.1/teams/ai/prompts/prompt_template.py
--rw-r--r--   0        0        0     2116 2024-02-28 17:27:33.988538 teams_ai-1.0.1/teams/ai/prompts/prompt_template_config.py
--rw-r--r--   0        0        0      614 2024-02-28 17:27:33.988538 teams_ai-1.0.1/teams/ai/prompts/rendered_prompt_section.py
--rw-r--r--   0        0        0      800 2024-02-28 17:27:33.989546 teams_ai-1.0.1/teams/ai/prompts/sections/__init__.py
--rw-r--r--   0        0        0     4104 2024-03-27 21:04:22.804466 teams_ai-1.0.1/teams/ai/prompts/sections/action_augmentation_section.py
--rw-r--r--   0        0        0     6894 2024-03-04 19:10:38.345727 teams_ai-1.0.1/teams/ai/prompts/sections/conversation_history_section.py
--rw-r--r--   0        0        0     2451 2024-03-04 19:10:38.351007 teams_ai-1.0.1/teams/ai/prompts/sections/data_source_section.py
--rw-r--r--   0        0        0     3361 2024-03-04 19:10:38.357972 teams_ai-1.0.1/teams/ai/prompts/sections/group_section.py
--rw-r--r--   0        0        0     9245 2024-03-04 19:10:38.363971 teams_ai-1.0.1/teams/ai/prompts/sections/layout_engine_section.py
--rw-r--r--   0        0        0     2941 2024-03-04 19:10:38.370157 teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section.py
--rw-r--r--   0        0        0     7305 2024-03-04 19:10:38.376193 teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section_base.py
--rw-r--r--   0        0        0     9006 2024-03-04 19:10:38.382234 teams_ai-1.0.1/teams/ai/prompts/sections/template_section.py
--rw-r--r--   0        0        0     3124 2024-03-04 19:10:38.388234 teams_ai-1.0.1/teams/ai/prompts/sections/text_section.py
--rw-r--r--   0        0        0      635 2024-02-28 17:27:33.994231 teams_ai-1.0.1/teams/ai/prompts/system_message.py
--rw-r--r--   0        0        0     4028 2024-03-04 19:10:38.394784 teams_ai-1.0.1/teams/ai/prompts/user_input_message.py
--rw-r--r--   0        0        0      800 2024-02-28 17:27:33.996243 teams_ai-1.0.1/teams/ai/prompts/user_message.py
--rw-r--r--   0        0        0      213 2024-02-28 17:27:33.997052 teams_ai-1.0.1/teams/ai/tokenizers/__init__.py
--rw-r--r--   0        0        0     1071 2024-02-28 17:27:33.998562 teams_ai-1.0.1/teams/ai/tokenizers/gpt_tokenizer.py
--rw-r--r--   0        0        0      993 2024-02-28 17:27:33.999575 teams_ai-1.0.1/teams/ai/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     1436 2024-03-04 19:10:38.399820 teams_ai-1.0.1/teams/ai/utilities.py
--rw-r--r--   0        0        0      621 2024-02-28 17:27:34.000614 teams_ai-1.0.1/teams/ai/validators/__init__.py
--rw-r--r--   0        0        0     4284 2024-03-04 19:10:38.405822 teams_ai-1.0.1/teams/ai/validators/action_response_validator.py
--rw-r--r--   0        0        0      777 2024-03-04 19:10:38.411023 teams_ai-1.0.1/teams/ai/validators/default_response_validator.py
--rw-r--r--   0        0        0     3045 2024-03-26 20:05:45.109561 teams_ai-1.0.1/teams/ai/validators/json_response_validator.py
--rw-r--r--   0        0        0     1286 2024-03-04 19:10:38.423061 teams_ai-1.0.1/teams/ai/validators/prompt_response_validator.py
--rw-r--r--   0        0        0      648 2024-02-28 17:27:34.002010 teams_ai-1.0.1/teams/ai/validators/validation.py
--rw-r--r--   0        0        0    24013 2024-03-04 19:10:38.429023 teams_ai-1.0.1/teams/app.py
--rw-r--r--   0        0        0      296 2024-02-28 17:27:34.013515 teams_ai-1.0.1/teams/app_error.py
--rw-r--r--   0        0        0     2433 2024-02-28 17:27:34.019518 teams_ai-1.0.1/teams/app_options.py
--rw-r--r--   0        0        0      566 2024-02-28 17:27:34.020527 teams_ai-1.0.1/teams/input_file.py
--rw-r--r--   0        0        0      154 2024-02-28 17:27:34.020845 teams_ai-1.0.1/teams/meetings/__init__.py
--rw-r--r--   0        0        0     3653 2024-02-28 17:27:34.028331 teams_ai-1.0.1/teams/meetings/meetings.py
--rw-r--r--   0        0        0      228 2024-02-28 17:27:34.029400 teams_ai-1.0.1/teams/message_extensions/__init__.py
--rw-r--r--   0        0        0    24315 2024-04-01 15:45:21.976862 teams_ai-1.0.1/teams/message_extensions/message_extensions.py
--rw-r--r--   0        0        0      241 2024-02-28 17:27:34.039795 teams_ai-1.0.1/teams/message_reaction_types.py
--rw-r--r--   0        0        0        0 2024-02-28 17:27:34.039795 teams_ai-1.0.1/teams/py.typed
--rw-r--r--   0        0        0      328 2024-02-28 17:27:34.041095 teams_ai-1.0.1/teams/query.py
--rw-r--r--   0        0        0      762 2024-02-28 17:27:34.049441 teams_ai-1.0.1/teams/route.py
--rw-r--r--   0        0        0      512 2024-03-04 19:10:38.436267 teams_ai-1.0.1/teams/state/__init__.py
--rw-r--r--   0        0        0     1373 2024-03-04 19:10:38.442230 teams_ai-1.0.1/teams/state/conversation_state.py
--rw-r--r--   0        0        0     3481 2024-03-04 19:10:38.447269 teams_ai-1.0.1/teams/state/memory.py
--rw-r--r--   0        0        0     4222 2024-04-01 15:45:21.983876 teams_ai-1.0.1/teams/state/state.py
--rw-r--r--   0        0        0     1118 2024-03-04 19:10:38.458550 teams_ai-1.0.1/teams/state/temp_state.py
--rw-r--r--   0        0        0      732 2024-03-04 19:10:38.463524 teams_ai-1.0.1/teams/state/todict.py
--rw-r--r--   0        0        0     2478 2024-03-26 18:27:31.059067 teams_ai-1.0.1/teams/state/turn_state.py
--rw-r--r--   0        0        0     1314 2024-03-04 19:10:38.469569 teams_ai-1.0.1/teams/state/user_state.py
--rw-r--r--   0        0        0      239 2024-02-28 17:27:34.059743 teams_ai-1.0.1/teams/task_modules/__init__.py
--rw-r--r--   0        0        0     6430 2024-04-01 15:45:21.991863 teams_ai-1.0.1/teams/task_modules/task_modules.py
--rw-r--r--   0        0        0      488 2024-02-28 17:27:34.071531 teams_ai-1.0.1/teams/task_modules/task_modules_options.py
--rw-r--r--   0        0        0     3825 2024-04-01 19:59:26.866077 teams_ai-1.0.1/teams/teams_adapter.py
--rw-r--r--   0        0        0     1190 2024-02-28 17:27:34.072531 teams_ai-1.0.1/teams/typing.py
--rw-r--r--   0        0        0      292 2024-02-28 17:27:34.072531 teams_ai-1.0.1/teams/user_agent.py
--rw-r--r--   0        0        0      200 2024-02-28 17:27:34.073532 teams_ai-1.0.1/teams/utils/json/__init__.py
--rw-r--r--   0        0        0      637 2024-03-27 21:04:22.850998 teams_ai-1.0.1/teams/utils/json/parse.py
--rw-r--r--   0        0        0     1747 2024-02-28 17:27:34.074530 teams_ai-1.0.1/teams/utils/json/parse_object.py
--rw-r--r--   0        0        0     4966 2024-04-01 15:45:22.007862 teams_ai-1.0.1/tests/adaptive_cards/test_adaptive_cards.py
--rw-r--r--   0        0        0     2746 2024-02-28 17:27:34.075531 teams_ai-1.0.1/tests/ai/augmentations/test_default_augmentation.py
--rw-r--r--   0        0        0     6562 2024-03-27 21:04:22.882484 teams_ai-1.0.1/tests/ai/augmentations/test_monologue_augmentation.py
--rw-r--r--   0        0        0     7587 2024-03-04 19:10:38.474809 teams_ai-1.0.1/tests/ai/augmentations/test_sequence_augmentation.py
--rw-r--r--   0        0        0     1502 2024-02-28 17:27:34.077308 teams_ai-1.0.1/tests/ai/data_sources/test_text_data_source.py
--rw-r--r--   0        0        0     6111 2024-04-01 15:45:22.009865 teams_ai-1.0.1/tests/ai/embeddings/test_azure_openai_embeddings.py
--rw-r--r--   0        0        0     5222 2024-04-01 15:45:22.009865 teams_ai-1.0.1/tests/ai/embeddings/test_openai_embeddings.py
--rw-r--r--   0        0        0     5006 2024-02-28 17:27:34.078742 teams_ai-1.0.1/tests/ai/models/test_openai_model.py
--rw-r--r--   0        0        0     6927 2024-03-26 18:27:31.075685 teams_ai-1.0.1/tests/ai/moderators/test_azure_content_safety_moderator.py
--rw-r--r--   0        0        0      828 2024-02-28 17:27:34.079758 teams_ai-1.0.1/tests/ai/moderators/test_default_moderator.py
--rw-r--r--   0        0        0     9480 2024-03-04 19:10:38.486811 teams_ai-1.0.1/tests/ai/moderators/test_openai_moderator.py
--rw-r--r--   0        0        0      692 2024-02-28 17:27:34.081309 teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/actions.json
--rw-r--r--   0        0        0      587 2024-02-28 17:27:34.081309 teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/skprompt.txt
--rw-r--r--   0        0        0      614 2024-02-28 17:27:34.082314 teams_ai-1.0.1/tests/ai/prompts/test_assets/include_images/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.0.1/tests/ai/prompts/test_assets/include_images/skprompt.txt
--rw-r--r--   0        0        0      366 2024-02-28 17:27:34.083314 teams_ai-1.0.1/tests/ai/prompts/test_assets/migrate_old_schema/config.json
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.083314 teams_ai-1.0.1/tests/ai/prompts/test_assets/migrate_old_schema/skprompt.txt
--rw-r--r--   0        0        0       11 2024-02-28 17:27:34.084313 teams_ai-1.0.1/tests/ai/prompts/test_assets/no_config/skprompt.txt
--rw-r--r--   0        0        0      582 2024-02-28 17:27:34.084313 teams_ai-1.0.1/tests/ai/prompts/test_assets/no_prompt/config.json
--rw-r--r--   0        0        0     1164 2024-02-28 17:27:34.085314 teams_ai-1.0.1/tests/ai/prompts/test_assistant_message.py
--rw-r--r--   0        0        0     7157 2024-03-04 19:10:38.492599 teams_ai-1.0.1/tests/ai/prompts/test_conversation_history.py
--rw-r--r--   0        0        0     1560 2024-02-28 17:27:34.085423 teams_ai-1.0.1/tests/ai/prompts/test_data_source_section.py
--rw-r--r--   0        0        0     2175 2024-02-28 17:27:34.085423 teams_ai-1.0.1/tests/ai/prompts/test_function_call_message.py
--rw-r--r--   0        0        0     2221 2024-02-28 17:27:34.086488 teams_ai-1.0.1/tests/ai/prompts/test_function_response_message.py
--rw-r--r--   0        0        0     2807 2024-02-28 17:27:34.086488 teams_ai-1.0.1/tests/ai/prompts/test_group_section.py
--rw-r--r--   0        0        0     6968 2024-02-28 17:27:34.086488 teams_ai-1.0.1/tests/ai/prompts/test_layout_engine.py
--rw-r--r--   0        0        0     9570 2024-03-04 19:10:38.498635 teams_ai-1.0.1/tests/ai/prompts/test_prompt_manager_v2.py
--rw-r--r--   0        0        0     8405 2024-02-28 17:27:34.087490 teams_ai-1.0.1/tests/ai/prompts/test_prompt_section_base.py
--rw-r--r--   0        0        0     1056 2024-02-28 17:27:34.087490 teams_ai-1.0.1/tests/ai/prompts/test_system_message.py
--rw-r--r--   0        0        0     9290 2024-03-04 19:10:38.503635 teams_ai-1.0.1/tests/ai/prompts/test_template_section.py
--rw-r--r--   0        0        0     2319 2024-02-28 17:27:34.088994 teams_ai-1.0.1/tests/ai/prompts/test_text_section.py
--rw-r--r--   0        0        0     7349 2024-03-04 19:10:38.509640 teams_ai-1.0.1/tests/ai/prompts/test_user_input_message.py
--rw-r--r--   0        0        0     1048 2024-02-28 17:27:34.089504 teams_ai-1.0.1/tests/ai/prompts/test_user_message.py
--rw-r--r--   0        0        0     1457 2024-02-28 17:27:34.089504 teams_ai-1.0.1/tests/ai/test_utilities.py
--rw-r--r--   0        0        0      853 2024-02-28 17:27:34.089504 teams_ai-1.0.1/tests/ai/tokenizers/test_gpt_tokenizer.py
--rw-r--r--   0        0        0     6169 2024-02-28 17:27:34.090510 teams_ai-1.0.1/tests/ai/validators/test_action_response_validator.py
--rw-r--r--   0        0        0      822 2024-02-28 17:27:34.090510 teams_ai-1.0.1/tests/ai/validators/test_default_response_validator.py
--rw-r--r--   0        0        0     5196 2024-02-28 17:27:34.091510 teams_ai-1.0.1/tests/ai/validators/test_json_response_validator.py
--rw-r--r--   0        0        0     4144 2024-03-26 18:27:31.075685 teams_ai-1.0.1/tests/state/test_conversation_state.py
--rw-r--r--   0        0        0     6119 2024-03-04 19:10:38.514847 teams_ai-1.0.1/tests/state/test_custom_turn_state.py
--rw-r--r--   0        0        0     1797 2024-03-26 18:27:31.075685 teams_ai-1.0.1/tests/state/test_temp_state.py
--rw-r--r--   0        0        0     6510 2024-03-26 18:27:31.092235 teams_ai-1.0.1/tests/state/test_turn_state.py
--rw-r--r--   0        0        0     3692 2024-03-26 18:27:31.099741 teams_ai-1.0.1/tests/state/test_user_state.py
--rw-r--r--   0        0        0     2250 2024-04-01 15:45:22.019885 teams_ai-1.0.1/tests/task_modules/test_task_modules.py
--rw-r--r--   0        0        0    29183 2024-02-28 17:27:34.095113 teams_ai-1.0.1/tests/test_app.py
--rw-r--r--   0        0        0    11702 2024-02-28 17:27:34.096123 teams_ai-1.0.1/tests/test_meetings.py
--rw-r--r--   0        0        0    32052 2024-02-28 17:27:34.106581 teams_ai-1.0.1/tests/test_message_extensions.py
--rw-r--r--   0        0        0      146 2024-02-28 17:27:34.106581 teams_ai-1.0.1/tests/utils/__init__.py
--rw-r--r--   0        0        0      526 2024-02-28 17:27:34.107578 teams_ai-1.0.1/tests/utils/activity.py
--rw-r--r--   0        0        0     1055 2024-02-28 17:27:34.107578 teams_ai-1.0.1/tests/utils/adapter.py
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 teams_ai-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-02-28 17:27:33.896122 teams_ai-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1913 2024-05-09 21:14:19.181479 teams_ai-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1303 2024-04-22 18:27:52.693426 teams_ai-1.1.0/README.md
+-rw-r--r--   0        0        0      644 2024-02-28 17:27:33.921639 teams_ai-1.1.0/teams/__init__.py
+-rw-r--r--   0        0        0      963 2024-02-28 17:27:33.922639 teams_ai-1.1.0/teams/activity_type.py
+-rw-r--r--   0        0        0      386 2024-04-01 15:45:21.915342 teams_ai-1.1.0/teams/adaptive_cards/__init__.py
+-rw-r--r--   0        0        0    10816 2024-05-09 16:06:14.138234 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards.py
+-rw-r--r--   0        0        0      471 2024-02-28 17:27:33.941901 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards_options.py
+-rw-r--r--   0        0        0      252 2024-02-28 17:27:33.941901 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards_search_params.py
+-rw-r--r--   0        0        0      344 2024-03-26 18:27:31.042285 teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards_search_result.py
+-rw-r--r--   0        0        0      183 2024-02-28 17:27:33.942826 teams_ai-1.1.0/teams/ai/__init__.py
+-rw-r--r--   0        0        0      321 2024-02-28 17:27:33.943872 teams_ai-1.1.0/teams/ai/actions/__init__.py
+-rw-r--r--   0        0        0     1001 2024-02-28 17:27:33.950724 teams_ai-1.1.0/teams/ai/actions/action_entry.py
+-rw-r--r--   0        0        0      641 2024-02-28 17:27:33.950724 teams_ai-1.1.0/teams/ai/actions/action_turn_context.py
+-rw-r--r--   0        0        0      502 2024-04-01 15:45:21.927348 teams_ai-1.1.0/teams/ai/actions/action_types.py
+-rw-r--r--   0        0        0     9031 2024-05-09 16:06:14.144681 teams_ai-1.1.0/teams/ai/ai.py
+-rw-r--r--   0        0        0      903 2024-04-01 15:45:21.942863 teams_ai-1.1.0/teams/ai/ai_options.py
+-rw-r--r--   0        0        0      425 2024-02-28 17:27:33.959629 teams_ai-1.1.0/teams/ai/augmentations/__init__.py
+-rw-r--r--   0        0        0     1635 2024-03-04 19:10:38.243854 teams_ai-1.1.0/teams/ai/augmentations/augmentation.py
+-rw-r--r--   0        0        0     2554 2024-03-04 19:10:38.249089 teams_ai-1.1.0/teams/ai/augmentations/default_augmentation.py
+-rw-r--r--   0        0        0    10072 2024-05-09 16:06:14.153198 teams_ai-1.1.0/teams/ai/augmentations/monologue_augmentation.py
+-rw-r--r--   0        0        0     7071 2024-03-04 19:10:38.262051 teams_ai-1.1.0/teams/ai/augmentations/sequence_augmentation.py
+-rw-r--r--   0        0        0      196 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/clients/__init__.py
+-rw-r--r--   0        0        0     7231 2024-04-22 18:27:52.706612 teams_ai-1.1.0/teams/ai/clients/llm_client.py
+-rw-r--r--   0        0        0      224 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/data_sources/__init__.py
+-rw-r--r--   0        0        0     1360 2024-03-04 19:10:38.273303 teams_ai-1.1.0/teams/ai/data_sources/data_source.py
+-rw-r--r--   0        0        0     2500 2024-03-04 19:10:38.279346 teams_ai-1.1.0/teams/ai/data_sources/text_data_source.py
+-rw-r--r--   0        0        0      625 2024-04-01 15:45:21.948864 teams_ai-1.1.0/teams/ai/embeddings/__init__.py
+-rw-r--r--   0        0        0     4379 2024-05-09 16:06:14.161855 teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings.py
+-rw-r--r--   0        0        0     1048 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings_options.py
+-rw-r--r--   0        0        0      894 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/embeddings/embeddings_model.py
+-rw-r--r--   0        0        0      802 2024-02-28 17:27:33.962205 teams_ai-1.1.0/teams/ai/embeddings/embeddings_response.py
+-rw-r--r--   0        0        0     3803 2024-02-28 17:27:33.968740 teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings.py
+-rw-r--r--   0        0        0      991 2024-02-28 17:27:33.968740 teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings_options.py
+-rw-r--r--   0        0        0      562 2024-02-28 17:27:33.968740 teams_ai-1.1.0/teams/ai/models/__init__.py
+-rw-r--r--   0        0        0      729 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/models/chat_completion_action.py
+-rw-r--r--   0        0        0     7173 2024-04-22 18:27:52.713613 teams_ai-1.1.0/teams/ai/models/openai_model.py
+-rw-r--r--   0        0        0     1302 2024-03-04 19:10:38.291151 teams_ai-1.1.0/teams/ai/models/prompt_completion_model.py
+-rw-r--r--   0        0        0      909 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/models/prompt_response.py
+-rw-r--r--   0        0        0      557 2024-03-05 21:42:08.164469 teams_ai-1.1.0/teams/ai/moderators/__init__.py
+-rw-r--r--   0        0        0     7695 2024-03-26 18:27:31.059067 teams_ai-1.1.0/teams/ai/moderators/azure_content_safety_moderator.py
+-rw-r--r--   0        0        0      656 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/moderators/default_moderator.py
+-rw-r--r--   0        0        0     1589 2024-03-04 19:10:38.297196 teams_ai-1.1.0/teams/ai/moderators/moderator.py
+-rw-r--r--   0        0        0     4332 2024-03-05 21:41:32.156765 teams_ai-1.1.0/teams/ai/moderators/openai_moderator.py
+-rw-r--r--   0        0        0      735 2024-05-09 15:32:43.716003 teams_ai-1.1.0/teams/ai/planners/__init__.py
+-rw-r--r--   0        0        0     6127 2024-04-01 15:45:21.959862 teams_ai-1.1.0/teams/ai/planners/action_planner.py
+-rw-r--r--   0        0        0    16702 2024-05-09 15:32:43.716003 teams_ai-1.1.0/teams/ai/planners/assistants_planner.py
+-rw-r--r--   0        0        0     2085 2024-02-29 18:07:09.525392 teams_ai-1.1.0/teams/ai/planners/plan.py
+-rw-r--r--   0        0        0     1065 2024-04-01 15:45:21.968867 teams_ai-1.1.0/teams/ai/planners/planner.py
+-rw-r--r--   0        0        0     1476 2024-02-28 17:27:33.969778 teams_ai-1.1.0/teams/ai/prompts/__init__.py
+-rw-r--r--   0        0        0      846 2024-02-28 17:27:33.975341 teams_ai-1.1.0/teams/ai/prompts/assistant_message.py
+-rw-r--r--   0        0        0     1066 2024-02-28 17:27:33.975782 teams_ai-1.1.0/teams/ai/prompts/augmentation_config.py
+-rw-r--r--   0        0        0     3285 2024-02-28 17:27:33.976301 teams_ai-1.1.0/teams/ai/prompts/completion_config.py
+-rw-r--r--   0        0        0      428 2024-02-28 17:27:33.976301 teams_ai-1.1.0/teams/ai/prompts/function_call.py
+-rw-r--r--   0        0        0     2992 2024-03-04 19:10:38.315390 teams_ai-1.1.0/teams/ai/prompts/function_call_message.py
+-rw-r--r--   0        0        0     3137 2024-03-04 19:10:38.321390 teams_ai-1.1.0/teams/ai/prompts/function_response_message.py
+-rw-r--r--   0        0        0     1511 2024-02-28 17:27:33.977950 teams_ai-1.1.0/teams/ai/prompts/message.py
+-rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.978714 teams_ai-1.1.0/teams/ai/prompts/prompt.py
+-rw-r--r--   0        0        0     2493 2024-03-04 19:10:38.326426 teams_ai-1.1.0/teams/ai/prompts/prompt_functions.py
+-rw-r--r--   0        0        0    14509 2024-05-09 16:06:14.171453 teams_ai-1.1.0/teams/ai/prompts/prompt_manager.py
+-rw-r--r--   0        0        0     1571 2024-02-28 17:27:33.986946 teams_ai-1.1.0/teams/ai/prompts/prompt_manager_options.py
+-rw-r--r--   0        0        0      478 2024-02-28 17:27:33.986946 teams_ai-1.1.0/teams/ai/prompts/prompt_section_layout.py
+-rw-r--r--   0        0        0     1156 2024-02-28 17:27:33.988031 teams_ai-1.1.0/teams/ai/prompts/prompt_template.py
+-rw-r--r--   0        0        0     2116 2024-02-28 17:27:33.988538 teams_ai-1.1.0/teams/ai/prompts/prompt_template_config.py
+-rw-r--r--   0        0        0      614 2024-02-28 17:27:33.988538 teams_ai-1.1.0/teams/ai/prompts/rendered_prompt_section.py
+-rw-r--r--   0        0        0      800 2024-02-28 17:27:33.989546 teams_ai-1.1.0/teams/ai/prompts/sections/__init__.py
+-rw-r--r--   0        0        0     4104 2024-03-27 21:04:22.804466 teams_ai-1.1.0/teams/ai/prompts/sections/action_augmentation_section.py
+-rw-r--r--   0        0        0     6894 2024-03-04 19:10:38.345727 teams_ai-1.1.0/teams/ai/prompts/sections/conversation_history_section.py
+-rw-r--r--   0        0        0     2451 2024-03-04 19:10:38.351007 teams_ai-1.1.0/teams/ai/prompts/sections/data_source_section.py
+-rw-r--r--   0        0        0     3361 2024-03-04 19:10:38.357972 teams_ai-1.1.0/teams/ai/prompts/sections/group_section.py
+-rw-r--r--   0        0        0     9245 2024-03-04 19:10:38.363971 teams_ai-1.1.0/teams/ai/prompts/sections/layout_engine_section.py
+-rw-r--r--   0        0        0     2941 2024-03-04 19:10:38.370157 teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section.py
+-rw-r--r--   0        0        0     7305 2024-03-04 19:10:38.376193 teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section_base.py
+-rw-r--r--   0        0        0     9006 2024-03-04 19:10:38.382234 teams_ai-1.1.0/teams/ai/prompts/sections/template_section.py
+-rw-r--r--   0        0        0     3124 2024-03-04 19:10:38.388234 teams_ai-1.1.0/teams/ai/prompts/sections/text_section.py
+-rw-r--r--   0        0        0      635 2024-02-28 17:27:33.994231 teams_ai-1.1.0/teams/ai/prompts/system_message.py
+-rw-r--r--   0        0        0     4028 2024-03-04 19:10:38.394784 teams_ai-1.1.0/teams/ai/prompts/user_input_message.py
+-rw-r--r--   0        0        0      800 2024-02-28 17:27:33.996243 teams_ai-1.1.0/teams/ai/prompts/user_message.py
+-rw-r--r--   0        0        0      213 2024-02-28 17:27:33.997052 teams_ai-1.1.0/teams/ai/tokenizers/__init__.py
+-rw-r--r--   0        0        0     1071 2024-02-28 17:27:33.998562 teams_ai-1.1.0/teams/ai/tokenizers/gpt_tokenizer.py
+-rw-r--r--   0        0        0      993 2024-02-28 17:27:33.999575 teams_ai-1.1.0/teams/ai/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     1436 2024-03-04 19:10:38.399820 teams_ai-1.1.0/teams/ai/utilities.py
+-rw-r--r--   0        0        0      621 2024-02-28 17:27:34.000614 teams_ai-1.1.0/teams/ai/validators/__init__.py
+-rw-r--r--   0        0        0     4415 2024-05-09 16:06:14.178969 teams_ai-1.1.0/teams/ai/validators/action_response_validator.py
+-rw-r--r--   0        0        0      777 2024-03-04 19:10:38.411023 teams_ai-1.1.0/teams/ai/validators/default_response_validator.py
+-rw-r--r--   0        0        0     3045 2024-03-26 20:05:45.109561 teams_ai-1.1.0/teams/ai/validators/json_response_validator.py
+-rw-r--r--   0        0        0     1286 2024-03-04 19:10:38.423061 teams_ai-1.1.0/teams/ai/validators/prompt_response_validator.py
+-rw-r--r--   0        0        0      648 2024-02-28 17:27:34.002010 teams_ai-1.1.0/teams/ai/validators/validation.py
+-rw-r--r--   0        0        0    28277 2024-05-09 16:06:14.179970 teams_ai-1.1.0/teams/app.py
+-rw-r--r--   0        0        0      296 2024-02-28 17:27:34.013515 teams_ai-1.1.0/teams/app_error.py
+-rw-r--r--   0        0        0     2753 2024-05-09 16:06:14.187482 teams_ai-1.1.0/teams/app_options.py
+-rw-r--r--   0        0        0      508 2024-05-09 16:06:14.188482 teams_ai-1.1.0/teams/auth/__init__.py
+-rw-r--r--   0        0        0     4037 2024-05-09 16:06:14.196032 teams_ai-1.1.0/teams/auth/auth.py
+-rw-r--r--   0        0        0     1987 2024-05-09 16:06:14.202995 teams_ai-1.1.0/teams/auth/auth_component.py
+-rw-r--r--   0        0        0     4763 2024-05-09 16:06:14.213113 teams_ai-1.1.0/teams/auth/auth_manager.py
+-rw-r--r--   0        0        0      702 2024-05-09 16:06:14.214126 teams_ai-1.1.0/teams/auth/auth_options.py
+-rw-r--r--   0        0        0      433 2024-05-09 16:06:14.227073 teams_ai-1.1.0/teams/auth/oauth/__init__.py
+-rw-r--r--   0        0        0     4090 2024-05-09 16:06:14.238600 teams_ai-1.1.0/teams/auth/oauth/oauth.py
+-rw-r--r--   0        0        0     4739 2024-05-09 16:06:14.247705 teams_ai-1.1.0/teams/auth/oauth/oauth_adaptive_card.py
+-rw-r--r--   0        0        0     3447 2024-05-09 16:06:14.254248 teams_ai-1.1.0/teams/auth/oauth/oauth_dialog.py
+-rw-r--r--   0        0        0     4432 2024-05-09 16:06:14.265765 teams_ai-1.1.0/teams/auth/oauth/oauth_message_extension.py
+-rw-r--r--   0        0        0     1303 2024-05-09 16:06:14.278305 teams_ai-1.1.0/teams/auth/oauth/oauth_options.py
+-rw-r--r--   0        0        0      448 2024-05-09 16:06:14.285836 teams_ai-1.1.0/teams/auth/sign_in_response.py
+-rw-r--r--   0        0        0      148 2024-05-09 16:06:14.299410 teams_ai-1.1.0/teams/dialogs/__init__.py
+-rw-r--r--   0        0        0     1810 2024-05-09 16:06:14.300410 teams_ai-1.1.0/teams/dialogs/dialog.py
+-rw-r--r--   0        0        0     1137 2024-04-09 18:41:37.993611 teams_ai-1.1.0/teams/input_file.py
+-rw-r--r--   0        0        0      154 2024-02-28 17:27:34.020845 teams_ai-1.1.0/teams/meetings/__init__.py
+-rw-r--r--   0        0        0     3655 2024-05-09 16:06:14.309928 teams_ai-1.1.0/teams/meetings/meetings.py
+-rw-r--r--   0        0        0      228 2024-02-28 17:27:34.029400 teams_ai-1.1.0/teams/message_extensions/__init__.py
+-rw-r--r--   0        0        0    24325 2024-05-09 16:06:14.334577 teams_ai-1.1.0/teams/message_extensions/message_extensions.py
+-rw-r--r--   0        0        0      241 2024-02-28 17:27:34.039795 teams_ai-1.1.0/teams/message_reaction_types.py
+-rw-r--r--   0        0        0        0 2024-02-28 17:27:34.039795 teams_ai-1.1.0/teams/py.typed
+-rw-r--r--   0        0        0      328 2024-02-28 17:27:34.041095 teams_ai-1.1.0/teams/query.py
+-rw-r--r--   0        0        0      762 2024-02-28 17:27:34.049441 teams_ai-1.1.0/teams/route.py
+-rw-r--r--   0        0        0      564 2024-05-09 16:06:14.350682 teams_ai-1.1.0/teams/state/__init__.py
+-rw-r--r--   0        0        0     1365 2024-05-09 16:06:14.364841 teams_ai-1.1.0/teams/state/conversation_state.py
+-rw-r--r--   0        0        0     3481 2024-03-04 19:10:38.447269 teams_ai-1.1.0/teams/state/memory.py
+-rw-r--r--   0        0        0     4884 2024-05-09 16:06:14.379408 teams_ai-1.1.0/teams/state/state.py
+-rw-r--r--   0        0        0     1216 2024-05-09 16:06:14.386924 teams_ai-1.1.0/teams/state/temp_state.py
+-rw-r--r--   0        0        0      603 2024-05-09 16:06:14.400866 teams_ai-1.1.0/teams/state/todict.py
+-rw-r--r--   0        0        0     2466 2024-05-09 16:06:14.423060 teams_ai-1.1.0/teams/state/turn_state.py
+-rw-r--r--   0        0        0     1306 2024-05-09 16:06:14.448917 teams_ai-1.1.0/teams/state/user_state.py
+-rw-r--r--   0        0        0      239 2024-02-28 17:27:34.059743 teams_ai-1.1.0/teams/task_modules/__init__.py
+-rw-r--r--   0        0        0     6431 2024-05-09 16:06:14.474558 teams_ai-1.1.0/teams/task_modules/task_modules.py
+-rw-r--r--   0        0        0      488 2024-02-28 17:27:34.071531 teams_ai-1.1.0/teams/task_modules/task_modules_options.py
+-rw-r--r--   0        0        0     5793 2024-04-17 20:51:17.950656 teams_ai-1.1.0/teams/teams_adapter.py
+-rw-r--r--   0        0        0      325 2024-04-09 18:41:38.006774 teams_ai-1.1.0/teams/teams_attachment_downloader/__init__.py
+-rw-r--r--   0        0        0     5533 2024-04-30 21:35:02.331772 teams_ai-1.1.0/teams/teams_attachment_downloader/teams_attachment_downloader.py
+-rw-r--r--   0        0        0      463 2024-04-09 18:41:38.022774 teams_ai-1.1.0/teams/teams_attachment_downloader/teams_attachment_downloader_options.py
+-rw-r--r--   0        0        0     1190 2024-02-28 17:27:34.072531 teams_ai-1.1.0/teams/typing.py
+-rw-r--r--   0        0        0      292 2024-02-28 17:27:34.072531 teams_ai-1.1.0/teams/user_agent.py
+-rw-r--r--   0        0        0      200 2024-02-28 17:27:34.073532 teams_ai-1.1.0/teams/utils/json/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-27 21:04:22.850998 teams_ai-1.1.0/teams/utils/json/parse.py
+-rw-r--r--   0        0        0     1747 2024-02-28 17:27:34.074530 teams_ai-1.1.0/teams/utils/json/parse_object.py
+-rw-r--r--   0        0        0     4966 2024-04-01 15:45:22.007862 teams_ai-1.1.0/tests/adaptive_cards/test_adaptive_cards.py
+-rw-r--r--   0        0        0     2746 2024-02-28 17:27:34.075531 teams_ai-1.1.0/tests/ai/augmentations/test_default_augmentation.py
+-rw-r--r--   0        0        0     6562 2024-03-27 21:04:22.882484 teams_ai-1.1.0/tests/ai/augmentations/test_monologue_augmentation.py
+-rw-r--r--   0        0        0     7587 2024-03-04 19:10:38.474809 teams_ai-1.1.0/tests/ai/augmentations/test_sequence_augmentation.py
+-rw-r--r--   0        0        0     8034 2024-05-09 16:06:14.498221 teams_ai-1.1.0/tests/ai/clients/test_llm_client.py
+-rw-r--r--   0        0        0     1502 2024-02-28 17:27:34.077308 teams_ai-1.1.0/tests/ai/data_sources/test_text_data_source.py
+-rw-r--r--   0        0        0     6111 2024-04-01 15:45:22.009865 teams_ai-1.1.0/tests/ai/embeddings/test_azure_openai_embeddings.py
+-rw-r--r--   0        0        0     5222 2024-04-01 15:45:22.009865 teams_ai-1.1.0/tests/ai/embeddings/test_openai_embeddings.py
+-rw-r--r--   0        0        0     5006 2024-02-28 17:27:34.078742 teams_ai-1.1.0/tests/ai/models/test_openai_model.py
+-rw-r--r--   0        0        0     6927 2024-03-26 18:27:31.075685 teams_ai-1.1.0/tests/ai/moderators/test_azure_content_safety_moderator.py
+-rw-r--r--   0        0        0      828 2024-02-28 17:27:34.079758 teams_ai-1.1.0/tests/ai/moderators/test_default_moderator.py
+-rw-r--r--   0        0        0     9480 2024-03-04 19:10:38.486811 teams_ai-1.1.0/tests/ai/moderators/test_openai_moderator.py
+-rw-r--r--   0        0        0    32822 2024-05-09 16:06:14.508755 teams_ai-1.1.0/tests/ai/planners/test_assistants_planner.py
+-rw-r--r--   0        0        0      692 2024-02-28 17:27:34.081309 teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/actions.json
+-rw-r--r--   0        0        0      587 2024-02-28 17:27:34.081309 teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/skprompt.txt
+-rw-r--r--   0        0        0      614 2024-02-28 17:27:34.082314 teams_ai-1.1.0/tests/ai/prompts/test_assets/include_images/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.082314 teams_ai-1.1.0/tests/ai/prompts/test_assets/include_images/skprompt.txt
+-rw-r--r--   0        0        0      366 2024-02-28 17:27:34.083314 teams_ai-1.1.0/tests/ai/prompts/test_assets/migrate_old_schema/config.json
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.083314 teams_ai-1.1.0/tests/ai/prompts/test_assets/migrate_old_schema/skprompt.txt
+-rw-r--r--   0        0        0       11 2024-02-28 17:27:34.084313 teams_ai-1.1.0/tests/ai/prompts/test_assets/no_config/skprompt.txt
+-rw-r--r--   0        0        0      582 2024-02-28 17:27:34.084313 teams_ai-1.1.0/tests/ai/prompts/test_assets/no_prompt/config.json
+-rw-r--r--   0        0        0     1164 2024-02-28 17:27:34.085314 teams_ai-1.1.0/tests/ai/prompts/test_assistant_message.py
+-rw-r--r--   0        0        0     7157 2024-03-04 19:10:38.492599 teams_ai-1.1.0/tests/ai/prompts/test_conversation_history.py
+-rw-r--r--   0        0        0     1560 2024-02-28 17:27:34.085423 teams_ai-1.1.0/tests/ai/prompts/test_data_source_section.py
+-rw-r--r--   0        0        0     2175 2024-02-28 17:27:34.085423 teams_ai-1.1.0/tests/ai/prompts/test_function_call_message.py
+-rw-r--r--   0        0        0     2221 2024-02-28 17:27:34.086488 teams_ai-1.1.0/tests/ai/prompts/test_function_response_message.py
+-rw-r--r--   0        0        0     2807 2024-02-28 17:27:34.086488 teams_ai-1.1.0/tests/ai/prompts/test_group_section.py
+-rw-r--r--   0        0        0     6968 2024-02-28 17:27:34.086488 teams_ai-1.1.0/tests/ai/prompts/test_layout_engine.py
+-rw-r--r--   0        0        0     9534 2024-05-09 16:06:14.528136 teams_ai-1.1.0/tests/ai/prompts/test_prompt_manager_v2.py
+-rw-r--r--   0        0        0     8405 2024-02-28 17:27:34.087490 teams_ai-1.1.0/tests/ai/prompts/test_prompt_section_base.py
+-rw-r--r--   0        0        0     1056 2024-02-28 17:27:34.087490 teams_ai-1.1.0/tests/ai/prompts/test_system_message.py
+-rw-r--r--   0        0        0     9290 2024-03-04 19:10:38.503635 teams_ai-1.1.0/tests/ai/prompts/test_template_section.py
+-rw-r--r--   0        0        0     2319 2024-02-28 17:27:34.088994 teams_ai-1.1.0/tests/ai/prompts/test_text_section.py
+-rw-r--r--   0        0        0     7349 2024-03-04 19:10:38.509640 teams_ai-1.1.0/tests/ai/prompts/test_user_input_message.py
+-rw-r--r--   0        0        0     1048 2024-02-28 17:27:34.089504 teams_ai-1.1.0/tests/ai/prompts/test_user_message.py
+-rw-r--r--   0        0        0     1457 2024-02-28 17:27:34.089504 teams_ai-1.1.0/tests/ai/test_utilities.py
+-rw-r--r--   0        0        0      853 2024-02-28 17:27:34.089504 teams_ai-1.1.0/tests/ai/tokenizers/test_gpt_tokenizer.py
+-rw-r--r--   0        0        0     6169 2024-02-28 17:27:34.090510 teams_ai-1.1.0/tests/ai/validators/test_action_response_validator.py
+-rw-r--r--   0        0        0      822 2024-02-28 17:27:34.090510 teams_ai-1.1.0/tests/ai/validators/test_default_response_validator.py
+-rw-r--r--   0        0        0     5196 2024-02-28 17:27:34.091510 teams_ai-1.1.0/tests/ai/validators/test_json_response_validator.py
+-rw-r--r--   0        0        0     2643 2024-05-09 16:06:14.538656 teams_ai-1.1.0/tests/auth/test_auth_manager.py
+-rw-r--r--   0        0        0     4144 2024-03-26 18:27:31.075685 teams_ai-1.1.0/tests/state/test_conversation_state.py
+-rw-r--r--   0        0        0     6282 2024-05-09 16:06:14.552991 teams_ai-1.1.0/tests/state/test_custom_turn_state.py
+-rw-r--r--   0        0        0      818 2024-05-09 16:06:14.565573 teams_ai-1.1.0/tests/state/test_state.py
+-rw-r--r--   0        0        0     1797 2024-04-10 20:07:23.487380 teams_ai-1.1.0/tests/state/test_temp_state.py
+-rw-r--r--   0        0        0     6677 2024-05-09 16:06:14.583128 teams_ai-1.1.0/tests/state/test_turn_state.py
+-rw-r--r--   0        0        0     3692 2024-03-26 18:27:31.099741 teams_ai-1.1.0/tests/state/test_user_state.py
+-rw-r--r--   0        0        0     2250 2024-04-01 15:45:22.019885 teams_ai-1.1.0/tests/task_modules/test_task_modules.py
+-rw-r--r--   0        0        0    30053 2024-04-25 20:02:47.968168 teams_ai-1.1.0/tests/test_app.py
+-rw-r--r--   0        0        0    11702 2024-02-28 17:27:34.096123 teams_ai-1.1.0/tests/test_meetings.py
+-rw-r--r--   0        0        0    32052 2024-02-28 17:27:34.106581 teams_ai-1.1.0/tests/test_message_extensions.py
+-rw-r--r--   0        0        0    14794 2024-05-06 18:56:24.275371 teams_ai-1.1.0/tests/test_teams_attachment_downloader.py
+-rw-r--r--   0        0        0      146 2024-02-28 17:27:34.106581 teams_ai-1.1.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0      526 2024-02-28 17:27:34.107578 teams_ai-1.1.0/tests/utils/activity.py
+-rw-r--r--   0        0        0     1055 2024-02-28 17:27:34.107578 teams_ai-1.1.0/tests/utils/adapter.py
+-rw-r--r--   0        0        0     2774 1970-01-01 00:00:00.000000 teams_ai-1.1.0/PKG-INFO
```

### Comparing `teams_ai-1.0.1/LICENSE` & `teams_ai-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/pyproject.toml` & `teams_ai-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 [tool.poetry]
 name = "teams-ai"
-version = "1.0.1"
+version = "1.1.0"
 description = "SDK focused on building AI based applications for Microsoft Teams."
 authors = ["Microsoft <teams@microsoft.com>"]
 readme = "README.md"
 repository = "https://github.com/microsoft/teams-ai"
 documentation = "https://learn.microsoft.com/en-us/microsoftteams/platform/bots/how-to/teams%20conversational%20ai/teams-conversation-ai-overview"
 keywords = ["microsoft", "teams", "ai", "bot"]
 packages = [
     { include = "teams" },
     { include = "tests" }
 ]
 
 [tool.poetry.dependencies]
-botbuilder-core = "^4.14.8"
-botbuilder-integration-aiohttp = "^4.14.8"
-botframework-connector = "^4.14.8"
+botbuilder-core = "^4.15.0"
+botbuilder-integration-aiohttp = "^4.15.0"
+botframework-connector = "^4.15.0"
 python = ">=3.8,<4.0"
 tiktoken = "^0.4.0"
 aiohttp = "^3.8.5"
 jsonschema = "^4.21.1"
 types-pyyaml = "^6.0.12.12"
 pyyaml = "^6.0.1"
 dataclasses-json = "^0.6.4"
-openai = "^1.11.1"
 azure-ai-contentsafety = "^1.0.0"
+msal = "^1.28.0"
+botbuilder-dialogs = "^4.14.8"
+openai = "^1.27.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
-pylint = "^2.17.4"
-pytest-cov = "^4.1.0"
+pytest = "^8.1.1"
+pylint = "^3.1.0"
+pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.21.1"
-black = ">=23.7,<25.0"
+black = "24.3.0"
 isort = "^5.12.0"
 mypy = "^1.5.0"
 httpx = "^0.26.0"
 
 [tool.poetry.scripts]
 lint = "scripts:lint"
 fmt = "scripts:fmt"
@@ -44,22 +46,24 @@
 ci = "scripts:ci"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
+preview = true
 line-length = 100
 target-version = ['py38']
+enable-unstable-feature = ['string_processing', 'multiline_string_handling']
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
-addopts = "-rx --cov-report html:coverage/html --cov-report lcov:coverage/lcov.info --cov=teams"
+addopts = "-rx --cov-report html:coverage/html --cov-report lcov:coverage/lcov.info --cov=teams --verbose"
 log_cli = true
 log_cli_level = "INFO"
 
 [tool.mypy]
 python_version = "3.8"
 ignore_missing_imports = true
 show_error_codes = true
```

### Comparing `teams_ai-1.0.1/README.md` & `teams_ai-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,54 @@
 # Teams AI Library
 
 Welcome to the Teams AI Library Python package! 
 
 This SDK is specifically designed to assist you in creating bots capable of interacting with Teams and Microsoft 365 applications. It is constructed using the [Bot Framework SDK](https://github.com/microsoft/botbuilder-python) as its foundation, simplifying the process of developing bots that interact with Teams' artificial intelligence capabilities. See the [Teams AI repo README.md](https://github.com/microsoft/teams-ai), for general information.
 
+Requirements:
+*   [Python](https://www.python.org/downloads/) (>=3.8, <4.0)
+*   [Poetry](https://python-poetry.org/docs/)
+
 ## Getting Started
 
 To get started, take a look at the [getting started docs](https://github.com/microsoft/teams-ai/blob/main/getting-started/README.md).
 
+### Install Dependencies
+
+```bash
+$: poetry install
+```
+
+### Build
+
+```bash
+$: poetry build
+```
+
+### Test
+
+```bash
+$: poetry run test
+```
+
+### Lint
+
+```bash
+$: poetry run lint
+```
+
+## Format
+
+```bash
+$: poetry run fmt
+```
+
+## Clean
+
+```bash
+$: poetry run clean
+```
+
+
 ## Migration
 
 If you're migrating an existing project, switching to add on the Teams AI Library layer is quick and simple. See the [migration guide](https://github.com/microsoft/teams-ai/blob/main/getting-started/MIGRATION/PYTHON.md).
```

### Comparing `teams_ai-1.0.1/teams/__init__.py` & `teams_ai-1.1.0/teams/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/activity_type.py` & `teams_ai-1.1.0/teams/activity_type.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/adaptive_cards/adaptive_cards.py` & `teams_ai-1.1.0/teams/adaptive_cards/adaptive_cards.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,20 @@
                         return hits is not None
                     # when verb is a string
                     return verb == action_verb
 
             return False
 
         def __call__(
-            func: Callable[[TurnContext, StateT, dict], Awaitable[Union[str, dict]]]
+            func: Callable[[TurnContext, StateT, dict], Awaitable[Union[str, dict]]],
         ) -> Callable[[TurnContext, StateT, dict], Awaitable[Union[str, dict]]]:
             async def __handler__(context: TurnContext, state: StateT) -> bool:
                 result = await func(context, state, context.activity.value["action"]["data"])
-                if context.turn_state.get(ActivityTypes.invoke_response) is None:
+
+                if context.turn_state.get(context._INVOKE_RESPONSE_KEY) is None:
                     if isinstance(result, str):
                         response = AdaptiveCardInvokeResponse(
                             status_code=200,
                             type="application/vnd.microsoft.activity.message",
                             value=result,
                         )
                     else:
@@ -158,15 +159,15 @@
                     return hits is not None
                 # when verb is a string
                 return verb == filter_value
 
             return False
 
         def __call__(
-            func: Callable[[TurnContext, StateT, dict], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, dict], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, dict], Awaitable[None]]:
             async def __handler__(context: TurnContext, state: StateT) -> bool:
                 await func(context, state, context.activity.value)
                 return True
 
             self._route_registry.append(Route[StateT](__selector__, __handler__))
             return func
@@ -225,15 +226,15 @@
 
             return False
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, Query[AdaptiveCardsSearchParams]],
                 Awaitable[List[AdaptiveCardsSearchResult]],
-            ]
+            ],
         ) -> Callable[
             [TurnContext, StateT, Query[AdaptiveCardsSearchParams]],
             Awaitable[List[AdaptiveCardsSearchResult]],
         ]:
             async def __handler__(context: TurnContext, state: StateT) -> bool:
                 params = context.activity.value
                 # Flatten search parameters
@@ -250,15 +251,15 @@
                     ),
                     parameters=AdaptiveCardsSearchParams(
                         query_text=params["queryText"] if params and params["queryText"] else "",
                         dataset=params["dataset"] if params and params["dataset"] else "",
                     ),
                 )
                 result = await func(context, state, query)
-                if context.turn_state.get(ActivityTypes.invoke_response) is None:
+                if context.turn_state.get(context._INVOKE_RESPONSE_KEY) is None:
                     # Format invoke response
                     response = {
                         "type": "application/vnd.microsoft.search.searchResponse",
                         "value": {"results": result},
                     }
                     await context.send_activity(
                         Activity(
```

### Comparing `teams_ai-1.0.1/teams/ai/actions/action_entry.py` & `teams_ai-1.1.0/teams/ai/actions/action_entry.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/actions/action_turn_context.py` & `teams_ai-1.1.0/teams/ai/actions/action_turn_context.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/ai.py` & `teams_ai-1.1.0/teams/ai/ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,20 +106,18 @@
 
             if not action_name:
                 action_name = func.__name__
 
             existing = self._actions.get(action_name)
 
             if existing and not existing.allow_overrides:
-                raise ApplicationError(
-                    f"""
+                raise ApplicationError(f"""
                     The AI.action() method was called with a previously 
                     registered action named \"{action_name}\".
-                    """
-                )
+                    """)
 
             self._actions[action_name] = ActionEntry[StateT](action_name, allow_overrides, func)
             return func
 
         return __call__
 
     async def run(
@@ -224,18 +222,16 @@
         self,
         _context: ActionTurnContext[dict],
         _state: StateT,
     ) -> str:
         status = _context.data.get("status")
         message = _context.data.get("message")
         raise ApplicationError(
-            (
-                "An AI request failed because an http error occurred. "
-                f"Status code:{status}. Message:{message}"
-            )
+            "An AI request failed because an http error occurred. "
+            f"Status code:{status}. Message:{message}"
         )
 
     async def _on_plan_ready(
         self,
         context: ActionTurnContext[Plan],
         _state: StateT,
     ) -> str:
```

### Comparing `teams_ai-1.0.1/teams/ai/ai_options.py` & `teams_ai-1.1.0/teams/ai/ai_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/augmentations/augmentation.py` & `teams_ai-1.1.0/teams/ai/augmentations/augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/augmentations/default_augmentation.py` & `teams_ai-1.1.0/teams/ai/augmentations/default_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/augmentations/monologue_augmentation.py` & `teams_ai-1.1.0/teams/ai/augmentations/monologue_augmentation.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,19 +139,30 @@
         actions = self._append_say_action(actions)
         self._section = ActionAugmentationSection(
             actions=actions,
             # pylint:disable=line-too-long
             call_to_action="\n".join(
                 [
                     "Return a JSON object with your thoughts and the next action to perform.",
-                    "Only respond with the JSON format below and base your plan on the actions above.",
-                    "If you're not sure what to do, you can always say something by returning a SAY action.",
+                    (
+                        "Only respond with the JSON format below and base your plan on the actions"
+                        " above."
+                    ),
+                    (
+                        "If you're not sure what to do, you can always say something by returning a"
+                        " SAY action."
+                    ),
                     "If you're told your JSON response has errors, do your best to fix them.",
                     "Response Format:",
-                    '{"thoughts":{"thought":"<your current thought>","reasoning":"<self reflect on why you made this decision>","plan":"- short bulleted\\n- list that conveys\\n- long-term plan"},"action":{"name":"<action name>","parameters":{"<name>":"<value>"}}}',
+                    (
+                        '{"thoughts":{"thought":"<your current thought>","reasoning":"<self reflect'
+                        ' on why you made this decision>","plan":"- short bulleted\\n- list that'
+                        ' conveys\\n- long-term plan"},"action":{"name":"<action'
+                        ' name>","parameters":{"<name>":"<value>"}}}'
+                    ),
                 ]
             ),
         )
         self._action_validator = ActionResponseValidator(actions, True)
 
     def create_prompt_section(self) -> Union[PromptSection, None]:
         """
```

### Comparing `teams_ai-1.0.1/teams/ai/augmentations/sequence_augmentation.py` & `teams_ai-1.1.0/teams/ai/augmentations/sequence_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/clients/llm_client.py` & `teams_ai-1.1.0/teams/ai/clients/llm_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     LLMClient class that's used to complete prompts.
     """
 
     _options: LLMClientOptions
 
     @property
     def options(self) -> LLMClientOptions:
-        return self.options
+        return self._options
 
     def __init__(self, options: LLMClientOptions) -> None:
         """
         Creates a new `LLMClient` instance.
 
         Args:
             options (LLMClientOptions): Options to configure the instance with.
```

### Comparing `teams_ai-1.0.1/teams/ai/data_sources/data_source.py` & `teams_ai-1.1.0/teams/ai/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/data_sources/text_data_source.py` & `teams_ai-1.1.0/teams/ai/data_sources/text_data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/embeddings/__init__.py` & `teams_ai-1.1.0/teams/ai/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings.py` & `teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,18 @@
             self.options.azure_api_version = "2023-05-15"
 
         endpoint = self.options.azure_endpoint.strip()
         if endpoint[-1] == "/":
             endpoint = endpoint[0 : (len(endpoint) - 1)]
 
         if not endpoint.lower().startswith("https://"):
-            raise ValueError(
-                f"""
+            raise ValueError(f"""
                 Client created with an invalid endpoint of \"{endpoint}\".
                 The endpoint must be a valid HTTPS url.
-                """
-            )
+                """)
 
         self.options.azure_endpoint = endpoint
 
     async def create_embeddings(
         self, inputs: Union[str, List[str], List[int], List[List[int]]], retry_count=0
     ) -> EmbeddingsResponse:
         """
```

### Comparing `teams_ai-1.0.1/teams/ai/embeddings/azure_openai_embeddings_options.py` & `teams_ai-1.1.0/teams/ai/embeddings/azure_openai_embeddings_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/embeddings/embeddings_model.py` & `teams_ai-1.1.0/teams/ai/embeddings/embeddings_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/embeddings/embeddings_response.py` & `teams_ai-1.1.0/teams/ai/embeddings/embeddings_response.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings.py` & `teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/embeddings/openai_embeddings_options.py` & `teams_ai-1.1.0/teams/ai/embeddings/openai_embeddings_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/models/__init__.py` & `teams_ai-1.1.0/teams/ai/models/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/models/chat_completion_action.py` & `teams_ai-1.1.0/teams/ai/models/chat_completion_action.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/models/openai_model.py` & `teams_ai-1.1.0/teams/ai/models/openai_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,18 +188,19 @@
                 max_tokens=max_tokens,
             )
 
             if self._options.logger is not None:
                 self._options.logger.debug("COMPLETION:\n%s", completion.model_dump_json())
 
             input: Optional[Message] = None
-            output_length = len(res.output)
+            last_message = len(res.output) - 1
 
-            if output_length > 0 and res.output[output_length - 1].role == "user":
-                input = res.output[output_length - 1]
+            # Skips the first message which is the prompt
+            if last_message > 0 and res.output[last_message].role == "user":
+                input = res.output[last_message]
 
             return PromptResponse[str](
                 input=input,
                 message=Message(
                     role=completion.choices[0].message.role,
                     content=completion.choices[0].message.content,
                 ),
```

### Comparing `teams_ai-1.0.1/teams/ai/models/prompt_completion_model.py` & `teams_ai-1.1.0/teams/ai/models/prompt_completion_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/models/prompt_response.py` & `teams_ai-1.1.0/teams/ai/models/prompt_response.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/moderators/__init__.py` & `teams_ai-1.1.0/teams/ai/moderators/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/moderators/azure_content_safety_moderator.py` & `teams_ai-1.1.0/teams/ai/moderators/azure_content_safety_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/moderators/default_moderator.py` & `teams_ai-1.1.0/teams/ai/moderators/default_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/moderators/moderator.py` & `teams_ai-1.1.0/teams/ai/moderators/moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/moderators/openai_moderator.py` & `teams_ai-1.1.0/teams/ai/moderators/openai_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/planners/__init__.py` & `teams_ai-1.1.0/teams/ai/planners/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,23 +4,28 @@
 """
 
 from .action_planner import (
     ActionPlanner,
     ActionPlannerOptions,
     ActionPlannerPromptFactory,
 )
-from .assistants_planner import AssistantsPlanner, AssistantsPlannerOptions
+from .assistants_planner import (
+    AssistantsPlanner,
+    AzureOpenAIAssistantsOptions,
+    OpenAIAssistantsOptions,
+)
 from .plan import Plan, PredictedCommand, PredictedDoCommand, PredictedSayCommand
 from .planner import Planner
 
 __all__ = [
     "ActionPlanner",
     "ActionPlannerOptions",
     "AssistantsPlanner",
-    "AssistantsPlannerOptions",
+    "OpenAIAssistantsOptions",
+    "AzureOpenAIAssistantsOptions",
     "ActionPlannerPromptFactory",
     "Plan",
     "PredictedCommand",
     "PredictedDoCommand",
     "PredictedSayCommand",
     "Planner",
 ]
```

### Comparing `teams_ai-1.0.1/teams/ai/planners/action_planner.py` & `teams_ai-1.1.0/teams/ai/planners/action_planner.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/planners/assistants_planner.py` & `teams_ai-1.1.0/teams/ai/planners/assistants_planner.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 """
 
 from __future__ import annotations
 
 import asyncio
 import json
 from dataclasses import dataclass
-from typing import Dict, Generic, List, Optional, TypeVar
+from importlib.metadata import version
+from typing import Dict, Generic, List, Optional, TypeVar, Union
 
 import openai
 from botbuilder.core import TurnContext
 from dataclasses_json import DataClassJsonMixin, dataclass_json
 from openai.types.beta.assistant import Assistant
 from openai.types.beta.assistant_create_params import AssistantCreateParams
 from openai.types.beta.threads import Run
@@ -39,17 +40,48 @@
 class AssistantsState(DataClassJsonMixin):
     thread_id: Optional[str] = ""
     run_id: Optional[str] = ""
     last_message_id: Optional[str] = ""
 
 
 @dataclass
-class AssistantsPlannerOptions:
+class AzureOpenAIAssistantsOptions:
     """
-    Options for configuring the AssistantsPlanner.
+    Options for configuring the AssistantsPlanner for AzureOpenAI.
+    """
+
+    api_key: str
+    "The AzureOpenAI API key."
+
+    default_model: str
+    "Default name of the Azure OpenAI deployment (model) to use."
+
+    assistant_id: str
+    "The ID of the assistant to use."
+
+    endpoint: str
+    "Deployment endpoint to use."
+
+    polling_interval: float = DEFAULT_POLLING_INTERVAL
+    "Optional. Polling interval in seconds. Defaults to 1 second"
+
+    assistants_state_variable: str = DEFAULT_ASSISTANTS_STATE_VARIABLE
+    "Optional. The state variable to use for storing the assistants state."
+
+    api_version: str = "2024-02-15-preview"
+    "Optional. Version of the API being called. Defaults to `2024-02-15-preview`."
+
+    organization: Optional[str] = None
+    "Optional. Organization to use when calling the API."
+
+
+@dataclass
+class OpenAIAssistantsOptions:
+    """
+    Options for configuring the AssistantsPlanner with OpenAI.
     """
 
     api_key: str
     "The OpenAI API key."
 
     assistant_id: str
     "The ID of the assistant to use."
@@ -64,50 +96,57 @@
     "Optional organization."
 
     endpoint: Optional[str] = None
     "Optional endpoint."
 
 
 class AssistantsPlanner(Generic[StateT], _UserAgent, Planner[StateT]):
-    "A planner that uses the OpenAI Assistants API."
+    "A planner that uses the Assistants API."
 
-    _options: AssistantsPlannerOptions
+    _options: Union[OpenAIAssistantsOptions, AzureOpenAIAssistantsOptions]
     _client: openai.AsyncOpenAI
 
     @property
-    def options(self) -> AssistantsPlannerOptions:
+    def options(self) -> Union[OpenAIAssistantsOptions, AzureOpenAIAssistantsOptions]:
         return self._options
 
     @property
     def client(self) -> openai.AsyncOpenAI:
         return self._client
 
     def __init__(
-        self, options: AssistantsPlannerOptions, client: Optional[openai.AsyncOpenAI] = None
+        self,
+        options: Union[OpenAIAssistantsOptions, AzureOpenAIAssistantsOptions],
     ) -> None:
         """
         Creates a new `AssistantsPlanner` instance.
 
         Args:
             options (AssistantsPlannerOptions): Options used to configure the planner.
             client (Optional[openai.AsyncOpenAI]): The OpenAI client.
 
         """
 
         self._options = options
-        self._client = (
-            client
-            if client is not None
-            else openai.AsyncOpenAI(
+
+        if isinstance(options, OpenAIAssistantsOptions):
+            self._client = openai.AsyncOpenAI(
                 api_key=options.api_key,
                 organization=options.organization,
                 default_headers={"User-Agent": self.user_agent},
                 base_url=options.endpoint,
             )
-        )
+        elif isinstance(options, AzureOpenAIAssistantsOptions):
+            self._client = openai.AsyncAzureOpenAI(
+                api_key=options.api_key,
+                api_version=options.api_version,
+                azure_endpoint=options.endpoint,
+                organization=options.organization if options.organization else None,
+                default_headers={"User-Agent": self.user_agent},
+            )
 
     async def begin_task(self, context: TurnContext, state: TurnState) -> Plan:
         """
         Starts a new task.
         This method is called when the AI system is ready to start a new task. The planner should
         generate a plan that the AI system will execute. Returning an empty plan signals that
         there is no work to be performed. The planner should take the users input
@@ -143,24 +182,25 @@
         thread_id = await self._ensure_thread_created(state)
 
         # Add the users input to the thread or send tool outputs
         if state.get(SUBMIT_TOOL_OUTPUTS_VARIABLE) is True:
             # Send the tool output to the assistant
             return await self._submit_action_results(state)
 
-        # Wait for any current runs to complete since you can'tadd messages
+        # Wait for any current runs to complete since you can't add messages
         # or start new runs if there's already one in progress
         await self._block_on_in_progress_runs(thread_id)
 
         # Submit user input
         return await self._submit_user_input(state)
 
     @staticmethod
     async def create_assistant(
         api_key: str,
+        api_version: Optional[str],
         organization: Optional[str],
         endpoint: Optional[str],
         request: AssistantCreateParams,
     ) -> Assistant:
         """
         Static method for programmatically creating an assistant.
 
@@ -169,24 +209,36 @@
             organization (Optional[str]): The optional organization.
             endpoint: (Optional[str]): The optional endpoint.
             request: (AssistantCreateParams): The parameters used to create the assistant.
 
         Returns:
             Assistant: The assistant.
         """
-        openai_client = openai.AsyncOpenAI(
-            api_key=api_key,
-            organization=organization if organization else None,
-            base_url=endpoint if endpoint else None,
-        )
+        client: openai.AsyncOpenAI
 
-        return await openai_client.beta.assistants.create(
+        if endpoint:
+            # Use AzureOpenAI
+            user_agent = f"teamsai-py/{version('teams-ai')}"
+            client = openai.AsyncAzureOpenAI(
+                api_key=api_key,
+                api_version=api_version if api_version else "2024-02-15-preview",
+                azure_endpoint=endpoint,
+                organization=organization if organization else None,
+                default_headers={"User-Agent": user_agent},
+            )
+        else:
+            # Use OpenAI
+            client = openai.AsyncOpenAI(
+                api_key=api_key,
+                organization=organization,
+            )
+
+        return await client.beta.assistants.create(
             model=request.get("model", ""),
             description=request.get("description"),
-            file_ids=request.get("file_ids", []),
             instructions=request.get("instructions"),
             metadata=request.get("metadata"),
             name=request.get("name"),
             tools=request.get("tools", []),
         )
 
     async def _ensure_thread_created(self, state: TurnState) -> str:
@@ -213,15 +265,15 @@
         action_outputs = state.temp.action_outputs
         tool_map = state.get(SUBMIT_TOOL_OUTPUTS_MAP)
         tool_outputs: List[ToolOutput] = []
 
         for action in action_outputs:
             output = action_outputs[action]
             if tool_map:
-                tool_call_id = tool_map[action]
+                tool_call_id = tool_map[action] if action in tool_map else None
                 if tool_call_id is not None:
                     # Add required output only
                     tool_outputs.append(ToolOutput(tool_call_id=tool_call_id, output=output))
 
         # Submit the tool outputs
         if assistants_state.thread_id and assistants_state.run_id:
             run = await self._client.beta.threads.runs.submit_tool_outputs(
@@ -242,19 +294,20 @@
                         assistants_state.thread_id, assistants_state.last_message_id
                     )
                 if results.status == "cancelled":
                     return Plan()
                 if results.status == "expired":
                     return Plan(commands=[PredictedDoCommand(action=ActionTypes.TOO_MANY_STEPS)])
 
-                if results.last_error:
-                    raise ApplicationError(
-                        f"Run failed {results.status}. ErrorCode: "
-                        + f"{results.last_error.code}. ErrorMessage: {results.last_error.message}"
-                    )
+                error_code = results.last_error.code if results.last_error is not None else ""
+                error_message = results.last_error.message if results.last_error is not None else ""
+                raise ApplicationError(
+                    f"Run failed {results.status}. ErrorCode: "
+                    + f"{error_code}. ErrorMessage: {error_message}"
+                )
         return Plan()
 
     async def _wait_for_run(
         self, thread_id: str, run_id: str, handle_actions: bool = False
     ) -> Optional[Run]:
         while True:
             await asyncio.sleep(self.options.polling_interval)
@@ -307,15 +360,21 @@
                     plan.commands.append(PredictedSayCommand(response=content.text.value))
 
         return plan
 
     async def _block_on_in_progress_runs(self, thread_id: str) -> None:
         # We loop until we're told the last run is completed
         while True:
-            run = await self._retrieve_last_run(thread_id)
+            runs = await self._client.beta.threads.runs.list(thread_id, limit=1)
+
+            if len(runs.data) == 0:
+                return
+
+            run = runs.data[0]
+
             if not run:
                 return
             if self._is_run_completed(run):
                 return
 
             # Wait for the current run to complete and then
             # loop to see if there's already a new run.
@@ -355,25 +414,26 @@
         # Update state and wait for the run to complete
         state.set(
             self._options.assistants_state_variable, AssistantsState(thread_id, run.id, message.id)
         )
         results = await self._wait_for_run(thread_id, run.id, True)
 
         if results:
-            if results.status == "required_action":
+            if results.status == "requires_action" and results.required_action is not None:
                 state.set(SUBMIT_TOOL_OUTPUTS_VARIABLE, True)
                 return self._generate_plan_from_tools(state, results.required_action)
             if results.status == "completed":
                 state.set(SUBMIT_TOOL_OUTPUTS_VARIABLE, False)
                 return await self._generate_plan_from_messages(thread_id, message.id)
             if results.status == "cancelled":
                 return Plan()
             if results.status == "expired":
                 return Plan(commands=[PredictedDoCommand(action=ActionTypes.TOO_MANY_STEPS)])
 
-            if results.last_error:
-                raise ApplicationError(
-                    f"Run failed {results.status}. ErrorCode: "
-                    + f"{results.last_error.code}. ErrorMessage: {results.last_error.message}"
-                )
+            error_code = results.last_error.code if results.last_error is not None else ""
+            error_message = results.last_error.message if results.last_error is not None else ""
+            raise ApplicationError(
+                f"Run failed {results.status}. ErrorCode: "
+                + f"{error_code}. ErrorMessage: {error_message}"
+            )
 
         return Plan()
```

### Comparing `teams_ai-1.0.1/teams/ai/planners/plan.py` & `teams_ai-1.1.0/teams/ai/planners/plan.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/planners/planner.py` & `teams_ai-1.1.0/teams/ai/planners/planner.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/__init__.py` & `teams_ai-1.1.0/teams/ai/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/assistant_message.py` & `teams_ai-1.1.0/teams/ai/prompts/assistant_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/augmentation_config.py` & `teams_ai-1.1.0/teams/ai/prompts/augmentation_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/completion_config.py` & `teams_ai-1.1.0/teams/ai/prompts/completion_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/function_call_message.py` & `teams_ai-1.1.0/teams/ai/prompts/function_call_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/function_response_message.py` & `teams_ai-1.1.0/teams/ai/prompts/function_response_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/message.py` & `teams_ai-1.1.0/teams/ai/prompts/message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/prompt.py` & `teams_ai-1.1.0/teams/ai/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/prompt_functions.py` & `teams_ai-1.1.0/teams/ai/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/prompt_manager.py` & `teams_ai-1.1.0/teams/ai/prompts/prompt_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,18 +222,16 @@
             PromptManager: The prompt manager for chaining.
 
         Raises:
             ApplicationError: If a prompt with the same name already exists.
         """
         if prompt.name in self._prompts:
             raise ApplicationError(
-                (
-                    "The PromptManager.add_prompt() method was called with a "
-                    f"previously registered prompt named '{prompt.name}'."
-                )
+                "The PromptManager.add_prompt() method was called with a "
+                f"previously registered prompt named '{prompt.name}'."
             )
 
         # Clone and cache prompt
         self._prompts[prompt.name] = deepcopy(prompt)
         return self
 
     async def get_prompt(self, name: str) -> PromptTemplate:
@@ -264,32 +262,28 @@
 
             # Load prompt config
             try:
                 with open(config_file, "r", encoding="utf-8") as file:
                     template_config = PromptTemplateConfig.from_dict(json.load(file))
             except Exception as e:
                 raise ApplicationError(
-                    (
-                        "PromptManager.get_prompt(): an error occurred while loading "
-                        f"'{config_file}'. The file is either invalid or missing."
-                    )
+                    "PromptManager.get_prompt(): an error occurred while loading "
+                    f"'{config_file}'. The file is either invalid or missing."
                 ) from e
 
             # Load prompt text
             sections: List[PromptSection] = []
             try:
                 with open(prompt_file, "r", encoding="utf-8") as file:
                     prompt = file.read()
                     sections.append(TemplateSection(prompt, self._options.role))
             except Exception as e:
                 raise ApplicationError(
-                    (
-                        "PromptManager.get_prompt(): an error occurred while loading "
-                        f"'{prompt_file}'. The file is either invalid or missing."
-                    )
+                    "PromptManager.get_prompt(): an error occurred while loading "
+                    f"'{prompt_file}'. The file is either invalid or missing."
                 ) from e
 
             # Load optional actions
             template_actions: List[ChatCompletionAction] = []
             try:
                 with open(actions_file, "r", encoding="utf-8") as file:
                     actions = json.load(file)
```

### Comparing `teams_ai-1.0.1/teams/ai/prompts/prompt_manager_options.py` & `teams_ai-1.1.0/teams/ai/prompts/prompt_manager_options.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/prompt_template.py` & `teams_ai-1.1.0/teams/ai/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/prompt_template_config.py` & `teams_ai-1.1.0/teams/ai/prompts/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/rendered_prompt_section.py` & `teams_ai-1.1.0/teams/ai/prompts/rendered_prompt_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/__init__.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/action_augmentation_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/action_augmentation_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/conversation_history_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/conversation_history_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/data_source_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/data_source_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/group_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/group_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/layout_engine_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/layout_engine_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/prompt_section_base.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/prompt_section_base.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/template_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/template_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/sections/text_section.py` & `teams_ai-1.1.0/teams/ai/prompts/sections/text_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/system_message.py` & `teams_ai-1.1.0/teams/ai/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/user_input_message.py` & `teams_ai-1.1.0/teams/ai/prompts/user_input_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/prompts/user_message.py` & `teams_ai-1.1.0/teams/ai/prompts/user_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/tokenizers/gpt_tokenizer.py` & `teams_ai-1.1.0/teams/ai/tokenizers/gpt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/tokenizers/tokenizer.py` & `teams_ai-1.1.0/teams/ai/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/utilities.py` & `teams_ai-1.1.0/teams/ai/utilities.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/validators/__init__.py` & `teams_ai-1.1.0/teams/ai/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/validators/action_response_validator.py` & `teams_ai-1.1.0/teams/ai/validators/action_response_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,42 +90,48 @@
 
         if message is None or func is None:
             if not self._required:
                 return Validation()
 
             return Validation(
                 valid=False,
-                feedback=f"No {self._noun} was specified. "
-                f"Call a {self._noun} with valid arguments.",
+                feedback=(
+                    f"No {self._noun} was specified. Call a {self._noun} with valid arguments."
+                ),
             )
 
         if func.name is None:
             return Validation(
                 valid=False,
                 feedback=f"{self._noun} name missing. Specify a valid {self._noun} name.",
             )
 
         if not func.name in self._actions:
             return Validation(
                 valid=False,
-                feedback=f'Unknown {self._noun} named "{func.name}". '
-                f"Specify a valid {self._noun} name.",
+                feedback=(
+                    f'Unknown {self._noun} named "{func.name}". Specify a valid {self._noun} name.'
+                ),
             )
 
         params: Dict[str, Any] = {}
         action = self._actions[func.name]
 
         if action.parameters is not None:
             validator = JSONResponseValidator(
                 schema=action.parameters,
-                missing_json_feedback=f"No arguments were sent with called {self._noun}. "
-                f'Call the "{func.name}" {self._noun} with required '
-                f"arguments as a valid JSON object.",
-                error_feedback=f"The {self._noun} arguments had errors. "
-                f'Apply these fixes and call "{func.name}" {self._noun} again:',
+                missing_json_feedback=(
+                    f"No arguments were sent with called {self._noun}. "
+                    f'Call the "{func.name}" {self._noun} with required '
+                    "arguments as a valid JSON object."
+                ),
+                error_feedback=(
+                    f"The {self._noun} arguments had errors. "
+                    f'Apply these fixes and call "{func.name}" {self._noun} again:'
+                ),
             )
 
             res = await validator.validate_response(
                 context=context,
                 memory=memory,
                 tokenizer=tokenizer,
                 remaining_attempts=remaining_attempts,
```

### Comparing `teams_ai-1.0.1/teams/ai/validators/default_response_validator.py` & `teams_ai-1.1.0/teams/ai/validators/default_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/validators/json_response_validator.py` & `teams_ai-1.1.0/teams/ai/validators/json_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/validators/prompt_response_validator.py` & `teams_ai-1.1.0/teams/ai/validators/prompt_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/ai/validators/validation.py` & `teams_ai-1.1.0/teams/ai/validators/validation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/app.py` & `teams_ai-1.1.0/teams/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     TypeVar,
     Union,
     cast,
 )
 
 from aiohttp.web import Request, Response
 from botbuilder.core import Bot, TurnContext
-from botbuilder.schema import ActivityTypes
+from botbuilder.schema import Activity, ActivityTypes, InvokeResponse
 from botbuilder.schema.teams import (
     FileConsentCardResponse,
     O365ConnectorCardActionQuery,
 )
 
 from .activity_type import (
     ActivityType,
@@ -33,23 +33,25 @@
     MessageReactionType,
     MessageUpdateType,
 )
 from .adaptive_cards.adaptive_cards import AdaptiveCards
 from .ai import AI
 from .app_error import ApplicationError
 from .app_options import ApplicationOptions
+from .auth import AuthManager, OAuth, OAuthOptions
 from .meetings.meetings import Meetings
 from .message_extensions.message_extensions import MessageExtensions
 from .route import Route, RouteHandler
 from .state import TurnState
 from .task_modules import TaskModules
 from .teams_adapter import TeamsAdapter
 from .typing import Typing
 
 StateT = TypeVar("StateT", bound=TurnState)
+IN_SIGN_IN_KEY = "__InSignInFlow__"
 
 
 class Application(Bot, Generic[StateT]):
     """
     Application class for routing and processing incoming requests.
 
     The Application object replaces the traditional ActivityHandler that
@@ -63,14 +65,15 @@
 
     typing: Typing
 
     _ai: Optional[AI[StateT]]
     _adaptive_card: AdaptiveCards[StateT]
     _options: ApplicationOptions
     _adapter: Optional[TeamsAdapter] = None
+    _auth: Optional[AuthManager[StateT]] = None
     _before_turn: List[RouteHandler[StateT]] = []
     _after_turn: List[RouteHandler[StateT]] = []
     _routes: List[Route[StateT]] = []
     _error: Optional[Callable[[TurnContext, Exception], Awaitable[None]]] = None
     _turn_state_factory: Optional[Callable[[TurnContext], Awaitable[StateT]]] = None
     _message_extensions: MessageExtensions[StateT]
     _task_modules: TaskModules[StateT]
@@ -90,57 +93,71 @@
         )
         self._task_modules = TaskModules[StateT](
             self._routes, options.task_modules.task_data_filter
         )
         self._meetings = Meetings[StateT](self._routes)
 
         if options.long_running_messages and (not options.adapter or not options.bot_app_id):
-            raise ApplicationError(
-                """
+            raise ApplicationError("""
                 The `ApplicationOptions.long_running_messages` property is unavailable because 
                 no adapter or `bot_app_id` was configured.
-                """
-            )
+                """)
 
         if options.adapter:
             self._adapter = options.adapter
 
+        if options.auth:
+            self._auth = AuthManager[StateT](default=options.auth.default)
+
+            for name, opts in options.auth.settings.items():
+                if isinstance(opts, OAuthOptions):
+                    self._auth.set(name, OAuth[StateT](opts))
+
     @property
     def adapter(self) -> TeamsAdapter:
         """
         The bot's adapter.
         """
 
         if not self._adapter:
-            raise ApplicationError(
-                """
+            raise ApplicationError("""
                 The Application.adapter property is unavailable because it was 
                 not configured when creating the Application.
-                """
-            )
+                """)
 
         return self._adapter
 
     @property
     def ai(self) -> AI[StateT]:
         """
         This property is only available if the Application was configured with 'ai' options.
         An exception will be thrown if you attempt to access it otherwise.
         """
 
         if not self._ai:
-            raise ApplicationError(
-                """
+            raise ApplicationError("""
                 The `Application.ai` property is unavailable because no AI options were configured.
-                """
-            )
+                """)
 
         return self._ai
 
     @property
+    def auth(self) -> AuthManager[StateT]:
+        """
+        The application's authentication manager
+        """
+        if not self._auth:
+            raise ApplicationError("""
+                The `Application.auth` property is unavailable because
+                no Auth options were configured.
+                """)
+
+        return self._auth
+
+    @property
     def options(self) -> ApplicationOptions:
         """
         The application's configured options.
         """
         return self._options
 
     @property
@@ -413,15 +430,15 @@
                 context.activity.type == ActivityTypes.invoke
                 and context.activity.name == "fileConsent/invoke"
                 and isinstance(context.activity.value, dict)
                 and context.activity.value.get("action") == "accept"
             )
 
         def __call__(
-            func: Callable[[TurnContext, StateT, FileConsentCardResponse], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, FileConsentCardResponse], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, FileConsentCardResponse], Awaitable[None]]:
             async def __handler__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
                 await func(context, state, context.activity.value)
                 return True
 
@@ -455,15 +472,15 @@
                 context.activity.type == ActivityTypes.invoke
                 and context.activity.name == "fileConsent/invoke"
                 and isinstance(context.activity.value, dict)
                 and context.activity.value.get("action") == "decline"
             )
 
         def __call__(
-            func: Callable[[TurnContext, StateT, FileConsentCardResponse], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, FileConsentCardResponse], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, FileConsentCardResponse], Awaitable[None]]:
             async def __handler__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
                 await func(context, state, context.activity.value)
                 return True
 
@@ -495,27 +512,70 @@
         def __selector__(context: TurnContext) -> bool:
             return (
                 context.activity.type == ActivityTypes.invoke
                 and context.activity.name == "actionableMessage/executeAction"
             )
 
         def __call__(
-            func: Callable[[TurnContext, StateT, O365ConnectorCardActionQuery], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, O365ConnectorCardActionQuery], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, O365ConnectorCardActionQuery], Awaitable[None]]:
             async def __handler__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
                 await func(context, state, context.activity.value)
                 return True
 
             self._routes.append(Route[StateT](__selector__, __handler__, True))
             return func
 
         return __call__
 
+    def handoff(
+        self,
+    ) -> Callable[
+        [Callable[[TurnContext, StateT, str], Awaitable[None]]],
+        Callable[[TurnContext, StateT, str], Awaitable[None]],
+    ]:
+        """
+        Registers a handler to handoff conversations from one copilot to another.
+         ```python
+        # Use this method as a decorator
+        @app.handoff
+        async def on_handoff(
+            context: TurnContext, state: TurnState, continuation: str
+        ):
+            print(query)
+        # Pass a function to this method
+        app.handoff()(on_handoff)
+        ```
+        """
+
+        def __selector__(context: TurnContext) -> bool:
+            return (
+                context.activity.type == ActivityTypes.invoke
+                and context.activity.name == "handoff/action"
+            )
+
+        def __call__(
+            func: Callable[[TurnContext, StateT, str], Awaitable[None]],
+        ) -> Callable[[TurnContext, StateT, str], Awaitable[None]]:
+            async def __handler__(context: TurnContext, state: StateT):
+                if not context.activity.value:
+                    return False
+                await func(context, state, context.activity.value["continuation"])
+                await context.send_activity(
+                    Activity(type=ActivityTypes.invoke_response, value=InvokeResponse(status=200))
+                )
+                return True
+
+            self._routes.append(Route[StateT](__selector__, __handler__, True))
+            return func
+
+        return __call__
+
     def before_turn(self, func: RouteHandler[StateT]) -> RouteHandler[StateT]:
         """
         Registers a new event listener that will be executed before turns.
         This method can be used as either a decorator or a method and
         is called in the order they are registered.
 
         ```python
@@ -616,22 +676,72 @@
 
             if self._turn_state_factory:
                 state = await self._turn_state_factory(context)
 
             await state.load(context, self._options.storage)
             state.temp.input = context.activity.text
 
+            # authentication
+            if (
+                self.options.auth
+                and self._auth
+                and (
+                    (
+                        (
+                            isinstance(self.options.auth.auto, bool)
+                            and self.options.auth.auto is True
+                        )
+                        or (
+                            callable(self.options.auth.auto)
+                            and self.options.auth.auto(context) is True
+                        )
+                    )
+                    or IN_SIGN_IN_KEY in state.user
+                )
+            ):
+                key: Optional[str] = (
+                    state.user[IN_SIGN_IN_KEY]
+                    if IN_SIGN_IN_KEY in state.user
+                    else self.options.auth.default
+                )
+
+                if key is not None:
+                    state.user[IN_SIGN_IN_KEY] = key
+                    res = await self._auth.sign_in(context, state, key=key)
+
+                    if res.status == "complete":
+                        del state.user[IN_SIGN_IN_KEY]
+
+                    if res.status == "pending":
+                        await state.save(context, self._options.storage)
+                        return
+
+                    if res.status == "error" and res.reason != "invalid-activity":
+                        del state.user[IN_SIGN_IN_KEY]
+                        raise ApplicationError(f"[{res.reason}] => {res.message}")
+
             # run before turn middleware
             for before_turn in self._before_turn:
                 is_ok = await before_turn(context, state)
 
                 if not is_ok:
                     await state.save(context, self._options.storage)
                     return
 
+            # download input files
+            if (
+                self._options.file_downloaders is not None
+                and len(self._options.file_downloaders) > 0
+            ):
+                input_files = state.temp.input_files if state.temp.input_files is not None else []
+                for file_downloader in self._options.file_downloaders:
+                    files = await file_downloader.download_files(context)
+                    input_files.append(files)
+                state.temp.input_files = input_files
+
             # run activity handlers
             is_ok, matches = await self._on_activity(context, state)
 
             if not is_ok:
                 await state.save(context, self._options.storage)
                 return
```

### Comparing `teams_ai-1.0.1/teams/app_options.py` & `teams_ai-1.1.0/teams/app_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,38 @@
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from logging import Logger
-from typing import Optional
+from typing import List, Optional
 
 from botbuilder.core import Storage
 
 from .adaptive_cards import AdaptiveCardsOptions
 from .ai import AIOptions
+from .auth import AuthOptions
+from .input_file import InputFileDownloader
 from .task_modules import TaskModulesOptions
 from .teams_adapter import TeamsAdapter
 
 
 @dataclass
 class ApplicationOptions:
     adapter: Optional[TeamsAdapter] = None
     """
     Optional. Options used to initialize your `BotAdapter`
     """
 
+    auth: Optional[AuthOptions] = None
+    """
+    Optional. Auth settings.
+    """
+
     bot_app_id: str = ""
     """
     Optional. `Application` ID of the bot.
     """
 
     storage: Optional[Storage] = None
     """
@@ -73,7 +80,12 @@
     Optional. Options used to customize the processing of Adaptive Card requests.
     """
 
     task_modules: TaskModulesOptions = field(default_factory=TaskModulesOptions)
     """
     Optional. Options used to customize the processing of Task Module requests.
     """
+
+    file_downloaders: List[InputFileDownloader] = field(default_factory=list)
+    """
+    Optional. Array of input file download plugins to use. 
+    """
```

### Comparing `teams_ai-1.0.1/teams/meetings/meetings.py` & `teams_ai-1.1.0/teams/meetings/meetings.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             return (
                 context.activity.type == ActivityTypes.event
                 and context.activity.channel_id == "msteams"
                 and context.activity.name == "application/vnd.microsoft.meetingStart"
             )
 
         def __call__(
-            func: Callable[[TurnContext, StateT, MeetingStartEventDetails], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, MeetingStartEventDetails], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, MeetingStartEventDetails], Awaitable[None]]:
             async def __handler__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
                 await func(context, state, context.activity.value)
                 return True
 
@@ -90,15 +90,15 @@
             return (
                 context.activity.type == ActivityTypes.event
                 and context.activity.channel_id == "msteams"
                 and context.activity.name == "application/vnd.microsoft.meetingEnd"
             )
 
         def __call__(
-            func: Callable[[TurnContext, StateT, MeetingEndEventDetails], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, MeetingEndEventDetails], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, MeetingEndEventDetails], Awaitable[None]]:
             async def __handler__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
                 await func(context, state, context.activity.value)
                 return True
```

### Comparing `teams_ai-1.0.1/teams/message_extensions/message_extensions.py` & `teams_ai-1.1.0/teams/message_extensions/message_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
             return self._activity_with_command_id(context.activity, command_id)
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, MessagingExtensionQuery],
                 Awaitable[MessagingExtensionResult],
-            ]
+            ],
         ) -> Callable[
             [TurnContext, StateT, MessagingExtensionQuery],
             Awaitable[MessagingExtensionResult],
         ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
@@ -144,15 +144,15 @@
 
             return self._activity_with_command_id(context.activity, command_id)
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, str],
                 Awaitable[MessagingExtensionResult],
-            ]
+            ],
         ) -> Callable[
             [TurnContext, StateT, str],
             Awaitable[MessagingExtensionResult],
         ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
@@ -203,15 +203,15 @@
                 or context.activity.name != "composeExtension/anonymousQueryLink"
             ):
                 return False
 
             return self._activity_with_command_id(context.activity, command_id)
 
         def __call__(
-            func: Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult]]
+            func: Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult]],
         ) -> Callable[[TurnContext, StateT, str], Awaitable[MessagingExtensionResult]]:
             async def __invoke__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
 
                 value = cast(
                     AppBasedLinkQuery,
@@ -258,15 +258,15 @@
                 return False
             return True
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT],
                 Awaitable[MessagingExtensionResult],
-            ]
+            ],
         ) -> Callable[[TurnContext, StateT], Awaitable[MessagingExtensionResult]]:
             async def __invoke__(context: TurnContext, state: StateT):
                 res = await func(context, state)
                 await self._invoke_action_response(context, res)
                 return True
 
             self._routes.append(Route[StateT](__selector__, __invoke__, True))
@@ -300,15 +300,15 @@
                 context.activity.type != ActivityTypes.invoke
                 or context.activity.name != "composeExtension/setting"
             ):
                 return False
             return True
 
         def __call__(
-            func: Callable[[TurnContext, StateT, Any], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, Any], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, Any], Awaitable[None]]:
             async def __invoke__(context: TurnContext, state: StateT):
                 value = {}
                 if context.activity.value:
                     value = context.activity.value
 
                 await func(context, state, value)
@@ -346,15 +346,15 @@
                 context.activity.type != ActivityTypes.invoke
                 or context.activity.name != "composeExtension/onCardButtonClicked"
             ):
                 return False
             return True
 
         def __call__(
-            func: Callable[[TurnContext, StateT, Any], Awaitable[None]]
+            func: Callable[[TurnContext, StateT, Any], Awaitable[None]],
         ) -> Callable[[TurnContext, StateT, Any], Awaitable[None]]:
             async def __invoke__(context: TurnContext, state: StateT):
                 value = {}
                 if context.activity.value:
                     value = context.activity.value
 
                 await func(context, state, value)
@@ -424,15 +424,15 @@
 
             return True
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, Activity],
                 Awaitable[Union[MessagingExtensionResult, TaskModuleTaskInfo, str, None]],
-            ]
+            ],
         ) -> Callable[
             [TurnContext, StateT, Activity],
             Awaitable[Union[MessagingExtensionResult, TaskModuleTaskInfo, str, None]],
         ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
@@ -489,15 +489,15 @@
 
             return self._activity_with_command_id(context.activity, command_id)
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT],
                 Awaitable[Union[TaskModuleTaskInfo, str]],
-            ]
+            ],
         ) -> Callable[
             [TurnContext, StateT],
             Awaitable[Union[TaskModuleTaskInfo, str]],
         ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 res = await func(context, state)
                 await self._invoke_task_response(context, res)
@@ -538,15 +538,15 @@
 
             return True
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, Any],
                 Awaitable[MessagingExtensionResult],
-            ]
+            ],
         ) -> Callable[
             [TurnContext, StateT, Any],
             Awaitable[MessagingExtensionResult],
         ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 res = await func(context, state, context.activity.value)
                 await self._invoke_action_response(context, res)
@@ -597,15 +597,15 @@
 
             return self._activity_with_command_id(context.activity, command_id)
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, Any],
                 Awaitable[Union[MessagingExtensionResult, TaskModuleTaskInfo, str, None]],
-            ]
+            ],
         ) -> Callable[
             [TurnContext, StateT, Any],
             Awaitable[Union[MessagingExtensionResult, TaskModuleTaskInfo, str, None]],
         ]:
             async def __invoke__(context: TurnContext, state: StateT):
                 if not context.activity.value:
                     return False
```

### Comparing `teams_ai-1.0.1/teams/route.py` & `teams_ai-1.1.0/teams/route.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/state/__init__.py` & `teams_ai-1.1.0/teams/state/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
 from .conversation_state import ConversationState
 from .memory import Memory, MemoryBase
-from .state import State, state
+from .state import State, StatePropertyAccessor, state
 from .temp_state import TempState
 from .todict import todict
 from .turn_state import TurnState
 from .user_state import UserState
 
 __all__ = [
     "ConversationState",
     "Memory",
     "MemoryBase",
     "state",
     "State",
+    "StatePropertyAccessor",
     "TurnState",
     "UserState",
     "TempState",
     "todict",
 ]
```

### Comparing `teams_ai-1.0.1/teams/state/conversation_state.py` & `teams_ai-1.1.0/teams/state/conversation_state.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from botbuilder.core import Storage, StoreItem, TurnContext
 
 from .state import State, state
 
 
 @state
-class ConversationState(State[Any]):
+class ConversationState(State):
     """
     Default Conversation State
     """
 
     @classmethod
     async def load(
         cls, context: TurnContext, storage: Optional[Storage] = None
@@ -39,11 +39,11 @@
         if not storage:
             return cls(__key__=key)
 
         data: Dict[str, Any] = await storage.read([key])
 
         if key in data:
             if isinstance(data[key], StoreItem):
-                return cls(__key__=key, **data[key].__dict__)
+                return cls(__key__=key, **vars(data[key]))
             return cls(__key__=key, **data[key])
 
         return cls(__key__=key, **data)
```

### Comparing `teams_ai-1.0.1/teams/state/memory.py` & `teams_ai-1.1.0/teams/state/memory.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/state/state.py` & `teams_ai-1.1.0/teams/state/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
 import json
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union, overload
+from copy import deepcopy
+from typing import Any, Callable, List, Optional, Type, TypeVar, Union, overload
 
+from botbuilder.core import StatePropertyAccessor as _StatePropertyAccessor
 from botbuilder.core import Storage, TurnContext
 
 from .todict import todict
 
 T = TypeVar("T")
 
 
@@ -31,19 +33,15 @@
         ...
     """
 
     def wrap(cls: Type[T]) -> Type[T]:
         init = cls.__init__
 
         def __init__(self, *args, **kwargs) -> None:
-            self.__deleted__ = []
-            self.__key__ = kwargs["__key__"] if "__key__" in kwargs else ""
-
-            for key, value in kwargs.items():
-                setattr(self, key, value)
+            State.__init__(self, args, kwargs)
 
             if init is not None:
                 init(self, *args, **kwargs)
 
         cls.__init__ = __init__  # type: ignore[method-assign]
 
         if not hasattr(cls, "save"):
@@ -53,15 +51,15 @@
 
     if _cls is None:
         return wrap
 
     return wrap(_cls)
 
 
-class State(Dict[str, T], ABC):
+class State(dict, ABC):
     """
     State
     """
 
     __key__: str
     """
     The Storage Key
@@ -69,104 +67,120 @@
 
     __deleted__: List[str]
     """
     Deleted Keys
     """
 
     def __init__(self, *args, **kwargs) -> None:  # pylint: disable=unused-argument
-        ...
+        super().__init__()
+        self.__key__ = kwargs["__key__"] if "__key__" in kwargs else ""
+        self.__deleted__ = []
+
+        # copy public attributes that are not functions
+        for name in dir(self):
+            value = object.__getattribute__(self, name)
+
+            if not name.startswith("_") and not callable(value):
+                self[name] = deepcopy(value)
+
+        for key, value in kwargs.items():
+            if not key in ("__key__", "__deleted__"):
+                self[key] = value
 
     async def save(self, _context: TurnContext, storage: Optional[Storage] = None) -> None:
         """
         Saves The State to Storage
 
         Args:
             context (TurnContext): the turn context.
             storage (Optional[Storage]): storage to save to.
         """
         if not storage or self.__key__ == "":
             return
 
-        data = self.__dict__.copy()
-        del data["__key__"]
-
         await storage.delete(self.__deleted__)
         await storage.write(
             {
-                self.__key__: data,
+                self.__key__: self.copy(),
             }
         )
 
+        self.__deleted__ = []
+
     @classmethod
     @abstractmethod
-    async def load(cls, context: TurnContext, storage: Optional[Storage] = None) -> "State[T]":
+    async def load(cls, context: TurnContext, storage: Optional[Storage] = None) -> "State":
         """
         Loads The State from Storage
 
         Args:
             context: (TurnContext): the turn context.
             storage (Optional[Storage]): storage to read from.
         """
+        return cls()
 
-    def clear(self) -> None:
-        return self.__dict__.clear()
-
-    def copy(self) -> Dict[str, T]:
-        return self.__dict__.copy()
-
-    def has_key(self, key: str) -> bool:
-        return key in self.__dict__
-
-    def update(self, *args, **kwargs) -> None:
-        return self.__dict__.update(*args, **kwargs)
-
-    def keys(self):
-        return self.__dict__.keys()
-
-    def values(self):
-        return self.__dict__.values()
-
-    def items(self):
-        return self.__dict__.items()
-
-    def pop(self, *args):
-        return self.__dict__.pop(*args)
+    def create_property(self, name: str) -> _StatePropertyAccessor:
+        return StatePropertyAccessor(self, name)
 
-    def __setitem__(self, key: str, item: T) -> None:
-        self.__dict__[key] = item
+    def __setitem__(self, key: str, item: Any) -> None:
+        super().__setitem__(key, item)
 
         if key in self.__deleted__:
             self.__deleted__.remove(key)
 
-    def __getitem__(self, key: str) -> T:
-        return self.__dict__[key]
-
     def __delitem__(self, key: str) -> None:
-        if key in self.__dict__ and isinstance(self.__dict__[key], State):
-            self.__deleted__.append(self.__dict__[key].__key__)
-        del self.__dict__[key]
+        if key in self and isinstance(self[key], State):
+            self.__deleted__.append(self[key].__key__)
 
-    def __setattr__(self, key: str, value: T) -> None:
-        super().__setattr__(key, value)
+        super().__delitem__(key)
 
-        if key in self.__deleted__:
-            self.__deleted__.remove(key)
+    def __setattr__(self, key: str, value: Any) -> None:
+        if key.startswith("_") or callable(value):
+            object.__setattr__(self, key, value)
+            return
 
-    def __delattr__(self, key: str) -> None:
-        if key in self.__dict__ and isinstance(self.__dict__[key], State):
-            self.__deleted__.append(self.__dict__[key].__key__)
-        super().__delattr__(key)
+        self[key] = value
 
-    def __repr__(self) -> str:
-        return repr(self.__dict__)
+    def __getattr__(self, key: str) -> Any:
+        return self[key]
 
-    def __len__(self) -> int:
-        return len(self.__dict__)
+    def __getattribute__(self, key: str) -> Any:
+        if key in self:
+            return self[key]
 
-    def __contains__(self, item: Any):
-        return item in self.__dict__
+        return object.__getattribute__(self, key)
 
-    def __iter__(self):
-        return iter(self.__dict__)
+    def __delattr__(self, key: str) -> None:
+        del self[key]
 
     def __str__(self) -> str:
         return json.dumps(todict(self))
+
+
+class StatePropertyAccessor(_StatePropertyAccessor):
+    _name: str
+    _state: State
+
+    def __init__(self, state: State, name: str) -> None:
+        self._name = name
+        self._state = state
+
+    async def get(
+        self,
+        turn_context: TurnContext,
+        default_value_or_factory: Optional[Union[Any, Callable[[], Optional[Any]]]] = None,
+    ) -> Optional[Any]:
+        value = self._state[self._name] if self._name in self._state else None
+
+        if value is None and default_value_or_factory is not None:
+            if callable(default_value_or_factory):
+                value = default_value_or_factory()
+            else:
+                value = default_value_or_factory
+
+        return value
+
+    async def delete(self, turn_context: TurnContext) -> None:
+        del self._state[self._name]
+
+    async def set(self, turn_context: TurnContext, value: Any) -> None:
+        self._state[self._name] = value
```

### Comparing `teams_ai-1.0.1/teams/state/temp_state.py` & `teams_ai-1.1.0/teams/state/temp_state.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional
 
 from botbuilder.core import Storage, TurnContext
 
 from ..input_file import InputFile
 from .state import State, state
 
 
 @state
-class TempState(State[Any]):
+class TempState(State):
     """
     Default Temp State
     """
 
     input: str = ""
     "Input passed from the user to the AI Library"
 
@@ -33,11 +33,14 @@
 
     auth_tokens: Dict[str, str] = {}
     "User authentication tokens"
 
     duplicate_token_exchange: Optional[bool] = None
     "Flag indicating whether a token exchange event has already been processed"
 
+    async def save(self, _context: TurnContext, storage: Optional[Storage] = None) -> None:
+        return
+
     @classmethod
     async def load(cls, context: TurnContext, storage: Optional[Storage] = None) -> "TempState":
         # pylint: disable=unused-argument
         return cls()
```

### Comparing `teams_ai-1.0.1/teams/state/todict.py` & `teams_ai-1.1.0/teams/state/todict.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,17 @@
     Converts a value to a
     dictionary recursively
     """
 
     if isinstance(value, dict):
         data = {}
         for key, val in value.items():
-            if key.startswith("_"):
-                continue
             data[key] = todict(val)
         return data
-    if hasattr(value, "_ast"):
-        return todict(value._ast())
-    if hasattr(value, "__iter__") and not isinstance(value, str):
+
+    if isinstance(value, list):
         return [todict(v) for v in value]
-    if hasattr(value, "__dict__"):
+
+    if isinstance(value, object) and hasattr(value, "__dict__"):
         return todict(value.__dict__)
+
     return value
```

### Comparing `teams_ai-1.0.1/teams/state/turn_state.py` & `teams_ai-1.1.0/teams/state/turn_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ConversationStateT = TypeVar("ConversationStateT", bound=ConversationState)
 UserStateT = TypeVar("UserStateT", bound=UserState)
 TempStateT = TypeVar("TempStateT", bound=TempState)
 
 
 @state
-class TurnState(MemoryBase, State[State[Any]], Generic[ConversationStateT, UserStateT, TempStateT]):
+class TurnState(MemoryBase, State, Generic[ConversationStateT, UserStateT, TempStateT]):
     """
     Default Turn State
     """
 
     conversation: ConversationStateT
     user: UserStateT
     temp: TempStateT
```

### Comparing `teams_ai-1.0.1/teams/state/user_state.py` & `teams_ai-1.1.0/teams/state/user_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from botbuilder.core import Storage, StoreItem, TurnContext
 
 from .state import State, state
 
 
 @state
-class UserState(State[Any]):
+class UserState(State):
     """
     Default User State
     """
 
     @classmethod
     async def load(cls, context: TurnContext, storage: Optional[Storage] = None) -> "UserState":
         activity = context.activity
@@ -37,11 +37,11 @@
         if not storage:
             return cls(__key__=key)
 
         data: Dict[str, Any] = await storage.read([key])
 
         if key in data:
             if isinstance(data[key], StoreItem):
-                return cls(__key__=key, **data[key].__dict__)
+                return cls(__key__=key, **vars(data[key]))
             return cls(__key__=key, **data[key])
 
         return cls(__key__=key, **data)
```

### Comparing `teams_ai-1.0.1/teams/task_modules/task_modules.py` & `teams_ai-1.1.0/teams/task_modules/task_modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         # Create route selector for the handler
         def __selector__(context: TurnContext) -> bool:
             return self._task_modules_selector(
                 context, verb, self._task_data_filter, FETCH_INVOKE_NAME
             )
 
         def __call__(
-            func: Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str]]]
+            func: Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str]]],
         ) -> Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str]]]:
             async def __handler__(context: TurnContext, state: StateT) -> bool:
                 # the selector already ensures data exists
                 result = await func(context, state, context.activity.value["data"])
                 await self._send_response(context, result)
                 return True
 
@@ -107,15 +107,15 @@
             return self._task_modules_selector(
                 context, verb, self._task_data_filter, SUBMIT_INVOKE_NAME
             )
 
         def __call__(
             func: Callable[
                 [TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str, None]]
-            ]
+            ],
         ) -> Callable[[TurnContext, StateT, dict], Awaitable[Union[TaskModuleTaskInfo, str, None]]]:
             async def __handler__(context: TurnContext, state: StateT) -> bool:
                 # the selector already ensures data exists
                 result = await func(context, state, context.activity.value["data"])
                 await self._send_response(context, result)
                 return True
 
@@ -143,15 +143,15 @@
                     return hits is not None
                 # when verb is a string
                 return verb == data[filter_field]
 
         return False
 
     async def _send_response(self, context: TurnContext, result):
-        if context.turn_state.get(ActivityTypes.invoke_response) is None:
+        if context.turn_state.get(context._INVOKE_RESPONSE_KEY) is None:
             if isinstance(result, str):
                 response = TaskModuleResponse(task=TaskModuleMessageResponse(value=result))
             elif isinstance(result, TaskModuleTaskInfo):
                 response = TaskModuleResponse(task=TaskModuleContinueResponse(value=result))
             else:
                 response = None
```

### Comparing `teams_ai-1.0.1/teams/teams_adapter.py` & `teams_ai-1.1.0/teams/teams_adapter.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,39 +2,70 @@
 Copyright (c) Microsoft Corporation. All rights reserved.
 Licensed under the MIT License.
 """
 
 from __future__ import annotations
 
 from logging import Logger
-from typing import Any, Optional, cast
+from typing import Any, Awaitable, Callable, Optional, cast
 
 from aiohttp import ClientResponse, ClientResponseError, ClientSession
 from aiohttp.web import Request, Response, WebSocketResponse
 from botbuilder.core import Bot
+from botbuilder.core.turn_context import TurnContext
 from botbuilder.integration.aiohttp import (
     CloudAdapter,
     ConfigurationBotFrameworkAuthentication,
+    ConfigurationServiceClientCredentialFactory,
+)
+from botbuilder.schema import Activity
+from botframework.connector import (
+    ConnectorClient,
+    HttpClientBase,
+    HttpRequest,
+    HttpResponseBase,
 )
-from botframework.connector import HttpClientBase, HttpRequest, HttpResponseBase
 from botframework.connector.auth import (
     AuthenticationConfiguration,
+    ClaimsIdentity,
     HttpClientFactory,
     ServiceClientCredentialsFactory,
 )
+from botframework.connector.auth.connector_factory import ConnectorFactory
+from botframework.connector.auth.user_token_client import UserTokenClient
 
 from .user_agent import _UserAgent
 
 
 class TeamsAdapter(CloudAdapter, _UserAgent):
     """
     An adapter that implements the Bot Framework Protocol
     and can be hosted in different cloud environments both public and private.
     """
 
+    _credentials_factory: ServiceClientCredentialsFactory
+    "The credentials factory used by the bot adapter to create a [ServiceClientCredentials] object."
+    _configuration: Any
+
+    @property
+    def credentials_factory(self) -> ServiceClientCredentialsFactory:
+        """
+        The bot's credentials factory.
+        """
+
+        return self._credentials_factory
+
+    @property
+    def configuration(self) -> Any:
+        """
+        The bot's configuration.
+        """
+
+        return self._configuration
+
     def __init__(
         self,
         configuration: Any,
         *,
         credentials_factory: Optional[ServiceClientCredentialsFactory] = None,
         auth_configuration: Optional[AuthenticationConfiguration] = None,
         http_client_factory: Optional[HttpClientFactory] = None,
@@ -50,14 +81,21 @@
                 credentials_factory=cast(ServiceClientCredentialsFactory, credentials_factory),
                 auth_configuration=cast(AuthenticationConfiguration, auth_configuration),
                 http_client_factory=_TeamsHttpClientFactory(parent=http_client_factory),
                 logger=cast(Logger, logger),
             )
         )
 
+        self._configuration = configuration
+        self._credentials_factory = (
+            cast(ServiceClientCredentialsFactory, credentials_factory)
+            if credentials_factory
+            else ConfigurationServiceClientCredentialFactory(configuration)
+        )
+
     async def process(
         self,
         request: Request,
         bot: Bot,
         ws_response: Optional[WebSocketResponse] = None,
     ) -> Optional[Response]:
         res = await super().process(
@@ -67,14 +105,38 @@
         )
 
         if res is not None:
             res.headers.add("User-Agent", self.user_agent)
 
         return res
 
+    def _create_turn_context(
+        self,
+        activity: Activity,
+        claims_identity: ClaimsIdentity,
+        oauth_scope: str,
+        connector_client: ConnectorClient,
+        user_token_client: UserTokenClient,
+        logic: Callable[[TurnContext], Awaitable],
+        connector_factory: ConnectorFactory,
+    ) -> TurnContext:
+        connector_client.config.add_user_agent(self.user_agent)
+        connector_client.conversations.config.add_user_agent(self.user_agent)
+        connector_client.attachments.config.add_user_agent(self.user_agent)
+
+        return super()._create_turn_context(
+            activity,
+            claims_identity,
+            oauth_scope,
+            connector_client,
+            user_token_client,
+            logic,
+            connector_factory,
+        )
+
 
 class _TeamsHttpClientFactory(HttpClientFactory):
     _parent: Optional[HttpClientFactory]
 
     def __init__(self, *, parent: Optional[HttpClientFactory] = None) -> None:
         self._parent = parent
```

### Comparing `teams_ai-1.0.1/teams/typing.py` & `teams_ai-1.1.0/teams/typing.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/utils/json/parse.py` & `teams_ai-1.1.0/teams/utils/json/parse.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/teams/utils/json/parse_object.py` & `teams_ai-1.1.0/teams/utils/json/parse_object.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/adaptive_cards/test_adaptive_cards.py` & `teams_ai-1.1.0/tests/adaptive_cards/test_adaptive_cards.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/augmentations/test_default_augmentation.py` & `teams_ai-1.1.0/tests/ai/augmentations/test_default_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/augmentations/test_monologue_augmentation.py` & `teams_ai-1.1.0/tests/ai/augmentations/test_monologue_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/augmentations/test_sequence_augmentation.py` & `teams_ai-1.1.0/tests/ai/augmentations/test_sequence_augmentation.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/data_sources/test_text_data_source.py` & `teams_ai-1.1.0/tests/ai/data_sources/test_text_data_source.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/embeddings/test_azure_openai_embeddings.py` & `teams_ai-1.1.0/tests/ai/embeddings/test_azure_openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/embeddings/test_openai_embeddings.py` & `teams_ai-1.1.0/tests/ai/embeddings/test_openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/models/test_openai_model.py` & `teams_ai-1.1.0/tests/ai/models/test_openai_model.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/moderators/test_azure_content_safety_moderator.py` & `teams_ai-1.1.0/tests/ai/moderators/test_azure_content_safety_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/moderators/test_default_moderator.py` & `teams_ai-1.1.0/tests/ai/moderators/test_default_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/moderators/test_openai_moderator.py` & `teams_ai-1.1.0/tests/ai/moderators/test_openai_moderator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/actions.json` & `teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/actions.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_assets/happy_path/config.json` & `teams_ai-1.1.0/tests/ai/prompts/test_assets/happy_path/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_assets/include_images/config.json` & `teams_ai-1.1.0/tests/ai/prompts/test_assets/include_images/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_assets/no_prompt/config.json` & `teams_ai-1.1.0/tests/ai/prompts/test_assets/no_prompt/config.json`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_assistant_message.py` & `teams_ai-1.1.0/tests/ai/prompts/test_assistant_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_conversation_history.py` & `teams_ai-1.1.0/tests/ai/prompts/test_conversation_history.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_data_source_section.py` & `teams_ai-1.1.0/tests/ai/prompts/test_data_source_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_function_call_message.py` & `teams_ai-1.1.0/tests/ai/prompts/test_function_call_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_function_response_message.py` & `teams_ai-1.1.0/tests/ai/prompts/test_function_response_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_group_section.py` & `teams_ai-1.1.0/tests/ai/prompts/test_group_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_layout_engine.py` & `teams_ai-1.1.0/tests/ai/prompts/test_layout_engine.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_prompt_manager_v2.py` & `teams_ai-1.1.0/tests/ai/prompts/test_prompt_manager_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,18 +78,16 @@
         prompt = MagicMock(spec=PromptTemplate)
         prompt.name = "test"
         self.prompt_manager.add_prompt(prompt)
         with self.assertRaises(ApplicationError) as context:
             self.prompt_manager.add_prompt(prompt)
         self.assertEqual(
             str(context.exception),
-            (
-                "The PromptManager.add_prompt() method was called with a "
-                "previously registered prompt named 'test'."
-            ),
+            "The PromptManager.add_prompt() method was called with a "
+            "previously registered prompt named 'test'.",
         )
 
     def test_has_prompt_from_file(self):
         self.assertTrue(self.prompt_manager.has_prompt("happy_path"))
 
     def test_has_prompt_not_found(self):
         self.assertFalse(self.prompt_manager.has_prompt("not_found"))
```

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_prompt_section_base.py` & `teams_ai-1.1.0/tests/ai/prompts/test_prompt_section_base.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_system_message.py` & `teams_ai-1.1.0/tests/ai/prompts/test_system_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_template_section.py` & `teams_ai-1.1.0/tests/ai/prompts/test_template_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_text_section.py` & `teams_ai-1.1.0/tests/ai/prompts/test_text_section.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_user_input_message.py` & `teams_ai-1.1.0/tests/ai/prompts/test_user_input_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/prompts/test_user_message.py` & `teams_ai-1.1.0/tests/ai/prompts/test_user_message.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/test_utilities.py` & `teams_ai-1.1.0/tests/ai/test_utilities.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/tokenizers/test_gpt_tokenizer.py` & `teams_ai-1.1.0/tests/ai/tokenizers/test_gpt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/validators/test_action_response_validator.py` & `teams_ai-1.1.0/tests/ai/validators/test_action_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/validators/test_default_response_validator.py` & `teams_ai-1.1.0/tests/ai/validators/test_default_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/ai/validators/test_json_response_validator.py` & `teams_ai-1.1.0/tests/ai/validators/test_json_response_validator.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/state/test_conversation_state.py` & `teams_ai-1.1.0/tests/state/test_conversation_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/state/test_custom_turn_state.py` & `teams_ai-1.1.0/tests/state/test_custom_turn_state.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         if not storage:
             return cls(__key__="other")
 
         data: Dict[str, Any] = await storage.read(["other"])
 
         if "other" in data:
             if isinstance(data["other"], StoreItem):
-                return cls(__key__="other", **data["other"].__dict__)
+                return cls(__key__="other", **vars(data["other"]))
             return cls(__key__="other", **data["other"])
         return cls(__key__="other")
 
 
 class CustomTurnState(TurnState):
     conversation: CustomConversationState
     user: CustomUserState
@@ -152,20 +152,23 @@
         self.assertEqual(turn_state.other.test, 0)
 
     async def test_should_json(self):
         context = self.create_mock_context()
         storage = MemoryStorage()
         turn_state = await CustomTurnState.load(context, storage)
 
-        self.assertFalse("test" in turn_state.other)
+        self.assertTrue("test" in turn_state.other)
         turn_state.other.test = 100
 
         await turn_state.save(context, storage)
         turn_state = await CustomTurnState.load(context, storage)
 
         self.assertTrue("other" in turn_state)
         self.assertTrue("test" in turn_state.other)
         self.assertEqual(turn_state.other.test, 100)
         self.assertEqual(str(turn_state.other), '{"test": 100}')
         self.assertEqual(
-            str(turn_state), '{"conversation": {}, "user": {}, "temp": {}, "other": {"test": 100}}'
+            str(turn_state),
+            '{"conversation": {}, "user": {}, "temp": {"action_outputs": {}, "auth_tokens": {},'
+            ' "duplicate_token_exchange": null, "input": "", "input_files": [], "last_output": ""},'
+            ' "other": {"test": 100}}',
         )
```

### Comparing `teams_ai-1.0.1/tests/state/test_temp_state.py` & `teams_ai-1.1.0/tests/state/test_temp_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/state/test_turn_state.py` & `teams_ai-1.1.0/tests/state/test_turn_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,18 @@
         turn_state = await AppTurnState.load(context, storage)
 
         turn_state.conversation["hello"] = "world"
         await turn_state.save(context, storage)
         turn_state = await AppTurnState.load(context, storage)
 
         self.assertEqual(
-            str(turn_state), '{"conversation": {"hello": "world"}, "user": {}, "temp": {}}'
+            str(turn_state),
+            '{"conversation": {"hello": "world"}, "user": {}, "temp": {"action_outputs": {},'
+            ' "auth_tokens": {}, "duplicate_token_exchange": null, "input": "",'
+            ' "input_files": [], "last_output": ""}}',
         )
 
     async def test_has(self):
         context = self.create_mock_context()
         storage = MemoryStorage()
 
         await storage.write(
```

### Comparing `teams_ai-1.0.1/tests/state/test_user_state.py` & `teams_ai-1.1.0/tests/state/test_user_state.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/task_modules/test_task_modules.py` & `teams_ai-1.1.0/tests/task_modules/test_task_modules.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/test_app.py` & `teams_ai-1.1.0/tests/test_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,7 +746,32 @@
                         },
                     },
                 ),
             )
         )
 
         on_file_consent_decline.assert_not_called()
+
+    @pytest.mark.asyncio
+    async def test_handoff(self):
+        on_handoff = mock.AsyncMock()
+        self.app.handoff()(on_handoff)
+
+        await self.app.on_turn(
+            TurnContext(
+                SimpleAdapter(),
+                Activity(
+                    id="1234",
+                    type="invoke",
+                    name="handoff/action",
+                    from_property=ChannelAccount(id="user", name="User Name"),
+                    recipient=ChannelAccount(id="bot", name="Bot Name"),
+                    conversation=ConversationAccount(id="convo", name="Convo Name"),
+                    channel_id="UnitTest",
+                    locale="en-uS",
+                    service_url="https://example.org",
+                    value={"continuation": "test"},
+                ),
+            )
+        )
+
+        on_handoff.assert_called_once()
```

### Comparing `teams_ai-1.0.1/tests/test_meetings.py` & `teams_ai-1.1.0/tests/test_meetings.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/test_message_extensions.py` & `teams_ai-1.1.0/tests/test_message_extensions.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/utils/activity.py` & `teams_ai-1.1.0/tests/utils/activity.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/tests/utils/adapter.py` & `teams_ai-1.1.0/tests/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `teams_ai-1.0.1/PKG-INFO` & `teams_ai-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,87 @@
 Metadata-Version: 2.1
 Name: teams-ai
-Version: 1.0.1
+Version: 1.1.0
 Summary: SDK focused on building AI based applications for Microsoft Teams.
 Home-page: https://github.com/microsoft/teams-ai
 Keywords: microsoft,teams,ai,bot
 Author: Microsoft
 Author-email: teams@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: azure-ai-contentsafety (>=1.0.0,<2.0.0)
-Requires-Dist: botbuilder-core (>=4.14.8,<5.0.0)
-Requires-Dist: botbuilder-integration-aiohttp (>=4.14.8,<5.0.0)
-Requires-Dist: botframework-connector (>=4.14.8,<5.0.0)
+Requires-Dist: botbuilder-core (>=4.15.0,<5.0.0)
+Requires-Dist: botbuilder-dialogs (>=4.14.8,<5.0.0)
+Requires-Dist: botbuilder-integration-aiohttp (>=4.15.0,<5.0.0)
+Requires-Dist: botframework-connector (>=4.15.0,<5.0.0)
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
-Requires-Dist: openai (>=1.11.1,<2.0.0)
+Requires-Dist: msal (>=1.28.0,<2.0.0)
+Requires-Dist: openai (>=1.27.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: types-pyyaml (>=6.0.12.12,<7.0.0.0)
 Project-URL: Documentation, https://learn.microsoft.com/en-us/microsoftteams/platform/bots/how-to/teams%20conversational%20ai/teams-conversation-ai-overview
 Project-URL: Repository, https://github.com/microsoft/teams-ai
 Description-Content-Type: text/markdown
 
 # Teams AI Library
 
 Welcome to the Teams AI Library Python package! 
 
 This SDK is specifically designed to assist you in creating bots capable of interacting with Teams and Microsoft 365 applications. It is constructed using the [Bot Framework SDK](https://github.com/microsoft/botbuilder-python) as its foundation, simplifying the process of developing bots that interact with Teams' artificial intelligence capabilities. See the [Teams AI repo README.md](https://github.com/microsoft/teams-ai), for general information.
 
+Requirements:
+*   [Python](https://www.python.org/downloads/) (>=3.8, <4.0)
+*   [Poetry](https://python-poetry.org/docs/)
+
 ## Getting Started
 
 To get started, take a look at the [getting started docs](https://github.com/microsoft/teams-ai/blob/main/getting-started/README.md).
 
+### Install Dependencies
+
+```bash
+$: poetry install
+```
+
+### Build
+
+```bash
+$: poetry build
+```
+
+### Test
+
+```bash
+$: poetry run test
+```
+
+### Lint
+
+```bash
+$: poetry run lint
+```
+
+## Format
+
+```bash
+$: poetry run fmt
+```
+
+## Clean
+
+```bash
+$: poetry run clean
+```
+
+
 ## Migration
 
 If you're migrating an existing project, switching to add on the Teams AI Library layer is quick and simple. See the [migration guide](https://github.com/microsoft/teams-ai/blob/main/getting-started/MIGRATION/PYTHON.md).
```

