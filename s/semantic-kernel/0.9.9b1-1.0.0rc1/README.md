# Comparing `tmp/semantic_kernel-0.9.9b1.tar.gz` & `tmp/semantic_kernel-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.9.9b1.tar", max compression
+gzip compressed data, was "semantic_kernel-1.0.0rc1.tar", max compression
```

## Comparing `semantic_kernel-0.9.9b1.tar` & `semantic_kernel-1.0.0rc1.tar`

### file list

```diff
@@ -1,232 +1,233 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-0.9.9b1/pip/README.md
--rw-r--r--   0        0        0     5410 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3250 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/function_call_behavior.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0    10535 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     4676 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     3118 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6683 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8451 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3983 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0     2464 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/contents/function_call.py
--rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    11081 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5364 2024-03-20 18:24:28.763758 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     6087 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     6075 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     3614 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    19750 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3719 2024-03-20 18:24:28.763758 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     3823 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6363 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3663 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0     2908 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/utils.py
--rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
--rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
--rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1741 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    13347 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0      735 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astradb_settings.py
--rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0     1160 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
--rw-r--r--   0        0        0    16963 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0    11118 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0      538 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
--rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      560 2024-05-16 18:28:06.371055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/memory_settings_base.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    13131 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0      518 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
--rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    15618 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0      460 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    21145 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      494 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/postgres_settings.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15880 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0      486 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/redis_settings.py
--rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    12496 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      908 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0     1268 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0    28989 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     3425 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/bing_connector_settings.py
--rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-0.9.9b1/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/const.py
--rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/author_role.py
--rw-r--r--   0        0        0    14167 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0    12594 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0     4032 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/function_call_content.py
--rw-r--r--   0        0        0     4509 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/function_result_content.py
--rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0    10964 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     2011 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/contents/types.py
--rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/README.md
--rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
--rw-r--r--   0        0        0     9954 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
--rw-r--r--   0        0        0     1919 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
--rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
--rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      316 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/events/__init__.py
--rw-r--r--   0        0        0     2068 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/events/function_invoked_event_args.py
--rw-r--r--   0        0        0     1420 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/events/function_invoking_event_args.py
--rw-r--r--   0        0        0     1725 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/events/kernel_events_args.py
--rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1176 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1319 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/memory_connector_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1750 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0     9648 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     6170 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0     8258 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    17761 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1991 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    24196 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      791 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    42096 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/kernel.py
--rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    11604 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5978 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4760 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      893 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4945 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     6785 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     5586 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4592 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2483 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     1894 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-0.9.9b1/semantic_kernel/py.typed
--rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-0.9.9b1/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7474 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      838 2024-05-16 18:28:06.381055 semantic_kernel-0.9.9b1/semantic_kernel/utils/experimental_decorator.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-0.9.9b1/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5104 1970-01-01 00:00:00.000000 semantic_kernel-0.9.9b1/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/pip/README.md
+-rw-r--r--   0        0        0     5411 2024-05-17 22:45:44.178248 semantic_kernel-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3250 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/function_call_behavior.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0    10535 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     4676 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     3118 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6683 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8451 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3983 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    11081 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5356 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     6087 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     6075 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     3614 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    23919 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3737 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     3823 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6363 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3663 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0     2908 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/utils.py
+-rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
+-rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
+-rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1741 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    13347 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0      735 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_settings.py
+-rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0     1160 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
+-rw-r--r--   0        0        0    16963 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    11118 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0      538 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
+-rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      560 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/memory_settings_base.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    13131 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0      518 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
+-rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    15618 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0      460 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    21145 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      494 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_settings.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15880 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0      486 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_settings.py
+-rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    12496 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      908 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0     1268 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0    28989 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     3425 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector_settings.py
+-rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/const.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    14167 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    12590 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     4032 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     4556 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0    10964 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     2011 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/README.md
+-rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
+-rw-r--r--   0        0        0     9954 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
+-rw-r--r--   0        0        0     1919 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
+-rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
+-rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/memory_connector_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
+-rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_context_base.py
+-rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_types.py
+-rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/functions/function_invocation_context.py
+-rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/prompts/prompt_render_context.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1750 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0    10657 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     6170 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0     7843 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    16893 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    24196 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      974 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    37221 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     6346 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/kernel_extensions/kernel_filters_extension.py
+-rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    12815 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5978 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4760 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      893 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4945 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     6744 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     5586 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4592 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2483 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     2069 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7474 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      838 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/utils/experimental_decorator.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     5105 1970-01-01 00:00:00.000000 semantic_kernel-1.0.0rc1/PKG-INFO
```

### Comparing `semantic_kernel-0.9.9b1/pip/README.md` & `semantic_kernel-1.0.0rc1/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/pyproject.toml` & `semantic_kernel-1.0.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.9.9b1"
+version = "1.0.0rc1"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/function_call_behavior.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/function_call_behavior.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from typing import Awaitable, Callable, Dict, Mapping, Optional, Union
 
 from openai import AsyncAzureOpenAI
-from pydantic import validate_call
+from pydantic import ConfigDict, validate_call
 
-from semantic_kernel.connectors.ai.open_ai.const import (
-    DEFAULT_AZURE_API_VERSION,
-    USER_AGENT,
-)
-from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
-    OpenAIHandler,
-    OpenAIModelTypes,
-)
+from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION, USER_AGENT
+from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler, OpenAIModelTypes
 from semantic_kernel.connectors.telemetry import APP_INFO, prepend_semantic_kernel_to_user_agent
 from semantic_kernel.exceptions import ServiceInitializationError
 from semantic_kernel.kernel_pydantic import HttpsUrl
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class AzureOpenAIConfigBase(OpenAIHandler):
     """Internal class for configuring a connection to an Azure OpenAI service."""
 
-    @validate_call(config=dict(arbitrary_types_allowed=True))
+    @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def __init__(
         self,
         deployment_name: str,
         ai_model_type: OpenAIModelTypes,
         endpoint: Optional[HttpsUrl] = None,
         base_url: Optional[HttpsUrl] = None,
         api_version: str = DEFAULT_AZURE_API_VERSION,
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import logging
 from copy import copy
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Optional, Tuple, Union
+from functools import reduce
+from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Optional, Union
 
 from openai import AsyncStream
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
-from semantic_kernel.connectors.ai.function_call_behavior import FunctionCallBehavior
-from semantic_kernel.connectors.ai.open_ai.contents.function_call import FunctionCall
+from semantic_kernel.connectors.ai.function_call_behavior import (
+    EnabledFunctions,
+    FunctionCallBehavior,
+    RequiredFunction,
+)
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
 from semantic_kernel.connectors.ai.open_ai.services.utils import update_settings_from_function_call_configuration
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.contents.author_role import AuthorRole
@@ -29,23 +33,34 @@
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import (
     FunctionCallInvalidArgumentsException,
     ServiceInvalidExecutionSettingsError,
     ServiceInvalidResponseError,
 )
-from semantic_kernel.utils.chat import store_results
+from semantic_kernel.filters.auto_function_invocation.auto_function_invocation_context import (
+    AutoFunctionInvocationContext,
+)
+from semantic_kernel.filters.filter_types import FilterTypes
+from semantic_kernel.functions.function_result import FunctionResult
+from semantic_kernel.kernel_extensions.kernel_filters_extension import _rebuild_auto_function_invocation_context
 
 if TYPE_CHECKING:
     from semantic_kernel.functions.kernel_arguments import KernelArguments
     from semantic_kernel.kernel import Kernel
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+class InvokeTermination(Exception):
+    """Exception for termination of function invocation."""
+
+    pass
+
+
 class OpenAIChatCompletionBase(OpenAIHandler, ChatCompletionClientBase):
     """OpenAI Chat completion class."""
 
     # region Overriding base class methods
     # most of the methods are overridden from the ChatCompletionClientBase class, otherwise it is mentioned
 
     # override from AIServiceClientBase
@@ -69,103 +84,164 @@
 
         Returns:
             List[ChatMessageContent] -- The completion result(s).
         """
 
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
-        if (
-            settings.function_call_behavior is not None
-            and settings.function_call_behavior.auto_invoke_kernel_functions
-            and (kernel is None or arguments is None)
-        ):
-            raise ServiceInvalidExecutionSettingsError(
-                "The kernel argument and arguments are required for auto invoking OpenAI tool calls."
-            )
+        if settings.function_call_behavior is not None and settings.function_call_behavior.auto_invoke_kernel_functions:
+            if kernel is None or arguments is None:
+                raise ServiceInvalidExecutionSettingsError(
+                    "The kernel and kernel arguments are required for auto invoking OpenAI tool calls."
+                )
+            if settings.number_of_responses > 1:
+                raise ServiceInvalidExecutionSettingsError(
+                    "Auto-invocation of tool calls may only be used with a "
+                    "OpenAIChatPromptExecutions.number_of_responses of 1."
+                )
+
         # behavior for non-function calling or for enable, but not auto-invoke.
-        settings = self._prepare_settings(settings, chat_history, stream_request=False, kernel=kernel)
+        self._prepare_settings(settings, chat_history, stream_request=False, kernel=kernel)
         if settings.function_call_behavior is None or (
             settings.function_call_behavior and not settings.function_call_behavior.auto_invoke_kernel_functions
         ):
             return await self._send_chat_request(settings)
 
         # loop for auto-invoke function calls
-        for _ in range(settings.function_call_behavior.max_auto_invoke_attempts):
+        for request_index in range(settings.function_call_behavior.max_auto_invoke_attempts):
             completions = await self._send_chat_request(settings)
-            if all(
-                not isinstance(item, FunctionCallContent) for completion in completions for item in completion.items
-            ):
+            # there is only one chat message, this was checked earlier
+            chat_history.add_message(message=completions[0])
+            # get the function call contents from the chat message
+            function_calls = [item for item in chat_history.messages[-1].items if isinstance(item, FunctionCallContent)]
+            if (fc_count := len(function_calls)) == 0:
                 return completions
-            await self._process_chat_response_with_tool_call(
-                completions=completions, chat_history=chat_history, kernel=kernel, arguments=arguments
+
+            logger.info(f"processing {fc_count} tool calls in parallel.")
+
+            # this function either updates the chat history with the function call results
+            # or returns the context, with terminate set to True
+            # in which case the loop will break and the function calls are returned.
+            results = await asyncio.gather(
+                *[
+                    self._process_function_call(
+                        function_call=function_call,
+                        chat_history=chat_history,
+                        kernel=kernel,
+                        arguments=arguments,
+                        function_call_count=fc_count,
+                        request_index=request_index,
+                        function_call_behavior=settings.function_call_behavior,
+                    )
+                    for function_call in function_calls
+                ],
             )
-            settings = self._prepare_settings(settings, chat_history, stream_request=False, kernel=kernel)
+
+            if any(result.terminate for result in results if result is not None):
+                return completions
+
+            self._update_settings(settings, chat_history, kernel=kernel)
+        else:
+            # do a final call, without function calling when the max has been reached.
+            settings.function_call_behavior.auto_invoke_kernel_functions = False
+            return await self._send_chat_request(settings)
 
     async def get_streaming_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
-    ) -> AsyncGenerator[List[StreamingChatMessageContent], Any]:
+    ) -> AsyncGenerator[List[StreamingChatMessageContent | None], Any]:
         """Executes a streaming chat completion request and returns the result.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to use for the chat completion.
             settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
                 for the chat completion request.
             kwargs {Dict[str, Any]} -- The optional arguments.
 
         Yields:
             List[StreamingChatMessageContent] -- A stream of
                 StreamingChatMessageContent when using Azure.
         """
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
-        if (
-            settings.function_call_behavior is not None
-            and settings.function_call_behavior.auto_invoke_kernel_functions
-            and (kernel is None or arguments is None)
-        ):
-            raise ServiceInvalidExecutionSettingsError(
-                "The kernel argument and arguments are required for OpenAI tool calling."
-            )
+        if settings.function_call_behavior is not None and settings.function_call_behavior.auto_invoke_kernel_functions:
+            if kernel is None or arguments is None:
+                raise ServiceInvalidExecutionSettingsError(
+                    "The kernel argument and arguments are required for OpenAI tool calling."
+                )
+            if settings.number_of_responses > 1:
+                raise ServiceInvalidExecutionSettingsError(
+                    "Auto-invocation of tool calls may only be used with a "
+                    "OpenAIChatPromptExecutions.number_of_responses of 1."
+                )
 
         # Prepare settings for streaming requests
-        settings = self._prepare_settings(settings, chat_history, stream_request=True, kernel=kernel)
+        self._prepare_settings(settings, chat_history, stream_request=True, kernel=kernel)
 
-        # Behavior for non-function calling or for enable, but not auto-invoke
-        if settings.function_call_behavior is None or (
-            settings.function_call_behavior and not settings.function_call_behavior.auto_invoke_kernel_functions
-        ):
-            async for content, _ in self._process_chat_stream_response(
-                response=await self._send_chat_stream_request(settings),
-                chat_history=chat_history,
-                kernel=kernel,
-                tool_call_behavior=None,  # type: ignore
-                arguments=arguments,
+        request_attempts = (
+            settings.function_call_behavior.max_auto_invoke_attempts if settings.function_call_behavior else 1
+        )
+        # hold the messages, if there are more than one response, it will not be used, so we flatten
+        for request_index in range(request_attempts):
+            all_messages: list[StreamingChatMessageContent] = []
+            function_call_returned = False
+            async for messages in self._send_chat_stream_request(settings):
+                for msg in messages:
+                    if msg is not None:
+                        all_messages.append(msg)
+                        if any(isinstance(item, FunctionCallContent) for item in msg.items):
+                            function_call_returned = True
+                yield messages
+
+            if (
+                settings.function_call_behavior is None
+                or (
+                    settings.function_call_behavior and not settings.function_call_behavior.auto_invoke_kernel_functions
+                )
+                or not function_call_returned
             ):
-                yield content
-            return
+                # no need to process function calls
+                # note that we don't check the FinishReason and instead check whether there are any tool calls,
+                # as the service may return a FinishReason of "stop" even if there are tool calls to be made,
+                # in particular if a required tool is specified.
+                return
+
+            # there is one response stream in the messages, combining now to create the full completion
+            full_completion: StreamingChatMessageContent = reduce(lambda x, y: x + y, all_messages)
+            chat_history.add_message(message=full_completion)
+
+            function_calls = [item for item in chat_history.messages[-1].items if isinstance(item, FunctionCallContent)]
+            fc_count = len(function_calls)
+
+            logger.info(f"processing {fc_count} tool calls in parallel.")
+
+            # this function either updates the chat history with the function call results
+            # or returns the context, with terminate set to True
+            # in which case the loop will break and the function calls are returned.
+            # Exceptions are not caught, that is up to the developer, can be done with a filter
+            results = await asyncio.gather(
+                *[
+                    self._process_function_call(
+                        function_call=function_call,
+                        chat_history=chat_history,
+                        kernel=kernel,
+                        arguments=arguments,
+                        function_call_count=fc_count,
+                        request_index=request_index,
+                        function_call_behavior=settings.function_call_behavior,
+                    )
+                    for function_call in function_calls
+                ],
+            )
+            if any(result.terminate for result in results if result is not None):
+                return
 
-        # Loop for auto-invoke function calls
-        for _ in range(settings.function_call_behavior.max_auto_invoke_attempts):
-            response = await self._send_chat_stream_request(settings)
-            finish_reason = None
-            async for content, finish_reason in self._process_chat_stream_response(
-                response=response,
-                chat_history=chat_history,
-                kernel=kernel,
-                tool_call_behavior=settings.function_call_behavior,  # type: ignore
-                arguments=arguments,
-            ):
-                if content:
-                    yield content
-            if finish_reason != FinishReason.TOOL_CALLS:
-                break
-            settings = self._prepare_settings(settings, chat_history, stream_request=True, kernel=kernel)
+            self._update_settings(settings, chat_history, kernel=kernel)
 
     def _chat_message_content_to_dict(self, message: "ChatMessageContent") -> Dict[str, Optional[str]]:
         msg = super()._chat_message_content_to_dict(message)
         if message.role == "assistant":
             if tool_calls := getattr(message, "tool_calls", None):
                 msg["tool_calls"] = [tool_call.model_dump() for tool_call in tool_calls]
             if function_call := getattr(message, "function_call", None):
@@ -185,74 +261,28 @@
         response = await self._send_request(request_settings=settings)
         response_metadata = self._get_metadata_from_chat_response(response)
         completions = [
             self._create_chat_message_content(response, choice, response_metadata) for choice in response.choices
         ]
         return completions
 
-    async def _send_chat_stream_request(self, settings: OpenAIChatPromptExecutionSettings) -> AsyncStream:
+    async def _send_chat_stream_request(
+        self, settings: OpenAIChatPromptExecutionSettings
+    ) -> AsyncGenerator[list["StreamingChatMessageContent | None"], None]:
         """Send the chat stream request"""
         response = await self._send_request(request_settings=settings)
         if not isinstance(response, AsyncStream):
             raise ServiceInvalidResponseError("Expected an AsyncStream[ChatCompletionChunk] response.")
-        return response
-
-    async def _process_chat_response_with_tool_call(
-        self,
-        completions: List["ChatMessageContent"],
-        chat_history: ChatHistory,
-        kernel: "Kernel",
-        arguments: "KernelArguments",
-    ) -> None:
-        """Process the completions in the chat response"""
-        for result in completions:
-            # An assistant message needs to be followed be a tool call response
-            chat_history = store_results(chat_history=chat_history, results=[result])
-            await self._process_tool_calls(result=result, kernel=kernel, chat_history=chat_history, arguments=arguments)
-
-    async def _process_chat_stream_response(
-        self,
-        response: AsyncStream,
-        chat_history: ChatHistory,
-        tool_call_behavior: FunctionCallBehavior,
-        kernel: Optional["Kernel"] = None,
-        arguments: Optional["KernelArguments"] = None,
-    ) -> AsyncGenerator[Tuple[List["StreamingChatMessageContent"], Optional["FinishReason"]], Any]:
-        """Process the chat stream response and handle tool calls if applicable."""
-        full_content = None
         async for chunk in response:
             if len(chunk.choices) == 0:
                 continue
-
             chunk_metadata = self._get_metadata_from_streaming_chat_response(chunk)
-            contents = [
+            yield [
                 self._create_streaming_chat_message_content(chunk, choice, chunk_metadata) for choice in chunk.choices
             ]
-            if not contents:
-                continue
-            if not tool_call_behavior or not tool_call_behavior.auto_invoke_kernel_functions:
-                yield contents, None
-                continue
-
-            full_content = contents[0] if full_content is None else full_content + contents[0]
-            finish_reason = getattr(full_content, "finish_reason", None)
-            if not any(isinstance(item, FunctionCallContent) for item in full_content.items) or finish_reason not in (
-                FinishReason.STOP,
-                FinishReason.TOOL_CALLS,
-                None,
-            ):
-                yield contents, finish_reason
-
-            if finish_reason == FinishReason.STOP:
-                tool_call_behavior.auto_invoke_kernel_functions = False
-                break
-            if finish_reason == FinishReason.TOOL_CALLS:
-                chat_history.add_message(message=full_content)
-                await self._process_tool_calls(full_content, kernel, chat_history, arguments)
-                yield None, finish_reason
 
     # endregion
     # region content creation
 
     def _create_chat_message_content(
         self, response: ChatCompletion, choice: Choice, response_metadata: Dict[str, Any]
     ) -> "ChatMessageContent":
@@ -358,83 +388,130 @@
 
     def _prepare_settings(
         self,
         settings: OpenAIChatPromptExecutionSettings,
         chat_history: ChatHistory,
         stream_request: bool = False,
         kernel: "Kernel | None" = None,
-    ) -> OpenAIChatPromptExecutionSettings:
+    ) -> None:
         """Prepare the prompt execution settings for the chat request."""
-        settings.messages = self._prepare_chat_history_for_request(chat_history)
         settings.stream = stream_request
         if not settings.ai_model_id:
             settings.ai_model_id = self.ai_model_id
+        self._update_settings(settings=settings, chat_history=chat_history, kernel=kernel)
 
+    def _update_settings(
+        self,
+        settings: OpenAIChatPromptExecutionSettings,
+        chat_history: ChatHistory,
+        kernel: "Kernel | None" = None,
+    ) -> None:
+        """Update the settings with the chat history."""
+        settings.messages = self._prepare_chat_history_for_request(chat_history)
         if settings.function_call_behavior and kernel:
             settings.function_call_behavior.configure(
                 kernel=kernel,
                 update_settings_callback=update_settings_from_function_call_configuration,
                 settings=settings,
             )
-        return settings
 
     # endregion
     # region tool calling
 
-    async def _process_tool_calls(
+    async def _process_function_call(
         self,
-        result: ChatMessageContent,
-        kernel: "Kernel",
+        function_call: FunctionCallContent,
         chat_history: ChatHistory,
-        arguments: "KernelArguments",
-    ) -> None:
-        """Processes the tool calls in parallel in the result and return it as part of the chat history."""
-        logger.info(f"processing {len(result.items)} tool calls in parallel.")
-        await asyncio.gather(
-            *[
-                self._process_tool_call(result=tc, kernel=kernel, chat_history=chat_history, arguments=arguments)
-                for tc in result.items
-            ]
-        )
-
-    async def _process_tool_call(
-        self,
-        result: ChatMessageContent,
         kernel: "Kernel",
-        chat_history: ChatHistory,
         arguments: "KernelArguments",
-    ) -> None:
-        """Processes the tool calls in the result and return it as part of the chat history."""
+        function_call_count: int,
+        request_index: int,
+        function_call_behavior: FunctionCallBehavior,
+    ) -> "AutoFunctionInvocationContext | None":
+        """Processes the tool calls in the result and update the chat history."""
         args_cloned = copy(arguments)
-        func: FunctionCall | None = result
-        if not func:
-            return
         try:
-            parsed_args = func.parse_arguments()
+            parsed_args = function_call.parse_arguments()
             if parsed_args:
                 args_cloned.update(parsed_args)
         except FunctionCallInvalidArgumentsException as exc:
-            logger.exception(f"Received invalid arguments for function {func.name}: {exc}. Trying tool call again.")
+            logger.exception(
+                f"Received invalid arguments for function {function_call.name}: {exc}. Trying tool call again."
+            )
             frc = FunctionResultContent.from_function_call_content_and_result(
-                function_call_content=result,
+                function_call_content=function_call,
                 result="The tool call arguments are malformed, please try again.",
             )
             chat_history.add_message(message=frc.to_chat_message_content())
             return
-        logger.info(f"Calling {func.name} function with args: {func.arguments}")
+
+        logger.info(f"Calling {function_call.name} function with args: {function_call.arguments}")
         try:
-            func_result = await kernel.invoke(**func.split_name_dict(), arguments=args_cloned)
+            if function_call.name is None:
+                raise ValueError("The function name is required.")
+            if isinstance(function_call_behavior, RequiredFunction):
+                if function_call.name != function_call_behavior.function_fully_qualified_name:
+                    raise ValueError(
+                        f"Only function: {function_call_behavior.function_fully_qualified_name} "
+                        f"is allowed, {function_call.name} is not allowed."
+                    )
+            if isinstance(function_call_behavior, EnabledFunctions):
+                enabled_functions = [
+                    func.fully_qualified_name
+                    for func in kernel.get_list_of_function_metadata(function_call_behavior.filters)
+                ]
+                if function_call.name not in enabled_functions:
+                    raise ValueError(
+                        f"Only functions: {enabled_functions} are allowed, {function_call.name} is not allowed."
+                    )
+            function_to_call = kernel.get_function(function_call.plugin_name, function_call.function_name)
         except Exception as exc:
-            logger.exception(f"Exception occurred while invoking function {func.name}, exception: {exc}")
+            logger.exception(f"Could not find function {function_call.name}: {exc}.")
             frc = FunctionResultContent.from_function_call_content_and_result(
-                function_call_content=result,
-                result=f"Exception occurred while invoking function {func.name}, exception: {exc}",
+                function_call_content=function_call,
+                result="The tool call could not be found, please try again and make sure to validate the name.",
             )
             chat_history.add_message(message=frc.to_chat_message_content())
             return
+
+        _rebuild_auto_function_invocation_context()
+        invocation_context = AutoFunctionInvocationContext(
+            function=function_to_call,
+            kernel=kernel,
+            arguments=args_cloned,
+            chat_history=chat_history,
+            function_result=FunctionResult(function=function_to_call.metadata, value=None),
+            function_count=function_call_count,
+            request_sequence_index=request_index,
+        )
+        if function_call.index is not None:
+            invocation_context.function_sequence_index = function_call.index
+
+        stack = kernel.construct_call_stack(
+            filter_type=FilterTypes.AUTO_FUNCTION_INVOCATION,
+            inner_function=self._inner_auto_function_invoke_handler,
+        )
+        await stack(invocation_context)
+
+        if invocation_context.terminate:
+            return invocation_context
+
         frc = FunctionResultContent.from_function_call_content_and_result(
-            function_call_content=result, result=func_result
+            function_call_content=function_call, result=invocation_context.function_result
         )
         chat_history.add_message(message=frc.to_chat_message_content())
 
+    async def _inner_auto_function_invoke_handler(self, context: AutoFunctionInvocationContext):
+        """Inner auto function invocation handler."""
+        try:
+            result = await context.function.invoke(context.kernel, context.arguments)
+            if result:
+                context.function_result = result
+        except Exception as exc:
+            logger.exception(f"Error invoking function {context.function.fully_qualified_name}: {exc}.")
+            value = f"An error occurred while invoking the function {context.function.fully_qualified_name}: {exc}"
+            assert context.function_result is not None
+            context.function_result.value = value
+            return
+
 
 # endregion
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from typing import Dict, Mapping, Optional
 
 from openai import AsyncOpenAI
-from pydantic import Field, validate_call
+from pydantic import ConfigDict, Field, validate_call
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_model_types import OpenAIModelTypes
 from semantic_kernel.connectors.telemetry import APP_INFO, prepend_semantic_kernel_to_user_agent
 from semantic_kernel.exceptions import ServiceInitializationError
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class OpenAIConfigBase(OpenAIHandler):
-    @validate_call(config=dict(arbitrary_types_allowed=True))
+    @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def __init__(
         self,
         ai_model_id: str = Field(min_length=1),
         api_key: Optional[str] = Field(min_length=1),
         ai_model_type: Optional[OpenAIModelTypes] = OpenAIModelTypes.CHAT,
         org_id: Optional[str] = None,
         service_id: Optional[str] = None,
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/services/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/astradb_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/memory_settings_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/memory_settings_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/bing_connector_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/telemetry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/document_loader.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_history.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_history.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_message_content.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,18 +254,18 @@
         if len(items) == 1 and isinstance(items[0], TextContent):
             kwargs["content"] = items[0].text
         elif all(isinstance(item, TextContent) for item in items):
             kwargs["content"] = "".join(item.text for item in items)  # type: ignore
         else:
             kwargs["items"] = items
         if "choice_index" in kwargs and cls is ChatMessageContent:
-            logger.warning(
+            logger.info(
                 "Seems like you are trying to create a StreamingChatMessageContent, "
                 "use StreamingChatMessageContent.from_element instead, ignoring that field "
-                " and creating a ChatMessageContent instance."
+                "and creating a ChatMessageContent instance."
             )
             kwargs.pop("choice_index")
         return cls(**kwargs)
 
     def to_prompt(self) -> str:
         """Convert the ChatMessageContent to a prompt.
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/function_call_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_call_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/function_result_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_result_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,16 @@
     def from_function_call_content_and_result(
         cls,
         function_call_content: "FunctionCallContent",
         result: "FunctionResult | TextContent | ChatMessageContent | Any",
         metadata: dict[str, Any] = {},
     ) -> "FunctionResultContent":
         """Create an instance from a FunctionCallContent and a result."""
-        metadata.update(function_call_content.metadata)
+        if function_call_content.metadata:
+            metadata.update(function_call_content.metadata)
         return cls(
             id=function_call_content.id,
             result=result,  # type: ignore
             name=function_call_content.name,
             ai_model_id=function_call_content.ai_model_id,
             metadata=metadata,
         )
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/kernel_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_content_mixin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/text_content.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/contents/types.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/contents/types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/http_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/math_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/time_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/wait_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/wait_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/function_exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,19 +39,24 @@
     pass
 
 
 class FunctionResultError(FunctionException):
     pass
 
 
+class PromptRenderingException(FunctionException):
+    pass
+
+
 __all__ = [
     "FunctionException",
     "FunctionInitializationError",
     "FunctionInvalidParamNameError",
     "FunctionInvalidNameError",
     "FunctionNameNotUniqueError",
     "FunctionSyntaxError",
     "PluginInitializationError",
     "PluginInvalidNameError",
     "FunctionExecutionException",
     "FunctionResultError",
+    "PromptRenderingException",
 ]
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,21 @@
     pass
 
 
 class KernelInvokeException(KernelException):
     pass
 
 
+class OperationCancelledException(KernelException):
+    pass
+
+
 __all__ = [
     "KernelException",
     "KernelFunctionAlreadyExistsError",
     "KernelFunctionNotFoundError",
     "KernelInvokeException",
     "KernelPluginNotFoundError",
     "KernelServiceNotFoundError",
     "KernelPluginInvalidConfigurationError",
+    "OperationCancelledException",
 ]
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/function_result.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/function_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_arguments.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod
 from collections.abc import AsyncGenerator
 from copy import copy, deepcopy
+from inspect import isasyncgen, isgenerator
 from typing import TYPE_CHECKING, Any, Callable
 
-from semantic_kernel.const import METADATA_EXCEPTION_KEY
+from semantic_kernel.filters.filter_types import FilterTypes
+from semantic_kernel.filters.functions.function_invocation_context import FunctionInvocationContext
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
+from semantic_kernel.kernel_extensions.kernel_filters_extension import _rebuild_function_invocation_context
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.prompt_template.const import (
     HANDLEBARS_TEMPLATE_FORMAT_NAME,
     JINJA2_TEMPLATE_FORMAT_NAME,
     KERNEL_TEMPLATE_FORMAT_NAME,
     TEMPLATE_FORMAT_TYPES,
 )
@@ -142,106 +145,124 @@
     def return_parameter(self) -> KernelParameterMetadata | None:
         return self.metadata.return_parameter
 
     async def __call__(
         self,
         kernel: Kernel,
         arguments: KernelArguments | None = None,
+        metadata: dict[str, Any] = {},
         **kwargs: Any,
-    ) -> FunctionResult:
+    ) -> FunctionResult | None:
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (Optional[KernelArguments]): The Kernel arguments.
                 Optional, defaults to None.
             kwargs (Dict[str, Any]): Additional keyword arguments that will be
 
         Returns:
             FunctionResult: The result of the function
         """
-        return await self.invoke(kernel, arguments, **kwargs)
+        return await self.invoke(kernel, arguments, metadata, **kwargs)
 
     @abstractmethod
-    async def _invoke_internal(
-        self,
-        kernel: Kernel,
-        arguments: KernelArguments,
-    ) -> FunctionResult:
+    async def _invoke_internal(self, context: FunctionInvocationContext) -> None:
+        """Internal invoke method of the the function with the given arguments.
+
+        This function should be implemented by the subclass.
+        It relies on updating the context with the result from the function.
+
+        Args:
+            context (FunctionInvocationContext): The invocation context.
+
+        """
         pass
 
     async def invoke(
         self,
         kernel: Kernel,
         arguments: KernelArguments | None = None,
+        metadata: dict[str, Any] = {},
         **kwargs: Any,
-    ) -> FunctionResult:
+    ) -> "FunctionResult | None":
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
             kwargs (Any): Additional keyword arguments that will be
                 added to the KernelArguments.
 
         Returns:
             FunctionResult: The result of the function
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
-        try:
-            return await self._invoke_internal(kernel, arguments)
-        except Exception as exc:
-            logger.error(f"Error occurred while invoking function {self.name}: {exc}")
-            return FunctionResult(
-                function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: exc, "arguments": arguments}
-            )
+        _rebuild_function_invocation_context()
+        function_context = FunctionInvocationContext(function=self, kernel=kernel, arguments=arguments)
+
+        stack = kernel.construct_call_stack(
+            filter_type=FilterTypes.FUNCTION_INVOCATION,
+            inner_function=self._invoke_internal,
+        )
+        await stack(function_context)
+
+        return function_context.result
 
     @abstractmethod
-    def _invoke_internal_stream(
-        self,
-        kernel: Kernel,
-        arguments: KernelArguments,
-    ) -> AsyncGenerator[FunctionResult | list[StreamingContentMixin | Any], Any]:
+    async def _invoke_internal_stream(self, context: FunctionInvocationContext) -> None:
         """Internal invoke method of the the function with the given arguments.
 
         The abstract method is defined without async because otherwise the typing fails.
         A implementation of this function should be async.
         """
         ...
 
     async def invoke_stream(
         self,
         kernel: Kernel,
         arguments: KernelArguments | None = None,
+        metadata: dict[str, Any] = {},
         **kwargs: Any,
     ) -> AsyncGenerator[FunctionResult | list[StreamingContentMixin | Any], Any]:
         """
         Invoke a stream async function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
             kwargs (Any): Additional keyword arguments that will be
                 added to the KernelArguments.
 
         Yields:
-            StreamingKernelContent or FunctionResult -- The results of the function,
+            KernelContent with the StreamingKernelMixin or FunctionResult --
+                The results of the function,
                 if there is an error a FunctionResult is yielded.
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
-        try:
-            async for partial_result in self._invoke_internal_stream(kernel, arguments):
-                yield partial_result
-        except Exception as e:
-            logger.error(f"Error occurred while invoking function {self.name}: {e}")
-            yield FunctionResult(
-                function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: e, "arguments": arguments}
-            )
+        _rebuild_function_invocation_context()
+        function_context = FunctionInvocationContext(function=self, kernel=kernel, arguments=arguments)
+
+        stack = kernel.construct_call_stack(
+            filter_type=FilterTypes.FUNCTION_INVOCATION,
+            inner_function=self._invoke_internal_stream,
+        )
+        await stack(function_context)
+
+        if function_context.result is not None:
+            if isasyncgen(function_context.result.value):
+                async for partial in function_context.result.value:
+                    yield partial
+            elif isgenerator(function_context.result.value):
+                for partial in function_context.result.value:
+                    yield partial
+            else:
+                yield function_context.result
 
     def function_copy(self, plugin_name: str | None = None) -> KernelFunction:
         """Copy the function, can also override the plugin_name.
 
         Args:
             plugin_name (str): The new plugin name.
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from inspect import isasyncgen, isasyncgenfunction, isawaitable, iscoroutinefunction, isgenerator, isgeneratorfunction
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable
+from typing import Any, Callable
 
 from pydantic import ValidationError
 
-from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
+from semantic_kernel.filters.functions.function_invocation_context import FunctionInvocationContext
 from semantic_kernel.functions.function_result import FunctionResult
-from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 
-if TYPE_CHECKING:
-    from semantic_kernel.kernel import Kernel
-
-
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class KernelFunctionFromMethod(KernelFunction):
     """Semantic Kernel Function from a method."""
 
     # some attributes are now properties, still listed here for documentation purposes
@@ -96,67 +91,57 @@
             ),
         }
 
         super().__init__(**args)
 
     async def _invoke_internal(
         self,
-        kernel: Kernel,
-        arguments: KernelArguments,
-    ) -> FunctionResult:
+        context: FunctionInvocationContext,
+    ) -> None:
         """Invoke the function with the given arguments."""
-        function_arguments = self.gather_function_parameters(kernel, arguments)
+        function_arguments = self.gather_function_parameters(context)
         result = self.method(**function_arguments)
         if isasyncgen(result):
             result = [x async for x in result]
         elif isawaitable(result):
             result = await result
         elif isgenerator(result):
             result = list(result)
-        if isinstance(result, FunctionResult):
-            return result
-        return FunctionResult(
-            function=self.metadata,
-            value=result,
-            metadata={"arguments": arguments, "used_arguments": function_arguments},
-        )
+        if not isinstance(result, FunctionResult):
+            result = FunctionResult(
+                function=self.metadata,
+                value=result,
+                metadata={"arguments": context.arguments, "used_arguments": function_arguments},
+            )
+        context.result = result
 
-    async def _invoke_internal_stream(
-        self,
-        kernel: Kernel,
-        arguments: KernelArguments,
-    ) -> AsyncGenerator[list[StreamingContentMixin] | Any, Any]:
+    async def _invoke_internal_stream(self, context: FunctionInvocationContext) -> None:
         if self.stream_method is None:
             raise NotImplementedError("Stream method not implemented")
-        function_arguments = self.gather_function_parameters(kernel, arguments)
-        if isasyncgenfunction(self.stream_method):
-            async for partial_result in self.stream_method(**function_arguments):
-                yield partial_result
-        elif isgeneratorfunction(self.stream_method):
-            for partial_result in self.stream_method(**function_arguments):
-                yield partial_result
+        function_arguments = self.gather_function_parameters(context)
+        context.result = FunctionResult(function=self.metadata, value=self.stream_method(**function_arguments))
 
-    def gather_function_parameters(self, kernel: Kernel, arguments: KernelArguments) -> dict[str, Any]:
+    def gather_function_parameters(self, context: FunctionInvocationContext) -> dict[str, Any]:
         """Gathers the function parameters from the arguments."""
         function_arguments: dict[str, Any] = {}
         for param in self.parameters:
             if param.name == "kernel":
-                function_arguments[param.name] = kernel
+                function_arguments[param.name] = context.kernel
                 continue
             if param.name == "service":
-                function_arguments[param.name] = kernel.select_ai_service(self, arguments)[0]
+                function_arguments[param.name] = context.kernel.select_ai_service(self, context.arguments)[0]
                 continue
             if param.name == "execution_settings":
-                function_arguments[param.name] = kernel.select_ai_service(self, arguments)[1]
+                function_arguments[param.name] = context.kernel.select_ai_service(self, context.arguments)[1]
                 continue
             if param.name == "arguments":
-                function_arguments[param.name] = arguments
+                function_arguments[param.name] = context.arguments
                 continue
-            if param.name in arguments:
-                value: Any = arguments[param.name]
+            if param.name in context.arguments:
+                value: Any = context.arguments[param.name]
                 if param.type_ and "," not in param.type_ and param.type_object:
                     if hasattr(param.type_object, "model_validate"):
                         try:
                             value = param.type_object.model_validate(value)
                         except Exception as exc:
                             raise FunctionExecutionException(
                                 f"Parameter {param.name} is expected to be parsed to {param.type_} but is not."
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 import os
 from html import unescape
-from typing import TYPE_CHECKING, Any, AsyncGenerator
+from typing import Any, AsyncGenerator
 
 import yaml
 from pydantic import Field, ValidationError, model_validator
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
-from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
-from semantic_kernel.contents.streaming_chat_message_content import StreamingChatMessageContent
-from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
-from semantic_kernel.contents.streaming_text_content import StreamingTextContent
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
+from semantic_kernel.exceptions.function_exceptions import PromptRenderingException
+from semantic_kernel.filters.filter_types import FilterTypes
+from semantic_kernel.filters.functions.function_invocation_context import FunctionInvocationContext
+from semantic_kernel.filters.prompts.prompt_render_context import PromptRenderContext
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import TEMPLATE_FORMAT_MAP, KernelFunction
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
+from semantic_kernel.functions.prompt_rendering_result import PromptRenderingResult
+from semantic_kernel.kernel_extensions.kernel_filters_extension import _rebuild_prompt_render_context
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME, TEMPLATE_FORMAT_TYPES
 from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 
-if TYPE_CHECKING:
-    from semantic_kernel.kernel import Kernel
-
 logger: logging.Logger = logging.getLogger(__name__)
 
 PROMPT_FILE_NAME = "skprompt.txt"
 CONFIG_FILE_NAME = "config.json"
 PROMPT_RETURN_PARAM = KernelParameterMetadata(
     name="return",
     description="The completion result",
@@ -99,25 +98,25 @@
             prompt_template = TEMPLATE_FORMAT_MAP[template_format](prompt_template_config=prompt_template_config)  # type: ignore
 
         try:
             metadata = KernelFunctionMetadata(
                 name=function_name,
                 plugin_name=plugin_name,
                 description=description,
-                parameters=prompt_template.prompt_template_config.get_kernel_parameter_metadata(),
+                parameters=prompt_template.prompt_template_config.get_kernel_parameter_metadata(),  # type: ignore
                 is_prompt=True,
                 is_asynchronous=True,
                 return_parameter=PROMPT_RETURN_PARAM,
             )
         except ValidationError as exc:
             raise FunctionInitializationError("Failed to create KernelFunctionMetadata") from exc
         super().__init__(
             metadata=metadata,
-            prompt_template=prompt_template,
-            prompt_execution_settings=prompt_execution_settings,
+            prompt_template=prompt_template,  # type: ignore
+            prompt_execution_settings=prompt_execution_settings or {},  # type: ignore
         )
 
     @model_validator(mode="before")
     @classmethod
     def rewrite_execution_settings(
         cls,
         data: dict[str, Any],
@@ -139,86 +138,116 @@
             data["prompt_execution_settings"] = {
                 prompt_execution_settings.service_id or "default": prompt_execution_settings
             }
         if isinstance(prompt_execution_settings, list):
             data["prompt_execution_settings"] = {s.service_id or "default": s for s in prompt_execution_settings}
         return data
 
-    async def _invoke_internal(
-        self,
-        kernel: Kernel,
-        arguments: KernelArguments,
-    ) -> FunctionResult:
+    async def _invoke_internal(self, context: FunctionInvocationContext) -> None:
         """Invokes the function with the given arguments."""
-        arguments = self.add_default_values(arguments)
-        service, execution_settings = kernel.select_ai_service(self, arguments)
-        prompt = await self.prompt_template.render(kernel, arguments)
-
-        if isinstance(service, ChatCompletionClientBase):
-            return await self._handle_complete_chat(
-                kernel=kernel,
-                service=service,
-                execution_settings=execution_settings,
-                prompt=prompt,
-                arguments=arguments,
+        prompt_render_result = await self._render_prompt(context)
+        if prompt_render_result.function_result is not None:
+            context.result = prompt_render_result.function_result
+            return
+
+        if isinstance(prompt_render_result.ai_service, ChatCompletionClientBase):
+            chat_history = ChatHistory.from_rendered_prompt(prompt_render_result.rendered_prompt)
+
+            # pass the kernel in for auto function calling
+            kwargs: dict[str, Any] = {}
+            if hasattr(prompt_render_result.execution_settings, "function_call_behavior"):
+                kwargs["kernel"] = context.kernel
+                kwargs["arguments"] = context.arguments
+
+            try:
+                chat_message_contents = await prompt_render_result.ai_service.get_chat_message_contents(
+                    chat_history=chat_history,
+                    settings=prompt_render_result.execution_settings,
+                    **kwargs,
+                )
+            except Exception as exc:
+                raise FunctionExecutionException(f"Error occurred while invoking function {self.name}: {exc}") from exc
+
+            if not chat_message_contents:
+                raise FunctionExecutionException(f"No completions returned while invoking function {self.name}")
+
+            context.result = self._create_function_result(
+                completions=chat_message_contents, chat_history=chat_history, arguments=context.arguments
             )
+            return
+
+        if isinstance(prompt_render_result.ai_service, TextCompletionClientBase):
+            try:
+                texts = await prompt_render_result.ai_service.get_text_contents(
+                    unescape(prompt_render_result.rendered_prompt), prompt_render_result.execution_settings
+                )
+            except Exception as exc:
+                raise FunctionExecutionException(f"Error occurred while invoking function {self.name}: {exc}") from exc
 
-        if isinstance(service, TextCompletionClientBase):
-            return await self._handle_text_complete(
-                service=service,
-                execution_settings=execution_settings,
-                prompt=prompt,
-                arguments=arguments,
+            context.result = self._create_function_result(
+                completions=texts, arguments=context.arguments, prompt=prompt_render_result.rendered_prompt
             )
+            return
 
-        raise ValueError(f"Service `{type(service).__name__}` is not a valid AI service")
+        raise ValueError(f"Service `{type(prompt_render_result.ai_service).__name__}` is not a valid AI service")
 
-    async def _handle_complete_chat(
-        self,
-        kernel: Kernel,
-        service: ChatCompletionClientBase,
-        execution_settings: PromptExecutionSettings,
-        prompt: str,
-        arguments: KernelArguments,
-    ) -> FunctionResult:
-        """Handles the chat service call."""
-        chat_history = ChatHistory.from_rendered_prompt(prompt)
+    async def _invoke_internal_stream(self, context: FunctionInvocationContext) -> None:
+        """Invokes the function stream with the given arguments."""
+        prompt_render_result = await self._render_prompt(context)
 
-        # pass the kernel in for auto function calling
-        kwargs: dict[str, Any] = {}
-        if hasattr(execution_settings, "function_call_behavior"):
-            kwargs["kernel"] = kernel
-            kwargs["arguments"] = arguments
+        if isinstance(prompt_render_result.ai_service, ChatCompletionClientBase):
+            # pass the kernel in for auto function calling
+            kwargs: dict[str, Any] = {}
+            if hasattr(prompt_render_result.execution_settings, "function_call_behavior"):
+                kwargs["kernel"] = context.kernel
+                kwargs["arguments"] = context.arguments
 
-        try:
-            completions = await service.get_chat_message_contents(
+            chat_history = ChatHistory.from_rendered_prompt(prompt_render_result.rendered_prompt)
+
+            value: AsyncGenerator = prompt_render_result.ai_service.get_streaming_chat_message_contents(
                 chat_history=chat_history,
-                settings=execution_settings,
+                settings=prompt_render_result.execution_settings,
                 **kwargs,
             )
-            if not completions:
-                raise FunctionExecutionException(f"No completions returned while invoking function {self.name}")
+        elif isinstance(prompt_render_result.ai_service, TextCompletionClientBase):
+            value = prompt_render_result.ai_service.get_streaming_text_contents(
+                prompt=prompt_render_result.rendered_prompt, settings=prompt_render_result.execution_settings
+            )
+        else:
+            raise FunctionExecutionException(
+                f"Service `{type(prompt_render_result.ai_service)}` is not a valid AI service"
+            )
 
-            return self._create_function_result(completions=completions, chat_history=chat_history, arguments=arguments)
-        except Exception as exc:
-            raise FunctionExecutionException(f"Error occurred while invoking function {self.name}: {exc}") from exc
+        context.result = FunctionResult(function=self.metadata, value=value)
 
-    async def _handle_text_complete(
-        self,
-        service: TextCompletionClientBase,
-        execution_settings: PromptExecutionSettings,
-        prompt: str,
-        arguments: KernelArguments,
-    ) -> FunctionResult:
-        """Handles the text service call."""
-        try:
-            completions = await service.get_text_contents(unescape(prompt), execution_settings)
-            return self._create_function_result(completions=completions, arguments=arguments, prompt=prompt)
-        except Exception as exc:
-            raise FunctionExecutionException(f"Error occurred while invoking function {self.name}: {exc}") from exc
+    async def _render_prompt(self, context: FunctionInvocationContext) -> PromptRenderingResult:
+        """Render the prompt and apply the prompt rendering filters."""
+        self.update_arguments_with_defaults(context.arguments)
+        service, execution_settings = context.kernel.select_ai_service(self, context.arguments)
+
+        _rebuild_prompt_render_context()
+        prompt_render_context = PromptRenderContext(function=self, kernel=context.kernel, arguments=context.arguments)
+
+        stack = context.kernel.construct_call_stack(
+            filter_type=FilterTypes.PROMPT_RENDERING,
+            inner_function=self._inner_render_prompt,
+        )
+        await stack(prompt_render_context)
+
+        if prompt_render_context.rendered_prompt is None:
+            raise PromptRenderingException("Prompt rendering failed, no rendered prompt was returned.")
+        return PromptRenderingResult(
+            rendered_prompt=prompt_render_context.rendered_prompt,
+            ai_service=service,
+            execution_settings=execution_settings,
+        )
+
+    async def _inner_render_prompt(self, context: PromptRenderContext) -> None:
+        """Render the prompt using the prompt template."""
+        context.rendered_prompt = await self.prompt_template.render(context.kernel, context.arguments)
 
     def _create_function_result(
         self,
         completions: list[ChatMessageContent] | list[TextContent],
         arguments: KernelArguments,
         chat_history: ChatHistory | None = None,
         prompt: str | None = None,
@@ -234,99 +263,19 @@
             metadata["prompt"] = prompt
         return FunctionResult(
             function=self.metadata,
             value=completions,
             metadata=metadata,
         )
 
-    async def _invoke_internal_stream(
-        self,
-        kernel: Kernel,
-        arguments: KernelArguments,
-    ) -> AsyncGenerator[FunctionResult | list[StreamingContentMixin], Any]:
-        """Invokes the function stream with the given arguments."""
-        arguments = self.add_default_values(arguments)
-        service, execution_settings = kernel.select_ai_service(self, arguments)
-        prompt = await self.prompt_template.render(kernel, arguments)
-
-        if isinstance(service, ChatCompletionClientBase):
-            async for content in self._handle_complete_chat_stream(
-                kernel=kernel,
-                service=service,
-                execution_settings=execution_settings,
-                prompt=prompt,
-                arguments=arguments,
-            ):
-                yield content  # type: ignore
-            return
-
-        if isinstance(service, TextCompletionClientBase):
-            async for content in self._handle_complete_text_stream(  # type: ignore
-                service=service,
-                execution_settings=execution_settings,
-                prompt=prompt,
-            ):
-                yield content  # type: ignore
-            return
-
-        raise FunctionExecutionException(f"Service `{type(service)}` is not a valid AI service")  # pragma: no cover
-
-    async def _handle_complete_chat_stream(
-        self,
-        kernel: Kernel,
-        service: ChatCompletionClientBase,
-        execution_settings: PromptExecutionSettings,
-        prompt: str,
-        arguments: KernelArguments,
-    ) -> AsyncGenerator[FunctionResult | list[StreamingChatMessageContent], Any]:
-        """Handles the chat service call."""
-
-        # pass the kernel in for auto function calling
-        kwargs: dict[str, Any] = {}
-        if hasattr(execution_settings, "function_call_behavior"):
-            kwargs["kernel"] = kernel
-            kwargs["arguments"] = arguments
-
-        chat_history = ChatHistory.from_rendered_prompt(prompt)
-        try:
-            async for partial_content in service.get_streaming_chat_message_contents(
-                chat_history=chat_history,
-                settings=execution_settings,
-                **kwargs,
-            ):
-                yield partial_content
-
-            return  # Exit after processing all iterations
-        except Exception as e:
-            logger.error(f"Error occurred while invoking function {self.name}: {e}")
-            yield FunctionResult(function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: e})
-
-    async def _handle_complete_text_stream(
-        self,
-        service: TextCompletionClientBase,
-        execution_settings: PromptExecutionSettings,
-        prompt: str,
-    ) -> AsyncGenerator[FunctionResult | list[StreamingTextContent], Any]:
-        """Handles the text service call."""
-        try:
-            async for partial_content in service.get_streaming_text_contents(
-                prompt=prompt, settings=execution_settings
-            ):
-                yield partial_content
-            return
-        except Exception as e:
-            logger.error(f"Error occurred while invoking function {self.name}: {e}")
-            yield FunctionResult(function=self.metadata, value=None, metadata={METADATA_EXCEPTION_KEY: e})
-
-    def add_default_values(self, arguments: KernelArguments) -> KernelArguments:
-        """Gathers the function parameters from the arguments."""
+    def update_arguments_with_defaults(self, arguments: KernelArguments) -> None:
+        """Update any missing values with their defaults."""
         for parameter in self.prompt_template.prompt_template_config.input_variables:
             if parameter.name not in arguments and parameter.default not in {None, "", False, 0}:
                 arguments[parameter.name] = parameter.default
-        return arguments
 
     @classmethod
     def from_yaml(cls, yaml_str: str, plugin_name: str | None = None) -> KernelFunctionFromPrompt:
         """Creates a new instance of the KernelFunctionFromPrompt class from a YAML string."""
         try:
             data = yaml.safe_load(yaml_str)
         except yaml.YAMLError as exc:  # pragma: no cover
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_parameter_metadata.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_parameter_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/kernel.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/kernel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # Copyright (c) Microsoft. All rights reserved.
 from __future__ import annotations
 
 import logging
 from copy import copy
 from functools import singledispatchmethod
-from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, Callable, Literal, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, AsyncGenerator, AsyncIterable, Literal, Type, TypeVar, Union
 
 from pydantic import Field, field_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.contents.streaming_content_mixin import StreamingContentMixin
-from semantic_kernel.events import FunctionInvokedEventArgs, FunctionInvokingEventArgs
 from semantic_kernel.exceptions import (
     KernelFunctionAlreadyExistsError,
     KernelFunctionNotFoundError,
     KernelInvokeException,
     KernelPluginNotFoundError,
     KernelServiceNotFoundError,
+    OperationCancelledException,
     ServiceInvalidTypeError,
     TemplateSyntaxError,
 )
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
+from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_plugin import KernelPlugin
-from semantic_kernel.kernel_pydantic import KernelBaseModel
+from semantic_kernel.kernel_extensions.kernel_filters_extension import KernelFilterExtension
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME, TEMPLATE_FORMAT_TYPES
 from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 from semantic_kernel.reliability.pass_through_without_retry import PassThroughWithoutRetry
 from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 from semantic_kernel.services.ai_service_selector import AIServiceSelector
@@ -45,21 +46,22 @@
         OpenAPIFunctionExecutionParameters,
     )
     from semantic_kernel.functions.kernel_function import KernelFunction
     from semantic_kernel.functions.types import KERNEL_FUNCTION_TYPE
 
 T = TypeVar("T")
 
+AI_SERVICE_CLIENT_TYPE = TypeVar("AI_SERVICE_CLIENT_TYPE", bound=AIServiceClientBase)
 ALL_SERVICE_TYPES = Union["TextCompletionClientBase", "ChatCompletionClientBase", "EmbeddingGeneratorBase"]
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
-class Kernel(KernelBaseModel):
+class Kernel(KernelFilterExtension):
     """
     The Kernel class is the main entry point for the Semantic Kernel. It provides the ability to run
     semantic/native functions, and manage plugins, memory, and AI services.
 
     Attributes:
         plugins (dict[str, KernelPlugin] | None): The plugins to be used by the kernel
         services (dict[str, AIServiceClientBase]): The services to be used by the kernel
@@ -70,25 +72,21 @@
 
     # region Init
 
     plugins: dict[str, KernelPlugin] = Field(default_factory=dict)
     services: dict[str, AIServiceClientBase] = Field(default_factory=dict)
     ai_service_selector: AIServiceSelector = Field(default_factory=AIServiceSelector)
     retry_mechanism: RetryMechanismBase = Field(default_factory=PassThroughWithoutRetry)
-    function_invoking_handlers: dict[
-        int, Callable[["Kernel", FunctionInvokingEventArgs], FunctionInvokingEventArgs]
-    ] = Field(default_factory=dict)
-    function_invoked_handlers: dict[int, Callable[["Kernel", FunctionInvokedEventArgs], FunctionInvokedEventArgs]] = (
-        Field(default_factory=dict)
-    )
 
     def __init__(
         self,
         plugins: KernelPlugin | dict[str, KernelPlugin] | list[KernelPlugin] | None = None,
-        services: AIServiceClientBase | list[AIServiceClientBase] | dict[str, AIServiceClientBase] | None = None,
+        services: (
+            AI_SERVICE_CLIENT_TYPE | list[AI_SERVICE_CLIENT_TYPE] | dict[str, AI_SERVICE_CLIENT_TYPE] | None
+        ) = None,
         ai_service_selector: AIServiceSelector | None = None,
         **kwargs: Any,
     ) -> None:
         """
         Initialize a new instance of the Kernel class.
 
         Args:
@@ -127,80 +125,67 @@
             return {p.name: p for p in plugins}
         return plugins
 
     @field_validator("services", mode="before")
     @classmethod
     def rewrite_services(
         cls,
-        services: AIServiceClientBase | list[AIServiceClientBase] | dict[str, AIServiceClientBase] | None = None,
-    ) -> dict[str, AIServiceClientBase]:
+        services: (
+            AI_SERVICE_CLIENT_TYPE | list[AI_SERVICE_CLIENT_TYPE] | dict[str, AI_SERVICE_CLIENT_TYPE] | None
+        ) = None,
+    ) -> dict[str, AI_SERVICE_CLIENT_TYPE]:
         """Rewrite services to a dictionary."""
         if not services:
             return {}
         if isinstance(services, AIServiceClientBase):
-            return {services.service_id or "default": services}
+            return {services.service_id if services.service_id else "default": services}  # type: ignore
         if isinstance(services, list):
-            return {s.service_id or "default": s for s in services}
+            return {s.service_id if s.service_id else "default": s for s in services}
         return services
 
     # endregion
     # region Invoke Functions
 
     async def invoke_stream(
         self,
         function: "KernelFunction" | None = None,
         arguments: KernelArguments | None = None,
         function_name: str | None = None,
         plugin_name: str | None = None,
-        return_function_results: bool | None = False,
+        metadata: dict[str, Any] = {},
+        return_function_results: bool = False,
         **kwargs: Any,
     ) -> AsyncGenerator[list["StreamingContentMixin"] | FunctionResult | list[FunctionResult], Any]:
         """Execute one or more stream functions.
 
         This will execute the functions in the order they are provided, if a list of functions is provided.
         When multiple functions are provided only the last one is streamed, the rest is executed as a pipeline.
 
         Arguments:
             functions (KernelFunction): The function or functions to execute,
             this value has precedence when supplying both this and using function_name and plugin_name,
             if this is none, function_name and plugin_name are used and cannot be None.
             arguments (KernelArguments): The arguments to pass to the function(s), optional
             function_name (str | None): The name of the function to execute
             plugin_name (str | None): The name of the plugin to execute
-            return_function_results (bool | None): If True, the function results are returned in addition to
-                the streaming content, otherwise only the streaming content is returned.
+            metadata (dict[str, Any]): The metadata to pass to the function(s)
+            return_function_results (bool): If True, the function results are yielded as a list[FunctionResult]
+            in addition to the streaming content, otherwise only the streaming content is yielded.
             kwargs (dict[str, Any]): arguments that can be used instead of supplying KernelArguments
 
         Yields:
             StreamingContentMixin: The content of the stream of the last function provided.
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
         if not function:
             if not function_name or not plugin_name:
                 raise KernelFunctionNotFoundError("No function(s) or function- and plugin-name provided")
             function = self.get_function(plugin_name, function_name)
 
-        function_invoking_args = self.on_function_invoking(function.metadata, arguments)
-        if function_invoking_args.is_cancel_requested:
-            logger.info(
-                f"Execution was cancelled on function invoking event of function: {function.fully_qualified_name}."
-            )
-            return
-        if function_invoking_args.updated_arguments:
-            logger.info(
-                "Arguments updated by function_invoking_handler in function, "
-                f"new arguments: {function_invoking_args.arguments}"
-            )
-            arguments = function_invoking_args.arguments
-        if function_invoking_args.is_skip_requested:
-            logger.info(
-                f"Execution was skipped on function invoking event of function: {function.fully_qualified_name}."
-            )
-            return
         function_result: list[list["StreamingContentMixin"] | Any] = []
 
         async for stream_message in function.invoke_stream(self, arguments):
             if isinstance(stream_message, FunctionResult) and (
                 exception := stream_message.metadata.get(METADATA_EXCEPTION_KEY, None)
             ):
                 raise KernelInvokeException(
@@ -223,95 +208,57 @@
 
     async def invoke(
         self,
         function: "KernelFunction" | None = None,
         arguments: KernelArguments | None = None,
         function_name: str | None = None,
         plugin_name: str | None = None,
+        metadata: dict[str, Any] = {},
         **kwargs: Any,
     ) -> FunctionResult | None:
         """Execute one or more functions.
 
         When multiple functions are passed the FunctionResult of each is put into a list.
 
         Arguments:
             function (KernelFunction): The function or functions to execute,
             this value has precedence when supplying both this and using function_name and plugin_name,
             if this is none, function_name and plugin_name are used and cannot be None.
             arguments (KernelArguments): The arguments to pass to the function(s), optional
             function_name (str | None): The name of the function to execute
             plugin_name (str | None): The name of the plugin to execute
+            metadata (dict[str, Any]): The metadata to pass to the function(s)
             kwargs (dict[str, Any]): arguments that can be used instead of supplying KernelArguments
 
         Returns:
             FunctionResult | list[FunctionResult] | None: The result of the function(s)
 
         """
         if arguments is None:
             arguments = KernelArguments(**kwargs)
         else:
             arguments.update(kwargs)
         if not function:
             if not function_name or not plugin_name:
-                raise KernelFunctionNotFoundError("No function or plugin name provided")
+                raise KernelFunctionNotFoundError("No function, or function name and plugin name provided")
             function = self.get_function(plugin_name, function_name)
-        function_invoking_args = self.on_function_invoking(function.metadata, arguments)
-        if function_invoking_args.is_cancel_requested:
-            logger.info(
-                f"Execution was cancelled on function invoking event of function: {function.fully_qualified_name}."
-            )
-            return None
-        if function_invoking_args.updated_arguments:
-            logger.info(
-                f"Arguments updated by function_invoking_handler, new arguments: {function_invoking_args.arguments}"
-            )
-            arguments = function_invoking_args.arguments
-        function_result = None
-        exception = None
+
         try:
-            function_result = await function.invoke(self, arguments)
+            return await function.invoke(kernel=self, arguments=arguments, metadata=metadata)
+        except OperationCancelledException as exc:
+            logger.info(f"Operation cancelled during function invocation. Message: {exc}")
+            return None
         except Exception as exc:
             logger.error(
                 "Something went wrong in function invocation. During function invocation:"
                 f" '{function.fully_qualified_name}'. Error description: '{str(exc)}'"
             )
-            exception = exc
-
-        # this allows a hook to alter the results before adding.
-        function_invoked_args = self.on_function_invoked(function.metadata, arguments, function_result, exception)
-        if function_invoked_args.exception:
             raise KernelInvokeException(
                 f"Error occurred while invoking function: '{function.fully_qualified_name}'"
-            ) from function_invoked_args.exception
-        if function_invoked_args.is_cancel_requested:
-            logger.info(
-                f"Execution was cancelled on function invoked event of function: {function.fully_qualified_name}."
-            )
-            return (
-                function_invoked_args.function_result
-                if function_invoked_args.function_result
-                else FunctionResult(function=function.metadata, value=None, metadata={})
-            )
-        if function_invoked_args.updated_arguments:
-            logger.info(
-                f"Arguments updated by function_invoked_handler in function {function.fully_qualified_name}"
-                ", new arguments: {function_invoked_args.arguments}"
-            )
-            arguments = function_invoked_args.arguments
-        if function_invoked_args.is_repeat_requested:
-            logger.info(
-                f"Execution was repeated on function invoked event of function: {function.fully_qualified_name}."
-            )
-            return await self.invoke(function=function, arguments=arguments)
-
-        return (
-            function_invoked_args.function_result
-            if function_invoked_args.function_result
-            else FunctionResult(function=function.metadata, value=None, metadata={})
-        )
+            ) from exc
 
     async def invoke_prompt(
         self,
         function_name: str,
         plugin_name: str,
         prompt: str,
         arguments: KernelArguments | None = None,
@@ -337,16 +284,14 @@
             FunctionResult | list[FunctionResult] | None: The result of the function(s)
         """
         if not arguments:
             arguments = KernelArguments(**kwargs)
         if not prompt:
             raise TemplateSyntaxError("The prompt is either null or empty.")
 
-        from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
-
         function = KernelFunctionFromPrompt(
             function_name=function_name,
             plugin_name=plugin_name,
             prompt=prompt,
             template_format=template_format,
         )
         return await self.invoke(function=function, arguments=arguments)
@@ -414,65 +359,14 @@
                     if len(output_function_result) <= choice.choice_index:
                         output_function_result.append(copy(choice))
                     else:
                         output_function_result[choice.choice_index] += choice
             yield FunctionResult(function=function.metadata, value=output_function_result)
 
     # endregion
-    # region Function Invoking/Invoked Events
-
-    def on_function_invoked(
-        self,
-        kernel_function_metadata: KernelFunctionMetadata,
-        arguments: KernelArguments,
-        function_result: FunctionResult | None = None,
-        exception: Exception | None = None,
-    ) -> FunctionInvokedEventArgs:
-        # TODO: include logic that uses function_result
-        args = FunctionInvokedEventArgs(
-            kernel_function_metadata=kernel_function_metadata,
-            arguments=arguments,
-            function_result=function_result,
-            exception=(
-                exception or function_result.metadata.get(METADATA_EXCEPTION_KEY, None) if function_result else None
-            ),
-        )
-        if self.function_invoked_handlers:
-            for handler in self.function_invoked_handlers.values():
-                handler(self, args)
-        return args
-
-    def on_function_invoking(
-        self, kernel_function_metadata: KernelFunctionMetadata, arguments: KernelArguments
-    ) -> FunctionInvokingEventArgs:
-        args = FunctionInvokingEventArgs(kernel_function_metadata=kernel_function_metadata, arguments=arguments)
-        if self.function_invoking_handlers:
-            for handler in self.function_invoking_handlers.values():
-                handler(self, args)
-        return args
-
-    def add_function_invoking_handler(
-        self, handler: Callable[["Kernel", FunctionInvokingEventArgs], FunctionInvokingEventArgs]
-    ) -> None:
-        self.function_invoking_handlers[id(handler)] = handler
-
-    def add_function_invoked_handler(
-        self, handler: Callable[["Kernel", FunctionInvokedEventArgs], FunctionInvokedEventArgs]
-    ) -> None:
-        self.function_invoked_handlers[id(handler)] = handler
-
-    def remove_function_invoking_handler(self, handler: Callable) -> None:
-        if id(handler) in self.function_invoking_handlers:
-            del self.function_invoking_handlers[id(handler)]
-
-    def remove_function_invoked_handler(self, handler: Callable) -> None:
-        if id(handler) in self.function_invoked_handlers:
-            del self.function_invoked_handlers[id(handler)]
-
-    # endregion
     # region Plugins & Functions
 
     def add_plugin(
         self,
         plugin: KernelPlugin | object | dict[str, Any] | None = None,
         plugin_name: str | None = None,
         parent_directory: str | None = None,
@@ -891,16 +785,16 @@
             raise KernelServiceNotFoundError(f"No service found of type {type}")
         if not (service := self.services.get(service_id)):
             raise KernelServiceNotFoundError(f"Service with service_id '{service_id}' does not exist")
         if type and not isinstance(service, type):
             raise ServiceInvalidTypeError(f"Service with service_id '{service_id}' is not of type {type}")
         return service
 
-    def get_services_by_type(self, type: Type[ALL_SERVICE_TYPES]) -> dict[str, "AIServiceClientBase"]:
-        return {service.service_id: service for service in self.services.values() if isinstance(service, type)}
+    def get_services_by_type(self, type: type[ALL_SERVICE_TYPES]) -> dict[str, ALL_SERVICE_TYPES]:
+        return {service.service_id: service for service in self.services.values() if isinstance(service, type)}  # type: ignore
 
     def get_prompt_execution_settings_from_service_id(
         self, service_id: str, type: Type[ALL_SERVICE_TYPES] | None = None
     ) -> PromptExecutionSettings:
         """Get the specific request settings from the service, instantiated with the service_id and ai_model_id."""
         service = self.get_service(service_id, type=type)
         return service.instantiate_prompt_execution_settings(
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/kernel_pydantic.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/kernel_pydantic.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_record.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/memory/null_memory.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     OpenAIChatPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.azure_chat_completion import AzureChatCompletion
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion import OpenAIChatCompletion
 from semantic_kernel.connectors.ai.open_ai.services.utils import kernel_function_metadata_to_openai_tool_format
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.function_call_content import FunctionCallContent
+from semantic_kernel.contents.function_result_content import FunctionResultContent
+from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions.planner_exceptions import PlannerInvalidConfigurationError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.planners.function_calling_stepwise_planner.function_calling_stepwise_planner_options import (
     FunctionCallingStepwisePlannerOptions,
@@ -111,15 +113,15 @@
         if not question:
             raise PlannerInvalidConfigurationError("Input question cannot be empty")
 
         if not arguments:
             arguments = KernelArguments(**kwargs)
 
         try:
-            chat_completion = kernel.get_service(service_id=self.service_id)
+            chat_completion: OpenAIChatCompletion | AzureChatCompletion = kernel.get_service(service_id=self.service_id)
         except Exception as exc:
             raise PlannerInvalidConfigurationError(
                 f"The OpenAI service `{self.service_id}` is not available. Please configure the AI service."
             ) from exc
 
         if not isinstance(chat_completion, (OpenAIChatCompletion, AzureChatCompletion)):
             raise PlannerInvalidConfigurationError(
@@ -178,21 +180,39 @@
                 args = function_call_content.parse_arguments()
                 return FunctionCallingStepwisePlannerResult(
                     final_answer=args.get("answer", ""),
                     chat_history=chat_history_for_steps,
                     iterations=i + 1,
                 )
 
-            try:
-                await chat_completion._process_tool_calls(
-                    result=chat_result, kernel=cloned_kernel, chat_history=chat_history_for_steps, arguments=arguments
-                )
-            except Exception as exc:
-                chat_history_for_steps.add_user_message(f"An error occurred during planner invocation: {exc}")
-                continue
+            for content in chat_result.items:
+                if not isinstance(content, FunctionCallContent):
+                    continue
+                try:
+                    context = await chat_completion._process_function_call(
+                        function_call=content,
+                        result=chat_result,
+                        kernel=cloned_kernel,
+                        chat_history=chat_history_for_steps,
+                        arguments=arguments,
+                        function_call_count=1,
+                        request_index=0,
+                        function_call_behavior=prompt_execution_settings.function_call_behavior,
+                    )
+                    frc = FunctionResultContent.from_function_call_content_and_result(
+                        function_call_content=content, result=context.function_result
+                    )
+                    chat_history_for_steps.add_message(message=frc.to_chat_message_content())
+                except Exception as exc:
+                    frc = FunctionResultContent.from_function_call_content_and_result(
+                        function_call_content=content,
+                        result=TextContent(text=f"An error occurred during planner invocation: {exc}"),
+                    )
+                    chat_history_for_steps.add_message(message=frc.to_chat_message_content())
+                    continue
 
         # We're done, but the model hasn't returned a final answer.
         return FunctionCallingStepwisePlannerResult(
             final_answer="",
             chat_history=chat_history_for_steps,
             iterations=i + 1,
         )
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/plan.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/plan.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/planner_options.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_options.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/const.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/const.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/input_variable.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/input_variable.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from html import escape
 from typing import TYPE_CHECKING, Any, List, Optional
 
 from pydantic import PrivateAttr, field_validator
 
-from semantic_kernel.exceptions import CodeBlockRenderException, TemplateRenderException
+from semantic_kernel.exceptions import TemplateRenderException
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME
 from semantic_kernel.prompt_template.input_variable import InputVariable
 from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.template_tokenizer import TemplateTokenizer
@@ -130,14 +130,14 @@
         for block in blocks:
             if isinstance(block, TextRenderer):
                 rendered_blocks.append(block.render(kernel, arguments))
                 continue
             if isinstance(block, CodeRenderer):
                 try:
                     rendered = await block.render_code(kernel, arguments)
-                except CodeBlockRenderException as exc:
+                except Exception as exc:
                     logger.error(f"Error rendering code block: {exc}")
                     raise TemplateRenderException(f"Error rendering code block: {exc}") from exc
                 rendered_blocks.append(rendered if allow_unsafe_function_output else escape(rendered))
         prompt = "".join(rendered_blocks)
         logger.debug(f"Rendered prompt: {prompt}")
         return prompt
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import asyncio
 import logging
 from html import escape
 from typing import TYPE_CHECKING, Any, Callable, Literal
 
 import nest_asyncio
 
+from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import HANDLEBARS_TEMPLATE_FORMAT_NAME
 
 if TYPE_CHECKING:
-    from semantic_kernel.functions.kernel_arguments import KernelArguments
     from semantic_kernel.functions.kernel_function import KernelFunction
     from semantic_kernel.kernel import Kernel
 
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
@@ -26,15 +26,18 @@
     allow_dangerously_set_content: bool = False,
 ) -> Callable[..., Any]:
     """Create a helper function for both the Handlebars and Jinja2 templating engines from a kernel function."""
     if not getattr(asyncio, "_nest_patched", False):
         nest_asyncio.apply()
 
     def func(*args, **kwargs):
-        arguments = base_arguments.copy()
+        arguments = KernelArguments()
+        if base_arguments and base_arguments.execution_settings:
+            arguments.execution_settings = base_arguments.execution_settings
+        arguments.update(base_arguments)
         arguments.update(kwargs)
 
         if len(args) > 0 and template_format == HANDLEBARS_TEMPLATE_FORMAT_NAME:
             this = args[0]
             actual_args = args[1:]
         else:
             this = None
```

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_selector.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/README.md` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/text/function_extension.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/text/text_chunker.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/utils/experimental_decorator.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/experimental_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/utils/naming.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/utils/null_logger.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/null_logger.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/semantic_kernel/utils/validation.py` & `semantic_kernel-1.0.0rc1/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.9.9b1/PKG-INFO` & `semantic_kernel-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.9.9b1
+Version: 1.0.0rc1
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

