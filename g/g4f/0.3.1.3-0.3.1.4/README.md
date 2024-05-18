# Comparing `tmp/g4f-0.3.1.3.tar.gz` & `tmp/g4f-0.3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.1.3.tar", last modified: Fri May 17 16:45:40 2024, max compression
+gzip compressed data, was "g4f-0.3.1.4.tar", last modified: Sat May 18 14:55:18 2024, max compression
```

## Comparing `g4f-0.3.1.3.tar` & `g4f-0.3.1.4.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.800188 g4f-0.3.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-17 16:45:36.000000 g4f-0.3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-17 16:45:36.000000 g4f-0.3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-17 16:45:40.796188 g4f-0.3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    52480 2024-05-17 16:45:36.000000 g4f-0.3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.756188 g4f-0.3.1.3/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.764188 g4f-0.3.1.3/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.768188 g4f-0.3.1.3/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.772188 g4f-0.3.1.3/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.772188 g4f-0.3.1.3/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.776188 g4f-0.3.1.3/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/PerplexityApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.776188 g4f-0.3.1.3/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.752188 g4f-0.3.1.3/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/css/dracula.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.788188 g4f-0.3.1.3/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.788188 g4f-0.3.1.3/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    48500 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.788188 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 16:45:40.800188 g4f-0.3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-17 16:45:36.000000 g4f-0.3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.084169 g4f-0.3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-18 14:55:14.000000 g4f-0.3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-18 14:55:14.000000 g4f-0.3.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-18 14:55:18.084169 g4f-0.3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52480 2024-05-18 14:55:14.000000 g4f-0.3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.040169 g4f-0.3.1.4/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.052169 g4f-0.3.1.4/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.052169 g4f-0.3.1.4/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.060169 g4f-0.3.1.4/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.060169 g4f-0.3.1.4/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.060169 g4f-0.3.1.4/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34879 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/PerplexityApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5620 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.064170 g4f-0.3.1.4/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.068169 g4f-0.3.1.4/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.036169 g4f-0.3.1.4/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/css/dracula.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    48500 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.072169 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.076170 g4f-0.3.1.4/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.080170 g4f-0.3.1.4/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-18 14:55:14.000000 g4f-0.3.1.4/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 14:55:18.080170 g4f-0.3.1.4/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 14:55:18.000000 g4f-0.3.1.4/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 14:55:18.084169 g4f-0.3.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-18 14:55:14.000000 g4f-0.3.1.4/setup.py
```

### Comparing `g4f-0.3.1.3/LICENSE` & `g4f-0.3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/PKG-INFO` & `g4f-0.3.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.3 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.4 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.1.3/README.md` & `g4f-0.3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Aichatos.py` & `g4f-0.3.1.4/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Aura.py` & `g4f-0.3.1.4/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Bing.py` & `g4f-0.3.1.4/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/BingCreateImages.py` & `g4f-0.3.1.4/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Blackbox.py` & `g4f-0.3.1.4/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/ChatForAi.py` & `g4f-0.3.1.4/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.1.4/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/ChatgptAi.py` & `g4f-0.3.1.4/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/ChatgptFree.py` & `g4f-0.3.1.4/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/ChatgptNext.py` & `g4f-0.3.1.4/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/ChatgptX.py` & `g4f-0.3.1.4/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Cnote.py` & `g4f-0.3.1.4/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Cohere.py` & `g4f-0.3.1.4/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/DeepInfra.py` & `g4f-0.3.1.4/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.1.4/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.1.4/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Ecosia.py` & `g4f-0.3.1.4/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Feedough.py` & `g4f-0.3.1.4/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/FlowGpt.py` & `g4f-0.3.1.4/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.1.4/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/FreeGpt.py` & `g4f-0.3.1.4/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/GeminiPro.py` & `g4f-0.3.1.4/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/GeminiProChat.py` & `g4f-0.3.1.4/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/GigaChat.py` & `g4f-0.3.1.4/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/GptTalkRu.py` & `g4f-0.3.1.4/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/HuggingChat.py` & `g4f-0.3.1.4/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/HuggingFace.py` & `g4f-0.3.1.4/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Koala.py` & `g4f-0.3.1.4/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Liaobots.py` & `g4f-0.3.1.4/g4f/Provider/Liaobots.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 
 from ..typing import AsyncResult, Messages
 from .base_provider import AsyncGeneratorProvider, ProviderModelMixin
 from .helper import get_connector
 from ..requests import raise_for_status
 
 models = {
+    "gpt-4o": {
+        "context": "8K",
+        "id": "gpt-4o-free",
+        "maxLength": 31200,
+        "model": "ChatGPT",
+        "name": "GPT-4o-free",
+        "provider": "OpenAI",
+        "tokenLimit": 7800,
+    },
     "gpt-3.5-turbo": {
         "id": "gpt-3.5-turbo",
         "name": "GPT-3.5-Turbo",
         "maxLength": 48000,
         "tokenLimit": 14000,
         "context": "16K",
     },
@@ -91,15 +100,15 @@
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     default_model = "gpt-3.5-turbo"
     models = list(models)
     model_aliases = {
         "claude-v2": "claude-2"
     }
-    _auth_code = None
+    _auth_code = ""
     _cookie_jar = None
 
     @classmethod
     async def create_async_generator(
         cls,
         model: str,
         messages: Messages,
@@ -116,43 +125,67 @@
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
         }
         async with ClientSession(
             headers=headers,
             cookie_jar=cls._cookie_jar,
             connector=get_connector(connector, proxy, True)
         ) as session:
-            cls._auth_code = auth if isinstance(auth, str) else cls._auth_code
+            data = {
+                "conversationId": str(uuid.uuid4()),
+                "model": models[cls.get_model(model)],
+                "messages": messages,
+                "key": "",
+                "prompt": kwargs.get("system_message", "You are a helpful assistant."),
+            }
             if not cls._auth_code:
                 async with session.post(
                     "https://liaobots.work/recaptcha/api/login",
                     data={"token": "abcdefghijklmnopqrst"},
                     verify_ssl=False
                 ) as response:
                     await raise_for_status(response)
+            try:
                 async with session.post(
                     "https://liaobots.work/api/user",
-                    json={"authcode": ""},
+                    json={"authcode": cls._auth_code},
                     verify_ssl=False
                 ) as response:
                     await raise_for_status(response)
                     cls._auth_code = (await response.json(content_type=None))["authCode"]
+                    if not cls._auth_code:
+                        raise RuntimeError("Empty auth code")
                     cls._cookie_jar = session.cookie_jar
-
-            data = {
-                "conversationId": str(uuid.uuid4()),
-                "model": models[cls.get_model(model)],
-                "messages": messages,
-                "key": "",
-                "prompt": kwargs.get("system_message", "You are a helpful assistant."),
-            }
-            async with session.post(
-                "https://liaobots.work/api/chat",
-                json=data,
-                headers={"x-auth-code": cls._auth_code},
-                verify_ssl=False
-            ) as response:
-                await raise_for_status(response)
-                async for chunk in response.content.iter_any():
-                    if b"<html coupert-item=" in chunk:
-                        raise RuntimeError("Invalid session")
-                    if chunk:
-                        yield chunk.decode(errors="ignore")
+                async with session.post(
+                    "https://liaobots.work/api/chat",
+                    json=data,
+                    headers={"x-auth-code": cls._auth_code},
+                    verify_ssl=False
+                ) as response:
+                    await raise_for_status(response)
+                    async for chunk in response.content.iter_any():
+                        if b"<html coupert-item=" in chunk:
+                            raise RuntimeError("Invalid session")
+                        if chunk:
+                            yield chunk.decode(errors="ignore")
+            except:
+                async with session.post(
+                    "https://liaobots.work/api/user",
+                    json={"authcode": "pTIQr4FTnVRfr"},
+                    verify_ssl=False
+                ) as response:
+                    await raise_for_status(response)
+                    cls._auth_code = (await response.json(content_type=None))["authCode"]
+                    if not cls._auth_code:
+                        raise RuntimeError("Empty auth code")
+                    cls._cookie_jar = session.cookie_jar
+                async with session.post(
+                    "https://liaobots.work/api/chat",
+                    json=data,
+                    headers={"x-auth-code": cls._auth_code},
+                    verify_ssl=False
+                ) as response:
+                    await raise_for_status(response)
+                    async for chunk in response.content.iter_any():
+                        if b"<html coupert-item=" in chunk:
+                            raise RuntimeError("Invalid session")
+                        if chunk:
+                            yield chunk.decode(errors="ignore")
```

### Comparing `g4f-0.3.1.3/g4f/Provider/Llama.py` & `g4f-0.3.1.4/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Local.py` & `g4f-0.3.1.4/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/MetaAI.py` & `g4f-0.3.1.4/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.1.4/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Ollama.py` & `g4f-0.3.1.4/g4f/Provider/Ollama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.1.4/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Pi.py` & `g4f-0.3.1.4/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Reka.py` & `g4f-0.3.1.4/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Replicate.py` & `g4f-0.3.1.4/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/ReplicateImage.py` & `g4f-0.3.1.4/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/Vercel.py` & `g4f-0.3.1.4/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.1.4/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/You.py` & `g4f-0.3.1.4/g4f/Provider/You.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/__init__.py` & `g4f-0.3.1.4/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/bing/conversation.py` & `g4f-0.3.1.4/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/bing/create_images.py` & `g4f-0.3.1.4/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/bing/upload_image.py` & `g4f-0.3.1.4/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/V50.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.1.4/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.1.4/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/Gemini.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import os
 import json
 import random
 import re
+import base64
 
 from aiohttp import ClientSession, BaseConnector
 
 from ..helper import get_connector
 
 try:
     from selenium.webdriver.common.by import By
@@ -18,15 +19,15 @@
 
 from ... import debug
 from ...typing import Messages, Cookies, ImageType, AsyncResult, AsyncIterator
 from ..base_provider import AsyncGeneratorProvider
 from ..helper import format_prompt, get_cookies
 from ...requests.raise_for_status import raise_for_status
 from ...errors import MissingAuthError, MissingRequirementsError
-from ...image import to_bytes, to_data_uri, ImageResponse
+from ...image import to_bytes, ImageResponse, ImageDataResponse
 from ...webdriver import get_browser, get_driver_cookies
 
 REQUEST_HEADERS = {
     "authority": "gemini.google.com",
     "origin": "https://gemini.google.com",
     "referer": "https://gemini.google.com/",
     'user-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36',
@@ -118,14 +119,15 @@
         messages: Messages,
         proxy: str = None,
         api_key: str = None,
         cookies: Cookies = None,
         connector: BaseConnector = None,
         image: ImageType = None,
         image_name: str = None,
+        response_format: str = None,
         **kwargs
     ) -> AsyncResult:
         prompt = format_prompt(messages)
         if api_key is not None:
             if cookies is None:
                 cookies = {}
             cookies["__Secure-1PSID"] = api_key
@@ -188,30 +190,30 @@
                         image_prompt = match.group(1)
                         content = content.replace(match.group(0), '')
 
                     yield content
                     if image_prompt:
                         images = [image[0][3][3] for image in response_part[4][0][12][7][0]]
                         resolved_images = []
-                        preview = []
-                        for image in images:
-                            async with client.get(image, allow_redirects=False) as fetch:
-                                image = fetch.headers["location"]
-                            async with client.get(image, allow_redirects=False) as fetch:
-                                image = fetch.headers["location"]
-                            resolved_images.append(image)
-                            preview.append(image.replace('=s512', '=s200'))
-                            # preview_url = image.replace('=s512', '=s200')
-                            # async with client.get(preview_url) as fetch:
-                            #     preview_data = to_data_uri(await fetch.content.read())
-                            # async with client.get(image) as fetch:
-                            #     data = to_data_uri(await fetch.content.read())
-                            # preview.append(preview_data)
-                            # resolved_images.append(data)
-                        yield ImageResponse(resolved_images, image_prompt, {"orginal_links": images, "preview": preview})
+                        if response_format == "b64_json":
+                            for image in images:
+                                async with client.get(image) as response:
+                                    data = base64.b64encode(await response.content.read()).decode()
+                                resolved_images.append(data)
+                            yield ImageDataResponse(resolved_images, image_prompt)
+                        else:
+                            preview = []
+                            for image in images:
+                                async with client.get(image, allow_redirects=False) as fetch:
+                                    image = fetch.headers["location"]
+                                async with client.get(image, allow_redirects=False) as fetch:
+                                    image = fetch.headers["location"]
+                                resolved_images.append(image)
+                                preview.append(image.replace('=s512', '=s200'))
+                            yield ImageResponse(resolved_images, image_prompt, {"orginal_links": images, "preview": preview})
 
     def build_request(
         prompt: str,
         conversation_id: str = "",
         response_id: str = "",
         choice_id: str = "",
         image_url: str = None,
```

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     working = True
     supports_gpt_35_turbo = True
     supports_gpt_4 = True
     supports_message_history = True
     supports_system_message = True
     default_model = None
     default_vision_model = "gpt-4o"
-    models = ["gpt-3.5-turbo", "gpt-4", "gpt-4-gizmo", "gpt-4o"]
+    models = ["gpt-3.5-turbo", "gpt-4", "gpt-4-gizmo", "gpt-4o", "auto"]
     model_aliases = {
         "text-davinci-002-render-sha": "gpt-3.5-turbo",
         "": "gpt-3.5-turbo",
         "gpt-4-turbo-preview": "gpt-4",
         "dall-e": "gpt-4",
     }
     _api_key: str = None
@@ -326,14 +326,15 @@
         action: str = "next",
         conversation_id: str = None,
         conversation: Conversation = None,
         parent_id: str = None,
         image: ImageType = None,
         image_name: str = None,
         return_conversation: bool = False,
+        max_retries: int = 3,
         **kwargs
     ) -> AsyncResult:
         """
         Create an asynchronous generator for the conversation.
 
         Args:
             model (str): The model name.
@@ -390,59 +391,29 @@
                     api_key = cls._api_key = None
                     cls._create_request_args()
                     if debug.logging:
                         print("OpenaiChat: Load default model failed")
                         print(f"{e.__class__.__name__}: {e}")
 
             arkose_token = None
+            proofTokens = None
             if cls.default_model is None:
                 error = None
                 try:
-                    arkose_token, api_key, cookies, headers = await getArkoseAndAccessToken(proxy)
+                    arkose_token, api_key, cookies, headers, proofTokens = await getArkoseAndAccessToken(proxy)
                     cls._create_request_args(cookies, headers)
                     cls._set_api_key(api_key)
                 except NoValidHarFileError as e:
                     error = e
                 if cls._api_key is None:
                     await cls.nodriver_access_token(proxy)
                 if cls._api_key is None and cls.needs_auth:
                     raise error
                 cls.default_model = cls.get_model(await cls.get_default_model(session, cls._headers))
 
-            async with session.post(
-                f"{cls.url}/backend-anon/sentinel/chat-requirements"
-                if cls._api_key is None else
-                f"{cls.url}/backend-api/sentinel/chat-requirements",
-                json={"conversation_mode_kind": "primary_assistant"},
-                headers=cls._headers
-            ) as response:
-                cls._update_request_args(session)
-                await raise_for_status(response)
-                data = await response.json()
-                blob = data["arkose"]["dx"]
-                need_arkose = data["arkose"]["required"]
-                chat_token = data["token"]
-                proofofwork = ""
-                if "proofofwork" in data:
-                    proofofwork = generate_proof_token(**data["proofofwork"], user_agent=cls._headers["user-agent"])
-
-            if need_arkose and arkose_token is None:
-                arkose_token, api_key, cookies, headers = await getArkoseAndAccessToken(proxy)
-                cls._create_request_args(cookies, headers)
-                cls._set_api_key(api_key)
-                if arkose_token is None:
-                    raise MissingAuthError("No arkose token found in .har file")
-                            
-            if debug.logging:
-                print(
-                    'Arkose:', False if not need_arkose else arkose_token[:12]+"...",
-                    'Turnstile:', data["turnstile"]["required"],
-                    'Proofofwork:', False if proofofwork is None else proofofwork[:12]+"...",
-                )
-
             try:
                 image_request = await cls.upload_image(session, cls._headers, image, image_name) if image else None
             except Exception as e:
                 image_request = None
                 if debug.logging:
                     print("OpenaiChat: Upload image failed")
                     print(f"{e.__class__.__name__}: {e}")
@@ -453,14 +424,51 @@
                 conversation = Conversation(conversation_id, str(uuid.uuid4()) if parent_id is None else parent_id)
             else:
                 conversation = copy(conversation)
             if cls._api_key is None:
                 auto_continue = False
             conversation.finish_reason = None
             while conversation.finish_reason is None:
+                async with session.post(
+                    f"{cls.url}/backend-anon/sentinel/chat-requirements"
+                    if cls._api_key is None else
+                    f"{cls.url}/backend-api/sentinel/chat-requirements",
+                    json={"p": generate_proof_token(True, user_agent=cls._headers["user-agent"], proofTokens=proofTokens)},
+                    headers=cls._headers
+                ) as response:
+                    cls._update_request_args(session)
+                    await raise_for_status(response)
+                    requirements = await response.json()
+                    need_arkose = requirements.get("arkose", {}).get("required")
+                    chat_token = requirements["token"]        
+
+                if need_arkose and arkose_token is None:
+                    arkose_token, api_key, cookies, headers, proofTokens = await getArkoseAndAccessToken(proxy)
+                    cls._create_request_args(cookies, headers)
+                    cls._set_api_key(api_key)
+                    if arkose_token is None:
+                        raise MissingAuthError("No arkose token found in .har file")
+
+                if "proofofwork" in requirements:
+                    proofofwork = generate_proof_token(
+                        **requirements["proofofwork"],
+                        user_agent=cls._headers["user-agent"],
+                        proofTokens=proofTokens
+                    )           
+                if debug.logging:
+                    print(
+                        'Arkose:', False if not need_arkose else arkose_token[:12]+"...",
+                        'Proofofwork:', False if proofofwork is None else proofofwork[:12]+"...",
+                    )
+                ws = None
+                if need_arkose:
+                    async with session.post("https://chatgpt.com/backend-api/register-websocket", headers=cls._headers) as response:
+                        wss_url = (await response.json()).get("wss_url")
+                    if wss_url:
+                        ws = await session.ws_connect(wss_url)    
                 websocket_request_id = str(uuid.uuid4())
                 data = {
                     "action": action,
                     "conversation_mode": {"kind": "primary_assistant"},
                     "force_paragen": False,
                     "force_rate_limit": False,
                     "conversation_id": conversation.conversation_id,
@@ -484,16 +492,22 @@
                 async with session.post(
                     f"{cls.url}/backend-anon/conversation" if cls._api_key is None else
                     f"{cls.url}/backend-api/conversation",
                     json=data,
                     headers=headers
                 ) as response:
                     cls._update_request_args(session)
+                    if response.status == 403 and max_retries > 0:
+                        max_retries -= 1
+                        if debug.logging:
+                            print(f"Retry: Error {response.status}: {await response.text()}")
+                        await asyncio.sleep(5)
+                        continue
                     await raise_for_status(response)
-                    async for chunk in cls.iter_messages_chunk(response.iter_lines(), session, conversation):
+                    async for chunk in cls.iter_messages_chunk(response.iter_lines(), session, conversation, ws):
                         if return_conversation:
                             history_disabled = False
                             return_conversation = False
                             yield conversation
                         yield chunk
                 if auto_continue and conversation.finish_reason == "max_tokens":
                     conversation.finish_reason = None
@@ -515,21 +529,22 @@
                 yield base64.b64decode(message["body"])
 
     @classmethod
     async def iter_messages_chunk(
         cls,
         messages: AsyncIterator,
         session: StreamSession,
-        fields: Conversation
+        fields: Conversation,
+        ws = None
     ) -> AsyncIterator:
         last_message: int = 0
         async for message in messages:
             if message.startswith(b'{"wss_url":'):
                 message = json.loads(message)
-                ws = await session.ws_connect(message["wss_url"])
+                ws = await session.ws_connect(message["wss_url"]) if ws is None else ws
                 try:
                     async for chunk in cls.iter_messages_chunk(
                         cls.iter_messages_ws(ws, message["conversation_id"], hasattr(ws, "recv")),
                         session, fields
                     ):
                         yield chunk
                 finally:
```

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/PerplexityApi.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/PerplexityApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.1.4/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.1.4/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.1.4/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.1.4/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.1.4/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.1.4/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.1.4/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.1.4/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.1.4/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.1.4/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.1.4/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.1.4/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.1.4/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.1.4/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/npm/package-lock.json` & `g4f-0.3.1.4/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/openai/crypt.py` & `g4f-0.3.1.4/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/openai/har_file.py` & `g4f-0.3.1.4/g4f/Provider/openai/har_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import uuid
 import random
 from urllib.parse import unquote
 from copy import deepcopy
 
 from .crypt import decrypt, encrypt
 from ...requests import StreamSession
+from ... import debug
 
 class NoValidHarFileError(Exception):
     ...
 
 class arkReq:
     def __init__(self, arkURL, arkBx, arkHeader, arkBody, arkCookies, userAgent):
         self.arkURL = arkURL
@@ -27,16 +28,18 @@
 
 arkPreURL = "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147"
 sessionUrl = "https://chatgpt.com/api/auth/session"
 chatArk: arkReq = None
 accessToken: str = None
 cookies: dict = None
 headers: dict = None
+proofTokens: list = []
 
 def readHAR():
+    global proofTokens
     dirPath = "./"
     harPath = []
     chatArks = []
     accessToken = None
     cookies = {}
     for root, dirs, files in os.walk(dirPath):
         for file in files:
@@ -50,23 +53,32 @@
         with open(path, 'rb') as file:
             try:
                 harFile = json.loads(file.read())
             except json.JSONDecodeError:
                 # Error: not a HAR file!
                 continue
             for v in harFile['log']['entries']:
+                v_headers = get_headers(v)
+                try:
+                    if "openai-sentinel-proof-token" in v_headers:
+                        proofTokens.append(json.loads(base64.b64decode(
+                            v_headers["openai-sentinel-proof-token"].split("gAAAAAB", 1)[-1].encode()
+                        ).decode()))
+                except Exception as e:
+                    if debug.logging:
+                        print(f"Read proof token: {e}")
                 if arkPreURL in v['request']['url']:
                     chatArks.append(parseHAREntry(v))
                 elif v['request']['url'] == sessionUrl:
                     try:
                         accessToken = json.loads(v["response"]["content"]["text"]).get("accessToken")
                     except KeyError:
                         continue
-                    cookies = {c['name']: c['value'] for c in v['request']['cookies']}
-                    headers = get_headers(v)
+                    cookies = {c['name']: c['value'] for c in v['request']['cookies'] if c['name'] != "oai-did"}
+                    headers = v_headers
     if not accessToken:
         raise NoValidHarFileError("No accessToken found in .har files")
     if not chatArks:
         return None, accessToken, cookies, headers
     return chatArks.pop(), accessToken, cookies, headers
 
 def get_headers(entry) -> dict:
@@ -97,15 +109,16 @@
     tmpArk.arkBody['rnd'] = str(random.random())
     tmpArk.arkHeader['x-ark-esync-value'] = bw
     return tmpArk
 
 async def sendRequest(tmpArk: arkReq, proxy: str = None):
     async with StreamSession(headers=tmpArk.arkHeader, cookies=tmpArk.arkCookies, proxies={"https": proxy}) as session:
         async with session.post(tmpArk.arkURL, data=tmpArk.arkBody) as response:
-            arkose = (await response.json()).get("token")
+            data = await response.json()
+            arkose = data.get("token")
     if "sup=1|rid=" not in arkose:
         return RuntimeError("No valid arkose token generated")
     return arkose
 
 def getBDA(arkReq: arkReq):
     bx = arkReq.arkBx
     
@@ -127,14 +140,14 @@
     return str(bt - (bt % 21600))
 
 def getN() -> str:
     timestamp = str(int(time.time()))
     return base64.b64encode(timestamp.encode()).decode()
 
 async def getArkoseAndAccessToken(proxy: str) -> tuple[str, str, dict, dict]:
-    global chatArk, accessToken, cookies, headers
+    global chatArk, accessToken, cookies, headers, proofTokens
     if chatArk is None or accessToken is None:
         chatArk, accessToken, cookies, headers = readHAR()
     if chatArk is None:
-        return None, accessToken, cookies, headers
+        return None, accessToken, cookies, headers, proofTokens
     newReq = genArkReq(chatArk)
-    return await sendRequest(newReq, proxy), accessToken, cookies, headers
+    return await sendRequest(newReq, proxy), accessToken, cookies, headers, proofTokens
```

### Comparing `g4f-0.3.1.3/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.1.4/g4f/Provider/openai/proofofwork.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 import random
 import hashlib
 import json
 import base64
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timezone
 
-def generate_proof_token(required: bool, seed: str, difficulty: str, user_agent: str):
+
+def generate_proof_token(required: bool, seed: str = "", difficulty: str = "", user_agent: str = None, proofTokens: list = None):
     if not required:
         return
 
-    cores = [8, 12, 16, 24]
-    screens = [3000, 4000, 6000]
-
-    core = random.choice(cores)
-    screen = random.choice(screens)
-
-    # Get current UTC time
-    now_utc = datetime.now(timezone.utc)
-    parse_time = now_utc.strftime('%a, %d %b %Y %H:%M:%S GMT')
-
-    config = [core + screen, parse_time, None, 0, user_agent, "https://tcr9i.chat.openai.com/v2/35536E1E-65B4-4D96-9D97-6ADB7EFF8147/api.js","dpl=53d243de46ff04dadd88d293f088c2dd728f126f","en","en-US",442,"plugins−[object PluginArray]","","alert"]
-
-    diff_len = len(difficulty) // 2
+    if proofTokens:
+        config = proofTokens[-1]
+    else:
+        screen = random.choice([3008, 4010, 6000]) * random.choice([1, 2, 4])
+        # Get current UTC time
+        now_utc = datetime.now(timezone.utc)
+        parse_time = now_utc.strftime('%a, %d %b %Y %H:%M:%S GMT')
+        config = [
+            screen, parse_time,
+            None, 0, user_agent,
+            "https://tcr9i.chat.openai.com/v2/35536E1E-65B4-4D96-9D97-6ADB7EFF8147/api.js",
+            "dpl=1440a687921de39ff5ee56b92807faaadce73f13","en","en-US",
+            None,
+            "plugins−[object PluginArray]",
+            random.choice(["_reactListeningcfilawjnerp", "_reactListening9ne2dfo1i47", "_reactListening410nzwhan2a"]),
+            random.choice(["alert", "ontransitionend", "onprogress"])
+        ]
 
+    diff_len = len(difficulty)
     for i in range(100000):
         config[3] = i
         json_data = json.dumps(config)
         base = base64.b64encode(json_data.encode()).decode()
         hash_value = hashlib.sha3_512((seed + base).encode()).digest()
 
         if hash_value.hex()[:diff_len] <= difficulty:
-            result = "gAAAAAB" + base
-            return result
+            return "gAAAAAB" + base
 
     fallback_base = base64.b64encode(f'"{seed}"'.encode()).decode()
     return "gAAAAABwQ8Lk5FbGpA2NcR9dShT6gYjU7VxZ4D" + fallback_base
```

### Comparing `g4f-0.3.1.3/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.1.4/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/selenium/Bard.py` & `g4f-0.3.1.4/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.1.4/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.1.4/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/selenium/Phind.py` & `g4f-0.3.1.4/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.1.4/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.1.4/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.1.4/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.1.4/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.1.4/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/Provider/you/har_file.py` & `g4f-0.3.1.4/g4f/Provider/you/har_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,11 +111,11 @@
             )
         return [await get_telemetry_id()]
     finally:
         try:
             if page is not None:
                 await page.close()
             if browser is not None:
-                await browser.close()
+                await browser.stop()
         except Exception as e:
             if debug.logging:
                 logging.error(e)
```

### Comparing `g4f-0.3.1.3/g4f/__init__.py` & `g4f-0.3.1.4/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/api/__init__.py` & `g4f-0.3.1.4/g4f/api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,22 @@
     temperature: Optional[float] = None
     max_tokens: Optional[int] = None
     stop: Union[list[str], str, None] = None
     api_key: Optional[str] = None
     web_search: Optional[bool] = None
     proxy: Optional[str] = None
 
+class ImagesGenerateForm(BaseModel):
+    model: Optional[str] = None
+    provider: Optional[str] = None
+    prompt: str
+    response_format: Optional[str] = None
+    api_key: Optional[str] = None
+    proxy: Optional[str] = None
+
 class AppConfig():
     list_ignored_providers: Optional[list[str]] = None
     g4f_api_key: Optional[str] = None
     ignore_cookie_files: bool = False
     defaults: dict = {}
 
     @classmethod
@@ -145,45 +153,61 @@
                 if config.api_key is None and request is not None:
                     auth_header = request.headers.get("Authorization")
                     if auth_header is not None:
                         auth_header = auth_header.split(None, 1)[-1]
                         if auth_header and auth_header != "Bearer":
                             config.api_key = auth_header
                 response = self.client.chat.completions.create(
-    **{
-        **AppConfig.defaults,
-        **config.dict(exclude_none=True),
-    },
-                    
+                    **{
+                        **AppConfig.defaults,
+                        **config.dict(exclude_none=True),
+                    },
                     ignored=AppConfig.list_ignored_providers
                 )
+                if not config.stream:
+                    return JSONResponse((await response).to_json())
+
+                async def streaming():
+                    try:
+                        async for chunk in response:
+                            yield f"data: {json.dumps(chunk.to_json())}\n\n"
+                    except GeneratorExit:
+                        pass
+                    except Exception as e:
+                        logging.exception(e)
+                        yield f'data: {format_exception(e, config)}\n\n'
+                    yield "data: [DONE]\n\n"
+                return StreamingResponse(streaming(), media_type="text/event-stream")
+
             except Exception as e:
                 logging.exception(e)
                 return Response(content=format_exception(e, config), status_code=500, media_type="application/json")
 
-            if not config.stream:
-                return JSONResponse((await response).to_json())
-
-            async def streaming():
-                try:
-                    async for chunk in response:
-                        yield f"data: {json.dumps(chunk.to_json())}\n\n"
-                except GeneratorExit:
-                    pass
-                except Exception as e:
-                    logging.exception(e)
-                    yield f'data: {format_exception(e, config)}\n\n'
-                yield "data: [DONE]\n\n"
-
-            return StreamingResponse(streaming(), media_type="text/event-stream")
-
         @self.app.post("/v1/completions")
         async def completions():
             return Response(content=json.dumps({'info': 'Not working yet.'}, indent=4), media_type="application/json")
 
+        @self.app.post("/v1/images/generations")
+        async def images_generate(config: ImagesGenerateForm, request: Request = None, provider: str = None):
+            try:
+                config.provider = provider if config.provider is None else config.provider
+                if config.api_key is None and request is not None:
+                    auth_header = request.headers.get("Authorization")
+                    if auth_header is not None:
+                        auth_header = auth_header.split(None, 1)[-1]
+                        if auth_header and auth_header != "Bearer":
+                            config.api_key = auth_header
+                response = self.client.images.generate(
+                    **config.dict(exclude_none=True),
+                )
+                return JSONResponse((await response).to_json())
+            except Exception as e:
+                logging.exception(e)
+                return Response(content=format_exception(e, config), status_code=500, media_type="application/json")
+
 def format_exception(e: Exception, config: ChatCompletionsForm) -> str:
     last_provider = g4f.get_last_provider(True)
     return json.dumps({
         "error": {"message": f"{e.__class__.__name__}: {e}"},
         "model": last_provider.get("model") if last_provider else config.model,
         "provider": last_provider.get("name") if last_provider else config.provider
     })
```

### Comparing `g4f-0.3.1.3/g4f/api/_logging.py` & `g4f-0.3.1.4/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/cli.py` & `g4f-0.3.1.4/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/client/async_client.py` & `g4f-0.3.1.4/g4f/client/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,42 @@
 from __future__ import annotations
 
 import time
 import random
 import string
 
-from .types import Client as BaseClient
-from .types import ProviderType, FinishReason
-from .stubs import ChatCompletion, ChatCompletionChunk, ImagesResponse, Image
-from .types import AsyncIterResponse, ImageProvider
-from .image_models import ImageModels
-from .helper import filter_json, find_stop, filter_none, cast_iter_async
-from .service import get_last_provider, get_model_and_provider
-from ..typing import Union, Messages, AsyncIterator, ImageType
-from ..errors import NoImageResponseError
+from ..typing import Union, Iterator, Messages, ImageType
+from ..providers.types import BaseProvider, ProviderType, FinishReason
 from ..image import ImageResponse as ImageProviderResponse
+from ..errors import NoImageResponseError
+from .stubs import ChatCompletion, ChatCompletionChunk, Image, ImagesResponse
+from .image_models import ImageModels
+from .types import IterResponse, ImageProvider
+from .types import Client as BaseClient
+from .service import get_model_and_provider, get_last_provider
+from .helper import find_stop, filter_json, filter_none
 
-try:
-    anext
-except NameError:
-    async def anext(iter):
-        async for chunk in iter:
-            return chunk
-
-async def iter_response(
-    response: AsyncIterator[str],
+def iter_response(
+    response: iter[str],
     stream: bool,
     response_format: dict = None,
     max_tokens: int = None,
     stop: list = None
-) -> AsyncIterResponse:
+) -> IterResponse:
     content = ""
     finish_reason = None
     completion_id = ''.join(random.choices(string.ascii_letters + string.digits, k=28))
-    count: int = 0
-    async for chunk in response:
+    for idx, chunk in enumerate(response):
         if isinstance(chunk, FinishReason):
             finish_reason = chunk.reason
             break
         content += str(chunk)
-        count += 1
-        if max_tokens is not None and count >= max_tokens:
+        if max_tokens is not None and idx + 1 >= max_tokens:
             finish_reason = "length"
-        first, content, chunk = find_stop(stop, content, chunk)
+        first, content, chunk = find_stop(stop, content, chunk if stream else None)
         if first != -1:
             finish_reason = "stop"
         if stream:
             yield ChatCompletionChunk(chunk, None, completion_id, int(time.time()))
         if finish_reason is not None:
             break
     finish_reason = "stop" if finish_reason is None else finish_reason
@@ -53,157 +44,128 @@
         yield ChatCompletionChunk(None, finish_reason, completion_id, int(time.time()))
     else:
         if response_format is not None and "type" in response_format:
             if response_format["type"] == "json_object":
                 content = filter_json(content)
         yield ChatCompletion(content, finish_reason, completion_id, int(time.time()))
 
-async def iter_append_model_and_provider(response: AsyncIterResponse) -> AsyncIterResponse:
+def iter_append_model_and_provider(response: IterResponse) -> IterResponse:
     last_provider = None
-    async for chunk in response:
+    for chunk in response:
         last_provider = get_last_provider(True) if last_provider is None else last_provider
         chunk.model = last_provider.get("model")
         chunk.provider =  last_provider.get("name")
         yield chunk
 
-class AsyncClient(BaseClient):
+class Client(BaseClient):
     def __init__(
         self,
         provider: ProviderType = None,
         image_provider: ImageProvider = None,
         **kwargs
-    ):
+    ) -> None:
         super().__init__(**kwargs)
         self.chat: Chat = Chat(self, provider)
         self.images: Images = Images(self, image_provider)
 
-def create_response(
-    messages: Messages,
-    model: str,
-    provider: ProviderType = None,
-    stream: bool = False,
-    proxy: str = None,
-    max_tokens: int = None,
-    stop: list[str] = None,
-    api_key: str = None,
-    **kwargs
-):
-    has_asnyc = hasattr(provider, "create_async_generator")
-    if has_asnyc:
-        create = provider.create_async_generator
-    else:
-        create = provider.create_completion
-    response = create(
-        model, messages,
-        stream=stream,            
-        **filter_none(
-            proxy=proxy,
-            max_tokens=max_tokens,
-            stop=stop,
-            api_key=api_key
-        ),
-        **kwargs
-    )
-    if not has_asnyc:
-        response = cast_iter_async(response)
-    return response
-
 class Completions():
-    def __init__(self, client: AsyncClient, provider: ProviderType = None):
-        self.client: AsyncClient = client
+    def __init__(self, client: Client, provider: ProviderType = None):
+        self.client: Client = client
         self.provider: ProviderType = provider
 
     def create(
         self,
         messages: Messages,
         model: str,
         provider: ProviderType = None,
         stream: bool = False,
         proxy: str = None,
+        response_format: dict = None,
         max_tokens: int = None,
         stop: Union[list[str], str] = None,
         api_key: str = None,
-        response_format: dict = None,
         ignored  : list[str] = None,
         ignore_working: bool = False,
         ignore_stream: bool = False,
         **kwargs
-    ) -> Union[ChatCompletion, AsyncIterator[ChatCompletionChunk]]:
+    ) -> Union[ChatCompletion, Iterator[ChatCompletionChunk]]:
         model, provider = get_model_and_provider(
             model,
             self.provider if provider is None else provider,
             stream,
             ignored,
             ignore_working,
-            ignore_stream
+            ignore_stream,
         )
+        
         stop = [stop] if isinstance(stop, str) else stop
-        response = create_response(
-            messages, model,
-            provider, stream,
-            proxy=self.client.get_proxy() if proxy is None else proxy,
-            max_tokens=max_tokens,
-            stop=stop,
-            api_key=self.client.api_key if api_key is None else api_key,
+        response = provider.create_completion(
+            model, messages,
+            stream=stream,            
+            **filter_none(
+                proxy=self.client.get_proxy() if proxy is None else proxy,
+                max_tokens=max_tokens,
+                stop=stop,
+                api_key=self.client.api_key if api_key is None else api_key
+            ),
             **kwargs
         )
         response = iter_response(response, stream, response_format, max_tokens, stop)
         response = iter_append_model_and_provider(response)
-        return response if stream else anext(response)
+        return response if stream else next(response)
 
 class Chat():
     completions: Completions
 
-    def __init__(self, client: AsyncClient, provider: ProviderType = None):
+    def __init__(self, client: Client, provider: ProviderType = None):
         self.completions = Completions(client, provider)
 
-async def iter_image_response(response: AsyncIterator) -> Union[ImagesResponse, None]:
-    async for chunk in response:
+def iter_image_response(response: Iterator) -> Union[ImagesResponse, None]:
+    for chunk in list(response):
         if isinstance(chunk, ImageProviderResponse):
             return ImagesResponse([Image(image) for image in chunk.get_list()])
 
-def create_image(client: AsyncClient, provider: ProviderType, prompt: str, model: str = "", **kwargs) -> AsyncIterator:
+def create_image(client: Client, provider: ProviderType, prompt: str, model: str = "", **kwargs) -> Iterator:
     prompt = f"create a image with: {prompt}"
     if provider.__name__ == "You":
         kwargs["chat_mode"] = "create"
-    return provider.create_async_generator(
+    return provider.create_completion(
         model,
         [{"role": "user", "content": prompt}],
         stream=True,
         proxy=client.get_proxy(),
         **kwargs
     )
 
 class Images():
-    def __init__(self, client: AsyncClient, provider: ImageProvider = None):
-        self.client: AsyncClient = client
+    def __init__(self, client: Client, provider: ImageProvider = None):
+        self.client: Client = client
         self.provider: ImageProvider = provider
         self.models: ImageModels = ImageModels(client)
 
-    async def generate(self, prompt, model: str = "", **kwargs) -> ImagesResponse:
+    def generate(self, prompt, model: str = None, **kwargs) -> ImagesResponse:
         provider = self.models.get(model, self.provider)
-        if hasattr(provider, "create_async_generator"):
+        if isinstance(provider, type) and issubclass(provider, BaseProvider):
             response = create_image(self.client, provider, prompt, **kwargs)
         else:
-            response = await provider.create_async(prompt)
-            return ImagesResponse([Image(image) for image in response.get_list()])
-        image = await iter_image_response(response)
+            response = list(provider.create(prompt))
+        image = iter_image_response(response)
         if image is None:
             raise NoImageResponseError()
         return image
 
-    async def create_variation(self, image: ImageType, model: str = None, **kwargs):
+    def create_variation(self, image: ImageType, model: str = None, **kwargs):
         provider = self.models.get(model, self.provider)
         result = None
-        if hasattr(provider, "create_async_generator"):
-            response = provider.create_async_generator(
+        if isinstance(provider, type) and issubclass(provider, BaseProvider):
+            response = provider.create_completion(
                 "",
                 [{"role": "user", "content": "create a image like this"}],
                 True,
                 image=image,
                 proxy=self.client.get_proxy(),
                 **kwargs
             )
             result = iter_image_response(response)
         if result is None:
             raise NoImageResponseError()
-        return result
+        return result
```

### Comparing `g4f-0.3.1.3/g4f/client/client.py` & `g4f-0.3.1.4/g4f/client/async_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,56 @@
 from __future__ import annotations
 
 import time
 import random
 import string
+import asyncio
+import base64
+from aiohttp import ClientSession, BaseConnector
 
-from ..typing import Union, Iterator, Messages, ImageType
-from ..providers.types import BaseProvider, ProviderType, FinishReason
-from ..image import ImageResponse as ImageProviderResponse
-from ..errors import NoImageResponseError
-from .stubs import ChatCompletion, ChatCompletionChunk, Image, ImagesResponse
-from .image_models import ImageModels
-from .types import IterResponse, ImageProvider
 from .types import Client as BaseClient
-from .service import get_model_and_provider, get_last_provider
-from .helper import find_stop, filter_json, filter_none
+from .types import ProviderType, FinishReason
+from .stubs import ChatCompletion, ChatCompletionChunk, ImagesResponse, Image
+from .types import AsyncIterResponse, ImageProvider
+from .image_models import ImageModels
+from .helper import filter_json, find_stop, filter_none, cast_iter_async
+from .service import get_last_provider, get_model_and_provider
+from ..Provider import ProviderUtils
+from ..typing import Union, Messages, AsyncIterator, ImageType
+from ..errors import NoImageResponseError, ProviderNotFoundError
+from ..requests.aiohttp import get_connector
+from ..image import ImageResponse as ImageProviderResponse, ImageDataResponse
+
+try:
+    anext
+except NameError:
+    async def anext(iter):
+        async for chunk in iter:
+            return chunk
 
-def iter_response(
-    response: iter[str],
+async def iter_response(
+    response: AsyncIterator[str],
     stream: bool,
     response_format: dict = None,
     max_tokens: int = None,
     stop: list = None
-) -> IterResponse:
+) -> AsyncIterResponse:
     content = ""
     finish_reason = None
     completion_id = ''.join(random.choices(string.ascii_letters + string.digits, k=28))
-    for idx, chunk in enumerate(response):
+    count: int = 0
+    async for chunk in response:
         if isinstance(chunk, FinishReason):
             finish_reason = chunk.reason
             break
         content += str(chunk)
-        if max_tokens is not None and idx + 1 >= max_tokens:
+        count += 1
+        if max_tokens is not None and count >= max_tokens:
             finish_reason = "length"
-        first, content, chunk = find_stop(stop, content, chunk if stream else None)
+        first, content, chunk = find_stop(stop, content, chunk)
         if first != -1:
             finish_reason = "stop"
         if stream:
             yield ChatCompletionChunk(chunk, None, completion_id, int(time.time()))
         if finish_reason is not None:
             break
     finish_reason = "stop" if finish_reason is None else finish_reason
@@ -44,128 +58,212 @@
         yield ChatCompletionChunk(None, finish_reason, completion_id, int(time.time()))
     else:
         if response_format is not None and "type" in response_format:
             if response_format["type"] == "json_object":
                 content = filter_json(content)
         yield ChatCompletion(content, finish_reason, completion_id, int(time.time()))
 
-def iter_append_model_and_provider(response: IterResponse) -> IterResponse:
+async def iter_append_model_and_provider(response: AsyncIterResponse) -> AsyncIterResponse:
     last_provider = None
-    for chunk in response:
+    async for chunk in response:
         last_provider = get_last_provider(True) if last_provider is None else last_provider
         chunk.model = last_provider.get("model")
         chunk.provider =  last_provider.get("name")
         yield chunk
 
-class Client(BaseClient):
+class AsyncClient(BaseClient):
     def __init__(
         self,
         provider: ProviderType = None,
         image_provider: ImageProvider = None,
         **kwargs
-    ) -> None:
+    ):
         super().__init__(**kwargs)
         self.chat: Chat = Chat(self, provider)
         self.images: Images = Images(self, image_provider)
 
+def create_response(
+    messages: Messages,
+    model: str,
+    provider: ProviderType = None,
+    stream: bool = False,
+    proxy: str = None,
+    max_tokens: int = None,
+    stop: list[str] = None,
+    api_key: str = None,
+    **kwargs
+):
+    has_asnyc = hasattr(provider, "create_async_generator")
+    if has_asnyc:
+        create = provider.create_async_generator
+    else:
+        create = provider.create_completion
+    response = create(
+        model, messages,
+        stream=stream,            
+        **filter_none(
+            proxy=proxy,
+            max_tokens=max_tokens,
+            stop=stop,
+            api_key=api_key
+        ),
+        **kwargs
+    )
+    if not has_asnyc:
+        response = cast_iter_async(response)
+    return response
+
 class Completions():
-    def __init__(self, client: Client, provider: ProviderType = None):
-        self.client: Client = client
+    def __init__(self, client: AsyncClient, provider: ProviderType = None):
+        self.client: AsyncClient = client
         self.provider: ProviderType = provider
 
     def create(
         self,
         messages: Messages,
         model: str,
         provider: ProviderType = None,
         stream: bool = False,
         proxy: str = None,
-        response_format: dict = None,
         max_tokens: int = None,
         stop: Union[list[str], str] = None,
         api_key: str = None,
+        response_format: dict = None,
         ignored  : list[str] = None,
         ignore_working: bool = False,
         ignore_stream: bool = False,
         **kwargs
-    ) -> Union[ChatCompletion, Iterator[ChatCompletionChunk]]:
+    ) -> Union[ChatCompletion, AsyncIterator[ChatCompletionChunk]]:
         model, provider = get_model_and_provider(
             model,
             self.provider if provider is None else provider,
             stream,
             ignored,
             ignore_working,
-            ignore_stream,
+            ignore_stream
         )
-        
         stop = [stop] if isinstance(stop, str) else stop
-        response = provider.create_completion(
-            model, messages,
-            stream=stream,            
-            **filter_none(
-                proxy=self.client.get_proxy() if proxy is None else proxy,
-                max_tokens=max_tokens,
-                stop=stop,
-                api_key=self.client.api_key if api_key is None else api_key
-            ),
+        response = create_response(
+            messages, model,
+            provider, stream,
+            proxy=self.client.get_proxy() if proxy is None else proxy,
+            max_tokens=max_tokens,
+            stop=stop,
+            api_key=self.client.api_key if api_key is None else api_key,
             **kwargs
         )
         response = iter_response(response, stream, response_format, max_tokens, stop)
         response = iter_append_model_and_provider(response)
-        return response if stream else next(response)
+        return response if stream else anext(response)
 
 class Chat():
     completions: Completions
 
-    def __init__(self, client: Client, provider: ProviderType = None):
+    def __init__(self, client: AsyncClient, provider: ProviderType = None):
         self.completions = Completions(client, provider)
 
-def iter_image_response(response: Iterator) -> Union[ImagesResponse, None]:
-    for chunk in list(response):
+async def iter_image_response(
+    response: AsyncIterator,
+    response_format: str = None,
+    connector: BaseConnector = None,
+    proxy: str = None
+) -> Union[ImagesResponse, None]:
+    async for chunk in response:
         if isinstance(chunk, ImageProviderResponse):
-            return ImagesResponse([Image(image) for image in chunk.get_list()])
+            if response_format == "b64_json":
+                async with ClientSession(
+                    connector=get_connector(connector, proxy)
+                ) as session:
+                    async def fetch_image(image):
+                        async with session.get(image) as response:
+                            return base64.b64encode(await response.content.read()).decode()
+                    images = await asyncio.gather(*[fetch_image(image) for image in chunk.get_list()])
+                return ImagesResponse([Image(None, image, chunk.alt) for image in images], int(time.time()))
+            return ImagesResponse([Image(image, None, chunk.alt) for image in chunk.get_list()], int(time.time()))
+        elif isinstance(chunk, ImageDataResponse):
+            return ImagesResponse([Image(None, image, chunk.alt) for image in chunk.get_list()], int(time.time()))
 
-def create_image(client: Client, provider: ProviderType, prompt: str, model: str = "", **kwargs) -> Iterator:
+def create_image(provider: ProviderType, prompt: str, model: str = "", **kwargs) -> AsyncIterator:
     prompt = f"create a image with: {prompt}"
     if provider.__name__ == "You":
         kwargs["chat_mode"] = "create"
-    return provider.create_completion(
+    return provider.create_async_generator(
         model,
         [{"role": "user", "content": prompt}],
         stream=True,
-        proxy=client.get_proxy(),
         **kwargs
     )
 
 class Images():
-    def __init__(self, client: Client, provider: ImageProvider = None):
-        self.client: Client = client
+    def __init__(self, client: AsyncClient, provider: ImageProvider = None):
+        self.client: AsyncClient = client
         self.provider: ImageProvider = provider
         self.models: ImageModels = ImageModels(client)
 
-    def generate(self, prompt, model: str = None, **kwargs) -> ImagesResponse:
-        provider = self.models.get(model, self.provider)
-        if isinstance(provider, type) and issubclass(provider, BaseProvider):
-            response = create_image(self.client, provider, prompt, **kwargs)
+    def get_provider(self, model: str, provider: ProviderType = None):
+        if isinstance(provider, str):
+            if provider in ProviderUtils.convert:
+                provider = ProviderUtils.convert[provider]
+            else:
+                raise ProviderNotFoundError(f'Provider not found: {provider}')
+        else:
+            provider = self.models.get(model, self.provider)
+        return provider
+
+    async def generate(
+        self,
+        prompt,
+        model: str = "",
+        provider: ProviderType = None,
+        response_format: str = None,
+        connector: BaseConnector = None,
+        proxy: str = None,
+        **kwargs
+    ) -> ImagesResponse:
+        provider = self.get_provider(model, provider)
+        if hasattr(provider, "create_async_generator"):
+            response = create_image(
+                provider,
+                prompt,
+                **filter_none(
+                    response_format=response_format,
+                    connector=connector,
+                    proxy=self.client.get_proxy() if proxy is None else proxy,
+                ),
+                **kwargs
+            )
         else:
-            response = list(provider.create(prompt))
-        image = iter_image_response(response)
+            response = await provider.create_async(prompt)
+            return ImagesResponse([Image(image) for image in response.get_list()])
+        image = await iter_image_response(response, response_format, connector, proxy)
         if image is None:
             raise NoImageResponseError()
         return image
 
-    def create_variation(self, image: ImageType, model: str = None, **kwargs):
-        provider = self.models.get(model, self.provider)
+    async def create_variation(
+        self,
+        image: ImageType,
+        model: str = None,
+        response_format: str = None,
+        connector: BaseConnector = None,
+        proxy: str = None,
+        **kwargs
+    ):
+        provider = self.get_provider(model, provider)
         result = None
-        if isinstance(provider, type) and issubclass(provider, BaseProvider):
-            response = provider.create_completion(
+        if hasattr(provider, "create_async_generator"):
+            response = provider.create_async_generator(
                 "",
                 [{"role": "user", "content": "create a image like this"}],
-                True,
+                stream=True,
                 image=image,
-                proxy=self.client.get_proxy(),
+                **filter_none(
+                    response_format=response_format,
+                    connector=connector,
+                    proxy=self.client.get_proxy() if proxy is None else proxy,
+                ),
                 **kwargs
             )
-            result = iter_image_response(response)
+            result = iter_image_response(response, response_format, connector, proxy)
         if result is None:
             raise NoImageResponseError()
-        return result
+        return result
```

### Comparing `g4f-0.3.1.3/g4f/client/helper.py` & `g4f-0.3.1.4/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/client/image_models.py` & `g4f-0.3.1.4/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/client/service.py` & `g4f-0.3.1.4/g4f/client/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Union
 
 from .. import debug, version
 from ..errors import ProviderNotFoundError, ModelNotFoundError, ProviderNotWorkingError, StreamNotSupportedError
-from ..models import Model, ModelUtils
+from ..models import Model, ModelUtils, default
 from ..Provider import ProviderUtils
 from ..providers.types import BaseRetryProvider, ProviderType
 from ..providers.retry_provider import IterProvider
 
 def convert_to_provider(provider: str) -> ProviderType:
     if " " in provider:
         provider_list = [ProviderUtils.convert[p] for p in provider.split() if p in ProviderUtils.convert]
@@ -56,15 +56,17 @@
 
     if isinstance(model, str):
         
         if model in ModelUtils.convert:
             model = ModelUtils.convert[model]
     
     if not provider:
-        if isinstance(model, str):
+        if not model:
+            model = default
+        elif isinstance(model, str):
             raise ModelNotFoundError(f'Model not found: {model}')
         provider = model.best_provider
 
     if not provider:
         raise ProviderNotFoundError(f'No provider found for model: {model}')
 
     if isinstance(model, Model):
```

### Comparing `g4f-0.3.1.3/g4f/client/stubs.py` & `g4f-0.3.1.4/g4f/stubs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from __future__ import annotations
 
 from typing import Union
 
 class Model():
     ...
 
@@ -74,22 +75,20 @@
 
 class ChatCompletionDelta(Model):
     content: Union[str, None] = None
 
     def __init__(self, content: Union[str, None]):
         if content is not None:
             self.content = content
-            self.role = "assistant"
 
     def to_json(self):
         return self.__dict__
 
 class ChatCompletionDeltaChoice(Model):
     def __init__(self, delta: ChatCompletionDelta, finish_reason: Union[str, None]):
-        self.index = 0
         self.delta = delta
         self.finish_reason = finish_reason
 
     def to_json(self):
         return {
             **self.__dict__,
             "delta": self.delta.to_json()
@@ -101,8 +100,8 @@
     def __init__(self, url: str) -> None:
         self.url = url
 
 class ImagesResponse(Model):
     data: list[Image]
 
     def __init__(self, data: list) -> None:
-        self.data = data
+        self.data = data
```

### Comparing `g4f-0.3.1.3/g4f/client/types.py` & `g4f-0.3.1.4/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/cookies.py` & `g4f-0.3.1.4/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/errors.py` & `g4f-0.3.1.4/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/__init__.py` & `g4f-0.3.1.4/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/index.html` & `g4f-0.3.1.4/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/css/dracula.min.css` & `g4f-0.3.1.4/g4f/gui/client/static/css/dracula.min.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/css/style.css` & `g4f-0.3.1.4/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.1.4/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.1.4/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.1.4/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.1.4/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/img/user.png` & `g4f-0.3.1.4/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.1.4/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.1.4/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.1.4/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/js/icons.js` & `g4f-0.3.1.4/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.1.4/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/server/android_gallery.py` & `g4f-0.3.1.4/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/server/api.py` & `g4f-0.3.1.4/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/server/backend.py` & `g4f-0.3.1.4/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/server/config.py` & `g4f-0.3.1.4/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/server/internet.py` & `g4f-0.3.1.4/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/server/js_api.py` & `g4f-0.3.1.4/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/server/website.py` & `g4f-0.3.1.4/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/gui/webview.py` & `g4f-0.3.1.4/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/image.py` & `g4f-0.3.1.4/g4f/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,26 @@
 class ImagePreview(ImageResponse):
     def __str__(self):
         return ""
 
     def to_string(self):
         return super().__str__()
 
+class ImageDataResponse():
+    def __init__(
+        self,
+        images: Union[str, list],
+        alt: str,
+    ):
+        self.images = images
+        self.alt = alt
+
+    def get_list(self) -> list[str]:
+        return [self.images] if isinstance(self.images, str) else self.images
+
 class ImageRequest:
     def __init__(
         self,
         options: dict = {}
     ):
         self.options = options
```

### Comparing `g4f-0.3.1.3/g4f/local/__init__.py` & `g4f-0.3.1.4/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/locals/models.py` & `g4f-0.3.1.4/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/locals/provider.py` & `g4f-0.3.1.4/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/models.py` & `g4f-0.3.1.4/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/providers/base_provider.py` & `g4f-0.3.1.4/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/providers/create_images.py` & `g4f-0.3.1.4/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/providers/helper.py` & `g4f-0.3.1.4/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/providers/retry_provider.py` & `g4f-0.3.1.4/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/providers/types.py` & `g4f-0.3.1.4/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/requests/__init__.py` & `g4f-0.3.1.4/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/requests/aiohttp.py` & `g4f-0.3.1.4/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/requests/curl_cffi.py` & `g4f-0.3.1.4/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/requests/defaults.py` & `g4f-0.3.1.4/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/requests/raise_for_status.py` & `g4f-0.3.1.4/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/stubs.py` & `g4f-0.3.1.4/g4f/client/stubs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from __future__ import annotations
 
 from typing import Union
 
 class Model():
     ...
 
@@ -75,33 +74,46 @@
 
 class ChatCompletionDelta(Model):
     content: Union[str, None] = None
 
     def __init__(self, content: Union[str, None]):
         if content is not None:
             self.content = content
+            self.role = "assistant"
 
     def to_json(self):
         return self.__dict__
 
 class ChatCompletionDeltaChoice(Model):
     def __init__(self, delta: ChatCompletionDelta, finish_reason: Union[str, None]):
+        self.index = 0
         self.delta = delta
         self.finish_reason = finish_reason
 
     def to_json(self):
         return {
             **self.__dict__,
             "delta": self.delta.to_json()
         }
 
 class Image(Model):
-    url: str
+    def __init__(self, url: str = None, b64_json: str = None, revised_prompt: str = None) -> None:
+        if url is not None:
+            self.url = url
+        if b64_json is not None:
+            self.b64_json = b64_json
+        if revised_prompt is not None:
+            self.revised_prompt = revised_prompt
 
-    def __init__(self, url: str) -> None:
-        self.url = url
+    def to_json(self):
+        return self.__dict__
 
 class ImagesResponse(Model):
-    data: list[Image]
+    def __init__(self, data: list[Image], created: int = 0) -> None:
+        self.data = data
+        self.created = created
 
-    def __init__(self, data: list) -> None:
-        self.data = data
+    def to_json(self):
+        return {
+            **self.__dict__,
+            "data": [image.to_json() for image in self.data]
+        }
```

### Comparing `g4f-0.3.1.3/g4f/typing.py` & `g4f-0.3.1.4/g4f/typing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/version.py` & `g4f-0.3.1.4/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f/webdriver.py` & `g4f-0.3.1.4/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f.egg-info/PKG-INFO` & `g4f-0.3.1.4/g4f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.3
+Version: 0.3.1.4
 Summary: The official gpt4free repository | various collection of powerful language models
 Home-page: https://github.com/xtekky/gpt4free
 Author: Tekky
 Author-email: <support@g4f.ai>
 Project-URL: Source Code, https://github.com/xtekky/gpt4free
 Project-URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues
 Keywords: python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.3 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.4 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.1.3/g4f.egg-info/SOURCES.txt` & `g4f-0.3.1.4/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/g4f.egg-info/requires.txt` & `g4f-0.3.1.4/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.3/setup.py` & `g4f-0.3.1.4/setup.py`

 * *Files identical despite different names*

