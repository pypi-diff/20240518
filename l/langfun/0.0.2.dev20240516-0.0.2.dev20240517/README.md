# Comparing `tmp/langfun-0.0.2.dev20240516.tar.gz` & `tmp/langfun-0.0.2.dev20240517.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240516.tar", last modified: Thu May 16 08:03:28 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240517.tar", last modified: Fri May 17 08:04:30 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240516.tar` & `langfun-0.0.2.dev20240517.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.902238 langfun-0.0.2.dev20240516/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.910238 langfun-0.0.2.dev20240516/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.910238 langfun-0.0.2.dev20240516/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.910238 langfun-0.0.2.dev20240516/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.914238 langfun-0.0.2.dev20240516/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.914238 langfun-0.0.2.dev20240516/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.914238 langfun-0.0.2.dev20240516/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.918238 langfun-0.0.2.dev20240516/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.918238 langfun-0.0.2.dev20240516/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.450535 langfun-0.0.2.dev20240517/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-17 08:04:30.450535 langfun-0.0.2.dev20240517/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.430535 langfun-0.0.2.dev20240517/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.438535 langfun-0.0.2.dev20240517/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.438535 langfun-0.0.2.dev20240517/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.438535 langfun-0.0.2.dev20240517/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.442535 langfun-0.0.2.dev20240517/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.442535 langfun-0.0.2.dev20240517/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.442535 langfun-0.0.2.dev20240517/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.442535 langfun-0.0.2.dev20240517/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.446535 langfun-0.0.2.dev20240517/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.446535 langfun-0.0.2.dev20240517/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.450535 langfun-0.0.2.dev20240517/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:04:30.450535 langfun-0.0.2.dev20240517/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-17 08:04:30.000000 langfun-0.0.2.dev20240517/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-17 08:04:30.000000 langfun-0.0.2.dev20240517/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:04:30.000000 langfun-0.0.2.dev20240517/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-17 08:04:30.000000 langfun-0.0.2.dev20240517/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 08:04:30.000000 langfun-0.0.2.dev20240517/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:04:30.450535 langfun-0.0.2.dev20240517/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-17 08:03:47.000000 langfun-0.0.2.dev20240517/setup.py
```

### Comparing `langfun-0.0.2.dev20240516/LICENSE` & `langfun-0.0.2.dev20240517/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/PKG-INFO` & `langfun-0.0.2.dev20240517/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240516
+Version: 0.0.2.dev20240517
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240516/README.md` & `langfun-0.0.2.dev20240517/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/__init__.py` & `langfun-0.0.2.dev20240517/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240517/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/component.py` & `langfun-0.0.2.dev20240517/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/component_test.py` & `langfun-0.0.2.dev20240517/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240517/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240517/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/console.py` & `langfun-0.0.2.dev20240517/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/console_test.py` & `langfun-0.0.2.dev20240517/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240517/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240517/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240517/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/language_model.py` & `langfun-0.0.2.dev20240517/langfun/core/language_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -562,20 +562,27 @@
         str(response) + '\n',
         title=f'\n[{call_counter}] LM RESPONSE{title_suffix}:',
         color='blue',
     )
 
   def score(
       self,
-      prompt: str | message_lib.Message,
+      prompt: str | message_lib.Message | list[message_lib.Message],
       completions: list[str | message_lib.Message],
       **kwargs,
   ) -> list[LMScoringResult]:
     """Scores the given prompt."""
-    prompt = message_lib.UserMessage.from_value(prompt)
+    if isinstance(prompt, list):
+      if len(prompt) != len(completions):
+        raise ValueError(
+            'prompt and completions must have the same length.'
+        )
+      prompt = [message_lib.UserMessage.from_value(p) for p in prompt]
+    else:
+      prompt = message_lib.UserMessage.from_value(prompt)
     completions = [message_lib.UserMessage.from_value(c) for c in completions]
 
     call_counter = self._call_counter
     self._call_counter += 1
     request_start = time.time()
 
     with component.context(override_attrs=True, **kwargs):
@@ -583,24 +590,25 @@
       elapse = time.time() - request_start
       self._debug_score(
           prompt, completions, scoring_results, call_counter, elapse
       )
       return scoring_results
 
   def _score(
-      self, prompt: message_lib.Message, completions: list[message_lib.Message]
+      self, prompt: message_lib.Message | list[message_lib.Message],
+      completions: list[message_lib.Message]
   ) -> list[LMScoringResult]:
     """Subclass to implement."""
     raise NotImplementedError(
         f'{self.__class__.__name__} does not support scoring.'
     )
 
   def _debug_score(
       self,
-      prompt: message_lib.Message,
+      prompt: message_lib.Message | list[message_lib.Message],
       completions: list[message_lib.Message],
       scoring_results: list[LMScoringResult],
       call_counter: int,
       elapse: float,
   ):
     debug = self.debug
     if isinstance(debug, bool):
@@ -611,23 +619,27 @@
 
     if debug & LMDebugMode.PROMPT:
       console.write(
           prompt,
           title=f'\n[{call_counter}] SCORING LM WITH PROMPT:',
           color='green',
       )
-      referred_modalities = prompt.referred_modalities()
-      if referred_modalities:
-        console.write(
-            pg.object_utils.kvlist_str(
-                [(k, repr(v), None) for k, v in referred_modalities.items()]
-            ),
-            title=f'\n[{call_counter}] MODALITY OBJECTS SENT TO LM:',
-            color='green',
-        )
+      if isinstance(prompt, list):
+        referred_modalities_lst = [p.referred_modalities() for p in prompt]
+      else:
+        referred_modalities_lst = [prompt.referred_modalities(),]
+      if referred_modalities_lst:
+        for referred_modalities in referred_modalities_lst:
+          console.write(
+              pg.object_utils.kvlist_str(
+                  [(k, repr(v), None) for k, v in referred_modalities.items()]
+              ),
+              title=f'\n[{call_counter}] MODALITY OBJECTS SENT TO LM:',
+              color='green',
+          )
 
     if debug & LMDebugMode.RESPONSE:
       console.write(
           '',
           title=(
               f'\n[{call_counter}] SCORING COMPLETED (in {elapse:.2f} seconds):'
           ),
```

### Comparing `langfun-0.0.2.dev20240516/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240517/langfun/core/language_model_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     )(prompts)
 
 
 class MockScoringModel(MockModel):
 
   def _score(
       self,
-      prompt: message_lib.Message,
+      prompt: message_lib.Message | list[message_lib.Message],
       completions: list[message_lib.Message],
       **kwargs
   ) -> list[lm_lib.LMScoringResult]:
     return [
         lm_lib.LMScoringResult(score=-i * 1.0) for i in range(len(completions))
     ]
 
@@ -504,14 +504,25 @@
                 ['1', '2'], debug=debug_mode),
             [
                 lm_lib.LMScoringResult(score=-0.0),
                 lm_lib.LMScoringResult(score=-1.0),
             ],
         )
 
+        self.assertEqual(
+            lm.score(
+                [message_lib.UserMessage('hi {{image}}', image=Image()),
+                 message_lib.UserMessage('hi {{image}}', image=Image())],
+                ['1', '2'], debug=debug_mode),
+            [
+                lm_lib.LMScoringResult(score=-0.0),
+                lm_lib.LMScoringResult(score=-1.0),
+            ],
+        )
+
       debug_info = string_io.getvalue()
       expected_included = [
           debug_prints[f]
           for f in lm_lib.LMDebugMode
           if f != lm_lib.LMDebugMode.NONE and f in debug_mode
       ]
       expected_excluded = [
@@ -524,14 +535,18 @@
         self.assertIn('[0] ' + expected_include, debug_info)
       for expected_exclude in expected_excluded:
         self.assertNotIn('[0] ' + expected_exclude, debug_info)
 
       if debug_mode & lm_lib.LMDebugMode.PROMPT:
         self.assertIn('[0] MODALITY OBJECTS SENT TO LM', debug_info)
 
+  def test_score_with_unmatched_prompt_and_completions(self):
+    with self.assertRaises(ValueError):
+      MockScoringModel().score(['hi',], ['1', '2', '3'])
+
   def test_score_with_unsupported_model(self):
     with self.assertRaises(NotImplementedError):
       MockModel().score('hi', ['1', '2'])
 
   def test_rate_to_max_concurrency_no_rpm_no_tpm(self) -> None:
     lm = MockModel()
     self.assertEqual(
```

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from typing import Annotated
 import langfun.core as lf
 
 
 class Fake(lf.LanguageModel):
   """The base class for all fake language models."""
 
-  def _score(self, prompt: lf.Message, completions: list[lf.Message]):
+  def _score(self, prompt: lf.Message| list[lf.Message],
+             completions: list[lf.Message]):
     return [lf.LMScoringResult(score=-i * 1.0) for i in range(len(completions))]
 
   def _sample(self, prompts: list[lf.Message]) -> list[lf.LMSamplingResult]:
     results = []
     for prompt in prompts:
       response = self._response_from(prompt)
       results.append(
```

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/vertexai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240517/langfun/core/llms/vertexai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240517/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240517/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/memory.py` & `langfun-0.0.2.dev20240517/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/message.py` & `langfun-0.0.2.dev20240517/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/message_test.py` & `langfun-0.0.2.dev20240517/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240517/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240517/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240517/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240517/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240517/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240517/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modality.py` & `langfun-0.0.2.dev20240517/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240517/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240517/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240517/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/sampling.py` & `langfun-0.0.2.dev20240517/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240517/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/scoring.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from langfun.core.structured import mapping
 from langfun.core.structured import prompting
 from langfun.core.structured import schema as schema_lib
 import pyglove as pg
 
 
 def score(
-    prompt: Union[str, pg.Symbolic],
+    prompt: Union[str, pg.Symbolic] | list[str | pg.Symbolic],
     completions: list[str | pg.Symbolic],
     schema: Union[
         schema_lib.Schema, Type[Any], list[Type[Any]], dict[str, Any], None
     ] = None,
     *,
     lm: lf.LanguageModel | None = None,
     examples: list[mapping.MappingExample] | None = None,
@@ -45,23 +45,35 @@
         schema = type(c)
       elif schema is not type(c):
         raise ValueError(
             '`schema` cannot be inferred from completions of different types: '
             f'{[type(c) for c in completions]}.'
         )
 
-  input_message = prompting.query(
-      prompt,
-      schema,
-      examples=examples,
-      protocol=protocol,
-      skip_lm=True,
-      returns_message=True,
-      **kwargs,
-  )
+  if isinstance(prompt, list):
+    prompts = []
+    for p in prompt:
+      prompts.append(
+          prompting.query_prompt(
+              p,
+              schema,
+              examples=examples,
+              protocol=protocol,
+              **kwargs,
+          )
+      )
+    input_message = prompts
+  else:
+    input_message = prompting.query_prompt(
+        prompt,
+        schema,
+        examples=examples,
+        protocol=protocol,
+        **kwargs,
+    )
   if lm is None:
     lm_override = lf.get_contextual_override('lm')
     if lm_override is None:
       raise ValueError('`lm` must be specified or provided from `lf.context`.')
     lm = lm_override.value
 
   results = lm.score(
```

### Comparing `langfun-0.0.2.dev20240516/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240517/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/subscription.py` & `langfun-0.0.2.dev20240517/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240517/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/template.py` & `langfun-0.0.2.dev20240517/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/template_test.py` & `langfun-0.0.2.dev20240517/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240517/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240517/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240517/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240517/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240516
+Version: 0.0.2.dev20240517
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240516/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240517/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240516/setup.py` & `langfun-0.0.2.dev20240517/setup.py`

 * *Files identical despite different names*

