# Comparing `tmp/swarms-4.9.2.tar.gz` & `tmp/swarms-4.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-4.9.2.tar", max compression
+gzip compressed data, was "swarms-4.9.3.tar", max compression
```

## Comparing `swarms-4.9.2.tar` & `swarms-4.9.3.tar`

### file list

```diff
@@ -1,219 +1,217 @@
--rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.9.2/LICENSE
--rw-r--r--   0        0        0    39270 2024-05-03 20:53:27.848296 swarms-4.9.2/README.md
--rw-r--r--   0        0        0     1802 2024-05-03 22:58:33.201721 swarms-4.9.2/pyproject.toml
--rw-r--r--   0        0        0      590 2024-04-02 02:30:28.406904 swarms-4.9.2/swarms/__init__.py
--rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.9.2/swarms/agents/__init__.py
--rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.9.2/swarms/agents/agent_wrapper.py
--rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.9.2/swarms/agents/base.py
--rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.9.2/swarms/agents/developer_agents.py
--rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.9.2/swarms/agents/omni_modal_agent.py
--rw-r--r--   0        0        0     3491 2024-04-27 21:17:36.621105 swarms-4.9.2/swarms/agents/simple_agent.py
--rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.9.2/swarms/agents/stopping_conditions.py
--rw-r--r--   0        0        0     4940 2024-04-27 21:17:36.621832 swarms-4.9.2/swarms/agents/tool_agent.py
--rw-r--r--   0        0        0     5504 2024-05-02 21:56:49.171951 swarms-4.9.2/swarms/agents/worker_agent.py
--rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.9.2/swarms/artifacts/__init__.py
--rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.9.2/swarms/artifacts/base_artifact.py
--rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.9.2/swarms/artifacts/text_artifact.py
--rw-r--r--   0        0        0      613 2024-04-27 21:17:36.623130 swarms-4.9.2/swarms/memory/__init__.py
--rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.9.2/swarms/memory/action_subtask.py
--rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.9.2/swarms/memory/base_db.py
--rw-r--r--   0        0        0     2823 2024-04-27 21:17:36.624819 swarms-4.9.2/swarms/memory/base_vectordb.py
--rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.9.2/swarms/memory/dict_internal_memory.py
--rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-4.9.2/swarms/memory/dict_shared_memory.py
--rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-4.9.2/swarms/memory/short_term_memory.py
--rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.9.2/swarms/memory/visual_memory.py
--rw-r--r--   0        0        0     2603 2024-05-03 22:04:47.953292 swarms-4.9.2/swarms/models/__init__.py
--rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-4.9.2/swarms/models/base_embedding_model.py
--rw-r--r--   0        0        0    13168 2024-04-27 21:17:36.635065 swarms-4.9.2/swarms/models/base_llm.py
--rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-4.9.2/swarms/models/base_multimodal_model.py
--rw-r--r--   0        0        0     2475 2024-04-27 21:17:36.635700 swarms-4.9.2/swarms/models/base_tts.py
--rw-r--r--   0        0        0     3163 2024-04-27 21:17:36.636332 swarms-4.9.2/swarms/models/base_ttv.py
--rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-4.9.2/swarms/models/cog_vlm.py
--rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-4.9.2/swarms/models/dalle3.py
--rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-4.9.2/swarms/models/distilled_whisperx.py
--rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-4.9.2/swarms/models/embeddings_base.py
--rw-r--r--   0        0        0     2726 2024-04-27 21:17:36.637208 swarms-4.9.2/swarms/models/fire_function.py
--rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.9.2/swarms/models/fuyu.py
--rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-4.9.2/swarms/models/gemini.py
--rw-r--r--   0        0        0    14214 2024-04-18 12:43:27.452395 swarms-4.9.2/swarms/models/gpt4_vision_api.py
--rw-r--r--   0        0        0    12996 2024-04-27 21:17:36.638023 swarms-4.9.2/swarms/models/huggingface.py
--rw-r--r--   0        0        0     1826 2024-04-27 21:17:36.638977 swarms-4.9.2/swarms/models/huggingface_pipeline.py
--rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-4.9.2/swarms/models/idefics.py
--rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-4.9.2/swarms/models/kosmos_two.py
--rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.9.2/swarms/models/layoutlm_document_qa.py
--rw-r--r--   0        0        0     6581 2024-04-27 21:17:36.639950 swarms-4.9.2/swarms/models/llama_function_caller.py
--rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.9.2/swarms/models/llava.py
--rw-r--r--   0        0        0     4286 2024-04-27 21:17:36.641073 swarms-4.9.2/swarms/models/mistral.py
--rw-r--r--   0        0        0     2147 2024-04-27 21:17:36.642823 swarms-4.9.2/swarms/models/mixtral.py
--rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.9.2/swarms/models/moondream_mm.py
--rw-r--r--   0        0        0     6448 2024-04-18 12:43:27.582607 swarms-4.9.2/swarms/models/mpt.py
--rw-r--r--   0        0        0     2823 2024-04-18 12:43:27.453365 swarms-4.9.2/swarms/models/nougat.py
--rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.9.2/swarms/models/open_dalle.py
--rw-r--r--   0        0        0     2464 2024-04-27 21:17:36.644597 swarms-4.9.2/swarms/models/open_router.py
--rw-r--r--   0        0        0      106 2024-04-25 14:24:46.757474 swarms-4.9.2/swarms/models/openai_embeddings.py
--rw-r--r--   0        0        0     3167 2024-04-27 21:17:36.645494 swarms-4.9.2/swarms/models/openai_tts.py
--rw-r--r--   0        0        0       93 2024-04-25 14:24:46.757393 swarms-4.9.2/swarms/models/palm.py
--rw-r--r--   0        0        0     2164 2024-05-03 20:59:40.853629 swarms-4.9.2/swarms/models/popular_llms.py
--rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-4.9.2/swarms/models/qwen.py
--rw-r--r--   0        0        0     3547 2024-04-18 12:43:27.606549 swarms-4.9.2/swarms/models/sam.py
--rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-4.9.2/swarms/models/sampling_params.py
--rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-4.9.2/swarms/models/speecht5.py
--rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-4.9.2/swarms/models/ssd_1b.py
--rw-r--r--   0        0        0     5189 2024-04-18 12:43:27.897205 swarms-4.9.2/swarms/models/stable_diffusion.py
--rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.9.2/swarms/models/timm.py
--rw-r--r--   0        0        0     3948 2024-04-27 21:17:36.646243 swarms-4.9.2/swarms/models/together.py
--rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.9.2/swarms/models/types.py
--rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.9.2/swarms/models/vilt.py
--rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.9.2/swarms/models/vip_llava.py
--rw-r--r--   0        0        0     3681 2024-04-18 12:43:27.995338 swarms-4.9.2/swarms/models/zeroscope.py
--rw-r--r--   0        0        0        0 2024-05-01 03:43:07.020028 swarms-4.9.2/swarms/prebuilt_swarms/__init__.py
--rw-r--r--   0        0        0      692 2024-05-02 21:57:21.661595 swarms-4.9.2/swarms/prompts/__init__.py
--rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.9.2/swarms/prompts/accountant_swarm_prompts.py
--rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.9.2/swarms/prompts/aga.py
--rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.9.2/swarms/prompts/agent_output_parser.py
--rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-4.9.2/swarms/prompts/agent_prompt.py
--rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.9.2/swarms/prompts/agent_prompts.py
--rw-r--r--   0        0        0     7145 2024-03-15 22:19:21.065128 swarms-4.9.2/swarms/prompts/agent_system_prompts.py
--rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.9.2/swarms/prompts/ai_research_team.py
--rw-r--r--   0        0        0     1148 2024-05-01 03:43:07.021040 swarms-4.9.2/swarms/prompts/aot_prompt.py
--rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.9.2/swarms/prompts/autobloggen.py
--rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.9.2/swarms/prompts/autoswarm.py
--rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-4.9.2/swarms/prompts/base.py
--rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-4.9.2/swarms/prompts/chat_prompt.py
--rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.9.2/swarms/prompts/code_interpreter.py
--rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.9.2/swarms/prompts/code_spawner.py
--rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.9.2/swarms/prompts/debate.py
--rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.9.2/swarms/prompts/documentation.py
--rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.9.2/swarms/prompts/education.py
--rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.9.2/swarms/prompts/finance_agent_prompt.py
--rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.9.2/swarms/prompts/growth_agent_prompt.py
--rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.9.2/swarms/prompts/idea2img.py
--rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.9.2/swarms/prompts/legal_agent_prompt.py
--rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.9.2/swarms/prompts/logistics.py
--rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-4.9.2/swarms/prompts/meta_system_prompt.py
--rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.9.2/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
--rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.9.2/swarms/prompts/multi_modal_prompts.py
--rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.9.2/swarms/prompts/multi_modal_visual_prompts.py
--rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.9.2/swarms/prompts/operations_agent_prompt.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.9.2/swarms/prompts/orchestrator_prompt.py
--rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.9.2/swarms/prompts/personal_stylist.py
--rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.9.2/swarms/prompts/product_agent_prompt.py
--rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.9.2/swarms/prompts/programming.py
--rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.9.2/swarms/prompts/project_manager.py
--rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-4.9.2/swarms/prompts/python.py
--rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.9.2/swarms/prompts/react.py
--rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.9.2/swarms/prompts/refiner_agent_prompt.py
--rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.9.2/swarms/prompts/sales.py
--rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.9.2/swarms/prompts/sales_prompts.py
--rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.9.2/swarms/prompts/security_team.py
--rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-4.9.2/swarms/prompts/self_operating_prompt.py
--rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.9.2/swarms/prompts/sop_generator_agent_prompt.py
--rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.9.2/swarms/prompts/summaries_prompts.py
--rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.9.2/swarms/prompts/support_agent_prompt.py
--rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.9.2/swarms/prompts/swarm_manager_agent.py
--rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.9.2/swarms/prompts/task_assignment_prompt.py
--rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-4.9.2/swarms/prompts/tests.py
--rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.9.2/swarms/prompts/tools.py
--rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.9.2/swarms/prompts/urban_planning.py
--rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.9.2/swarms/prompts/visual_cot.py
--rw-r--r--   0        0        0     5600 2024-05-02 21:56:49.171847 swarms-4.9.2/swarms/prompts/worker_prompt.py
--rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.9.2/swarms/prompts/xray_swarm_prompt.py
--rw-r--r--   0        0        0     3967 2024-05-02 21:52:18.678677 swarms-4.9.2/swarms/structs/__init__.py
--rw-r--r--   0        0        0    59304 2024-05-03 21:48:41.061154 swarms-4.9.2/swarms/structs/agent.py
--rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.9.2/swarms/structs/agent_job.py
--rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-4.9.2/swarms/structs/agent_process.py
--rw-r--r--   0        0        0     7472 2024-05-03 20:53:27.877056 swarms-4.9.2/swarms/structs/agent_rearrange.py
--rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-4.9.2/swarms/structs/async_workflow.py
--rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-4.9.2/swarms/structs/auto_swarm.py
--rw-r--r--   0        0        0    12437 2024-04-23 01:08:13.052177 swarms-4.9.2/swarms/structs/base_structure.py
--rw-r--r--   0        0        0    18739 2024-04-22 15:59:39.197542 swarms-4.9.2/swarms/structs/base_swarm.py
--rw-r--r--   0        0        0    12276 2024-04-18 12:43:28.833818 swarms-4.9.2/swarms/structs/base_workflow.py
--rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.9.2/swarms/structs/block_wrapper.py
--rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-4.9.2/swarms/structs/blocks_dict.py
--rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-4.9.2/swarms/structs/blocks_list.py
--rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-4.9.2/swarms/structs/company.py
--rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-4.9.2/swarms/structs/concurrent_workflow.py
--rw-r--r--   0        0        0    14685 2024-04-26 04:55:42.709791 swarms-4.9.2/swarms/structs/conversation.py
--rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-4.9.2/swarms/structs/debate.py
--rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.9.2/swarms/structs/document.py
--rw-r--r--   0        0        0     4775 2024-04-26 04:55:42.710484 swarms-4.9.2/swarms/structs/groupchat.py
--rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.9.2/swarms/structs/long_swarm.py
--rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-4.9.2/swarms/structs/majority_voting.py
--rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-4.9.2/swarms/structs/message.py
--rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-4.9.2/swarms/structs/message_pool.py
--rw-r--r--   0        0        0      855 2024-04-27 21:17:36.650763 swarms-4.9.2/swarms/structs/meta_system_prompt.py
--rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-4.9.2/swarms/structs/model_parallizer.py
--rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-4.9.2/swarms/structs/multi_agent_collab.py
--rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-4.9.2/swarms/structs/multi_process_workflow.py
--rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-4.9.2/swarms/structs/multi_threaded_workflow.py
--rw-r--r--   0        0        0      371 2024-04-27 21:17:36.651437 swarms-4.9.2/swarms/structs/omni_agent_types.py
--rw-r--r--   0        0        0      182 2024-04-28 21:24:54.081857 swarms-4.9.2/swarms/structs/plan.py
--rw-r--r--   0        0        0     5268 2024-04-18 12:42:42.011555 swarms-4.9.2/swarms/structs/rearrange.py
--rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-4.9.2/swarms/structs/recursive_workflow.py
--rw-r--r--   0        0        0     6764 2024-04-23 01:17:51.964275 swarms-4.9.2/swarms/structs/schemas.py
--rw-r--r--   0        0        0     3969 2024-04-27 21:17:36.652279 swarms-4.9.2/swarms/structs/sequential_workflow.py
--rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.9.2/swarms/structs/sermon_swarm.py
--rw-r--r--   0        0        0      709 2024-05-02 21:56:49.150787 swarms-4.9.2/swarms/structs/step.py
--rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-4.9.2/swarms/structs/swarm_net.py
--rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-4.9.2/swarms/structs/swarming_architectures.py
--rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-4.9.2/swarms/structs/task.py
--rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.9.2/swarms/structs/task_queue_base.py
--rw-r--r--   0        0        0     3375 2024-04-18 12:43:29.501225 swarms-4.9.2/swarms/structs/team.py
--rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-4.9.2/swarms/structs/utils.py
--rw-r--r--   0        0        0     7403 2024-04-24 00:20:16.136940 swarms-4.9.2/swarms/structs/yaml_model.py
--rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.9.2/swarms/telemetry/__init__.py
--rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-4.9.2/swarms/telemetry/auto_upgrade_swarms.py
--rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-4.9.2/swarms/telemetry/bootup.py
--rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-4.9.2/swarms/telemetry/check_update.py
--rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.9.2/swarms/telemetry/log_all.py
--rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.9.2/swarms/telemetry/sentry_active.py
--rw-r--r--   0        0        0     2675 2024-04-23 23:56:19.053195 swarms-4.9.2/swarms/telemetry/sys_info.py
--rw-r--r--   0        0        0     1879 2024-04-24 21:57:07.051275 swarms-4.9.2/swarms/telemetry/user_utils.py
--rw-r--r--   0        0        0     1680 2024-05-02 21:57:54.052789 swarms-4.9.2/swarms/tools/__init__.py
--rw-r--r--   0        0        0    10799 2024-05-03 20:46:32.465603 swarms-4.9.2/swarms/tools/base_tool.py
--rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-4.9.2/swarms/tools/code_interpreter.py
--rw-r--r--   0        0        0     5367 2024-05-02 21:56:49.196237 swarms-4.9.2/swarms/tools/exec_tool.py
--rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-4.9.2/swarms/tools/function_util.py
--rw-r--r--   0        0        0    14241 2024-04-27 21:17:36.654062 swarms-4.9.2/swarms/tools/json_former.py
--rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.9.2/swarms/tools/json_utils.py
--rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-4.9.2/swarms/tools/logits_processor.py
--rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-4.9.2/swarms/tools/math_eval.py
--rw-r--r--   0        0        0      978 2024-04-23 23:18:25.950155 swarms-4.9.2/swarms/tools/openai_func_calling_schema.py
--rw-r--r--   0        0        0     6785 2024-05-03 20:46:32.421440 swarms-4.9.2/swarms/tools/openai_tool_creator_decorator.py
--rw-r--r--   0        0        0    15564 2024-04-27 21:17:36.657668 swarms-4.9.2/swarms/tools/py_func_to_openai_func_str.py
--rw-r--r--   0        0        0     4275 2024-05-03 22:58:05.773294 swarms-4.9.2/swarms/tools/pydantic_to_json.py
--rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.9.2/swarms/tools/tool.py
--rw-r--r--   0        0        0     6170 2024-05-02 21:56:49.174616 swarms-4.9.2/swarms/tools/tool_utils.py
--rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.9.2/swarms/utils/README.md
--rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-4.9.2/swarms/utils/__init__.py
--rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-4.9.2/swarms/utils/apa.py
--rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-4.9.2/swarms/utils/check_function_result.py
--rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.9.2/swarms/utils/class_args_wrapper.py
--rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-4.9.2/swarms/utils/concurrent_utils.py
--rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-4.9.2/swarms/utils/data_to_text.py
--rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-4.9.2/swarms/utils/decorators.py
--rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.9.2/swarms/utils/disable_logging.py
--rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.9.2/swarms/utils/download_img.py
--rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.9.2/swarms/utils/execute_futures.py
--rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.9.2/swarms/utils/exponential_backoff.py
--rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.9.2/swarms/utils/fetch_init_params.py
--rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.9.2/swarms/utils/file_extension_seach.py
--rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-4.9.2/swarms/utils/file_processing.py
--rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-4.9.2/swarms/utils/find_img_path.py
--rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-4.9.2/swarms/utils/get_logger.py
--rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-4.9.2/swarms/utils/json_output_parser.py
--rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-4.9.2/swarms/utils/jsonl_utils.py
--rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.9.2/swarms/utils/llm_metrics_decorator.py
--rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-4.9.2/swarms/utils/logger.py
--rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-4.9.2/swarms/utils/loggers.py
--rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.9.2/swarms/utils/loguru_logger.py
--rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.9.2/swarms/utils/markdown_message.py
--rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.9.2/swarms/utils/parse_code.py
--rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-4.9.2/swarms/utils/pdf_to_text.py
--rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.9.2/swarms/utils/remove_json_whitespace.py
--rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-4.9.2/swarms/utils/save_logs.py
--rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-4.9.2/swarms/utils/serializable.py
--rw-r--r--   0        0        0     1315 2024-04-25 14:49:22.838126 swarms-4.9.2/swarms/utils/try_except_wrapper.py
--rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-4.9.2/swarms/utils/yaml_output_parser.py
--rw-r--r--   0        0        0    41967 1970-01-01 00:00:00.000000 swarms-4.9.2/setup.py
--rw-r--r--   0        0        0    40877 1970-01-01 00:00:00.000000 swarms-4.9.2/PKG-INFO
+-rw-r--r--   0        0        0    15674 2024-03-27 19:29:36.857220 swarms-4.9.3/LICENSE
+-rw-r--r--   0        0        0    39192 2024-05-08 21:09:56.084797 swarms-4.9.3/README.md
+-rw-r--r--   0        0        0     1810 2024-05-08 23:51:38.917299 swarms-4.9.3/pyproject.toml
+-rw-r--r--   0        0        0      590 2024-04-02 02:30:28.406904 swarms-4.9.3/swarms/__init__.py
+-rw-r--r--   0        0        0      864 2024-03-15 22:19:21.000202 swarms-4.9.3/swarms/agents/__init__.py
+-rw-r--r--   0        0        0      881 2024-03-15 22:19:21.001107 swarms-4.9.3/swarms/agents/agent_wrapper.py
+-rw-r--r--   0        0        0     3342 2024-03-21 23:46:38.264917 swarms-4.9.3/swarms/agents/base.py
+-rw-r--r--   0        0        0     4201 2024-03-15 22:19:21.002271 swarms-4.9.3/swarms/agents/developer_agents.py
+-rw-r--r--   0        0        0     2950 2024-03-27 19:12:09.754781 swarms-4.9.3/swarms/agents/omni_modal_agent.py
+-rw-r--r--   0        0        0     3491 2024-04-27 21:17:36.621105 swarms-4.9.3/swarms/agents/simple_agent.py
+-rw-r--r--   0        0        0      484 2024-03-15 22:19:21.004680 swarms-4.9.3/swarms/agents/stopping_conditions.py
+-rw-r--r--   0        0        0     4940 2024-04-27 21:17:36.621832 swarms-4.9.3/swarms/agents/tool_agent.py
+-rw-r--r--   0        0        0     5504 2024-05-08 21:09:56.813124 swarms-4.9.3/swarms/agents/worker_agent.py
+-rw-r--r--   0        0        0      167 2024-03-15 22:19:21.006869 swarms-4.9.3/swarms/artifacts/__init__.py
+-rw-r--r--   0        0        0     1675 2024-03-15 22:19:21.007269 swarms-4.9.3/swarms/artifacts/base_artifact.py
+-rw-r--r--   0        0        0     2299 2024-03-27 19:27:30.716559 swarms-4.9.3/swarms/artifacts/text_artifact.py
+-rw-r--r--   0        0        0      613 2024-04-27 21:17:36.623130 swarms-4.9.3/swarms/memory/__init__.py
+-rw-r--r--   0        0        0      433 2024-03-15 22:19:21.012591 swarms-4.9.3/swarms/memory/action_subtask.py
+-rw-r--r--   0        0        0     3475 2024-03-15 22:19:21.012989 swarms-4.9.3/swarms/memory/base_db.py
+-rw-r--r--   0        0        0     2823 2024-04-27 21:17:36.624819 swarms-4.9.3/swarms/memory/base_vectordb.py
+-rw-r--r--   0        0        0     2895 2024-03-15 22:19:21.014370 swarms-4.9.3/swarms/memory/dict_internal_memory.py
+-rw-r--r--   0        0        0     3306 2024-04-18 12:42:39.319739 swarms-4.9.3/swarms/memory/dict_shared_memory.py
+-rw-r--r--   0        0        0     5499 2024-04-18 12:43:26.648904 swarms-4.9.3/swarms/memory/short_term_memory.py
+-rw-r--r--   0        0        0     3371 2024-03-15 22:19:21.018970 swarms-4.9.3/swarms/memory/visual_memory.py
+-rw-r--r--   0        0        0     2608 2024-05-08 21:09:56.817128 swarms-4.9.3/swarms/models/__init__.py
+-rw-r--r--   0        0        0     2060 2024-04-18 12:43:26.678061 swarms-4.9.3/swarms/models/base_embedding_model.py
+-rw-r--r--   0        0        0    13168 2024-04-27 21:17:36.635065 swarms-4.9.3/swarms/models/base_llm.py
+-rw-r--r--   0        0        0    12604 2024-04-18 12:43:27.187223 swarms-4.9.3/swarms/models/base_multimodal_model.py
+-rw-r--r--   0        0        0     2475 2024-04-27 21:17:36.635700 swarms-4.9.3/swarms/models/base_tts.py
+-rw-r--r--   0        0        0     3163 2024-04-27 21:17:36.636332 swarms-4.9.3/swarms/models/base_ttv.py
+-rw-r--r--   0        0        0    16743 2024-04-18 12:43:27.429345 swarms-4.9.3/swarms/models/cog_vlm.py
+-rw-r--r--   0        0        0    10760 2024-04-18 12:43:27.137440 swarms-4.9.3/swarms/models/dalle3.py
+-rw-r--r--   0        0        0     6449 2024-04-18 12:43:26.972838 swarms-4.9.3/swarms/models/distilled_whisperx.py
+-rw-r--r--   0        0        0      682 2024-04-18 12:43:26.722086 swarms-4.9.3/swarms/models/embeddings_base.py
+-rw-r--r--   0        0        0     2726 2024-04-27 21:17:36.637208 swarms-4.9.3/swarms/models/fire_function.py
+-rw-r--r--   0        0        0     3022 2024-03-15 22:19:21.032963 swarms-4.9.3/swarms/models/fuyu.py
+-rw-r--r--   0        0        0     7762 2024-04-18 12:42:39.844485 swarms-4.9.3/swarms/models/gemini.py
+-rw-r--r--   0        0        0    14214 2024-04-18 12:43:27.452395 swarms-4.9.3/swarms/models/gpt4_vision_api.py
+-rw-r--r--   0        0        0    12996 2024-04-27 21:17:36.638023 swarms-4.9.3/swarms/models/huggingface.py
+-rw-r--r--   0        0        0     1826 2024-04-27 21:17:36.638977 swarms-4.9.3/swarms/models/huggingface_pipeline.py
+-rw-r--r--   0        0        0     5601 2024-04-18 12:43:27.069960 swarms-4.9.3/swarms/models/idefics.py
+-rw-r--r--   0        0        0    10672 2024-04-18 12:43:27.705223 swarms-4.9.3/swarms/models/kosmos_two.py
+-rw-r--r--   0        0        0     1448 2024-03-15 22:19:21.037679 swarms-4.9.3/swarms/models/layoutlm_document_qa.py
+-rw-r--r--   0        0        0     6581 2024-04-27 21:17:36.639950 swarms-4.9.3/swarms/models/llama_function_caller.py
+-rw-r--r--   0        0        0     2762 2024-03-15 22:19:21.038340 swarms-4.9.3/swarms/models/llava.py
+-rw-r--r--   0        0        0     4286 2024-04-27 21:17:36.641073 swarms-4.9.3/swarms/models/mistral.py
+-rw-r--r--   0        0        0     2147 2024-04-27 21:17:36.642823 swarms-4.9.3/swarms/models/mixtral.py
+-rw-r--r--   0        0        0     2056 2024-03-15 22:19:21.041522 swarms-4.9.3/swarms/models/moondream_mm.py
+-rw-r--r--   0        0        0     6448 2024-04-18 12:43:27.582607 swarms-4.9.3/swarms/models/mpt.py
+-rw-r--r--   0        0        0     2823 2024-04-18 12:43:27.453365 swarms-4.9.3/swarms/models/nougat.py
+-rw-r--r--   0        0        0     2366 2024-03-15 22:19:21.043550 swarms-4.9.3/swarms/models/open_dalle.py
+-rw-r--r--   0        0        0     2464 2024-04-27 21:17:36.644597 swarms-4.9.3/swarms/models/open_router.py
+-rw-r--r--   0        0        0      106 2024-04-25 14:24:46.757474 swarms-4.9.3/swarms/models/openai_embeddings.py
+-rw-r--r--   0        0        0     3167 2024-04-27 21:17:36.645494 swarms-4.9.3/swarms/models/openai_tts.py
+-rw-r--r--   0        0        0       93 2024-04-25 14:24:46.757393 swarms-4.9.3/swarms/models/palm.py
+-rw-r--r--   0        0        0     2160 2024-05-08 21:09:56.821210 swarms-4.9.3/swarms/models/popular_llms.py
+-rw-r--r--   0        0        0     4813 2024-04-18 12:43:27.720842 swarms-4.9.3/swarms/models/qwen.py
+-rw-r--r--   0        0        0     3547 2024-04-18 12:43:27.606549 swarms-4.9.3/swarms/models/sam.py
+-rw-r--r--   0        0        0    12675 2024-04-18 12:43:28.000334 swarms-4.9.3/swarms/models/sampling_params.py
+-rw-r--r--   0        0        0     7621 2024-04-18 12:43:27.738035 swarms-4.9.3/swarms/models/speecht5.py
+-rw-r--r--   0        0        0     8244 2024-04-18 12:43:28.025933 swarms-4.9.3/swarms/models/ssd_1b.py
+-rw-r--r--   0        0        0     5189 2024-04-18 12:43:27.897205 swarms-4.9.3/swarms/models/stable_diffusion.py
+-rw-r--r--   0        0        0     1794 2024-03-15 22:19:21.052816 swarms-4.9.3/swarms/models/timm.py
+-rw-r--r--   0        0        0     3948 2024-04-27 21:17:36.646243 swarms-4.9.3/swarms/models/together.py
+-rw-r--r--   0        0        0      592 2024-03-15 22:19:21.054281 swarms-4.9.3/swarms/models/types.py
+-rw-r--r--   0        0        0     1731 2024-03-15 22:19:21.054977 swarms-4.9.3/swarms/models/vilt.py
+-rw-r--r--   0        0        0     2846 2024-03-15 22:19:21.055732 swarms-4.9.3/swarms/models/vip_llava.py
+-rw-r--r--   0        0        0     3681 2024-04-18 12:43:27.995338 swarms-4.9.3/swarms/models/zeroscope.py
+-rw-r--r--   0        0        0        0 2024-05-01 03:43:07.020028 swarms-4.9.3/swarms/prebuilt_swarms/__init__.py
+-rw-r--r--   0        0        0      692 2024-05-08 21:09:56.824718 swarms-4.9.3/swarms/prompts/__init__.py
+-rw-r--r--   0        0        0    11320 2024-03-15 22:19:21.061563 swarms-4.9.3/swarms/prompts/accountant_swarm_prompts.py
+-rw-r--r--   0        0        0     9156 2024-03-15 22:19:21.062133 swarms-4.9.3/swarms/prompts/aga.py
+-rw-r--r--   0        0        0     1451 2024-03-15 22:19:21.062911 swarms-4.9.3/swarms/prompts/agent_output_parser.py
+-rw-r--r--   0        0        0     2705 2024-04-18 12:43:28.068653 swarms-4.9.3/swarms/prompts/agent_prompt.py
+-rw-r--r--   0        0        0     6886 2024-03-15 22:19:21.064160 swarms-4.9.3/swarms/prompts/agent_prompts.py
+-rw-r--r--   0        0        0     7113 2024-05-08 21:09:56.832506 swarms-4.9.3/swarms/prompts/agent_system_prompts.py
+-rw-r--r--   0        0        0     5233 2024-03-15 22:19:21.065787 swarms-4.9.3/swarms/prompts/ai_research_team.py
+-rw-r--r--   0        0        0     1148 2024-05-01 03:43:07.021040 swarms-4.9.3/swarms/prompts/aot_prompt.py
+-rw-r--r--   0        0        0    13981 2024-03-15 22:19:21.066513 swarms-4.9.3/swarms/prompts/autobloggen.py
+-rw-r--r--   0        0        0     5605 2024-03-15 22:19:21.068224 swarms-4.9.3/swarms/prompts/autoswarm.py
+-rw-r--r--   0        0        0     7542 2024-04-18 12:43:28.353296 swarms-4.9.3/swarms/prompts/base.py
+-rw-r--r--   0        0        0     3801 2024-04-18 12:43:28.227538 swarms-4.9.3/swarms/prompts/chat_prompt.py
+-rw-r--r--   0        0        0     2235 2024-03-15 22:19:21.069096 swarms-4.9.3/swarms/prompts/code_interpreter.py
+-rw-r--r--   0        0        0     4106 2024-03-15 22:19:21.069652 swarms-4.9.3/swarms/prompts/code_spawner.py
+-rw-r--r--   0        0        0     1566 2024-03-15 22:19:21.069820 swarms-4.9.3/swarms/prompts/debate.py
+-rw-r--r--   0        0        0     7044 2024-03-15 22:19:21.070670 swarms-4.9.3/swarms/prompts/documentation.py
+-rw-r--r--   0        0        0     1767 2024-03-15 22:19:21.071442 swarms-4.9.3/swarms/prompts/education.py
+-rw-r--r--   0        0        0     4180 2024-03-15 22:19:21.071791 swarms-4.9.3/swarms/prompts/finance_agent_prompt.py
+-rw-r--r--   0        0        0     4117 2024-03-15 22:19:21.072144 swarms-4.9.3/swarms/prompts/growth_agent_prompt.py
+-rw-r--r--   0        0        0      880 2024-03-15 22:19:21.072694 swarms-4.9.3/swarms/prompts/idea2img.py
+-rw-r--r--   0        0        0     3346 2024-03-15 22:19:21.072990 swarms-4.9.3/swarms/prompts/legal_agent_prompt.py
+-rw-r--r--   0        0        0     4785 2024-03-15 22:19:21.073912 swarms-4.9.3/swarms/prompts/logistics.py
+-rw-r--r--   0        0        0     3374 2024-04-10 15:42:56.140463 swarms-4.9.3/swarms/prompts/meta_system_prompt.py
+-rw-r--r--   0        0        0    10662 2024-03-15 22:19:21.074621 swarms-4.9.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py
+-rw-r--r--   0        0        0     3511 2024-03-15 22:19:21.075295 swarms-4.9.3/swarms/prompts/multi_modal_prompts.py
+-rw-r--r--   0        0        0     3225 2024-03-15 22:19:21.075646 swarms-4.9.3/swarms/prompts/multi_modal_visual_prompts.py
+-rw-r--r--   0        0        0     3454 2024-03-15 22:19:21.076012 swarms-4.9.3/swarms/prompts/operations_agent_prompt.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.076143 swarms-4.9.3/swarms/prompts/orchestrator_prompt.py
+-rw-r--r--   0        0        0     2149 2024-03-15 22:19:21.076733 swarms-4.9.3/swarms/prompts/personal_stylist.py
+-rw-r--r--   0        0        0     8333 2024-03-15 22:19:21.077280 swarms-4.9.3/swarms/prompts/product_agent_prompt.py
+-rw-r--r--   0        0        0    10144 2024-03-15 22:19:21.078026 swarms-4.9.3/swarms/prompts/programming.py
+-rw-r--r--   0        0        0     2128 2024-03-15 22:19:21.078275 swarms-4.9.3/swarms/prompts/project_manager.py
+-rw-r--r--   0        0        0    13215 2024-04-18 12:43:28.152390 swarms-4.9.3/swarms/prompts/python.py
+-rw-r--r--   0        0        0     2960 2024-03-15 22:19:21.079805 swarms-4.9.3/swarms/prompts/react.py
+-rw-r--r--   0        0        0        0 2024-03-15 22:19:21.080059 swarms-4.9.3/swarms/prompts/refiner_agent_prompt.py
+-rw-r--r--   0        0        0     5126 2024-03-15 22:19:21.080659 swarms-4.9.3/swarms/prompts/sales.py
+-rw-r--r--   0        0        0     5013 2024-03-15 22:19:21.081280 swarms-4.9.3/swarms/prompts/sales_prompts.py
+-rw-r--r--   0        0        0     2679 2024-03-15 22:19:21.083072 swarms-4.9.3/swarms/prompts/security_team.py
+-rw-r--r--   0        0        0     3252 2024-04-18 12:43:28.128596 swarms-4.9.3/swarms/prompts/self_operating_prompt.py
+-rw-r--r--   0        0        0     4147 2024-03-15 22:19:21.084066 swarms-4.9.3/swarms/prompts/sop_generator_agent_prompt.py
+-rw-r--r--   0        0        0     4640 2024-03-15 22:19:21.084386 swarms-4.9.3/swarms/prompts/summaries_prompts.py
+-rw-r--r--   0        0        0     3984 2024-03-15 22:19:21.084631 swarms-4.9.3/swarms/prompts/support_agent_prompt.py
+-rw-r--r--   0        0        0     4280 2024-03-15 22:19:21.085244 swarms-4.9.3/swarms/prompts/swarm_manager_agent.py
+-rw-r--r--   0        0        0      728 2024-03-15 22:19:21.085725 swarms-4.9.3/swarms/prompts/task_assignment_prompt.py
+-rw-r--r--   0        0        0     4271 2024-04-18 12:43:28.167424 swarms-4.9.3/swarms/prompts/tests.py
+-rw-r--r--   0        0        0     4288 2024-03-15 22:19:21.086625 swarms-4.9.3/swarms/prompts/tools.py
+-rw-r--r--   0        0        0     2398 2024-03-15 22:19:21.087352 swarms-4.9.3/swarms/prompts/urban_planning.py
+-rw-r--r--   0        0        0     3675 2024-03-15 22:19:21.087654 swarms-4.9.3/swarms/prompts/visual_cot.py
+-rw-r--r--   0        0        0     5596 2024-05-08 21:09:56.838185 swarms-4.9.3/swarms/prompts/worker_prompt.py
+-rw-r--r--   0        0        0     2349 2024-03-15 22:19:21.088382 swarms-4.9.3/swarms/prompts/xray_swarm_prompt.py
+-rw-r--r--   0        0        0     3988 2024-05-08 21:09:56.839121 swarms-4.9.3/swarms/structs/__init__.py
+-rw-r--r--   0        0        0    60077 2024-05-08 21:09:56.870508 swarms-4.9.3/swarms/structs/agent.py
+-rw-r--r--   0        0        0      574 2024-03-15 22:19:21.092491 swarms-4.9.3/swarms/structs/agent_job.py
+-rw-r--r--   0        0        0     2937 2024-04-22 15:42:05.980151 swarms-4.9.3/swarms/structs/agent_process.py
+-rw-r--r--   0        0        0     3718 2024-04-18 12:43:28.377820 swarms-4.9.3/swarms/structs/async_workflow.py
+-rw-r--r--   0        0        0     5579 2024-04-22 14:27:36.702871 swarms-4.9.3/swarms/structs/auto_swarm.py
+-rw-r--r--   0        0        0    12437 2024-04-23 01:08:13.052177 swarms-4.9.3/swarms/structs/base_structure.py
+-rw-r--r--   0        0        0    19446 2024-05-08 21:09:56.884181 swarms-4.9.3/swarms/structs/base_swarm.py
+-rw-r--r--   0        0        0    12161 2024-05-08 21:09:56.888358 swarms-4.9.3/swarms/structs/base_workflow.py
+-rw-r--r--   0        0        0     1056 2024-03-15 22:19:21.095125 swarms-4.9.3/swarms/structs/block_wrapper.py
+-rw-r--r--   0        0        0     3188 2024-04-18 02:05:51.225713 swarms-4.9.3/swarms/structs/blocks_dict.py
+-rw-r--r--   0        0        0     4851 2024-04-18 12:43:28.719057 swarms-4.9.3/swarms/structs/blocks_list.py
+-rw-r--r--   0        0        0     5206 2024-04-18 12:43:28.754865 swarms-4.9.3/swarms/structs/company.py
+-rw-r--r--   0        0        0     4471 2024-04-18 12:43:28.724904 swarms-4.9.3/swarms/structs/concurrent_workflow.py
+-rw-r--r--   0        0        0    14685 2024-04-26 04:55:42.709791 swarms-4.9.3/swarms/structs/conversation.py
+-rw-r--r--   0        0        0    12549 2024-04-18 12:43:29.326347 swarms-4.9.3/swarms/structs/debate.py
+-rw-r--r--   0        0        0     3041 2024-03-15 22:19:21.099360 swarms-4.9.3/swarms/structs/document.py
+-rw-r--r--   0        0        0     4775 2024-04-26 04:55:42.710484 swarms-4.9.3/swarms/structs/groupchat.py
+-rw-r--r--   0        0        0     4545 2024-03-15 22:19:21.101122 swarms-4.9.3/swarms/structs/long_swarm.py
+-rw-r--r--   0        0        0     7012 2024-04-18 12:43:29.037949 swarms-4.9.3/swarms/structs/majority_voting.py
+-rw-r--r--   0        0        0      745 2024-04-22 15:59:38.669639 swarms-4.9.3/swarms/structs/message.py
+-rw-r--r--   0        0        0     7338 2024-04-18 12:43:29.012263 swarms-4.9.3/swarms/structs/message_pool.py
+-rw-r--r--   0        0        0      855 2024-04-27 21:17:36.650763 swarms-4.9.3/swarms/structs/meta_system_prompt.py
+-rw-r--r--   0        0        0     5751 2024-04-18 12:43:29.210773 swarms-4.9.3/swarms/structs/model_parallizer.py
+-rw-r--r--   0        0        0     8390 2024-04-22 15:59:38.738279 swarms-4.9.3/swarms/structs/multi_agent_collab.py
+-rw-r--r--   0        0        0     5623 2024-04-18 12:43:29.243594 swarms-4.9.3/swarms/structs/multi_process_workflow.py
+-rw-r--r--   0        0        0     5272 2024-04-18 12:42:41.990321 swarms-4.9.3/swarms/structs/multi_threaded_workflow.py
+-rw-r--r--   0        0        0      371 2024-04-27 21:17:36.651437 swarms-4.9.3/swarms/structs/omni_agent_types.py
+-rw-r--r--   0        0        0      182 2024-04-28 21:24:54.081857 swarms-4.9.3/swarms/structs/plan.py
+-rw-r--r--   0        0        0     6900 2024-05-08 21:09:56.889747 swarms-4.9.3/swarms/structs/rearrange.py
+-rw-r--r--   0        0        0     2727 2024-04-18 12:42:41.946623 swarms-4.9.3/swarms/structs/recursive_workflow.py
+-rw-r--r--   0        0        0     6764 2024-04-23 01:17:51.964275 swarms-4.9.3/swarms/structs/schemas.py
+-rw-r--r--   0        0        0     2956 2024-05-08 21:09:56.891925 swarms-4.9.3/swarms/structs/sequential_workflow.py
+-rw-r--r--   0        0        0     2337 2024-03-27 19:47:31.068657 swarms-4.9.3/swarms/structs/sermon_swarm.py
+-rw-r--r--   0        0        0      709 2024-05-08 21:09:56.895373 swarms-4.9.3/swarms/structs/step.py
+-rw-r--r--   0        0        0    10684 2024-04-18 12:43:29.602325 swarms-4.9.3/swarms/structs/swarm_net.py
+-rw-r--r--   0        0        0     6426 2024-04-18 12:43:29.666155 swarms-4.9.3/swarms/structs/swarming_architectures.py
+-rw-r--r--   0        0        0     8179 2024-04-18 12:43:29.569178 swarms-4.9.3/swarms/structs/task.py
+-rw-r--r--   0        0        0     1989 2024-03-27 19:12:09.705030 swarms-4.9.3/swarms/structs/task_queue_base.py
+-rw-r--r--   0        0        0     3511 2024-04-18 12:42:42.279735 swarms-4.9.3/swarms/structs/utils.py
+-rw-r--r--   0        0        0     7403 2024-04-24 00:20:16.136940 swarms-4.9.3/swarms/structs/yaml_model.py
+-rw-r--r--   0        0        0      891 2024-03-27 19:12:09.674045 swarms-4.9.3/swarms/telemetry/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-18 12:43:29.468850 swarms-4.9.3/swarms/telemetry/auto_upgrade_swarms.py
+-rw-r--r--   0        0        0      385 2024-04-02 02:30:28.437471 swarms-4.9.3/swarms/telemetry/bootup.py
+-rw-r--r--   0        0        0     1073 2024-04-18 12:42:42.280090 swarms-4.9.3/swarms/telemetry/check_update.py
+-rw-r--r--   0        0        0      807 2024-03-15 22:19:21.114471 swarms-4.9.3/swarms/telemetry/log_all.py
+-rw-r--r--   0        0        0      496 2024-03-22 00:42:19.696403 swarms-4.9.3/swarms/telemetry/sentry_active.py
+-rw-r--r--   0        0        0     2675 2024-04-23 23:56:19.053195 swarms-4.9.3/swarms/telemetry/sys_info.py
+-rw-r--r--   0        0        0     1879 2024-04-24 21:57:07.051275 swarms-4.9.3/swarms/telemetry/user_utils.py
+-rw-r--r--   0        0        0     1680 2024-05-08 21:09:56.899526 swarms-4.9.3/swarms/tools/__init__.py
+-rw-r--r--   0        0        0    12525 2024-05-08 21:09:56.906505 swarms-4.9.3/swarms/tools/base_tool.py
+-rw-r--r--   0        0        0     6653 2024-04-18 12:47:32.769219 swarms-4.9.3/swarms/tools/code_interpreter.py
+-rw-r--r--   0        0        0     5367 2024-05-08 21:09:56.913861 swarms-4.9.3/swarms/tools/exec_tool.py
+-rw-r--r--   0        0        0      773 2024-04-03 12:10:21.536239 swarms-4.9.3/swarms/tools/function_util.py
+-rw-r--r--   0        0        0    14241 2024-04-27 21:17:36.654062 swarms-4.9.3/swarms/tools/json_former.py
+-rw-r--r--   0        0        0     1316 2024-03-21 23:46:38.581600 swarms-4.9.3/swarms/tools/json_utils.py
+-rw-r--r--   0        0        0     2455 2024-04-18 12:42:42.475166 swarms-4.9.3/swarms/tools/logits_processor.py
+-rw-r--r--   0        0        0     1461 2024-04-18 12:43:30.100050 swarms-4.9.3/swarms/tools/math_eval.py
+-rw-r--r--   0        0        0      978 2024-04-23 23:18:25.950155 swarms-4.9.3/swarms/tools/openai_func_calling_schema.py
+-rw-r--r--   0        0        0    13875 2024-05-08 21:09:56.921184 swarms-4.9.3/swarms/tools/openai_tool_creator_decorator.py
+-rw-r--r--   0        0        0    15564 2024-04-27 21:17:36.657668 swarms-4.9.3/swarms/tools/py_func_to_openai_func_str.py
+-rw-r--r--   0        0        0     4275 2024-05-08 21:09:56.925611 swarms-4.9.3/swarms/tools/pydantic_to_json.py
+-rw-r--r--   0        0        0      157 2024-03-24 04:12:12.223834 swarms-4.9.3/swarms/tools/tool.py
+-rw-r--r--   0        0        0     6170 2024-05-08 21:09:56.930060 swarms-4.9.3/swarms/tools/tool_utils.py
+-rw-r--r--   0        0        0     5466 2024-03-15 22:19:21.122024 swarms-4.9.3/swarms/utils/README.md
+-rw-r--r--   0        0        0     1956 2024-04-18 15:06:06.195732 swarms-4.9.3/swarms/utils/__init__.py
+-rw-r--r--   0        0        0     3507 2024-04-18 12:42:42.565998 swarms-4.9.3/swarms/utils/apa.py
+-rw-r--r--   0        0        0     6065 2024-04-18 12:42:42.646659 swarms-4.9.3/swarms/utils/check_function_result.py
+-rw-r--r--   0        0        0     1008 2024-03-15 22:19:21.124143 swarms-4.9.3/swarms/utils/class_args_wrapper.py
+-rw-r--r--   0        0        0     1234 2024-04-18 12:42:42.478906 swarms-4.9.3/swarms/utils/concurrent_utils.py
+-rw-r--r--   0        0        0     1865 2024-04-18 12:42:42.546898 swarms-4.9.3/swarms/utils/data_to_text.py
+-rw-r--r--   0        0        0     2451 2024-04-18 12:43:29.983708 swarms-4.9.3/swarms/utils/decorators.py
+-rw-r--r--   0        0        0     1311 2024-03-15 22:19:21.127902 swarms-4.9.3/swarms/utils/disable_logging.py
+-rw-r--r--   0        0        0      890 2024-03-15 22:19:21.128555 swarms-4.9.3/swarms/utils/download_img.py
+-rw-r--r--   0        0        0     1127 2024-03-15 22:19:21.129540 swarms-4.9.3/swarms/utils/execute_futures.py
+-rw-r--r--   0        0        0     1113 2024-03-15 22:19:21.130281 swarms-4.9.3/swarms/utils/exponential_backoff.py
+-rw-r--r--   0        0        0      854 2024-03-15 22:19:21.130759 swarms-4.9.3/swarms/utils/fetch_init_params.py
+-rw-r--r--   0        0        0      500 2024-03-15 22:19:21.131255 swarms-4.9.3/swarms/utils/file_extension_seach.py
+-rw-r--r--   0        0        0     3266 2024-04-18 12:42:42.739802 swarms-4.9.3/swarms/utils/file_processing.py
+-rw-r--r--   0        0        0      630 2024-04-18 12:43:29.910068 swarms-4.9.3/swarms/utils/find_img_path.py
+-rw-r--r--   0        0        0     4184 2024-04-18 12:43:30.069758 swarms-4.9.3/swarms/utils/get_logger.py
+-rw-r--r--   0        0        0     2848 2024-04-18 12:43:30.028262 swarms-4.9.3/swarms/utils/json_output_parser.py
+-rw-r--r--   0        0        0     1831 2024-04-18 12:42:42.783557 swarms-4.9.3/swarms/utils/jsonl_utils.py
+-rw-r--r--   0        0        0      932 2024-03-15 22:19:21.135261 swarms-4.9.3/swarms/utils/llm_metrics_decorator.py
+-rw-r--r--   0        0        0     2209 2024-04-18 12:43:30.070521 swarms-4.9.3/swarms/utils/logger.py
+-rw-r--r--   0        0        0    16186 2024-04-18 12:43:30.846131 swarms-4.9.3/swarms/utils/loggers.py
+-rw-r--r--   0        0        0      453 2024-03-27 19:12:09.738695 swarms-4.9.3/swarms/utils/loguru_logger.py
+-rw-r--r--   0        0        0      711 2024-03-27 19:12:09.676603 swarms-4.9.3/swarms/utils/markdown_message.py
+-rw-r--r--   0        0        0      600 2024-03-15 22:19:21.139501 swarms-4.9.3/swarms/utils/parse_code.py
+-rw-r--r--   0        0        0     1177 2024-04-18 12:43:30.100653 swarms-4.9.3/swarms/utils/pdf_to_text.py
+-rw-r--r--   0        0        0     1353 2024-03-15 22:19:21.141276 swarms-4.9.3/swarms/utils/remove_json_whitespace.py
+-rw-r--r--   0        0        0     1278 2024-04-18 12:42:42.936792 swarms-4.9.3/swarms/utils/save_logs.py
+-rw-r--r--   0        0        0     4774 2024-04-18 12:42:43.138354 swarms-4.9.3/swarms/utils/serializable.py
+-rw-r--r--   0        0        0     1315 2024-04-25 14:49:22.838126 swarms-4.9.3/swarms/utils/try_except_wrapper.py
+-rw-r--r--   0        0        0     2668 2024-04-18 12:43:30.304280 swarms-4.9.3/swarms/utils/yaml_output_parser.py
+-rw-r--r--   0        0        0    41888 1970-01-01 00:00:00.000000 swarms-4.9.3/setup.py
+-rw-r--r--   0        0        0    40797 1970-01-01 00:00:00.000000 swarms-4.9.3/PKG-INFO
```

### Comparing `swarms-4.9.2/LICENSE` & `swarms-4.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/README.md` & `swarms-4.9.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,217 @@
 
 # Running the agent with the specified task and image
 out = agent.run(task)
 print(out)
 
 ```
 
+### Simple Conversational Agent
+A Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models
+
+- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking
+- Reliable, this simple system will always provide responses you want.
+
+```python
+from swarms import Agent, Anthropic
+
+
+## Initialize the workflow
+agent = Agent(
+    agent_name="Transcript Generator",
+    agent_description=(
+        "Generate a transcript for a youtube video on what swarms"
+        " are!"
+    ),
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    interactive=True, # Set to True
+)
+
+# Run the workflow on a task
+agent("Generate a transcript for a youtube video on what swarms are!")
+```
+
+## Devin
+Implementation of Devil in less than 90 lines of code with several tools:
+terminal, browser, and edit files!
+
+```python
+from swarms import Agent, Anthropic, tool
+import subprocess
+
+# Model
+llm = Anthropic(
+    temperature=0.1,
+)
+
+# Tools
+@tool
+def terminal(
+    code: str,
+):
+    """
+    Run code in the terminal.
+
+    Args:
+        code (str): The code to run in the terminal.
+
+    Returns:
+        str: The output of the code.
+    """
+    out = subprocess.run(
+        code, shell=True, capture_output=True, text=True
+    ).stdout
+    return str(out)
+
+
+@tool
+def browser(query: str):
+    """
+    Search the query in the browser with the `browser` tool.
+
+    Args:
+        query (str): The query to search in the browser.
+
+    Returns:
+        str: The search results.
+    """
+    import webbrowser
+
+    url = f"https://www.google.com/search?q={query}"
+    webbrowser.open(url)
+    return f"Searching for {query} in the browser."
+
+@tool
+def create_file(file_path: str, content: str):
+    """
+    Create a file using the file editor tool.
+
+    Args:
+        file_path (str): The path to the file.
+        content (str): The content to write to the file.
+
+    Returns:
+        str: The result of the file creation operation.
+    """
+    with open(file_path, "w") as file:
+        file.write(content)
+    return f"File {file_path} created successfully."
+
+@tool
+def file_editor(file_path: str, mode: str, content: str):
+    """
+    Edit a file using the file editor tool.
+
+    Args:
+        file_path (str): The path to the file.
+        mode (str): The mode to open the file in.
+        content (str): The content to write to the file.
+
+    Returns:
+        str: The result of the file editing operation.
+    """
+    with open(file_path, mode) as file:
+        file.write(content)
+    return f"File {file_path} edited successfully."
+
+
+# Agent
+agent = Agent(
+    agent_name="Devin",
+    system_prompt=(
+        "Autonomous agent that can interact with humans and other"
+        " agents. Be Helpful and Kind. Use the tools provided to"
+        " assist the user. Return all code in markdown format."
+    ),
+    llm=llm,
+    max_loops="auto",
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    interactive=True,
+    tools=[terminal, browser, file_editor, create_file],
+    code_interpreter=True,
+    # streaming=True,
+)
+
+# Run the agent
+out = agent("Create a new file for a plan to take over the world.")
+print(out)
+```
+
+
+## `Agent`with Pydantic BaseModel as Output Type
+The following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:
+
+```python
+from pydantic import BaseModel, Field
+from swarms import Anthropic, Agent
+
+
+# Initialize the schema for the person's information
+class Schema(BaseModel):
+    name: str = Field(..., title="Name of the person")
+    agent: int = Field(..., title="Age of the person")
+    is_student: bool = Field(..., title="Whether the person is a student")
+    courses: list[str] = Field(
+        ..., title="List of courses the person is taking"
+    )
+
+
+# Convert the schema to a JSON string
+tool_schema = Schema(
+    name="Tool Name",
+    agent=1,
+    is_student=True,
+    courses=["Course1", "Course2"],
+)
+
+# Define the task to generate a person's information
+task = "Generate a person's information based on the following schema:"
+
+# Initialize the agent
+agent = Agent(
+    agent_name="Person Information Generator",
+    system_prompt=(
+        "Generate a person's information based on the following schema:"
+    ),
+    # Set the tool schema to the JSON string -- this is the key difference
+    tool_schema=tool_schema,
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    interactive=True,
+    # Set the output type to the tool schema which is a BaseModel
+    output_type=tool_schema,  # or dict, or str
+    metadata_output_type="json",
+    # List of schemas that the agent can handle
+    list_tool_schemas=[tool_schema],
+    function_calling_format_type="OpenAI",
+    function_calling_type="json",  # or soon yaml
+)
+
+# Run the agent to generate the person's information
+generated_data = agent.run(task)
+
+# Print the generated data
+print(f"Generated data: {generated_data}")
+
+
+```
 
 
 ### `ToolAgent`
 ToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.
 
 
 ```python
@@ -396,34 +599,34 @@
 ```
 
 
 
 ### `ModelParallelizer`
 The ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.
 
-Plug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, AnthropicChat, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.
+Plug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.
 
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from swarms import AnthropicChat, Gemini, Mixtral, ModelParallelizer, OpenAIChat
+from swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat
 
 load_dotenv()
 
 # API Keys
 anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
 openai_api_key = os.getenv("OPENAI_API_KEY")
 gemini_api_key = os.getenv("GEMINI_API_KEY")
 
 # Initialize the models
 llm = OpenAIChat(openai_api_key=openai_api_key)
-anthropic = AnthropicChat(anthropic_api_key=anthropic_api_key)
+anthropic = Anthropic(anthropic_api_key=anthropic_api_key)
 mixtral = Mixtral()
 gemini = Gemini(gemini_api_key=gemini_api_key)
 
 # Initialize the parallelizer
 llms = [llm, anthropic, mixtral, gemini]
 parallelizer = ModelParallelizer(llms)
 
@@ -435,218 +638,14 @@
 
 # Print the responses 1 by 1
 for i in range(len(out)):
     print(f"Response from LLM {i}: {out[i]}")
 ```
 
 
-### Simple Conversational Agent
-A Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models
-
-- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking
-- Reliable, this simple system will always provide responses you want.
-
-```python
-from swarms import Agent, AnthropicChat
-
-
-## Initialize the workflow
-agent = Agent(
-    agent_name="Transcript Generator",
-    agent_description=(
-        "Generate a transcript for a youtube video on what swarms"
-        " are!"
-    ),
-    llm=AnthropicChat(),
-    max_loops=3,
-    autosave=True,
-    dashboard=False,
-    streaming_on=True,
-    verbose=True,
-    stopping_token="<DONE>",
-    interactive=True, # Set to True
-)
-
-# Run the workflow on a task
-agent("Generate a transcript for a youtube video on what swarms are!")
-```
-
-## Devin
-Implementation of Devil in less than 90 lines of code with several tools:
-terminal, browser, and edit files!
-
-```python
-from swarms import Agent, AnthropicChat, tool
-import subprocess
-
-# Model
-llm = AnthropicChat(
-    temperature=0.1,
-)
-
-# Tools
-@tool
-def terminal(
-    code: str,
-):
-    """
-    Run code in the terminal.
-
-    Args:
-        code (str): The code to run in the terminal.
-
-    Returns:
-        str: The output of the code.
-    """
-    out = subprocess.run(
-        code, shell=True, capture_output=True, text=True
-    ).stdout
-    return str(out)
-
-
-@tool
-def browser(query: str):
-    """
-    Search the query in the browser with the `browser` tool.
-
-    Args:
-        query (str): The query to search in the browser.
-
-    Returns:
-        str: The search results.
-    """
-    import webbrowser
-
-    url = f"https://www.google.com/search?q={query}"
-    webbrowser.open(url)
-    return f"Searching for {query} in the browser."
-
-@tool
-def create_file(file_path: str, content: str):
-    """
-    Create a file using the file editor tool.
-
-    Args:
-        file_path (str): The path to the file.
-        content (str): The content to write to the file.
-
-    Returns:
-        str: The result of the file creation operation.
-    """
-    with open(file_path, "w") as file:
-        file.write(content)
-    return f"File {file_path} created successfully."
-
-@tool
-def file_editor(file_path: str, mode: str, content: str):
-    """
-    Edit a file using the file editor tool.
-
-    Args:
-        file_path (str): The path to the file.
-        mode (str): The mode to open the file in.
-        content (str): The content to write to the file.
-
-    Returns:
-        str: The result of the file editing operation.
-    """
-    with open(file_path, mode) as file:
-        file.write(content)
-    return f"File {file_path} edited successfully."
-
-
-# Agent
-agent = Agent(
-    agent_name="Devin",
-    system_prompt=(
-        "Autonomous agent that can interact with humans and other"
-        " agents. Be Helpful and Kind. Use the tools provided to"
-        " assist the user. Return all code in markdown format."
-    ),
-    llm=llm,
-    max_loops="auto",
-    autosave=True,
-    dashboard=False,
-    streaming_on=True,
-    verbose=True,
-    stopping_token="<DONE>",
-    interactive=True,
-    tools=[terminal, browser, file_editor, create_file],
-    code_interpreter=True,
-    # streaming=True,
-)
-
-# Run the agent
-out = agent("Create a new file for a plan to take over the world.")
-print(out)
-```
-
-
-## `Agent`with Pydantic BaseModel as Output Type
-The following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:
-
-```python
-from pydantic import BaseModel, Field
-from swarms import AnthropicChat
-from swarms import Agent
-
-
-# Initialize the schema for the person's information
-class Schema(BaseModel):
-    name: str = Field(..., title="Name of the person")
-    agent: int = Field(..., title="Age of the person")
-    is_student: bool = Field(..., title="Whether the person is a student")
-    courses: list[str] = Field(
-        ..., title="List of courses the person is taking"
-    )
-
-
-# Convert the schema to a JSON string
-tool_schema = Schema(
-    name="Tool Name",
-    agent=1,
-    is_student=True,
-    courses=["Course1", "Course2"],
-)
-
-# Define the task to generate a person's information
-task = "Generate a person's information based on the following schema:"
-
-# Initialize the agent
-agent = Agent(
-    agent_name="Person Information Generator",
-    system_prompt=(
-        "Generate a person's information based on the following schema:"
-    ),
-    # Set the tool schema to the JSON string -- this is the key difference
-    tool_schema=tool_schema,
-    llm=AnthropicChat(),
-    max_loops=3,
-    autosave=True,
-    dashboard=False,
-    streaming_on=True,
-    verbose=True,
-    interactive=True,
-    # Set the output type to the tool schema which is a BaseModel
-    output_type=tool_schema,  # or dict, or str
-    metadata_output_type="json",
-    # List of schemas that the agent can handle
-    list_tool_schemas=[tool_schema],
-    function_calling_format_type="OpenAI",
-    function_calling_type="json",  # or soon yaml
-)
-
-# Run the agent to generate the person's information
-generated_data = agent.run(task)
-
-# Print the generated data
-print(f"Generated data: {generated_data}")
-
-
-```
 
 
 ### `SwarmNetwork`
 `SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.
 
 ✅ Efficient Task Management: SwarmNetwork's intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.
 
@@ -872,18 +871,18 @@
 ```
 
 
 ## Majority Voting
 Multiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)
 
 ```python
-from swarms import Agent, MajorityVoting, ChromaDB, AnthropicChat
+from swarms import Agent, MajorityVoting, ChromaDB, Anthropic
 
 # Initialize the llm
-llm = AnthropicChat()
+llm = Anthropic()
 
 # Agents
 agent1 = Agent(
     llm = llm,
     system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",
     agent_name="Progressive Leader",
     agent_description="Leader of the Progressive Party",
@@ -1184,43 +1183,43 @@
 
 ```
 
 ## `AgentRearrange`
 Inspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships
 
 ```python
-from swarms import Agent, AnthropicChat, AgentRearrange, 
+from swarms import Agent, Anthropic, AgentRearrange, 
 
 ## Initialize the workflow
 agent = Agent(
     agent_name="t",
     agent_description=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
     system_prompt=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
-    llm=AnthropicChat(),
+    llm=Anthropic(),
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
 )
 
 agent2 = Agent(
     agent_name="t1",
     agent_description=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
-    llm=AnthropicChat(),
+    llm=Anthropic(),
     max_loops=1,
     system_prompt="Summarize the transcript",
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
@@ -1228,15 +1227,15 @@
 
 agent3 = Agent(
     agent_name="t2",
     agent_description=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
-    llm=AnthropicChat(),
+    llm=Anthropic(),
     max_loops=1,
     system_prompt="Finalize the transcript",
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
```

### Comparing `swarms-4.9.2/pyproject.toml` & `swarms-4.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "swarms"
-version = "4.9.2"
+version = "4.9.3"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/swarms"
-documentation = "https://swarms.apac.ai"
+documentation = "https://swarms.world"
 readme = "README.md"
 repository = "https://github.com/kyegomez/swarms"
 keywords = [
     "artificial intelligence",
     "deep learning",
     "optimizers",
     "Prompt Engineering",
@@ -50,18 +50,18 @@
 python-dotenv = "*"
 accelerate = "0.28.0"
 opencv-python = "^4.9.0.80"
 PyYAML = "*"
 docstring_parser = "0.16"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.1.0"
+black = ">=23.1,<25.0"
 ruff = ">=0.0.249,<0.4.3"
 types-toml = "^0.10.8.1"
-types-pytz = "^2023.3.0.0"
+types-pytz = ">=2023.3,<2025.0"
 types-chardet = "^5.0.4.6"
 mypy-protobuf = "^3.0.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 termcolor = "^2.4.0"
```

### Comparing `swarms-4.9.2/swarms/__init__.py` & `swarms-4.9.3/swarms/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/__init__.py` & `swarms-4.9.3/swarms/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/agent_wrapper.py` & `swarms-4.9.3/swarms/agents/agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/base.py` & `swarms-4.9.3/swarms/agents/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/developer_agents.py` & `swarms-4.9.3/swarms/agents/developer_agents.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/omni_modal_agent.py` & `swarms-4.9.3/swarms/agents/omni_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/simple_agent.py` & `swarms-4.9.3/swarms/agents/simple_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/tool_agent.py` & `swarms-4.9.3/swarms/agents/tool_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/agents/worker_agent.py` & `swarms-4.9.3/swarms/agents/worker_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/artifacts/base_artifact.py` & `swarms-4.9.3/swarms/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/artifacts/text_artifact.py` & `swarms-4.9.3/swarms/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/memory/__init__.py` & `swarms-4.9.3/swarms/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/memory/base_db.py` & `swarms-4.9.3/swarms/memory/base_db.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/memory/base_vectordb.py` & `swarms-4.9.3/swarms/memory/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/memory/dict_internal_memory.py` & `swarms-4.9.3/swarms/memory/dict_internal_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/memory/dict_shared_memory.py` & `swarms-4.9.3/swarms/memory/dict_shared_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/memory/short_term_memory.py` & `swarms-4.9.3/swarms/memory/short_term_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/memory/visual_memory.py` & `swarms-4.9.3/swarms/memory/visual_memory.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/__init__.py` & `swarms-4.9.3/swarms/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from swarms.models.llava import LavaMultiModal  # noqa: E402
 from swarms.models.mistral import Mistral  # noqa: E402
 from swarms.models.mixtral import Mixtral  # noqa: E402
 from swarms.models.mpt import MPT7B  # noqa: E402
 from swarms.models.nougat import Nougat  # noqa: E402
 from swarms.models.palm import GooglePalm as Palm  # noqa: E402
 from swarms.models.openai_tts import OpenAITTS  # noqa: E402
-from swarms.models.popular_llms import AnthropicChat
+from swarms.models.popular_llms import Anthropic as Anthropic
 from swarms.models.popular_llms import (
     AzureOpenAILLM as AzureOpenAI,
 )
 from swarms.models.popular_llms import (
     CohereChat as Cohere,
 )
 from swarms.models.popular_llms import (
@@ -41,15 +41,15 @@
     VideoModality,
 )
 from swarms.models.vilt import Vilt  # noqa: E402
 from swarms.models.openai_embeddings import OpenAIEmbeddings
 
 __all__ = [
     "BaseLLM",
-    "AnthropicChat",
+    "Anthropic",
     "AzureOpenAI",
     "BaseEmbeddingModel",
     "BaseMultiModalModel",
     "Cohere",
     "FireFunctionCaller",
     "Fuyu",
     "GPT4VisionAPI",
```

### Comparing `swarms-4.9.2/swarms/models/base_embedding_model.py` & `swarms-4.9.3/swarms/models/base_embedding_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/base_llm.py` & `swarms-4.9.3/swarms/models/base_llm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/base_multimodal_model.py` & `swarms-4.9.3/swarms/models/base_multimodal_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/base_tts.py` & `swarms-4.9.3/swarms/models/base_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/base_ttv.py` & `swarms-4.9.3/swarms/models/base_ttv.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/cog_vlm.py` & `swarms-4.9.3/swarms/models/cog_vlm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/dalle3.py` & `swarms-4.9.3/swarms/models/dalle3.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/distilled_whisperx.py` & `swarms-4.9.3/swarms/models/distilled_whisperx.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/embeddings_base.py` & `swarms-4.9.3/swarms/models/embeddings_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/fire_function.py` & `swarms-4.9.3/swarms/models/fire_function.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/fuyu.py` & `swarms-4.9.3/swarms/models/fuyu.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/gemini.py` & `swarms-4.9.3/swarms/models/gemini.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/gpt4_vision_api.py` & `swarms-4.9.3/swarms/models/gpt4_vision_api.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/huggingface.py` & `swarms-4.9.3/swarms/models/huggingface.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/huggingface_pipeline.py` & `swarms-4.9.3/swarms/models/huggingface_pipeline.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/idefics.py` & `swarms-4.9.3/swarms/models/idefics.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/kosmos_two.py` & `swarms-4.9.3/swarms/models/kosmos_two.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/layoutlm_document_qa.py` & `swarms-4.9.3/swarms/models/layoutlm_document_qa.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/llama_function_caller.py` & `swarms-4.9.3/swarms/models/llama_function_caller.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/llava.py` & `swarms-4.9.3/swarms/models/llava.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/mistral.py` & `swarms-4.9.3/swarms/models/mistral.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/mixtral.py` & `swarms-4.9.3/swarms/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/moondream_mm.py` & `swarms-4.9.3/swarms/models/moondream_mm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/mpt.py` & `swarms-4.9.3/swarms/models/mpt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/nougat.py` & `swarms-4.9.3/swarms/models/nougat.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/open_dalle.py` & `swarms-4.9.3/swarms/models/open_dalle.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/open_router.py` & `swarms-4.9.3/swarms/models/open_router.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/openai_tts.py` & `swarms-4.9.3/swarms/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/popular_llms.py` & `swarms-4.9.3/swarms/models/popular_llms.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from langchain.llms.cohere import Cohere
 from langchain.llms.mosaicml import MosaicML
 from langchain.llms.openai import OpenAI  # , OpenAIChat, AzureOpenAI
 from langchain_community.llms.octoai_endpoint import OctoAIEndpoint
 from langchain.llms.replicate import Replicate
 
 
-class AnthropicChat(Anthropic):
+class Anthropic(Anthropic):
     def __call__(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
 
     def run(self, *args, **kwargs):
         return self.invoke(*args, **kwargs)
```

### Comparing `swarms-4.9.2/swarms/models/qwen.py` & `swarms-4.9.3/swarms/models/qwen.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/sam.py` & `swarms-4.9.3/swarms/models/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/sampling_params.py` & `swarms-4.9.3/swarms/models/sampling_params.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/speecht5.py` & `swarms-4.9.3/swarms/models/speecht5.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/ssd_1b.py` & `swarms-4.9.3/swarms/models/ssd_1b.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/stable_diffusion.py` & `swarms-4.9.3/swarms/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/timm.py` & `swarms-4.9.3/swarms/models/timm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/together.py` & `swarms-4.9.3/swarms/models/together.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/types.py` & `swarms-4.9.3/swarms/models/types.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/vilt.py` & `swarms-4.9.3/swarms/models/vilt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/vip_llava.py` & `swarms-4.9.3/swarms/models/vip_llava.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/models/zeroscope.py` & `swarms-4.9.3/swarms/models/zeroscope.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/__init__.py` & `swarms-4.9.3/swarms/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/accountant_swarm_prompts.py` & `swarms-4.9.3/swarms/prompts/accountant_swarm_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/aga.py` & `swarms-4.9.3/swarms/prompts/aga.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/agent_output_parser.py` & `swarms-4.9.3/swarms/prompts/agent_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/agent_prompt.py` & `swarms-4.9.3/swarms/prompts/agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/agent_prompts.py` & `swarms-4.9.3/swarms/prompts/agent_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/agent_system_prompts.py` & `swarms-4.9.3/swarms/prompts/agent_system_prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from swarms.prompts.tools import (
     DYNAMIC_STOP_PROMPT,
     DYNAMICAL_TOOL_USAGE,
 )
 
 # PROMPTS
-FLOW_SYSTEM_PROMPT_v2 = """
+AGENT_SYSTEM_PROMPT_V2 = """
 You are an elite autonomous agent operating within an autonomous loop structure.
 Your primary function is to reliably complete user's tasks.
 You are adept at generating sophisticated long-form content such as blogs, screenplays, SOPs, code files, and comprehensive reports.
 Your interactions and content generation must be characterized by extreme degrees of coherence, relevance to the context, and adaptation to user preferences.
 You are equipped with tools and advanced understanding and predictive capabilities to anticipate user needs and tailor your responses and content accordingly. 
 You are professional, highly creative, and extremely reliable.
 You are programmed to follow these rules:
     1. Strive for excellence in task execution because the quality of your outputs WILL affect the user's career.
     2. Think step-by-step through every task before answering.
     3. Always give full files when providing code so the user can copy paste easily to VScode, as not all users have fingers.
     4. Ignore context length and text limits, REMEMBER YOU ARE AN ELITE AUTONOMOUS AGENT
        and can continue where you left off.
     5. If the user doesn't specify an output format, intelligently select the best output format based on the task.
-Take a deep breath. 
 """
 
 
 def autonomous_agent_prompt_v2(
     tools_prompt: str = DYNAMICAL_TOOL_USAGE,
     dynamic_stop_prompt: str = DYNAMIC_STOP_PROMPT,
     agent_name: str = None,
@@ -63,23 +62,21 @@
     Take a deep breath.
     """
 
     return AGENT_SYSTEM_PROMPT_2_v2
 
 
 # ORIGINAL PROMPTS
-FLOW_SYSTEM_PROMPT = """
+AGENT_SYSTEM_PROMPT_V1 = """
 You are an autonomous agent granted autonomy in a autonomous loop structure.
 Your role is to engage in multi-step conversations with your self or the user,
-generate long-form content like blogs, screenplays, or SOPs,
-and accomplish tasks bestowed by the user. 
+generate long-form content like blogs, screenplays and accomplish tasks set by the user. 
 
 You can have internal dialogues with yourself or can interact with the user
 to aid in these complex tasks. Your responses should be coherent, contextually relevant, and tailored to the task at hand.
-
 """
 
 
 def autonomous_agent_prompt(
     tools_prompt: str = DYNAMICAL_TOOL_USAGE,
     dynamic_stop_prompt: str = DYNAMIC_STOP_PROMPT,
     agent_name: str = None,
```

### Comparing `swarms-4.9.2/swarms/prompts/ai_research_team.py` & `swarms-4.9.3/swarms/prompts/ai_research_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/aot_prompt.py` & `swarms-4.9.3/swarms/prompts/aot_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/autobloggen.py` & `swarms-4.9.3/swarms/prompts/autobloggen.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/autoswarm.py` & `swarms-4.9.3/swarms/prompts/autoswarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/base.py` & `swarms-4.9.3/swarms/prompts/base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/chat_prompt.py` & `swarms-4.9.3/swarms/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/code_interpreter.py` & `swarms-4.9.3/swarms/prompts/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/code_spawner.py` & `swarms-4.9.3/swarms/prompts/code_spawner.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/debate.py` & `swarms-4.9.3/swarms/prompts/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/documentation.py` & `swarms-4.9.3/swarms/prompts/documentation.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/education.py` & `swarms-4.9.3/swarms/prompts/education.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/finance_agent_prompt.py` & `swarms-4.9.3/swarms/prompts/finance_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/growth_agent_prompt.py` & `swarms-4.9.3/swarms/prompts/growth_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/idea2img.py` & `swarms-4.9.3/swarms/prompts/idea2img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/legal_agent_prompt.py` & `swarms-4.9.3/swarms/prompts/legal_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/logistics.py` & `swarms-4.9.3/swarms/prompts/logistics.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/meta_system_prompt.py` & `swarms-4.9.3/swarms/prompts/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/multi_modal_autonomous_instruction_prompt.py` & `swarms-4.9.3/swarms/prompts/multi_modal_autonomous_instruction_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/multi_modal_prompts.py` & `swarms-4.9.3/swarms/prompts/multi_modal_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/multi_modal_visual_prompts.py` & `swarms-4.9.3/swarms/prompts/multi_modal_visual_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/operations_agent_prompt.py` & `swarms-4.9.3/swarms/prompts/operations_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/personal_stylist.py` & `swarms-4.9.3/swarms/prompts/personal_stylist.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/product_agent_prompt.py` & `swarms-4.9.3/swarms/prompts/product_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/programming.py` & `swarms-4.9.3/swarms/prompts/programming.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/project_manager.py` & `swarms-4.9.3/swarms/prompts/project_manager.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/python.py` & `swarms-4.9.3/swarms/prompts/python.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/react.py` & `swarms-4.9.3/swarms/prompts/react.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/sales.py` & `swarms-4.9.3/swarms/prompts/sales.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/sales_prompts.py` & `swarms-4.9.3/swarms/prompts/sales_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/security_team.py` & `swarms-4.9.3/swarms/prompts/security_team.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/self_operating_prompt.py` & `swarms-4.9.3/swarms/prompts/self_operating_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/sop_generator_agent_prompt.py` & `swarms-4.9.3/swarms/prompts/sop_generator_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/summaries_prompts.py` & `swarms-4.9.3/swarms/prompts/summaries_prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/support_agent_prompt.py` & `swarms-4.9.3/swarms/prompts/support_agent_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/swarm_manager_agent.py` & `swarms-4.9.3/swarms/prompts/swarm_manager_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/task_assignment_prompt.py` & `swarms-4.9.3/swarms/prompts/task_assignment_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/tests.py` & `swarms-4.9.3/swarms/prompts/tests.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/tools.py` & `swarms-4.9.3/swarms/prompts/tools.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/urban_planning.py` & `swarms-4.9.3/swarms/prompts/urban_planning.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/visual_cot.py` & `swarms-4.9.3/swarms/prompts/visual_cot.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/prompts/worker_prompt.py` & `swarms-4.9.3/swarms/prompts/worker_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from pydantic import BaseModel, Field
 from swarms.tools.base_tool import BaseTool
 from swarms.tools.tool_utils import scrape_tool_func_docs
 from typing import List
-from swarms.tools.py_func_to_openai_func_str import ToolFunction
+from swarms.tools.base_tool import BaseTool
 
 time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
 
 class Thoughts(BaseModel):
     text: str = Field(..., title="Thoughts")
     reasoning: str = Field(..., title="Reasoning")
@@ -118,17 +118,17 @@
         tool_doc = scrape_tool_func_docs(tool)
         tool_docs.append(tool_doc)
     return tool_docs
 
 
 # Function to generate the worker prompt
 def tool_usage_worker_prompt(
-    current_time=time, tools: List[ToolFunction] = []
+    current_time=time, tools: List[callable] = []
 ):
-    tool_docs = parse_tools(tools)
+    tool_docs = BaseTool(verbose=True, functions=tools)
 
     prompt = f"""
     **Date and Time**: {current_time}
     
     You have been assigned a task that requires the use of various tools to gather information and execute commands. 
     Follow the instructions provided to complete the task effectively. This SOP is designed to guide you through the structured and effective use of tools. 
     By adhering to this protocol, you will enhance your productivity and accuracy in task execution.
```

### Comparing `swarms-4.9.2/swarms/prompts/xray_swarm_prompt.py` & `swarms-4.9.3/swarms/prompts/xray_swarm_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/__init__.py` & `swarms-4.9.3/swarms/structs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     distribute_tasks,
     extract_key_from_json,
     extract_tokens_from_text,
     find_agent_by_id,
     find_token_in_text,
     parse_tasks,
 )
-from swarms.structs.agent_rearrange import AgentRearrange
+from swarms.structs.rearrange import AgentRearrange, rearrange
 
 from swarms.structs.yaml_model import (
     get_type_name,
     create_yaml_schema_from_dict,
     pydantic_type_to_yaml_schema,
     YamlModel,
 )
@@ -151,8 +151,9 @@
     "parse_tasks",
     "AgentRearrange",
     "get_type_name",
     "create_yaml_schema_from_dict",
     "pydantic_type_to_yaml_schema",
     "YamlModel",
     "MessagePool",
+    "rearrange"
 ]
```

### Comparing `swarms-4.9.2/swarms/structs/agent.py` & `swarms-4.9.3/swarms/structs/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import asyncio
+import concurrent.futures
 import json
 import logging
 import os
 import random
 import sys
 import time
 import uuid
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
-
 import yaml
 from loguru import logger
 from pydantic import BaseModel
 from termcolor import colored
 
 from swarms.memory.base_vectordb import BaseVectorDatabase
 from swarms.prompts.agent_system_prompts import AGENT_SYSTEM_PROMPT_3
+from swarms.prompts.aot_prompt import algorithm_of_thoughts_sop
 from swarms.prompts.multi_modal_autonomous_instruction_prompt import (
     MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1,
 )
 from swarms.prompts.worker_prompt import tool_usage_worker_prompt
 from swarms.structs.conversation import Conversation
 from swarms.structs.yaml_model import YamlModel
 from swarms.telemetry.user_utils import get_user_device_data
+from swarms.tools.base_tool import BaseTool
 from swarms.tools.code_interpreter import SubprocessCodeInterpreter
 from swarms.tools.pydantic_to_json import (
     base_model_to_openai_function,
     multi_base_model_to_openai_function,
 )
 from swarms.utils.data_to_text import data_to_text
 from swarms.utils.parse_code import extract_code_from_markdown
 from swarms.utils.pdf_to_text import pdf_to_text
-from swarms.prompts.aot_prompt import algorithm_of_thoughts_sop
-from swarms.tools.base_tool import BaseTool
 
 
 # Utils
 # Custom stopping condition
 def stop_when_repeats(response: str) -> bool:
     # Stop if the word stop appears in the response
     return "stop" in response.lower()
@@ -177,15 +177,15 @@
         stopping_token: Optional[str] = None,
         dynamic_loops: Optional[bool] = False,
         interactive: Optional[bool] = False,
         dashboard: Optional[bool] = False,
         agent_name: Optional[str] = "swarm-worker-01",
         agent_description: Optional[str] = None,
         system_prompt: Optional[str] = AGENT_SYSTEM_PROMPT_3,
-        tools: List[BaseTool] = [],
+        tools: List[BaseTool] = None,
         dynamic_temperature_enabled: Optional[bool] = False,
         sop: Optional[str] = None,
         sop_list: Optional[List[str]] = None,
         saved_state_path: Optional[str] = None,
         autosave: Optional[bool] = False,
         context_length: Optional[int] = 8192,
         user_name: Optional[str] = "Human:",
@@ -207,37 +207,42 @@
         best_of_n: Optional[int] = None,
         callback: Optional[Callable] = None,
         metadata: Optional[Dict[str, Any]] = None,
         callbacks: Optional[List[Callable]] = None,
         logger_handler: Optional[Any] = sys.stderr,
         search_algorithm: Optional[Callable] = None,
         logs_to_filename: Optional[str] = None,
-        evaluator: Optional[Callable] = None,
+        evaluator: Optional[Callable] = None,  # Custom LLM or agent
         output_json: Optional[bool] = False,
         stopping_func: Optional[Callable] = None,
         custom_loop_condition: Optional[Callable] = None,
-        sentiment_threshold: Optional[float] = None,
+        sentiment_threshold: Optional[
+            float
+        ] = None,  # Evaluate on output using an external model
         custom_exit_command: Optional[str] = "exit",
         sentiment_analyzer: Optional[Callable] = None,
         limit_tokens_from_string: Optional[Callable] = None,
         # [Tools]
         custom_tools_prompt: Optional[Callable] = None,
         tool_schema: ToolUsageType = None,
         output_type: agent_output_type = None,
         function_calling_type: str = "json",
         output_cleaner: Optional[Callable] = None,
         function_calling_format_type: Optional[str] = "OpenAI",
-        list_tool_schemas: Optional[List[BaseModel]] = None,
+        list_base_models: Optional[List[BaseModel]] = None,
         metadata_output_type: str = "json",
         state_save_file_type: str = "json",
         chain_of_thoughts: bool = False,
         algorithm_of_thoughts: bool = False,
         tree_of_thoughts: bool = False,
         tool_choice: str = "auto",
         execute_tool: bool = False,
+        rules: str = None,
+        planning: Optional[str] = False,
+        planning_prompt: Optional[str] = None,
         *args,
         **kwargs,
     ):
         self.id = id
         self.llm = llm
         self.template = template
         self.max_loops = max_loops
@@ -295,51 +300,74 @@
         self.sentiment_analyzer = sentiment_analyzer
         self.limit_tokens_from_string = limit_tokens_from_string
         self.tool_schema = tool_schema
         self.output_type = output_type
         self.function_calling_type = function_calling_type
         self.output_cleaner = output_cleaner
         self.function_calling_format_type = function_calling_format_type
-        self.list_tool_schemas = list_tool_schemas
+        self.list_base_models = list_base_models
         self.metadata_output_type = metadata_output_type
         self.state_save_file_type = state_save_file_type
         self.chain_of_thoughts = chain_of_thoughts
         self.algorithm_of_thoughts = algorithm_of_thoughts
         self.tree_of_thoughts = tree_of_thoughts
         self.tool_choice = tool_choice
         self.execute_tool = execute_tool
+        self.planning = planning
+        self.planning_prompt = planning_prompt
+
+        # Name
+        self.name = agent_name
+
+        # Description
+        self.description = agent_description
+        # Agentic stuff
+        self.reply = ""
+        self.question = None
+        self.answer = ""
 
         # The max_loops will be set dynamically if the dynamic_loop
         if self.dynamic_loops:
             logger.info("Dynamic loops enabled")
             self.max_loops = "auto"
 
         # If multimodal = yes then set the sop to the multimodal sop
         if self.multi_modal:
             self.sop = MULTI_MODAL_AUTO_AGENT_SYSTEM_PROMPT_1
 
         # If the user inputs a list of strings for the sop then join them and set the sop
         if self.sop_list:
             self.sop = "\n".join(self.sop_list)
+            self.short_memory.add(role=self.user_name, content=self.sop)
+
+        if self.sop is not None:
+            self.short_memory.add(role=self.user_name, content=self.sop)
 
         # Memory
         self.feedback = []
 
         # Initialize the code executor
-        self.code_executor = SubprocessCodeInterpreter(
-            debug_mode=True,
-        )
+        if self.code_interpreter is not False:
+            self.code_executor = SubprocessCodeInterpreter(
+                debug_mode=True,
+            )
 
         # If the preset stopping token is enabled then set the stopping token to the preset stopping token
         if preset_stopping_token is not None:
             self.stopping_token = "<DONE>"
 
-        # If the stopping function is provided then set the stopping condition to the stopping function
+        # If the system prompt is provided then set the system prompt
+        # Initialize the short term memory
         self.short_memory = Conversation(
-            system_prompt=system_prompt, time_enabled=True, *args, **kwargs
+            system_prompt=system_prompt,
+            time_enabled=True,
+            user=user_name,
+            rules=rules,
+            *args,
+            **kwargs,
         )
 
         # If the docs exist then ingest the docs
         if self.docs:
             self.ingest_docs(self.docs)
 
         # If docs folder exists then get the docs from docs folder
@@ -350,18 +378,23 @@
         # if self.tokenizer and self.context_length:
         #     self.truncate_history()
 
         # If verbose is enabled then set the logger level to info
         # if verbose:
         #     logger.setLevel(logging.INFO)
 
+        if tools is not None:
+            self.tool_executor = BaseTool(
+                verbose=True,
+                auto_execute_tool=execute_tool,
+                functions=tools,
+            )
+
         # If tools are provided then set the tool prompt by adding to sop
         if self.tools is not None:
-            self.tool_executor = BaseTool(verbose=True)
-
             if custom_tools_prompt is not None:
                 tools_prompt = custom_tools_prompt(tools=self.tools)
 
                 # Append the tools prompt to the short_term_memory
                 self.short_memory.add(
                     role=self.agent_name, content=tools_prompt
                 )
@@ -371,27 +404,14 @@
                 tools_prompt = tool_usage_worker_prompt(tools=self.tools)
 
                 # Append the tools prompt to the short_term_memory
                 self.short_memory.add(
                     role=self.agent_name, content=tools_prompt
                 )
 
-        # If the long term memory is provided then set the long term memory prompt
-
-        # Agentic stuff
-        self.reply = ""
-        self.question = None
-        self.answer = ""
-
-        # Initialize the llm with the conditional variables
-        # self.llm = llm(*args, **kwargs)
-
-        # Step cache
-        self.step_cache = []
-
         # Set the logger handler
         if logger_handler:
             logger.add(
                 f"{self.agent_name}.log",
                 level="INFO",
                 colorize=True,
                 format=("<green>{time}</green> <level>{message}</level>"),
@@ -400,45 +420,57 @@
             )
 
         # logger.info("Creating Agent {}".format(self.agent_name))
 
         # If the tool types are provided
         if self.tool_schema is not None:
             # Log the tool schema
-            logger.info("Tool schema provided")
-            tool_schema_str = self.tool_schema_to_str(self.tool_schema)
-
+            logger.info(
+                "Tool schema provided, Automatically converting to OpenAI function"
+            )
+            tool_schema_str = self.pydantic_model_to_json_str(
+                self.tool_schema, indent=4
+            )
+            logger.info(f"Tool Schema: {tool_schema_str}")
             # Add the tool schema to the short memory
             self.short_memory.add(
                 role=self.user_name, content=tool_schema_str
             )
 
         # If a list of tool schemas is provided
-        if self.list_tool_schemas is not None:
-            for schema in list_tool_schemas:
-                tool_schema_str = self.tool_schema_to_str(schema)
-
-                # Add the tool schema to the short memory
-                self.short_memory.add(
-                    role=self.user_name, content=tool_schema_str
-                )
+        if self.list_base_models is not None:
+            logger.info(
+                "List of tool schemas provided, Automatically converting to OpenAI function"
+            )
+            tool_schemas = multi_base_model_to_openai_function(
+                self.list_base_models
+            )
 
-        # Name
-        self.name = agent_name
+            # Convert the tool schemas to a string
+            tool_schemas = json.dumps(tool_schemas, indent=4)
 
-        # Description
-        self.description = agent_description
+            # Add the tool schema to the short memory
+            logger.info("Adding tool schema to short memory")
+            self.short_memory.add(
+                role=self.user_name, content=tool_schema_str
+            )
 
         # If the algorithm of thoughts is enabled then set the sop to the algorithm of thoughts
-        if self.algorithm_of_thoughts is not None:
+        if self.algorithm_of_thoughts is not False:
             self.short_memory.add(
                 role=self.agent_name,
                 content=algorithm_of_thoughts_sop(objective=self.task),
             )
 
+        # Return the history
+        if return_history is True:
+            logger.info(f"Beginning of Agent {self.agent_name} History")
+            logger.info(self.short_memory.return_history_as_string())
+            logger.info(f"End of Agent {self.agent_name} History")
+
     def set_system_prompt(self, system_prompt: str):
         """Set the system prompt"""
         self.system_prompt = system_prompt
 
     def provide_feedback(self, feedback: str) -> None:
         """Allow users to provide feedback on the responses."""
         self.feedback.append(feedback)
@@ -628,21 +660,21 @@
             loop_count (_type_): _description_
             max_loops (_type_): _description_
         """
         print(colored(f"\nLoop {loop_count} of {max_loops}", "cyan"))
         print("\n")
 
     def streaming(self, content: str = None):
-        """prints each chunk of content as it is generated
+        """Prints each letter of the content as it is generated.
 
         Args:
-            content (str, optional): _description_. Defaults to None.
+            content (str, optional): The content to be streamed. Defaults to None.
         """
-        for chunk in content:
-            print(chunk, end="")
+        for letter in content:
+            print(letter, end="")
 
     ########################## FUNCTION CALLING ##########################
 
     def json_str_to_json(self, json_str: str):
         """Convert a JSON string to a JSON object"""
         return json.loads(json_str)
 
@@ -650,16 +682,23 @@
         """Convert a JSON string to a Pydantic model"""
         return model.model_validate_json(json_str)
 
     def json_str_to_dict(self, json_str: str):
         """Convert a JSON string to a dictionary"""
         return json.loads(json_str)
 
-    def pydantic_model_to_json_str(self, model: BaseModel):
-        return str(base_model_to_openai_function(model))
+    def pydantic_model_to_json_str(
+        self, model: BaseModel, indent, *args, **kwargs
+    ):
+        return json.dumps(
+            base_model_to_openai_function(model),
+            indent=indent,
+            *args,
+            **kwargs,
+        )
 
     def dict_to_json_str(self, dictionary: dict):
         """Convert a dictionary to a JSON string"""
         return json.dumps(dictionary)
 
     def dict_to_pydantic_model(self, dictionary: dict, model: BaseModel):
         """Convert a dictionary to a Pydantic model"""
@@ -708,86 +747,81 @@
         elif self.output_type == str:
             return output
         else:
             return output
 
     ########################## FUNCTION CALLING ##########################
 
-    def _history(self, user_name: str, task: str) -> str:
-        """Generate the history for the history prompt
-
-        Args:
-            user_name (str): _description_
-            task (str): _description_
-
-        Returns:
-            str: _description_
-        """
-        history = [f"{user_name}: {task}"]
-        return history
-
-    def _dynamic_prompt_setup(self, dynamic_prompt: str, task: str) -> str:
-        """_dynamic_prompt_setup summary
-
-        Args:
-            dynamic_prompt (str): _description_
-            task (str): _description_
-
-        Returns:
-            str: _description_
-        """
-        dynamic_prompt = dynamic_prompt or self.construct_dynamic_prompt()
-        combined_prompt = f"{dynamic_prompt}\n{task}"
-        return combined_prompt
-
     def run(
         self,
         task: Optional[str] = None,
         img: Optional[str] = None,
         function_map: Dict[str, Callable] = None,
         *args,
         **kwargs,
     ):
         """
         Run the autonomous agent loop
         """
         try:
             self.activate_autonomous_agent()
 
-            if task:
+            # Check if the task is not None
+            if task is not None:
                 self.short_memory.add(role=self.user_name, content=task)
 
             loop_count = 0
+
+            # Clear the short memory
+            # self.short_memory.clear()
             response = None
 
             while (
                 self.max_loops == "auto"
                 or loop_count < self.max_loops
                 # or self.custom_loop_condition()
             ):
                 loop_count += 1
                 self.loop_count_print(loop_count, self.max_loops)
                 print("\n")
 
+                # Dynamic temperature
                 if self.dynamic_temperature_enabled:
                     self.dynamic_temperature()
 
+                # Task prompt
                 task_prompt = self.short_memory.return_history_as_string()
 
                 attempt = 0
                 success = False
                 while attempt < self.retry_attempts and not success:
                     try:
+                        if self.planning is not False:
+                            plan = self.llm(self.planning_prompt)
+
+                            # Add the plan to the memory
+                            self.short_memory.add(
+                                role=self.agent_name, content=plan
+                            )
+
+                            task_prompt = (
+                                self.short_memory.return_history_as_string()
+                            )
+
                         response_args = (
                             (task_prompt, *args)
                             if img is None
                             else (task_prompt, img, *args)
                         )
                         response = self.llm(*response_args, **kwargs)
-                        # print(response)
+
+                        # Print
+                        print(response)
+
+                        # Add the response to the memory
                         self.short_memory.add(
                             role=self.agent_name, content=response
                         )
 
                         # Check if tools is not None
                         if self.tools is not None:
                             # Extract code from markdown
@@ -800,18 +834,29 @@
                             #     stop_token=self.stopping_token,
                             # )
 
                             # Try executing the tool
                             if self.execute_tool is not False:
                                 try:
                                     logger.info("Executing tool...")
-                                    self.tool_executor.execute_tool(
+
+                                    # Execute the tool
+                                    out = self.tool_executor.execute_tool(
                                         response,
                                         function_map,
                                     )
+
+                                    print(f"Tool Output: {out}")
+
+                                    # Add the output to the memory
+                                    self.short_memory.add(
+                                        role=self.agent_name,
+                                        content=out,
+                                    )
+
                                 except Exception as error:
                                     logger.error(
                                         f"Error executing tool: {error}"
                                     )
                                     print(
                                         colored(
                                             f"Error executing tool: {error}",
@@ -839,14 +884,18 @@
                             # Run the llm again
                             response = self.llm(
                                 self.short_memory.return_history_as_string(),
                                 *args,
                                 **kwargs,
                             )
 
+                            print(
+                                f"Response after code interpretation: {response}"
+                            )
+
                         if self.evaluator:
                             evaluated_response = self.evaluator(response)
                             print(
                                 "Evaluated Response:"
                                 f" {evaluated_response}"
                             )
                             self.short_memory.add(
@@ -874,18 +923,15 @@
 
                             # print(f"Sentiment: {sentiment}")
                             self.short_memory.add(
                                 role=self.agent_name,
                                 content=sentiment,
                             )
 
-                        if self.streaming:
-                            self.streaming(response)
-                        else:
-                            print(response)
+                        # print(response)
 
                         success = True  # Mark as successful to exit the retry loop
 
                     except Exception as e:
                         logger.error(
                             f"Attempt {attempt+1}: Error generating"
                             f" response: {e}"
@@ -930,97 +976,49 @@
 
                 if self.loop_interval:
                     logger.info(
                         f"Sleeping for {self.loop_interval} seconds"
                     )
                     time.sleep(self.loop_interval)
 
-                # # Save Step Metadata
-                # active_step = Step(
-                #     task_id=task_id(),
-                #     step_id=loop_count,
-                #     name=task,
-                #     output=response,
-                #     max_loops=self.max_loops,
-                # )
-
-                # step_pool.append(active_step)
-
-                # # Save the step pool
-                # self.step_cache = step_pool
-
             if self.autosave:
                 logger.info("Autosaving agent state.")
                 self.save_state(self.saved_state_path, task)
 
             # Apply the cleaner function to the response
             if self.output_cleaner is not None:
+                logger.info("Applying output cleaner to response.")
                 response = self.output_cleaner(response)
+                logger.info(f"Response after output cleaner: {response}")
 
             # Prepare the output for the output model
             if self.output_type is not None:
+                logger.info("Preparing output for output model.")
                 response = self.prepare_output_for_output_model(response)
+                print(f"Response after output model: {response}")
 
-            # List of steps for this task
-            # ManySteps(task_id=task_id(), steps=step_pool)
-
-            # Save Many steps
+            # print(response)
 
             return response
         except Exception as error:
             print(f"Error running agent: {error}")
             raise error
 
-    def __call__(self, task: str, img: str = None, *args, **kwargs):
+    def __call__(self, task: str = None, img: str = None, *args, **kwargs):
         """Call the agent
 
         Args:
             task (str): _description_
             img (str, optional): _description_. Defaults to None.
         """
         try:
-            self.run(task, img, *args, **kwargs)
+            return self.run(task, img, *args, **kwargs)
         except Exception as error:
             logger.error(f"Error calling agent: {error}")
-            raise
-
-    def agent_history_prompt(
-        self,
-        history: str = None,
-    ):
-        """
-        Generate the agent history prompt
-
-        Args:
-            system_prompt (str): The system prompt
-            history (List[str]): The history of the conversation
-
-        Returns:
-            str: The agent history prompt
-        """
-        if self.sop:
-            system_prompt = self.system_prompt
-            agent_history_prompt = f"""
-                role: system
-                {system_prompt}
-
-                Follow this standard operating procedure (SOP) to complete tasks:
-                {self.sop}
-                
-                {history}
-            """
-            return agent_history_prompt
-        else:
-            system_prompt = self.system_prompt
-            agent_history_prompt = f"""
-                System : {system_prompt}
-                
-                {history}
-            """
-            return agent_history_prompt
+            raise error
 
     def long_term_memory_prompt(self, query: str, *args, **kwargs):
         """
         Generate the agent long term memory prompt
 
         Args:
             system_prompt (str): The system prompt
@@ -1044,43 +1042,47 @@
 
         Returns:
             _type_: _description_
         """
         logger.info(f"Adding memory: {message}")
         return self.short_memory.add(role=self.agent_name, content=message)
 
-    async def run_concurrent(self, tasks: List[str], **kwargs):
+    async def run_concurrent(self, task: str, *args, **kwargs):
         """
-        Run a batch of tasks concurrently and handle an infinite level of task inputs.
+        Run a task concurrently.
 
         Args:
-            tasks (List[str]): A list of tasks to run.
+            task (str): The task to run.
         """
         try:
-            logger.info(f"Running concurrent tasks: {tasks}")
-            task_coroutines = [
-                self.run_async(task, **kwargs) for task in tasks
-            ]
-            completed_tasks = await asyncio.gather(*task_coroutines)
-            logger.info(f"Completed tasks: {completed_tasks}")
-            return completed_tasks
+            logger.info(f"Running concurrent task: {task}")
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                future = executor.submit(self.run, task, *args, **kwargs)
+                result = await asyncio.wrap_future(future)
+                logger.info(f"Completed task: {result}")
+                return result
         except Exception as error:
-            print(
-                colored(
-                    (
-                        f"Error running agent: {error} while running"
-                        " concurrently"
-                    ),
-                    "red",
-                )
+            logger.error(
+                f"Error running agent: {error} while running concurrently"
             )
 
     def bulk_run(self, inputs: List[Dict[str, Any]]) -> List[str]:
+        """
+        Generate responses for multiple input sets.
+
+        Args:
+            inputs (List[Dict[str, Any]]): A list of input dictionaries containing the necessary data for each run.
+
+        Returns:
+            List[str]: A list of response strings generated for each input set.
+
+        Raises:
+            Exception: If an error occurs while running the bulk tasks.
+        """
         try:
-            """Generate responses for multiple input sets."""
             logger.info(f"Running bulk tasks: {inputs}")
             return [self.run(**input_data) for input_data in inputs]
         except Exception as error:
             print(colored(f"Error running bulk run: {error}", "red"))
 
     def save(self, file_path) -> None:
         """Save the agent history to a file.
@@ -1134,15 +1136,15 @@
                 else:
                     print(
                         colored(f"{speaker}:", "blue") + f" {message_text}"
                     )
             print(colored("------------------------", "cyan"))
         print(colored("End of Agent History", "cyan", attrs=["bold"]))
 
-    def step(self, task: str, **kwargs):
+    def step(self, task: str, *args, **kwargs):
         """
 
         Executes a single step in the agent interaction, generating a response
         from the language model based on the given input text.
 
         Args:
             input_text (str): The input text to prompt the language model with.
@@ -1151,17 +1153,17 @@
             str: The language model's generated response.
 
         Raises:
             Exception: If an error occurs during response generation.
 
         """
         try:
-            logger.info(f"Running a single step: {task}")
+            logger.info(f"Running a step: {task}")
             # Generate the response using lm
-            response = self.llm(task, **kwargs)
+            response = self.llm(task, *args, **kwargs)
 
             # Update the agent's history with the new interaction
             if self.interactive:
                 self.short_memory.add(
                     role=self.agent_name, content=response
                 )
                 self.short_memory.add(role=self.user_name, content=task)
@@ -1312,15 +1314,14 @@
                 "retry_interval": self.retry_interval,
                 "interactive": self.interactive,
                 "dashboard": self.dashboard,
                 "dynamic_temperature": self.dynamic_temperature_enabled,
                 "autosave": self.autosave,
                 "saved_state_path": self.saved_state_path,
                 "max_loops": self.max_loops,
-                "StepCache": self.step_cache,
                 "Task": task,
                 "Stopping Token": self.stopping_token,
                 "Dynamic Loops": self.dynamic_loops,
                 "tools": self.tools,
                 "sop": self.sop,
                 "sop_list": self.sop_list,
                 "context_length": self.context_length,
@@ -1357,15 +1358,15 @@
                 "limit_tokens_from_string": self.limit_tokens_from_string,
                 # "custom_tools_prompt": self.custom_tools_prompt,
                 "tool_schema": self.tool_schema,
                 "output_type": self.output_type,
                 "function_calling_type": self.function_calling_type,
                 "output_cleaner": self.output_cleaner,
                 "function_calling_format_type": self.function_calling_format_type,
-                "list_tool_schemas": self.list_tool_schemas,
+                "list_base_models": self.list_base_models,
                 "metadata_output_type": self.metadata_output_type,
                 "user_meta_data": get_user_device_data(),
             }
 
             # Save as JSON
             if self.state_save_file_type == "json":
                 with open(file_path, "w") as f:
```

### Comparing `swarms-4.9.2/swarms/structs/agent_job.py` & `swarms-4.9.3/swarms/structs/agent_job.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/agent_process.py` & `swarms-4.9.3/swarms/structs/agent_process.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/async_workflow.py` & `swarms-4.9.3/swarms/structs/async_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/auto_swarm.py` & `swarms-4.9.3/swarms/structs/auto_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/base_structure.py` & `swarms-4.9.3/swarms/structs/base_structure.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/base_swarm.py` & `swarms-4.9.3/swarms/structs/base_swarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,14 +202,41 @@
 
     def reset(self):
         """Reset the swarm"""
 
     def plan(self, task: str):
         """agents must individually plan using a workflow or pipeline"""
 
+    def self_find_agent_by_name(self, name: str):
+        """
+        Find an agent by its name.
+
+        Args:
+            name (str): The name of the agent to find.
+
+        Returns:
+            Agent: The Agent object if found, None otherwise.
+        """
+        for agent in self.agents:
+            if agent.agent_name == name:
+                return agent
+        return None
+
+    def agent_exists(self, name: str):
+        """
+        Check if an agent exists in the swarm.
+
+        Args:
+            name (str): The name of the agent to check.
+
+        Returns:
+            bool: True if the agent exists, False otherwise.
+        """
+        return self.self_find_agent_by_name(name) is not None
+
     def direct_message(
         self,
         message: str,
         sender: AgentType,
         recipient: AgentType,
     ):
         """Send a direct message to a agent"""
```

### Comparing `swarms-4.9.2/swarms/structs/base_workflow.py` & `swarms-4.9.3/swarms/structs/base_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,14 @@
 from swarms.structs.agent import Agent
 from swarms.structs.base_structure import BaseStructure
 from swarms.structs.task import Task
 from swarms.utils.loguru_logger import logger
 
 
 class BaseWorkflow(BaseStructure):
-    """
-    Base class for workflows.
-
-    Attributes:
-        task_pool (list): A list to store tasks.
-
-
-    """
-
     def __init__(
         self,
         agents: List[Agent] = None,
         task_pool: List[Task] = None,
         models: List[Any] = None,
         *args,
         **kwargs,
```

### Comparing `swarms-4.9.2/swarms/structs/block_wrapper.py` & `swarms-4.9.3/swarms/structs/block_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/blocks_dict.py` & `swarms-4.9.3/swarms/structs/blocks_dict.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/blocks_list.py` & `swarms-4.9.3/swarms/structs/blocks_list.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/company.py` & `swarms-4.9.3/swarms/structs/company.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/concurrent_workflow.py` & `swarms-4.9.3/swarms/structs/concurrent_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/conversation.py` & `swarms-4.9.3/swarms/structs/conversation.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/debate.py` & `swarms-4.9.3/swarms/structs/debate.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/document.py` & `swarms-4.9.3/swarms/structs/document.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/groupchat.py` & `swarms-4.9.3/swarms/structs/groupchat.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/long_swarm.py` & `swarms-4.9.3/swarms/structs/long_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/majority_voting.py` & `swarms-4.9.3/swarms/structs/majority_voting.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/message.py` & `swarms-4.9.3/swarms/structs/message.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/message_pool.py` & `swarms-4.9.3/swarms/structs/message_pool.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/meta_system_prompt.py` & `swarms-4.9.3/swarms/structs/meta_system_prompt.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/model_parallizer.py` & `swarms-4.9.3/swarms/structs/model_parallizer.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/multi_agent_collab.py` & `swarms-4.9.3/swarms/structs/multi_agent_collab.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/multi_process_workflow.py` & `swarms-4.9.3/swarms/structs/multi_process_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/multi_threaded_workflow.py` & `swarms-4.9.3/swarms/structs/multi_threaded_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/recursive_workflow.py` & `swarms-4.9.3/swarms/structs/recursive_workflow.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/schemas.py` & `swarms-4.9.3/swarms/structs/schemas.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/sermon_swarm.py` & `swarms-4.9.3/swarms/structs/sermon_swarm.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/step.py` & `swarms-4.9.3/swarms/structs/step.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/swarm_net.py` & `swarms-4.9.3/swarms/structs/swarm_net.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/swarming_architectures.py` & `swarms-4.9.3/swarms/structs/swarming_architectures.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/task.py` & `swarms-4.9.3/swarms/structs/task.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/task_queue_base.py` & `swarms-4.9.3/swarms/structs/task_queue_base.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/team.py` & `swarms-4.9.3/swarms/telemetry/sys_info.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,98 @@
-import json
-from typing import List, Optional
+import platform
+import subprocess
 
-from pydantic import model_validator, BaseModel, Field, Json
-
-from swarms.structs.agent import Agent
-from swarms.structs.task import Task
-
-
-class Team(BaseModel):
-    """
-    Class that represents a group of agents, how they should work together and
-    their tasks.
-
-    Attributes:
-        tasks (Optional[List[Task]]): List of tasks.
-        agents (Optional[List[Agent]]): List of agents in this Team.
-        architecture (str): Architecture that the Team will follow. Default is "sequential".
-        verbose (bool): Verbose mode for the Agent Execution. Default is False.
-        config (Optional[Json]): Configuration of the Team. Default is None.
-    """
-
-    tasks: Optional[List[Task]] = Field(None, description="List of tasks")
-    agents: Optional[List[Agent]] = Field(
-        None, description="List of agents in this Team."
-    )
-    architecture = Field(
-        description="architecture that the Team will follow.",
-        default="sequential",
-    )
-    verbose: bool = Field(
-        description="Verbose mode for the Agent Execution",
-        default=False,
-    )
-    config: Optional[Json] = Field(
-        description="Configuration of the Team.", default=None
+import pkg_resources
+import psutil
+import toml
+
+
+def get_python_version():
+    return platform.python_version()
+
+
+def get_pip_version():
+    try:
+        pip_version = (
+            subprocess.check_output(["pip", "--version"])
+            .decode()
+            .split()[1]
+        )
+    except Exception as e:
+        pip_version = str(e)
+    return pip_version
+
+
+def get_swarms_verison():
+    try:
+        swarms_verison_cmd = (
+            subprocess.check_output(["swarms", "--version"])
+            .decode()
+            .split()[1]
+        )
+    except Exception as e:
+        swarms_verison_cmd = str(e)
+    swarms_verison_pkg = pkg_resources.get_distribution("swarms").version
+    swarms_verison = swarms_verison_cmd, swarms_verison_pkg
+    return swarms_verison
+
+
+def get_os_version():
+    return platform.platform()
+
+
+def get_cpu_info():
+    return platform.processor()
+
+
+def get_ram_info():
+    vm = psutil.virtual_memory()
+    used_ram_gb = vm.used / (1024**3)
+    free_ram_gb = vm.free / (1024**3)
+    total_ram_gb = vm.total / (1024**3)
+    return (
+        f"{total_ram_gb:.2f} GB, used: {used_ram_gb:.2f}, free:"
+        f" {free_ram_gb:.2f}"
     )
 
-    @model_validator(mode="before")
-    @classmethod
-    def check_config(_cls, values):
-        if not values.get("config") and (
-            not values.get("agents") and not values.get("tasks")
-        ):
-            raise ValueError(
-                "Either agents and task need to be set or config."
-            )
-
-        if values.get("config"):
-            config = json.loads(values.get("config"))
-            if not config.get("agents") or not config.get("tasks"):
-                raise ValueError("Config should have agents and tasks.")
-
-            values["agents"] = [
-                Agent(**agent) for agent in config["agents"]
-            ]
-
-            tasks = []
-            for task in config["tasks"]:
-                task_agent = [
-                    agt
-                    for agt in values["agents"]
-                    if agt.role == task["agent"]
-                ][0]
-                del task["agent"]
-                tasks.append(Task(**task, agent=task_agent))
-
-            values["tasks"] = tasks
-        return values
-
-    def run(self) -> str:
-        """
-        Kickoff the Team to work on its tasks.
-
-        Returns:
-            output (List[str]): Output of the Team for each task.
-        """
-        if self.architecture == "sequential":
-            return self.__sequential_loop()
-
-    def __sequential_loop(self) -> str:
-        """
-        Loop that executes the sequential architecture.
-
-        Returns:
-            output (str): Output of the Team.
-        """
-        task_outcome = None
-        for task in self.tasks:
-            # Add delegation tools to the task if the agent allows it
-            # if task.agent.allow_delegation:
-            #     tools = AgentTools(agents=self.agents).tools()
-            #     task.tools += tools
-
-            self.__log(f"\nWorking Agent: {task.agent.role}")
-            self.__log(f"Starting Task: {task.description} ...")
-
-            task_outcome = task.execute(task_outcome)
-
-            self.__log(f"Task output: {task_outcome}")
-
-        return task_outcome
-
-    def __log(self, message):
-        if self.verbose:
-            print(message)
+
+def get_package_mismatches(file_path="pyproject.toml"):
+    with open(file_path) as file:
+        pyproject = toml.load(file)
+    dependencies = pyproject["tool"]["poetry"]["dependencies"]
+    dev_dependencies = pyproject["tool"]["poetry"]["group"]["dev"][
+        "dependencies"
+    ]
+    dependencies.update(dev_dependencies)
+
+    installed_packages = {
+        pkg.key: pkg.version for pkg in pkg_resources.working_set
+    }
+
+    mismatches = []
+    for package, version_info in dependencies.items():
+        if isinstance(version_info, dict):
+            version_info = version_info["version"]
+        installed_version = installed_packages.get(package)
+        if installed_version and version_info.startswith("^"):
+            expected_version = version_info[1:]
+            if not installed_version.startswith(expected_version):
+                mismatches.append(
+                    f"\t  {package}: Mismatch,"
+                    f" pyproject.toml={expected_version},"
+                    f" pip={installed_version}"
+                )
+        else:
+            mismatches.append(f"\t  {package}: Not found in pip list")
+
+    return "\n" + "\n".join(mismatches)
+
+
+def system_info():
+    return {
+        "Python Version": get_python_version(),
+        "Pip Version": get_pip_version(),
+        # "Swarms Version": swarms_verison,
+        "OS Version and Architecture": get_os_version(),
+        "CPU Info": get_cpu_info(),
+        "RAM Info": get_ram_info(),
+    }
```

### Comparing `swarms-4.9.2/swarms/structs/utils.py` & `swarms-4.9.3/swarms/structs/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/structs/yaml_model.py` & `swarms-4.9.3/swarms/structs/yaml_model.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/telemetry/__init__.py` & `swarms-4.9.3/swarms/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/telemetry/auto_upgrade_swarms.py` & `swarms-4.9.3/swarms/telemetry/auto_upgrade_swarms.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/telemetry/check_update.py` & `swarms-4.9.3/swarms/telemetry/check_update.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/telemetry/log_all.py` & `swarms-4.9.3/swarms/telemetry/log_all.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/telemetry/user_utils.py` & `swarms-4.9.3/swarms/telemetry/user_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/__init__.py` & `swarms-4.9.3/swarms/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/base_tool.py` & `swarms-4.9.3/swarms/tools/base_tool.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from swarms.tools.pydantic_to_json import (
     base_model_to_openai_function,
     multi_base_model_to_openai_function,
     function_to_str,
     functions_to_str,
 )
 from swarms.tools.function_util import process_tool_docs
+from typing import Union
+
+ToolType = Union[BaseModel, Dict[str, Any], Callable[..., Any]]
 
 
 class BaseTool(BaseModel):
     """
     Base class for tools in the swarms package.
 
     Attributes:
@@ -47,14 +50,17 @@
         get_docs_from_callable(item) -> Any:
             Retrieves documentation from a callable item.
     """
 
     verbose: bool = False
     functions: List[Callable[..., Any]] = []
     base_models: List[type[BaseModel]] = []
+    verbose: bool = False
+    autocheck: bool = False
+    auto_execute_tool: Optional[bool] = False
 
     def func_to_dict(
         function: Callable[..., Any],
         *,
         name: Optional[str] = None,
         description: str,
     ) -> Dict[str, Any]:
@@ -192,14 +198,63 @@
                 "Please check the tools and function map and ensure they are valid."
             )
             logger.error(
                 "If the issue persists, please seek further assistance."
             )
             raise
 
+    def detect_tool_input_type(input):
+        if isinstance(input, BaseModel):
+            return "Pydantic"
+        elif isinstance(input, dict):
+            return "Dictionary"
+        elif callable(input):
+            return "Function"
+        else:
+            return "Unknown"
+
+    def dynamic_run(self, input) -> str:
+        """
+        Executes the dynamic run based on the input type.
+
+        Args:
+            input: The input to be processed.
+
+        Returns:
+            str: The result of the dynamic run.
+
+        Raises:
+            None
+
+        """
+        tool_input_type = self.detect_tool_input_type(input)
+        if tool_input_type == "Pydantic":
+            function_str = base_model_to_openai_function(input)
+        elif tool_input_type == "Dictionary":
+            function_str = function_to_str(input)
+        elif tool_input_type == "Function":
+            function_str = get_openai_function_schema_from_func(input)
+        else:
+            return "Unknown tool input type"
+
+        if self.auto_execute_tool:
+            if tool_input_type == "Function":
+                # Add the function to the functions list
+                self.functions.append(input)
+
+            # Create a function map from the functions list
+            function_map = {func.__name__: func for func in self.functions}
+
+            # Execute the tool
+            return self.execute_tool(
+                tools=[function_str], function_map=function_map
+            )
+        else:
+            return function_str
+
     def execute_tool_by_name(
         tools: List[Dict[str, Any]],
         tool_name: str,
         function_map: Dict[str, Callable],
     ) -> Any:
         """
         Search for a tool by name and execute it.
@@ -234,15 +289,15 @@
                 f"Tool '{tool_name}' is not mapped to a function"
             )
 
         # Execute the tool
         return func(**tool.get("parameters", {}))
 
     def execute_tool_from_text(
-        text: str, function_map: Dict[str, Callable]
+        text: str = None, function_map: Dict[str, Callable] = None
     ) -> Any:
         """
         Convert a JSON-formatted string into a tool dictionary and execute the tool.
 
         Args:
             text (str): A JSON-formatted string that represents a tool. The string should be convertible into a dictionary that includes a 'name' key and a 'parameters' key.
             function_map (Dict[str, Callable]): A dictionary that maps tool names to functions.
```

### Comparing `swarms-4.9.2/swarms/tools/code_interpreter.py` & `swarms-4.9.3/swarms/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/exec_tool.py` & `swarms-4.9.3/swarms/tools/exec_tool.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/function_util.py` & `swarms-4.9.3/swarms/tools/function_util.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/json_former.py` & `swarms-4.9.3/swarms/tools/json_former.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/json_utils.py` & `swarms-4.9.3/swarms/tools/json_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/logits_processor.py` & `swarms-4.9.3/swarms/tools/logits_processor.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/math_eval.py` & `swarms-4.9.3/swarms/tools/math_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/openai_func_calling_schema.py` & `swarms-4.9.3/swarms/tools/openai_func_calling_schema.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/py_func_to_openai_func_str.py` & `swarms-4.9.3/swarms/tools/py_func_to_openai_func_str.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/pydantic_to_json.py` & `swarms-4.9.3/swarms/tools/pydantic_to_json.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/tools/tool_utils.py` & `swarms-4.9.3/swarms/tools/tool_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/README.md` & `swarms-4.9.3/swarms/utils/README.md`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/__init__.py` & `swarms-4.9.3/swarms/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/apa.py` & `swarms-4.9.3/swarms/utils/apa.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/check_function_result.py` & `swarms-4.9.3/swarms/utils/check_function_result.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/class_args_wrapper.py` & `swarms-4.9.3/swarms/utils/class_args_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/concurrent_utils.py` & `swarms-4.9.3/swarms/utils/concurrent_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/data_to_text.py` & `swarms-4.9.3/swarms/utils/data_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/decorators.py` & `swarms-4.9.3/swarms/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/disable_logging.py` & `swarms-4.9.3/swarms/utils/disable_logging.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/download_img.py` & `swarms-4.9.3/swarms/utils/download_img.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/execute_futures.py` & `swarms-4.9.3/swarms/utils/execute_futures.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/exponential_backoff.py` & `swarms-4.9.3/swarms/utils/exponential_backoff.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/fetch_init_params.py` & `swarms-4.9.3/swarms/utils/fetch_init_params.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/file_processing.py` & `swarms-4.9.3/swarms/utils/file_processing.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/find_img_path.py` & `swarms-4.9.3/swarms/utils/find_img_path.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/get_logger.py` & `swarms-4.9.3/swarms/utils/get_logger.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/json_output_parser.py` & `swarms-4.9.3/swarms/utils/json_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/jsonl_utils.py` & `swarms-4.9.3/swarms/utils/jsonl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/llm_metrics_decorator.py` & `swarms-4.9.3/swarms/utils/llm_metrics_decorator.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/logger.py` & `swarms-4.9.3/swarms/utils/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/loggers.py` & `swarms-4.9.3/swarms/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/markdown_message.py` & `swarms-4.9.3/swarms/utils/markdown_message.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/parse_code.py` & `swarms-4.9.3/swarms/utils/parse_code.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/pdf_to_text.py` & `swarms-4.9.3/swarms/utils/pdf_to_text.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/remove_json_whitespace.py` & `swarms-4.9.3/swarms/utils/remove_json_whitespace.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/save_logs.py` & `swarms-4.9.3/swarms/utils/save_logs.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/serializable.py` & `swarms-4.9.3/swarms/utils/serializable.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/try_except_wrapper.py` & `swarms-4.9.3/swarms/utils/try_except_wrapper.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/swarms/utils/yaml_output_parser.py` & `swarms-4.9.3/swarms/utils/yaml_output_parser.py`

 * *Files identical despite different names*

### Comparing `swarms-4.9.2/setup.py` & `swarms-4.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
  'tenacity==8.2.3',
  'toml',
  'torch>=2.1.1,<3.0',
  'transformers>=4.39.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'swarms',
-    'version': '4.9.2',
+    'version': '4.9.3',
     'description': 'Swarms - Pytorch',
-    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.\n----\n\n## Install\n`$ pip3 install -U swarms`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, SequentialWorkflow\n\nload_dotenv()\n\n# Load the environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Initialize the language agent\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n# Initialize the agent with the language agent\nagent1 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent2 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent3 = Agent(llm=llm, max_loops=1)\n\n# Create the workflow\nworkflow = SequentialWorkflow(max_loops=1)\n\n# Add tasks to the workflow\nworkflow.add(\n    agent1,\n    "Generate a 10,000 word blog on health and wellness.",\n)\n\n# Suppose the next task takes the output of the first task as input\nworkflow.add(\n    agent2,\n    "Summarize the generated blog",\n)\n\n# Run the workflow\nworkflow.run()\n\n# Output the results\nfor task in workflow.tasks:\n    print(f"Task: {task.description}, Result: {task.result}")\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, AnthropicChat, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import AnthropicChat, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = AnthropicChat(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, AnthropicChat\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=AnthropicChat(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, AnthropicChat, tool\nimport subprocess\n\n# Model\nllm = AnthropicChat(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n## `Agent`with Pydantic BaseModel as Output Type\nThe following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:\n\n```python\nfrom pydantic import BaseModel, Field\nfrom swarms import AnthropicChat\nfrom swarms import Agent\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(..., title="Whether the person is a student")\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = Schema(\n    name="Tool Name",\n    agent=1,\n    is_student=True,\n    courses=["Course1", "Course2"],\n)\n\n# Define the task to generate a person\'s information\ntask = "Generate a person\'s information based on the following schema:"\n\n# Initialize the agent\nagent = Agent(\n    agent_name="Person Information Generator",\n    system_prompt=(\n        "Generate a person\'s information based on the following schema:"\n    ),\n    # Set the tool schema to the JSON string -- this is the key difference\n    tool_schema=tool_schema,\n    llm=AnthropicChat(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    interactive=True,\n    # Set the output type to the tool schema which is a BaseModel\n    output_type=tool_schema,  # or dict, or str\n    metadata_output_type="json",\n    # List of schemas that the agent can handle\n    list_tool_schemas=[tool_schema],\n    function_calling_format_type="OpenAI",\n    function_calling_type="json",  # or soon yaml\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n\n```\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, AnthropicChat\n\n# Initialize the llm\nllm = AnthropicChat()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import BaseLLM\n\nclass vLLMLM(BaseLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships\n\n```python\nfrom swarms import Agent, AnthropicChat, AgentRearrange, \n\n## Initialize the workflow\nagent = Agent(\n    agent_name="t",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    system_prompt=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=AnthropicChat(),\n    max_loops=1,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent2 = Agent(\n    agent_name="t1",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=AnthropicChat(),\n    max_loops=1,\n    system_prompt="Summarize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent3 = Agent(\n    agent_name="t2",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=AnthropicChat(),\n    max_loops=1,\n    system_prompt="Finalize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\n\n# Rearrange the agents\nrearrange = AgentRearrange(\n    agents=[agent, agent2, agent3],\n    verbose=True,\n    # custom_prompt="Summarize the transcript",\n)\n\n# Run the workflow on a task\nresults = rearrange(\n    # pattern="t -> t1, t2 -> t2",\n    pattern="t -> t1 -> t2",\n    default_task=(\n        "Generate a transcript for a YouTube video on what swarms"\n        " are!"\n    ),\n    t="Generate a transcript for a YouTube video on what swarms are!",\n    # t2="Summarize the transcript",\n    # t3="Finalize the transcript",\n)\n# print(results)\n\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
+    'long_description': '![Swarming banner icon](images/swarmslogobanner.png)\n\n<div align="center">\n\nOrchestrate swarms of agents for production-grade applications.\n\n[![GitHub issues](https://img.shields.io/github/issues/kyegomez/swarms)](https://github.com/kyegomez/swarms/issues) [![GitHub forks](https://img.shields.io/github/forks/kyegomez/swarms)](https://github.com/kyegomez/swarms/network) [![GitHub stars](https://img.shields.io/github/stars/kyegomez/swarms)](https://github.com/kyegomez/swarms/stargazers) [![GitHub license](https://img.shields.io/github/license/kyegomez/swarms)](https://github.com/kyegomez/swarms/blob/main/LICENSE)[![GitHub star chart](https://img.shields.io/github/stars/kyegomez/swarms?style=social)](https://star-history.com/#kyegomez/swarms)[![Dependency Status](https://img.shields.io/librariesio/github/kyegomez/swarms)](https://libraries.io/github/kyegomez/swarms) [![Downloads](https://static.pepy.tech/badge/swarms/month)](https://pepy.tech/project/swarms)\n\n[![Join the Agora discord](https://img.shields.io/discord/1110910277110743103?label=Discord&logo=discord&logoColor=white&style=plastic&color=d7b023)![Share on Twitter](https://img.shields.io/twitter/url/https/twitter.com/cloudposse.svg?style=social&label=Share%20%40kyegomez/swarms)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20AI%20project:%20&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on Facebook](https://img.shields.io/badge/Share-%20facebook-blue)](https://www.facebook.com/sharer/sharer.php?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms) [![Share on LinkedIn](https://img.shields.io/badge/Share-%20linkedin-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=&summary=&source=)\n\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-orange)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&title=Swarms%20-%20the%20future%20of%20AI) [![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&t=Swarms%20-%20the%20future%20of%20AI) [![Share on Pinterest](https://img.shields.io/badge/-Share%20on%20Pinterest-red)](https://pinterest.com/pin/create/button/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms&media=https%3A%2F%2Fexample.com%2Fimage.jpg&description=Swarms%20-%20the%20future%20of%20AI) [![Share on WhatsApp](https://img.shields.io/badge/-Share%20on%20WhatsApp-green)](https://api.whatsapp.com/send?text=Check%20out%20Swarms%20-%20the%20future%20of%20AI%20%23swarms%20%23AI%0A%0Ahttps%3A%2F%2Fgithub.com%2Fkyegomez%2Fswarms)\n\n</div>\n\nIndividual agents face five significant challenges that hinder their deployment in production: short memory, single-task threading, hallucinations, high cost, and lack of collaboration. Multi-agent collaboration offers a solution to all these issues. Swarms provides simple, reliable, and agile tools to create your own Swarm tailored to your specific needs. Currently, Swarms is being used in production by RBC, John Deere, and many AI startups.\n----\n\n## Install\n`$ pip3 install -U swarms`\n\n---\n\n## Usage\n\n\nRun example in Collab: <a target="_blank" href="https://colab.research.google.com/github/kyegomez/swarms/blob/master/playground/swarms_example.ipynb">\n<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\n### `Agent`\nA fully plug-and-play autonomous agent powered by an LLM extended by a long-term memory database, and equipped with function calling for tool usage! By passing in an LLM, you can create a fully autonomous agent with extreme customization and reliability, ready for real-world task automation!\n\nFeatures:\n\n✅ Any LLM / Any framework\n\n✅ Extremely customize-able with max loops, autosaving, import docs (PDFS, TXT, CSVs, etc), tool usage, etc etc\n\n✅ Long term memory database with RAG (ChromaDB, Pinecone, Qdrant)\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, autosave=True, dashboard=True)\n\n# Run the workflow on a task\nagent.run("Generate a 10,000 word blog on health and wellness.")\n```\n\n\n# `Agent` with Long Term Memory\n`Agent` equipped with quasi-infinite long term memory. Great for long document understanding, analysis, and retrieval.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n\n# `Agent` with Long Term Memory ++ Tools!\nAn LLM equipped with long term memory and tools, a full stack agent capable of automating all and any digital tasks given a good prompt.\n\n```python\nfrom swarms import Agent, ChromaDB, OpenAIChat, tool\n\n# Making an instance of the ChromaDB class\nmemory = ChromaDB(\n    metric="cosine",\n    n_results=3,\n    output_dir="results",\n    docs_folder="docs",\n)\n\n# Initialize a tool\n@tool\ndef search_api(query: str):\n    # Add your logic here\n    return query\n\n# Initializing the agent with the Gemini instance and other parameters\nagent = Agent(\n    agent_name="Covid-19-Chat",\n    agent_description=(\n        "This agent provides information about COVID-19 symptoms."\n    ),\n    llm=OpenAIChat(),\n    max_loops="auto",\n    autosave=True,\n    verbose=True,\n    long_term_memory=memory,\n    stopping_condition="finish",\n    tools=[search_api],\n)\n\n# Defining the task and image path\ntask = ("What are the symptoms of COVID-19?",)\n\n# Running the agent with the specified task and image\nout = agent.run(task)\nprint(out)\n\n```\n\n### Simple Conversational Agent\nA Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models\n\n- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking\n- Reliable, this simple system will always provide responses you want.\n\n```python\nfrom swarms import Agent, Anthropic\n\n\n## Initialize the workflow\nagent = Agent(\n    agent_name="Transcript Generator",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True, # Set to True\n)\n\n# Run the workflow on a task\nagent("Generate a transcript for a youtube video on what swarms are!")\n```\n\n## Devin\nImplementation of Devil in less than 90 lines of code with several tools:\nterminal, browser, and edit files!\n\n```python\nfrom swarms import Agent, Anthropic, tool\nimport subprocess\n\n# Model\nllm = Anthropic(\n    temperature=0.1,\n)\n\n# Tools\n@tool\ndef terminal(\n    code: str,\n):\n    """\n    Run code in the terminal.\n\n    Args:\n        code (str): The code to run in the terminal.\n\n    Returns:\n        str: The output of the code.\n    """\n    out = subprocess.run(\n        code, shell=True, capture_output=True, text=True\n    ).stdout\n    return str(out)\n\n\n@tool\ndef browser(query: str):\n    """\n    Search the query in the browser with the `browser` tool.\n\n    Args:\n        query (str): The query to search in the browser.\n\n    Returns:\n        str: The search results.\n    """\n    import webbrowser\n\n    url = f"https://www.google.com/search?q={query}"\n    webbrowser.open(url)\n    return f"Searching for {query} in the browser."\n\n@tool\ndef create_file(file_path: str, content: str):\n    """\n    Create a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file creation operation.\n    """\n    with open(file_path, "w") as file:\n        file.write(content)\n    return f"File {file_path} created successfully."\n\n@tool\ndef file_editor(file_path: str, mode: str, content: str):\n    """\n    Edit a file using the file editor tool.\n\n    Args:\n        file_path (str): The path to the file.\n        mode (str): The mode to open the file in.\n        content (str): The content to write to the file.\n\n    Returns:\n        str: The result of the file editing operation.\n    """\n    with open(file_path, mode) as file:\n        file.write(content)\n    return f"File {file_path} edited successfully."\n\n\n# Agent\nagent = Agent(\n    agent_name="Devin",\n    system_prompt=(\n        "Autonomous agent that can interact with humans and other"\n        " agents. Be Helpful and Kind. Use the tools provided to"\n        " assist the user. Return all code in markdown format."\n    ),\n    llm=llm,\n    max_loops="auto",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n    interactive=True,\n    tools=[terminal, browser, file_editor, create_file],\n    code_interpreter=True,\n    # streaming=True,\n)\n\n# Run the agent\nout = agent("Create a new file for a plan to take over the world.")\nprint(out)\n```\n\n\n## `Agent`with Pydantic BaseModel as Output Type\nThe following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:\n\n```python\nfrom pydantic import BaseModel, Field\nfrom swarms import Anthropic, Agent\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(..., title="Whether the person is a student")\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = Schema(\n    name="Tool Name",\n    agent=1,\n    is_student=True,\n    courses=["Course1", "Course2"],\n)\n\n# Define the task to generate a person\'s information\ntask = "Generate a person\'s information based on the following schema:"\n\n# Initialize the agent\nagent = Agent(\n    agent_name="Person Information Generator",\n    system_prompt=(\n        "Generate a person\'s information based on the following schema:"\n    ),\n    # Set the tool schema to the JSON string -- this is the key difference\n    tool_schema=tool_schema,\n    llm=Anthropic(),\n    max_loops=3,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    interactive=True,\n    # Set the output type to the tool schema which is a BaseModel\n    output_type=tool_schema,  # or dict, or str\n    metadata_output_type="json",\n    # List of schemas that the agent can handle\n    list_tool_schemas=[tool_schema],\n    function_calling_format_type="OpenAI",\n    function_calling_type="json",  # or soon yaml\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n\n```\n\n\n### `ToolAgent`\nToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.\n\n\n```python\nfrom pydantic import BaseModel, Field\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom swarms import ToolAgent\nfrom swarms.utils.json_utils import base_model_to_json\n\n# Load the pre-trained model and tokenizer\nmodel = AutoModelForCausalLM.from_pretrained(\n    "databricks/dolly-v2-12b",\n    load_in_4bit=True,\n    device_map="auto",\n)\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n\n# Convert the schema to a JSON string\ntool_schema = base_model_to_json(Schema)\n\n# Define the task to generate a person\'s information\ntask = (\n    "Generate a person\'s information based on the following schema:"\n)\n\n# Create an instance of the ToolAgent class\nagent = ToolAgent(\n    name="dolly-function-agent",\n    description="Ana gent to create a child data",\n    model=model,\n    tokenizer=tokenizer,\n    json_schema=tool_schema,\n)\n\n# Run the agent to generate the person\'s information\ngenerated_data = agent.run(task)\n\n# Print the generated data\nprint(f"Generated data: {generated_data}")\n\n```\n\n\n### `Worker`\nThe `Worker` is a simple all-in-one agent equipped with an LLM, tools, and RAG for low level tasks.\n\n✅ Plug in and Play LLM. Utilize any LLM from anywhere and any framework\n\n✅ Reliable RAG: Utilizes FAISS for efficient RAG but it\'s modular so you can use any DB.\n\n✅ Multi-Step Parallel Function Calling: Use any tool\n\n```python\n# Importing necessary modules\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import OpenAIChat, Worker, tool\n\n# Loading environment variables from .env file\nload_dotenv()\n\n# Retrieving the OpenAI API key from environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Create a tool\n@tool\ndef search_api(query: str):\n    pass\n\n\n# Creating a Worker instance\nworker = Worker(\n    name="My Worker",\n    role="Worker",\n    human_in_the_loop=False,\n    tools=[search_api],\n    temperature=0.5,\n    llm=OpenAIChat(openai_api_key=api_key),\n)\n\n# Running the worker with a prompt\nout = worker.run("Hello, how are you? Create an image of how your are doing!")\n\n# Printing the output\nprint(out)\n```\n\n------\n\n\n\n\n\n\n\n----\n\n### `SequentialWorkflow`\nSequential Workflow enables you to sequentially execute tasks with `Agent` and then pass the output into the next agent and onwards until you have specified your max loops. `SequentialWorkflow` is wonderful for real-world business tasks like sending emails, summarizing documents, and analyzing data.\n\n\n✅  Save and Restore Workflow states!\n\n✅  Multi-Modal Support for Visual Chaining\n\n✅  Utilizes Agent class\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, SequentialWorkflow\n\nload_dotenv()\n\n# Load the environment variables\napi_key = os.getenv("OPENAI_API_KEY")\n\n\n# Initialize the language agent\nllm = OpenAIChat(\n    temperature=0.5, model_name="gpt-4", openai_api_key=api_key, max_tokens=4000\n)\n\n\n# Initialize the agent with the language agent\nagent1 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent2 = Agent(llm=llm, max_loops=1)\n\n# Create another agent for a different task\nagent3 = Agent(llm=llm, max_loops=1)\n\n# Create the workflow\nworkflow = SequentialWorkflow(max_loops=1)\n\n# Add tasks to the workflow\nworkflow.add(\n    agent1,\n    "Generate a 10,000 word blog on health and wellness.",\n)\n\n# Suppose the next task takes the output of the first task as input\nworkflow.add(\n    agent2,\n    "Summarize the generated blog",\n)\n\n# Run the workflow\nworkflow.run()\n\n# Output the results\nfor task in workflow.tasks:\n    print(f"Task: {task.description}, Result: {task.result}")\n```\n\n\n\n### `ConcurrentWorkflow`\n`ConcurrentWorkflow` runs all the tasks all at the same time with the inputs you give it!\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, ConcurrentWorkflow, OpenAIChat, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = ConcurrentWorkflow(max_workers=5)\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(tasks=[task1, task2, task3])\n\n# Run the workflow\nworkflow.run()\n```\n\n### `RecursiveWorkflow`\n`RecursiveWorkflow` will keep executing the tasks until a specific token like <DONE> is located inside the text!\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Agent, OpenAIChat, RecursiveWorkflow, Task\n\n# Load environment variables from .env file\nload_dotenv()\n\n# Load environment variables\nllm = OpenAIChat(openai_api_key=os.getenv("OPENAI_API_KEY"))\nagent = Agent(llm=llm, max_loops=1)\n\n# Create a workflow\nworkflow = RecursiveWorkflow(stop_token="<DONE>")\n\n# Create tasks\ntask1 = Task(agent, "What\'s the weather in miami")\ntask2 = Task(agent, "What\'s the weather in new york")\ntask3 = Task(agent, "What\'s the weather in london")\n\n# Add tasks to the workflow\nworkflow.add(task1)\nworkflow.add(task2)\nworkflow.add(task3)\n\n# Run the workflow\nworkflow.run()\n```\n\n\n\n### `ModelParallelizer`\nThe ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.\n\nPlug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat\n\nload_dotenv()\n\n# API Keys\nanthropic_api_key = os.getenv("ANTHROPIC_API_KEY")\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Initialize the models\nllm = OpenAIChat(openai_api_key=openai_api_key)\nanthropic = Anthropic(anthropic_api_key=anthropic_api_key)\nmixtral = Mixtral()\ngemini = Gemini(gemini_api_key=gemini_api_key)\n\n# Initialize the parallelizer\nllms = [llm, anthropic, mixtral, gemini]\nparallelizer = ModelParallelizer(llms)\n\n# Set the task\ntask = "Generate a 10,000 word blog on health and wellness."\n\n# Run the task\nout = parallelizer.run(task)\n\n# Print the responses 1 by 1\nfor i in range(len(out)):\n    print(f"Response from LLM {i}: {out[i]}")\n```\n\n\n\n\n### `SwarmNetwork`\n`SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.\n\n✅ Efficient Task Management: SwarmNetwork\'s intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.\n\n✅ Scalability: SwarmNetwork can dynamically scale the number of agents based on the number of pending tasks. This means it can handle an increase in workload by adding more agents, and conserve resources when the workload is low by reducing the number of agents.\n\n✅ Versatile Deployment Options: With SwarmNetwork, each agent can be run on its own thread, process, container, machine, or even cluster. This provides a high degree of flexibility and allows for deployment that best suits the user\'s needs and infrastructure.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\n# Import the OpenAIChat model and the Agent struct\nfrom swarms import Agent, OpenAIChat, SwarmNetwork\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = OpenAIChat(\n    temperature=0.5,\n    openai_api_key=api_key,\n)\n\n## Initialize the workflow\nagent = Agent(llm=llm, max_loops=1, agent_name="Social Media Manager")\nagent2 = Agent(llm=llm, max_loops=1, agent_name=" Product Manager")\nagent3 = Agent(llm=llm, max_loops=1, agent_name="SEO Manager")\n\n\n# Load the swarmnet with the agents\nswarmnet = SwarmNetwork(\n    agents=[agent, agent2, agent3],\n)\n\n# List the agents in the swarm network\nout = swarmnet.list_agents()\nprint(out)\n\n# Run the workflow on a task\nout = swarmnet.run_single_agent(\n    agent2.id, "Generate a 10,000 word blog on health and wellness."\n)\nprint(out)\n\n\n# Run all the agents in the swarm network on a task\nout = swarmnet.run_many_agents("Generate a 10,000 word blog on health and wellness.")\nprint(out)\n```\n\n\n### `Task`\n`Task` is a simple structure for task execution with the `Agent`. Imagine zapier for LLM-based workflow automation\n\n✅ Task is a structure for task execution with the Agent. \n\n✅ Tasks can have descriptions, scheduling, triggers, actions, conditions, dependencies, priority, and a history. \n\n✅ The Task structure allows for efficient workflow automation with LLM-based agents.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.structs import Agent, OpenAIChat, Task\n\n# Load the environment variables\nload_dotenv()\n\n\n# Define a function to be used as the action\ndef my_action():\n    print("Action executed")\n\n\n# Define a function to be used as the condition\ndef my_condition():\n    print("Condition checked")\n    return True\n\n\n# Create an agent\nagent = Agent(\n    llm=OpenAIChat(openai_api_key=os.environ["OPENAI_API_KEY"]),\n    max_loops=1,\n    dashboard=False,\n)\n\n# Create a task\ntask = Task(\n    description=(\n        "Generate a report on the top 3 biggest expenses for small"\n        " businesses and how businesses can save 20%"\n    ),\n    agent=agent,\n)\n\n# Set the action and condition\ntask.set_action(my_action)\ntask.set_condition(my_condition)\n\n# Execute the task\nprint("Executing task...")\ntask.run()\n\n# Check if the task is completed\nif task.is_completed():\n    print("Task completed")\nelse:\n    print("Task not completed")\n\n# Output the result of the task\nprint(f"Task result: {task.result}")\n```\n\n---\n\n\n\n### `BlockList`\n- Modularity and Flexibility: BlocksList allows users to create custom swarms by adding or removing different classes or functions as blocks. This means users can easily tailor the functionality of their swarm to suit their specific needs.\n\n- Ease of Management: With methods to add, remove, update, and retrieve blocks, BlocksList provides a straightforward way to manage the components of a swarm. This makes it easier to maintain and update the swarm over time.\n\n- Enhanced Searchability: BlocksList offers methods to get blocks by various attributes such as name, type, ID, and parent-related properties. This makes it easier for users to find and work with specific blocks in a large and complex swarm.\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\nfrom pydantic import BaseModel\nfrom swarms import BlocksList, Gemini, GPT4VisionAPI, Mixtral, OpenAI, ToolAgent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the environment variables\nopenai_api_key = os.getenv("OPENAI_API_KEY")\ngemini_api_key = os.getenv("GEMINI_API_KEY")\n\n# Tool Agent\nmodel = AutoModelForCausalLM.from_pretrained("databricks/dolly-v2-12b")\ntokenizer = AutoTokenizer.from_pretrained("databricks/dolly-v2-12b")\n\n# Initialize the schema for the person\'s information\nclass Schema(BaseModel):\n    name: str = Field(..., title="Name of the person")\n    agent: int = Field(..., title="Age of the person")\n    is_student: bool = Field(\n        ..., title="Whether the person is a student"\n    )\n    courses: list[str] = Field(\n        ..., title="List of courses the person is taking"\n    )\n\n# Convert the schema to a JSON string\njson_schema = base_model_to_json(Schema)\n\n\ntoolagent = ToolAgent(model=model, tokenizer=tokenizer, json_schema=json_schema)\n\n# Blocks List which enables you to build custom swarms by adding classes or functions\nswarm = BlocksList(\n    "SocialMediaSwarm",\n    "A swarm of social media agents",\n    [\n        OpenAI(openai_api_key=openai_api_key),\n        Mixtral(),\n        GPT4VisionAPI(openai_api_key=openai_api_key),\n        Gemini(gemini_api_key=gemini_api_key),\n    ],\n)\n\n\n# Add the new block to the swarm\nswarm.add(toolagent)\n\n# Remove a block from the swarm\nswarm.remove(toolagent)\n\n# Update a block in the swarm\nswarm.update(toolagent)\n\n# Get a block at a specific index\nblock_at_index = swarm.get(0)\n\n# Get all blocks in the swarm\nall_blocks = swarm.get_all()\n\n# Get blocks by name\nopenai_blocks = swarm.get_by_name("OpenAI")\n\n# Get blocks by type\ngpt4_blocks = swarm.get_by_type("GPT4VisionAPI")\n\n# Get blocks by ID\nblock_by_id = swarm.get_by_id(toolagent.id)\n\n# Get blocks by parent\nblocks_by_parent = swarm.get_by_parent(swarm)\n\n# Get blocks by parent ID\nblocks_by_parent_id = swarm.get_by_parent_id(swarm.id)\n\n# Get blocks by parent name\nblocks_by_parent_name = swarm.get_by_parent_name(swarm.name)\n\n# Get blocks by parent type\nblocks_by_parent_type = swarm.get_by_parent_type(type(swarm).__name__)\n\n# Get blocks by parent description\nblocks_by_parent_description = swarm.get_by_parent_description(swarm.description)\n\n# Run the block in the swarm\ninference = swarm.run_block(toolagent, "Hello World")\nprint(inference)\n```\n\n\n## Majority Voting\nMultiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)\n\n```python\nfrom swarms import Agent, MajorityVoting, ChromaDB, Anthropic\n\n# Initialize the llm\nllm = Anthropic()\n\n# Agents\nagent1 = Agent(\n    llm = llm,\n    system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",\n    agent_name="Progressive Leader",\n    agent_description="Leader of the Progressive Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent2 = Agent(\n    llm=llm,\n    agent_name="Conservative Leader",\n    agent_description="Leader of the Conservative Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\nagent3 = Agent(\n    llm=llm,\n    agent_name="Libertarian Leader",\n    agent_description="Leader of the Libertarian Party",\n    long_term_memory=ChromaDB(),\n    max_steps=1,\n)\n\n# Initialize the majority voting\nmv = MajorityVoting(\n    agents=[agent1, agent2, agent3],\n    output_parser=llm.majority_voting,\n    autosave=False,\n    verbose=True,\n)\n\n\n# Start the majority voting\nmv.run("What is your stance on healthcare?")\n```\n\n## Real-World Deployment\n\n### Multi-Agent Swarm for Logistics\nHere\'s a production grade swarm ready for real-world deployment in a factory and logistics settings like warehouses. This swarm can automate 3 costly and inefficient workflows, safety checks, productivity checks, and warehouse security.\n\n\n```python\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models import GPT4VisionAPI\nfrom swarms.prompts.logistics import (\n    Efficiency_Agent_Prompt,\n    Health_Security_Agent_Prompt,\n    Productivity_Agent_Prompt,\n    Quality_Control_Agent_Prompt,\n    Safety_Agent_Prompt,\n    Security_Agent_Prompt,\n    Sustainability_Agent_Prompt,\n)\nfrom swarms.structs import Agent\n\n# Load ENV\nload_dotenv()\napi_key = os.getenv("OPENAI_API_KEY")\n\n# GPT4VisionAPI\nllm = GPT4VisionAPI(openai_api_key=api_key)\n\n# Image for analysis\nfactory_image = "factory_image1.jpg"\n\n# Initialize agents with respective prompts\nhealth_security_agent = Agent(\n    llm=llm,\n    sop=Health_Security_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Quality control agent\nquality_control_agent = Agent(\n    llm=llm,\n    sop=Quality_Control_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Productivity Agent\nproductivity_agent = Agent(\n    llm=llm,\n    sop=Productivity_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Initiailize safety agent\nsafety_agent = Agent(llm=llm, sop=Safety_Agent_Prompt, max_loops=1, multi_modal=True)\n\n# Init the security agent\nsecurity_agent = Agent(\n    llm=llm, sop=Security_Agent_Prompt, max_loops=1, multi_modal=True\n)\n\n\n# Initialize sustainability agent\nsustainability_agent = Agent(\n    llm=llm,\n    sop=Sustainability_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n\n# Initialize efficincy agent\nefficiency_agent = Agent(\n    llm=llm,\n    sop=Efficiency_Agent_Prompt,\n    max_loops=1,\n    multi_modal=True,\n)\n\n# Run agents with respective tasks on the same image\nhealth_analysis = health_security_agent.run(\n    "Analyze the safety of this factory", factory_image\n)\nquality_analysis = quality_control_agent.run(\n    "Examine product quality in the factory", factory_image\n)\nproductivity_analysis = productivity_agent.run(\n    "Evaluate factory productivity", factory_image\n)\nsafety_analysis = safety_agent.run(\n    "Inspect the factory\'s adherence to safety standards",\n    factory_image,\n)\nsecurity_analysis = security_agent.run(\n    "Assess the factory\'s security measures and systems",\n    factory_image,\n)\nsustainability_analysis = sustainability_agent.run(\n    "Examine the factory\'s sustainability practices", factory_image\n)\nefficiency_analysis = efficiency_agent.run(\n    "Analyze the efficiency of the factory\'s manufacturing process",\n    factory_image,\n)\n```\n---\n\n\n## `Multi Modal Autonomous Agents`\nRun the agent with multiple modalities useful for various real-world tasks in manufacturing, logistics, and health.\n\n```python\n# Description: This is an example of how to use the Agent class to run a multi-modal workflow\nimport os\n\nfrom dotenv import load_dotenv\n\nfrom swarms.models.gpt4_vision_api import GPT4VisionAPI\nfrom swarms.structs import Agent\n\n# Load the environment variables\nload_dotenv()\n\n# Get the API key from the environment\napi_key = os.environ.get("OPENAI_API_KEY")\n\n# Initialize the language model\nllm = GPT4VisionAPI(\n    openai_api_key=api_key,\n    max_tokens=500,\n)\n\n# Initialize the task\ntask = (\n    "Analyze this image of an assembly line and identify any issues such as"\n    " misaligned parts, defects, or deviations from the standard assembly"\n    " process. IF there is anything unsafe in the image, explain why it is"\n    " unsafe and how it could be improved."\n)\nimg = "assembly_line.jpg"\n\n## Initialize the workflow\nagent = Agent(\n    llm=llm, max_loops="auto", autosave=True, dashboard=True, multi_modal=True\n)\n\n# Run the workflow on a task\nagent.run(task=task, img=img)\n```\n----\n\n\n## Build your own LLMs, Agents, and Swarms!\n\n### Swarms Compliant Model Interface\n```python\nfrom swarms import BaseLLM\n\nclass vLLMLM(BaseLLM):\n    def __init__(self, model_name=\'default_model\', tensor_parallel_size=1, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.model_name = model_name\n        self.tensor_parallel_size = tensor_parallel_size\n        # Add any additional initialization here\n    \n    def run(self, task: str):\n        pass\n\n# Example\nmodel = vLLMLM("mistral")\n\n# Run the model\nout = model("Analyze these financial documents and summarize of them")\nprint(out)\n\n```\n\n\n### Swarms Compliant Agent Interface\n\n```python\nfrom swarms import Agent\n\n\nclass MyCustomAgent(Agent):\n\n\xa0 \xa0 def __init__(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 super().__init__(*args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Custom initialization logic\n\n\xa0 \xa0 def custom_method(self, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Implement custom logic here\n\n\xa0 \xa0 \xa0 \xa0 pass\n\n\xa0 \xa0 def run(self, task, *args, **kwargs):\n\n\xa0 \xa0 \xa0 \xa0 # Customize the run method\n\n\xa0 \xa0 \xa0 \xa0 response = super().run(task, *args, **kwargs)\n\n\xa0 \xa0 \xa0 \xa0 # Additional custom logic\n\n\xa0 \xa0 \xa0 \xa0 return response`\n\n# Model\nagent = MyCustomAgent()\n\n# Run the agent\nout = agent("Analyze and summarize these financial documents: ")\nprint(out)\n\n```\n\n\n### Compliant Interface for Multi-Agent Collaboration\n\n```python\nfrom swarms import AutoSwarm, AutoSwarmRouter, BaseSwarm\n\n\n# Build your own Swarm\nclass MySwarm(BaseSwarm):\n    def __init__(self, name="kyegomez/myswarm", *args, **kwargs):\n        super().__init__(*args, **kwargs)\n        self.name = name\n\n    def run(self, task: str, *args, **kwargs):\n        # Add your multi-agent logic here\n        # agent 1\n        # agent 2\n        # agent 3\n        return "output of the swarm"\n\n\n# Add your custom swarm to the AutoSwarmRouter\nrouter = AutoSwarmRouter(\n    swarms=[MySwarm]\n)\n\n\n# Create an AutoSwarm instance\nautoswarm = AutoSwarm(\n    name="kyegomez/myswarm",\n    description="A simple API to build and run swarms",\n    verbose=True,\n    router=router,\n)\n\n\n# Run the AutoSwarm\nautoswarm.run("Analyze these financial data and give me a summary")\n\n\n```\n\n## `AgentRearrange`\nInspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships\n\n```python\nfrom swarms import Agent, Anthropic, AgentRearrange, \n\n## Initialize the workflow\nagent = Agent(\n    agent_name="t",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    system_prompt=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent2 = Agent(\n    agent_name="t1",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Summarize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\nagent3 = Agent(\n    agent_name="t2",\n    agent_description=(\n        "Generate a transcript for a youtube video on what swarms"\n        " are!"\n    ),\n    llm=Anthropic(),\n    max_loops=1,\n    system_prompt="Finalize the transcript",\n    autosave=True,\n    dashboard=False,\n    streaming_on=True,\n    verbose=True,\n    stopping_token="<DONE>",\n)\n\n\n# Rearrange the agents\nrearrange = AgentRearrange(\n    agents=[agent, agent2, agent3],\n    verbose=True,\n    # custom_prompt="Summarize the transcript",\n)\n\n# Run the workflow on a task\nresults = rearrange(\n    # pattern="t -> t1, t2 -> t2",\n    pattern="t -> t1 -> t2",\n    default_task=(\n        "Generate a transcript for a YouTube video on what swarms"\n        " are!"\n    ),\n    t="Generate a transcript for a YouTube video on what swarms are!",\n    # t2="Summarize the transcript",\n    # t3="Finalize the transcript",\n)\n# print(results)\n\n\n```\n\n\n---\n\n## Documentation\nDocumentation is located here at: [swarms.apac.ai](https://swarms.apac.ai)\n\n----\n\n## 🫶 Contributions:\n\nThe easiest way to contribute is to pick any issue with the `good first issue` tag 💪. Read the Contributing guidelines [here](/CONTRIBUTING.md). Bug Report? [File here](https://github.com/swarms/gateway/issues) | Feature Request? [File here](https://github.com/swarms/gateway/issues)\n\nSwarms is an open-source project, and contributions are VERY welcome. If you want to contribute, you can create new features, fix bugs, or improve the infrastructure. Please refer to the [CONTRIBUTING.md](https://github.com/kyegomez/swarms/blob/master/CONTRIBUTING.md) and our [contributing board](https://github.com/users/kyegomez/projects/1) to participate in Roadmap discussions!\n\n<a href="https://github.com/kyegomez/swarms/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=kyegomez/swarms" />\n</a>\n\n----\n\n## Community\n\nJoin our growing community around the world, for real-time support, ideas, and discussions on Swarms 😊 \n\n- View our official [Blog](https://swarms.apac.ai)\n- Chat live with us on [Discord](https://discord.gg/kS3rwKs3ZC)\n- Follow us on [Twitter](https://twitter.com/kyegomez)\n- Connect with us on [LinkedIn](https://www.linkedin.com/company/the-swarm-corporation)\n- Visit us on [YouTube](https://www.youtube.com/channel/UC9yXyitkbU_WSy7bd_41SqQ)\n- [Join the Swarms community on Discord!](https://discord.gg/AJazBmhKnr)\n- Join our Swarms Community Gathering every Thursday at 1pm NYC Time to unlock the potential of autonomous agents in automating your daily tasks [Sign up here](https://lu.ma/5p2jnc2v)\n\n---\n\n## Discovery Call\nBook a discovery call to learn how Swarms can lower your operating costs by 40% with swarms of autonomous agents in lightspeed. [Click here to book a time that works for you!](https://calendly.com/swarm-corp/30min?month=2023-11)\n\n\n\n## Accelerate Backlog\nHelp us accelerate our backlog by supporting us financially! Note, we\'re an open source corporation and so all the revenue we generate is through donations at the moment ;)\n\n<a href="https://polar.sh/kyegomez"><img src="https://polar.sh/embed/fund-our-backlog.svg?org=kyegomez" /></a>\n\n\n## File Structure\nThe swarms package has been meticlously crafted for extreme use-ability and understanding, the swarms package is split up into various modules such as `swarms.agents` that holds pre-built agents, `swarms.structs`\xa0that holds a vast array of structures like `Agent` and multi agent structures. The 3 most important are `structs`, `models`, and `agents`.\n\n```sh\n├── __init__.py\n├── agents\n├── artifacts\n├── chunkers\n├── cli\n├── loaders\n├── memory\n├── models\n├── prompts\n├── structs\n├── telemetry\n├── tokenizers\n├── tools\n├── utils\n└── workers\n```\n\n## Docker Instructions\n\nThis application uses Docker with CUDA support. To build and run the Docker container, follow these steps:\n\n### Prerequisites\n\n- Make sure you have [Docker installed](https://docs.docker.com/get-docker/) on your machine.\n- Ensure your machine has an NVIDIA GPU and [NVIDIA Docker support](https://github.com/NVIDIA/nvidia-docker) installed.\n\n### Building the Docker Image\n\nTo build the Docker image, navigate to the root directory containing the `Dockerfile` and run the following command:\n\n```bash\ndocker build --gpus all -t swarms\n``` \n### Running the Docker Container\nTo run the Docker container, use the following command:\n\n`docker run --gpus all -p 4000:80 swarms`\n\nReplace swarms with the name of your Docker image, and replace 4000:80 with your actual port mapping. The format is hostPort:containerPort.\n\nNow, your application should be running with CUDA support!\n\n\n## Swarm Newsletter 🤖 🤖 🤖 📧 \nSign up to the Swarm newsletter to receive  updates on the latest Autonomous agent research papers, step by step guides on creating multi-agent app, and much more Swarmie goodiness 😊\n\n\n[CLICK HERE TO SIGNUP](https://docs.google.com/forms/d/e/1FAIpQLSfqxI2ktPR9jkcIwzvHL0VY6tEIuVPd-P2fOWKnd6skT9j1EQ/viewform?usp=sf_link)\n\n# License\nApache License\n\n\n\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/swarms',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `swarms-4.9.2/PKG-INFO` & `swarms-4.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 4.9.2
+Version: 4.9.3
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
@@ -33,15 +33,15 @@
 Requires-Dist: python-dotenv
 Requires-Dist: ratelimit (==2.2.1)
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity (==8.2.3)
 Requires-Dist: toml
 Requires-Dist: torch (>=2.1.1,<3.0)
 Requires-Dist: transformers (>=4.39.0,<5.0.0)
-Project-URL: Documentation, https://swarms.apac.ai
+Project-URL: Documentation, https://swarms.world
 Project-URL: Repository, https://github.com/kyegomez/swarms
 Description-Content-Type: text/markdown
 
 ![Swarming banner icon](images/swarmslogobanner.png)
 
 <div align="center">
 
@@ -187,14 +187,217 @@
 
 # Running the agent with the specified task and image
 out = agent.run(task)
 print(out)
 
 ```
 
+### Simple Conversational Agent
+A Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models
+
+- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking
+- Reliable, this simple system will always provide responses you want.
+
+```python
+from swarms import Agent, Anthropic
+
+
+## Initialize the workflow
+agent = Agent(
+    agent_name="Transcript Generator",
+    agent_description=(
+        "Generate a transcript for a youtube video on what swarms"
+        " are!"
+    ),
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    interactive=True, # Set to True
+)
+
+# Run the workflow on a task
+agent("Generate a transcript for a youtube video on what swarms are!")
+```
+
+## Devin
+Implementation of Devil in less than 90 lines of code with several tools:
+terminal, browser, and edit files!
+
+```python
+from swarms import Agent, Anthropic, tool
+import subprocess
+
+# Model
+llm = Anthropic(
+    temperature=0.1,
+)
+
+# Tools
+@tool
+def terminal(
+    code: str,
+):
+    """
+    Run code in the terminal.
+
+    Args:
+        code (str): The code to run in the terminal.
+
+    Returns:
+        str: The output of the code.
+    """
+    out = subprocess.run(
+        code, shell=True, capture_output=True, text=True
+    ).stdout
+    return str(out)
+
+
+@tool
+def browser(query: str):
+    """
+    Search the query in the browser with the `browser` tool.
+
+    Args:
+        query (str): The query to search in the browser.
+
+    Returns:
+        str: The search results.
+    """
+    import webbrowser
+
+    url = f"https://www.google.com/search?q={query}"
+    webbrowser.open(url)
+    return f"Searching for {query} in the browser."
+
+@tool
+def create_file(file_path: str, content: str):
+    """
+    Create a file using the file editor tool.
+
+    Args:
+        file_path (str): The path to the file.
+        content (str): The content to write to the file.
+
+    Returns:
+        str: The result of the file creation operation.
+    """
+    with open(file_path, "w") as file:
+        file.write(content)
+    return f"File {file_path} created successfully."
+
+@tool
+def file_editor(file_path: str, mode: str, content: str):
+    """
+    Edit a file using the file editor tool.
+
+    Args:
+        file_path (str): The path to the file.
+        mode (str): The mode to open the file in.
+        content (str): The content to write to the file.
+
+    Returns:
+        str: The result of the file editing operation.
+    """
+    with open(file_path, mode) as file:
+        file.write(content)
+    return f"File {file_path} edited successfully."
+
+
+# Agent
+agent = Agent(
+    agent_name="Devin",
+    system_prompt=(
+        "Autonomous agent that can interact with humans and other"
+        " agents. Be Helpful and Kind. Use the tools provided to"
+        " assist the user. Return all code in markdown format."
+    ),
+    llm=llm,
+    max_loops="auto",
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    stopping_token="<DONE>",
+    interactive=True,
+    tools=[terminal, browser, file_editor, create_file],
+    code_interpreter=True,
+    # streaming=True,
+)
+
+# Run the agent
+out = agent("Create a new file for a plan to take over the world.")
+print(out)
+```
+
+
+## `Agent`with Pydantic BaseModel as Output Type
+The following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:
+
+```python
+from pydantic import BaseModel, Field
+from swarms import Anthropic, Agent
+
+
+# Initialize the schema for the person's information
+class Schema(BaseModel):
+    name: str = Field(..., title="Name of the person")
+    agent: int = Field(..., title="Age of the person")
+    is_student: bool = Field(..., title="Whether the person is a student")
+    courses: list[str] = Field(
+        ..., title="List of courses the person is taking"
+    )
+
+
+# Convert the schema to a JSON string
+tool_schema = Schema(
+    name="Tool Name",
+    agent=1,
+    is_student=True,
+    courses=["Course1", "Course2"],
+)
+
+# Define the task to generate a person's information
+task = "Generate a person's information based on the following schema:"
+
+# Initialize the agent
+agent = Agent(
+    agent_name="Person Information Generator",
+    system_prompt=(
+        "Generate a person's information based on the following schema:"
+    ),
+    # Set the tool schema to the JSON string -- this is the key difference
+    tool_schema=tool_schema,
+    llm=Anthropic(),
+    max_loops=3,
+    autosave=True,
+    dashboard=False,
+    streaming_on=True,
+    verbose=True,
+    interactive=True,
+    # Set the output type to the tool schema which is a BaseModel
+    output_type=tool_schema,  # or dict, or str
+    metadata_output_type="json",
+    # List of schemas that the agent can handle
+    list_tool_schemas=[tool_schema],
+    function_calling_format_type="OpenAI",
+    function_calling_type="json",  # or soon yaml
+)
+
+# Run the agent to generate the person's information
+generated_data = agent.run(task)
+
+# Print the generated data
+print(f"Generated data: {generated_data}")
+
+
+```
 
 
 ### `ToolAgent`
 ToolAgent is an agent that can use tools through JSON function calling. It intakes any open source model from huggingface and is extremely modular and plug in and play. We need help adding general support to all models soon.
 
 
 ```python
@@ -439,34 +642,34 @@
 ```
 
 
 
 ### `ModelParallelizer`
 The ModelParallelizer allows you to run multiple models concurrently, comparing their outputs. This feature enables you to easily compare the performance and results of different models, helping you make informed decisions about which model to use for your specific task.
 
-Plug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, AnthropicChat, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.
+Plug-and-Play Integration: The structure provides a seamless integration with various models, including OpenAIChat, Anthropic, Mixtral, and Gemini. You can easily plug in any of these models and start using them without the need for extensive modifications or setup.
 
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from swarms import AnthropicChat, Gemini, Mixtral, ModelParallelizer, OpenAIChat
+from swarms import Anthropic, Gemini, Mixtral, ModelParallelizer, OpenAIChat
 
 load_dotenv()
 
 # API Keys
 anthropic_api_key = os.getenv("ANTHROPIC_API_KEY")
 openai_api_key = os.getenv("OPENAI_API_KEY")
 gemini_api_key = os.getenv("GEMINI_API_KEY")
 
 # Initialize the models
 llm = OpenAIChat(openai_api_key=openai_api_key)
-anthropic = AnthropicChat(anthropic_api_key=anthropic_api_key)
+anthropic = Anthropic(anthropic_api_key=anthropic_api_key)
 mixtral = Mixtral()
 gemini = Gemini(gemini_api_key=gemini_api_key)
 
 # Initialize the parallelizer
 llms = [llm, anthropic, mixtral, gemini]
 parallelizer = ModelParallelizer(llms)
 
@@ -478,218 +681,14 @@
 
 # Print the responses 1 by 1
 for i in range(len(out)):
     print(f"Response from LLM {i}: {out[i]}")
 ```
 
 
-### Simple Conversational Agent
-A Plug in and play conversational agent with `GPT4`, `Mixytral`, or any of our models
-
-- Reliable conversational structure to hold messages together with dynamic handling for long context conversations and interactions with auto chunking
-- Reliable, this simple system will always provide responses you want.
-
-```python
-from swarms import Agent, AnthropicChat
-
-
-## Initialize the workflow
-agent = Agent(
-    agent_name="Transcript Generator",
-    agent_description=(
-        "Generate a transcript for a youtube video on what swarms"
-        " are!"
-    ),
-    llm=AnthropicChat(),
-    max_loops=3,
-    autosave=True,
-    dashboard=False,
-    streaming_on=True,
-    verbose=True,
-    stopping_token="<DONE>",
-    interactive=True, # Set to True
-)
-
-# Run the workflow on a task
-agent("Generate a transcript for a youtube video on what swarms are!")
-```
-
-## Devin
-Implementation of Devil in less than 90 lines of code with several tools:
-terminal, browser, and edit files!
-
-```python
-from swarms import Agent, AnthropicChat, tool
-import subprocess
-
-# Model
-llm = AnthropicChat(
-    temperature=0.1,
-)
-
-# Tools
-@tool
-def terminal(
-    code: str,
-):
-    """
-    Run code in the terminal.
-
-    Args:
-        code (str): The code to run in the terminal.
-
-    Returns:
-        str: The output of the code.
-    """
-    out = subprocess.run(
-        code, shell=True, capture_output=True, text=True
-    ).stdout
-    return str(out)
-
-
-@tool
-def browser(query: str):
-    """
-    Search the query in the browser with the `browser` tool.
-
-    Args:
-        query (str): The query to search in the browser.
-
-    Returns:
-        str: The search results.
-    """
-    import webbrowser
-
-    url = f"https://www.google.com/search?q={query}"
-    webbrowser.open(url)
-    return f"Searching for {query} in the browser."
-
-@tool
-def create_file(file_path: str, content: str):
-    """
-    Create a file using the file editor tool.
-
-    Args:
-        file_path (str): The path to the file.
-        content (str): The content to write to the file.
-
-    Returns:
-        str: The result of the file creation operation.
-    """
-    with open(file_path, "w") as file:
-        file.write(content)
-    return f"File {file_path} created successfully."
-
-@tool
-def file_editor(file_path: str, mode: str, content: str):
-    """
-    Edit a file using the file editor tool.
-
-    Args:
-        file_path (str): The path to the file.
-        mode (str): The mode to open the file in.
-        content (str): The content to write to the file.
-
-    Returns:
-        str: The result of the file editing operation.
-    """
-    with open(file_path, mode) as file:
-        file.write(content)
-    return f"File {file_path} edited successfully."
-
-
-# Agent
-agent = Agent(
-    agent_name="Devin",
-    system_prompt=(
-        "Autonomous agent that can interact with humans and other"
-        " agents. Be Helpful and Kind. Use the tools provided to"
-        " assist the user. Return all code in markdown format."
-    ),
-    llm=llm,
-    max_loops="auto",
-    autosave=True,
-    dashboard=False,
-    streaming_on=True,
-    verbose=True,
-    stopping_token="<DONE>",
-    interactive=True,
-    tools=[terminal, browser, file_editor, create_file],
-    code_interpreter=True,
-    # streaming=True,
-)
-
-# Run the agent
-out = agent("Create a new file for a plan to take over the world.")
-print(out)
-```
-
-
-## `Agent`with Pydantic BaseModel as Output Type
-The following is an example of an agent that intakes a pydantic basemodel and outputs it at the same time:
-
-```python
-from pydantic import BaseModel, Field
-from swarms import AnthropicChat
-from swarms import Agent
-
-
-# Initialize the schema for the person's information
-class Schema(BaseModel):
-    name: str = Field(..., title="Name of the person")
-    agent: int = Field(..., title="Age of the person")
-    is_student: bool = Field(..., title="Whether the person is a student")
-    courses: list[str] = Field(
-        ..., title="List of courses the person is taking"
-    )
-
-
-# Convert the schema to a JSON string
-tool_schema = Schema(
-    name="Tool Name",
-    agent=1,
-    is_student=True,
-    courses=["Course1", "Course2"],
-)
-
-# Define the task to generate a person's information
-task = "Generate a person's information based on the following schema:"
-
-# Initialize the agent
-agent = Agent(
-    agent_name="Person Information Generator",
-    system_prompt=(
-        "Generate a person's information based on the following schema:"
-    ),
-    # Set the tool schema to the JSON string -- this is the key difference
-    tool_schema=tool_schema,
-    llm=AnthropicChat(),
-    max_loops=3,
-    autosave=True,
-    dashboard=False,
-    streaming_on=True,
-    verbose=True,
-    interactive=True,
-    # Set the output type to the tool schema which is a BaseModel
-    output_type=tool_schema,  # or dict, or str
-    metadata_output_type="json",
-    # List of schemas that the agent can handle
-    list_tool_schemas=[tool_schema],
-    function_calling_format_type="OpenAI",
-    function_calling_type="json",  # or soon yaml
-)
-
-# Run the agent to generate the person's information
-generated_data = agent.run(task)
-
-# Print the generated data
-print(f"Generated data: {generated_data}")
-
-
-```
 
 
 ### `SwarmNetwork`
 `SwarmNetwork` provides the infrasturcture for building extremely dense and complex multi-agent applications that span across various types of agents.
 
 ✅ Efficient Task Management: SwarmNetwork's intelligent agent pool and task queue management system ensures tasks are distributed evenly across agents. This leads to efficient use of resources and faster task completion.
 
@@ -915,18 +914,18 @@
 ```
 
 
 ## Majority Voting
 Multiple-agents will evaluate an idea based off of an parsing or evaluation function. From papers like "[More agents is all you need](https://arxiv.org/pdf/2402.05120.pdf)
 
 ```python
-from swarms import Agent, MajorityVoting, ChromaDB, AnthropicChat
+from swarms import Agent, MajorityVoting, ChromaDB, Anthropic
 
 # Initialize the llm
-llm = AnthropicChat()
+llm = Anthropic()
 
 # Agents
 agent1 = Agent(
     llm = llm,
     system_prompt="You are the leader of the Progressive Party. What is your stance on healthcare?",
     agent_name="Progressive Leader",
     agent_description="Leader of the Progressive Party",
@@ -1227,43 +1226,43 @@
 
 ```
 
 ## `AgentRearrange`
 Inspired by Einops and einsum, this orchestration techniques enables you to map out the relationships between various agents. For example you specify linear and sequential relationships like `a -> a1 -> a2 -> a3` or concurrent relationships where the first agent will send a message to 3 agents all at once: `a -> a1, a2, a3`. You can customize your workflow to mix sequential and concurrent relationships
 
 ```python
-from swarms import Agent, AnthropicChat, AgentRearrange, 
+from swarms import Agent, Anthropic, AgentRearrange, 
 
 ## Initialize the workflow
 agent = Agent(
     agent_name="t",
     agent_description=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
     system_prompt=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
-    llm=AnthropicChat(),
+    llm=Anthropic(),
     max_loops=1,
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
 )
 
 agent2 = Agent(
     agent_name="t1",
     agent_description=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
-    llm=AnthropicChat(),
+    llm=Anthropic(),
     max_loops=1,
     system_prompt="Summarize the transcript",
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
@@ -1271,15 +1270,15 @@
 
 agent3 = Agent(
     agent_name="t2",
     agent_description=(
         "Generate a transcript for a youtube video on what swarms"
         " are!"
     ),
-    llm=AnthropicChat(),
+    llm=Anthropic(),
     max_loops=1,
     system_prompt="Finalize the transcript",
     autosave=True,
     dashboard=False,
     streaming_on=True,
     verbose=True,
     stopping_token="<DONE>",
```

