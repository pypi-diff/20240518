# Comparing `tmp/g4f-0.3.1.2.tar.gz` & `tmp/g4f-0.3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g4f-0.3.1.2.tar", last modified: Thu May 16 18:09:32 2024, max compression
+gzip compressed data, was "g4f-0.3.1.3.tar", last modified: Fri May 17 16:45:40 2024, max compression
```

## Comparing `g4f-0.3.1.2.tar` & `g4f-0.3.1.3.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.112183 g4f-0.3.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-16 18:09:21.000000 g4f-0.3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 18:09:21.000000 g4f-0.3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-16 18:09:32.112183 g4f-0.3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    52480 2024-05-16 18:09:21.000000 g4f-0.3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.072182 g4f-0.3.1.2/g4f/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.080182 g4f-0.3.1.2/g4f/Provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Aichatos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Aura.py
--rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Bing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/BingCreateImages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatForAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Chatgpt4Online.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptFree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptNext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ChatgptX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Cnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/DeepInfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/DeepInfraImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/DuckDuckGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Ecosia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Feedough.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/FlowGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/FreeChatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/FreeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GeminiPro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GeminiProChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GigaChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/GptTalkRu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/HuggingChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/HuggingFace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Koala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Liaobots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Local.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/MetaAI.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/MetaAIAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/PerplexityLabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Pi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Reka.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/ReplicateImage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/WhiteRabbitNeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/You.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/base_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.080182 g4f-0.3.1.2/g4f/Provider/bing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/bing/upload_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.088182 g4f-0.3.1.2/g4f/Provider/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Acytoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/AiAsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/AiChatOnline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/AiService.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Aibn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Aichat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Ails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Aivvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Berlin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/ChatAnywhere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/ChatgptDuo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/CodeLinkAva.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Cromicle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/DfeHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/EasyChat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Equing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/FakeGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/FastGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Forefront.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/GPTalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/GeekGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/GetGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/H2o.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Hashnode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Lockchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Myshell.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/NoowAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Opchatgpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/OpenAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/V50.py
--rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Vercel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Vitalentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/VoiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Wewordle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Wuguokai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Ylokh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/Yqcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/deprecated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.088182 g4f-0.3.1.2/g4f/Provider/gigachat_crt/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.088182 g4f-0.3.1.2/g4f/Provider/needs_auth/
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/OpenRouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/OpenaiAccount.py
--rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/OpenaiChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/PerplexityApi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Raycast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/Theb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/ThebApi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/needs_auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/not_working/
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/AItianhu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/Bestim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemoAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/ChatgptLogin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/Chatxyz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/Gpt6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptChatly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptForLove.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptGo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/GptGod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/OnlineGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/not_working/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/npm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/npm/node_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/node_modules/.package-lock.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/npm/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.092182 g4f-0.3.1.2/g4f/Provider/openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/openai/proofofwork.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/Provider/selenium/
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/AItianhuSpace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/Bard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/MyShell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/PerplexityAi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/Phind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/TalkAi.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/selenium/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/Provider/unfinished/
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/AiChatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/ChatAiGpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/Komo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/MikuChat.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/unfinished/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/Provider/you/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/you/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/Provider/you/har_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/api/
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/api/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.096182 g4f-0.3.1.2/g4f/client/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/image_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/
--rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.068182 g4f-0.3.1.2/g4f/gui/client/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/css/dracula.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/gpt.png
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/img/user.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.100183 g4f-0.3.1.2/g4f/gui/client/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    48500 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/chat.v1.js
--rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/highlight.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/highlightjs-copy.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/icons.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/
--rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/630.index.js
--rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/900.index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/gui_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/gui/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/android_gallery.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/js_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/server/website.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/gui/webview.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/local/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/locals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/locals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/locals/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/locals/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.104183 g4f-0.3.1.2/g4f/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/base_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/create_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/retry_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/providers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.108183 g4f-0.3.1.2/g4f/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/curl_cffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/requests/raise_for_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/stubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-16 18:09:21.000000 g4f-0.3.1.2/g4f/webdriver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:09:32.108183 g4f-0.3.1.2/g4f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 18:09:32.000000 g4f-0.3.1.2/g4f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:09:32.112183 g4f-0.3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-16 18:09:21.000000 g4f-0.3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.800188 g4f-0.3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-17 16:45:36.000000 g4f-0.3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-17 16:45:36.000000 g4f-0.3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-17 16:45:40.796188 g4f-0.3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    52480 2024-05-17 16:45:36.000000 g4f-0.3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.756188 g4f-0.3.1.3/g4f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.764188 g4f-0.3.1.3/g4f/Provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Aichatos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Aura.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21427 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Bing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/BingCreateImages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatForAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Chatgpt4Online.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptFree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptNext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ChatgptX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Cnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/DeepInfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/DeepInfraImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/DuckDuckGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Ecosia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Feedough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/FlowGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/FreeChatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/FreeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GeminiPro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GeminiProChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GigaChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/GptTalkRu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/HuggingChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/HuggingFace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Koala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Liaobots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/MetaAI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/MetaAIAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/PerplexityLabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Pi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Reka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/ReplicateImage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/WhiteRabbitNeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/You.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/base_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.768188 g4f-0.3.1.3/g4f/Provider/bing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/bing/upload_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.772188 g4f-0.3.1.3/g4f/Provider/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Acytoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/AiAsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/AiChatOnline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/AiService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Aibn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Aichat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Ails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Aivvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/ChatAnywhere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/ChatgptDuo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/CodeLinkAva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Cromicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/DfeHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/EasyChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Equing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/FakeGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/FastGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Forefront.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/GPTalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/GeekGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/GetGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/H2o.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Hashnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Lockchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Myshell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/NoowAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Opchatgpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/OpenAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/V50.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12167 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Vercel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Vitalentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/VoiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Wewordle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Wuguokai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Ylokh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/Yqcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/deprecated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.772188 g4f-0.3.1.3/g4f/Provider/gigachat_crt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.776188 g4f-0.3.1.3/g4f/Provider/needs_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/OpenRouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/OpenaiAccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33891 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/OpenaiChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/PerplexityApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Raycast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/Theb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/ThebApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/needs_auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.776188 g4f-0.3.1.3/g4f/Provider/not_working/
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/AItianhu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/Bestim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemoAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/ChatgptLogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/Chatxyz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/Gpt6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptChatly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptForLove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptGo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/GptGod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/OnlineGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/not_working/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/npm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/npm/node_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/node_modules/.package-lock.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   219092 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/npm/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/openai/proofofwork.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/selenium/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/AItianhuSpace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/Bard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/MyShell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/PerplexityAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/Phind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/TalkAi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/selenium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/unfinished/
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/AiChatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/ChatAiGpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/Komo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/MikuChat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/unfinished/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.780188 g4f-0.3.1.3/g4f/Provider/you/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/you/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/Provider/you/har_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/api/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/image_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/gui/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    12827 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.752188 g4f-0.3.1.3/g4f/gui/client/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.784188 g4f-0.3.1.3/g4f/gui/client/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/css/dracula.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.788188 g4f-0.3.1.3/g4f/gui/client/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/gpt.png
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/img/user.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.788188 g4f-0.3.1.3/g4f/gui/client/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    48500 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/chat.v1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   118841 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/highlight.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/highlightjs-copy.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/icons.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.788188 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/630.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   767022 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/900.index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/gui_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/gui/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/android_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15354 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/js_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/server/website.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/gui/webview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/local/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/locals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/locals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/locals/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/locals/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9675 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/base_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/create_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/retry_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/providers/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/curl_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/requests/raise_for_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/stubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 16:45:36.000000 g4f-0.3.1.3/g4f/webdriver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:45:40.792188 g4f-0.3.1.3/g4f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55676 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-17 16:45:40.000000 g4f-0.3.1.3/g4f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 16:45:40.800188 g4f-0.3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-17 16:45:36.000000 g4f-0.3.1.3/setup.py
```

### Comparing `g4f-0.3.1.2/LICENSE` & `g4f-0.3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/PKG-INFO` & `g4f-0.3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.2
+Version: 0.3.1.3
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
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.3 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.1.2/README.md` & `g4f-0.3.1.3/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Aichatos.py` & `g4f-0.3.1.3/g4f/Provider/Aichatos.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Aura.py` & `g4f-0.3.1.3/g4f/Provider/Aura.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Bing.py` & `g4f-0.3.1.3/g4f/Provider/Bing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/BingCreateImages.py` & `g4f-0.3.1.3/g4f/Provider/BingCreateImages.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Blackbox.py` & `g4f-0.3.1.3/g4f/Provider/Blackbox.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/ChatForAi.py` & `g4f-0.3.1.3/g4f/Provider/ChatForAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Chatgpt4Online.py` & `g4f-0.3.1.3/g4f/Provider/Chatgpt4Online.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/ChatgptAi.py` & `g4f-0.3.1.3/g4f/Provider/ChatgptAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/ChatgptFree.py` & `g4f-0.3.1.3/g4f/Provider/ChatgptFree.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/ChatgptNext.py` & `g4f-0.3.1.3/g4f/Provider/ChatgptNext.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/ChatgptX.py` & `g4f-0.3.1.3/g4f/Provider/ChatgptX.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Cnote.py` & `g4f-0.3.1.3/g4f/Provider/Cnote.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Cohere.py` & `g4f-0.3.1.3/g4f/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/DeepInfra.py` & `g4f-0.3.1.3/g4f/Provider/DeepInfra.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/DeepInfraImage.py` & `g4f-0.3.1.3/g4f/Provider/DeepInfraImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/DuckDuckGo.py` & `g4f-0.3.1.3/g4f/Provider/DuckDuckGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Ecosia.py` & `g4f-0.3.1.3/g4f/Provider/Ecosia.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Feedough.py` & `g4f-0.3.1.3/g4f/Provider/Feedough.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/FlowGpt.py` & `g4f-0.3.1.3/g4f/Provider/FlowGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/FreeChatgpt.py` & `g4f-0.3.1.3/g4f/Provider/FreeChatgpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/FreeGpt.py` & `g4f-0.3.1.3/g4f/Provider/FreeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/GeminiPro.py` & `g4f-0.3.1.3/g4f/Provider/GeminiPro.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/GeminiProChat.py` & `g4f-0.3.1.3/g4f/Provider/GeminiProChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/GigaChat.py` & `g4f-0.3.1.3/g4f/Provider/GigaChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/GptTalkRu.py` & `g4f-0.3.1.3/g4f/Provider/GptTalkRu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/HuggingChat.py` & `g4f-0.3.1.3/g4f/Provider/HuggingChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/HuggingFace.py` & `g4f-0.3.1.3/g4f/Provider/HuggingFace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Koala.py` & `g4f-0.3.1.3/g4f/Provider/Koala.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Liaobots.py` & `g4f-0.3.1.3/g4f/Provider/Liaobots.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Llama.py` & `g4f-0.3.1.3/g4f/Provider/Llama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Local.py` & `g4f-0.3.1.3/g4f/Provider/Local.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/MetaAI.py` & `g4f-0.3.1.3/g4f/Provider/MetaAI.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/MetaAIAccount.py` & `g4f-0.3.1.3/g4f/Provider/MetaAIAccount.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Ollama.py` & `g4f-0.3.1.3/g4f/Provider/Ollama.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/PerplexityLabs.py` & `g4f-0.3.1.3/g4f/Provider/PerplexityLabs.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Pi.py` & `g4f-0.3.1.3/g4f/Provider/Pi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Reka.py` & `g4f-0.3.1.3/g4f/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Replicate.py` & `g4f-0.3.1.3/g4f/Provider/Replicate.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/ReplicateImage.py` & `g4f-0.3.1.3/g4f/Provider/ReplicateImage.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/Vercel.py` & `g4f-0.3.1.3/g4f/Provider/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/WhiteRabbitNeo.py` & `g4f-0.3.1.3/g4f/Provider/WhiteRabbitNeo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/You.py` & `g4f-0.3.1.3/g4f/Provider/You.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,34 +96,35 @@
                 "selectedChatMode": chat_mode,
             }
             params = {
                 "userFiles": upload,
                 "selectedChatMode": chat_mode,
             }
             if chat_mode == "custom":
-                # print(f"You model: {model}")
-                params["selectedAIModel"] = model.replace("-", "_")
-            
+                if debug.logging:
+                    print(f"You model: {model}")
+                params["selectedAiModel"] = model.replace("-", "_")
+
             async with (session.post if chat_mode == "default" else session.get)(
                 f"{cls.url}/api/streamingSearch",
                 data=data,
                 params=params,
                 headers=headers,
                 cookies=cookies
             ) as response:
                 await raise_for_status(response)
                 async for line in response.iter_lines():
                     if line.startswith(b'event: '):
                         event = line[7:].decode()
                     elif line.startswith(b'data: '):
                         if event in ["youChatUpdate", "youChatToken"]:
                             data = json.loads(line[6:])
-                        if event == "youChatToken" and event in data:
+                        if event == "youChatToken" and event in data and data[event]:
                             yield data[event]
-                        elif event == "youChatUpdate" and "t" in data and data["t"] is not None:
+                        elif event == "youChatUpdate" and "t" in data and data["t"]:
                             if chat_mode == "create":
                                 match = re.search(r"!\[(.+?)\]\((.+?)\)", data["t"])
                                 if match:
                                     if match.group(1) == "fig":
                                         yield ImagePreview(match.group(2), messages[-1]["content"])
                                     else:
                                         yield ImageResponse(match.group(2), match.group(1))
```

### Comparing `g4f-0.3.1.2/g4f/Provider/__init__.py` & `g4f-0.3.1.3/g4f/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/bing/conversation.py` & `g4f-0.3.1.3/g4f/Provider/bing/conversation.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/bing/create_images.py` & `g4f-0.3.1.3/g4f/Provider/bing/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/bing/upload_image.py` & `g4f-0.3.1.3/g4f/Provider/bing/upload_image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Acytoo.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Acytoo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/AiAsk.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/AiAsk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/AiChatOnline.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/AiChatOnline.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/AiService.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/AiService.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Aibn.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Aibn.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Aichat.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Aichat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Ails.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Ails.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Aivvm.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Aivvm.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Berlin.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Berlin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/ChatAnywhere.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/ChatAnywhere.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/ChatgptDuo.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/ChatgptDuo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/CodeLinkAva.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/CodeLinkAva.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Cromicle.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Cromicle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/DfeHub.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/DfeHub.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/EasyChat.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/EasyChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Equing.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Equing.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/FakeGpt.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/FakeGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/FastGpt.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/FastGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Forefront.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Forefront.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/GPTalk.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/GPTalk.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/GeekGpt.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/GeekGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/GetGpt.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/GetGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/H2o.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/H2o.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Hashnode.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Hashnode.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Lockchat.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Lockchat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Myshell.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Myshell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/NoowAi.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/NoowAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Opchatgpts.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Opchatgpts.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/OpenAssistant.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/OpenAssistant.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Phind.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/V50.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/V50.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Vercel.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Vercel.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Vitalentum.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Vitalentum.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/VoiGpt.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/VoiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Wewordle.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Wewordle.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Wuguokai.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Wuguokai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Ylokh.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Ylokh.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/Yqcloud.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/Yqcloud.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/deprecated/__init__.py` & `g4f-0.3.1.3/g4f/Provider/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt` & `g4f-0.3.1.3/g4f/Provider/gigachat_crt/russian_trusted_root_ca_pem.crt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/Gemini.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/Gemini.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/Groq.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/Groq.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/OpenRouter.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/OpenRouter.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/Openai.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/Openai.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/OpenaiChat.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/OpenaiChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/PerplexityApi.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/PerplexityApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/Poe.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/Poe.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/Raycast.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/Raycast.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/Theb.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/Theb.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/needs_auth/ThebApi.py` & `g4f-0.3.1.3/g4f/Provider/needs_auth/ThebApi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/AItianhu.py` & `g4f-0.3.1.3/g4f/Provider/not_working/AItianhu.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/Bestim.py` & `g4f-0.3.1.3/g4f/Provider/not_working/Bestim.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/ChatBase.py` & `g4f-0.3.1.3/g4f/Provider/not_working/ChatBase.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemo.py` & `g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/ChatgptDemoAi.py` & `g4f-0.3.1.3/g4f/Provider/not_working/ChatgptDemoAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/ChatgptLogin.py` & `g4f-0.3.1.3/g4f/Provider/not_working/ChatgptLogin.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/Chatxyz.py` & `g4f-0.3.1.3/g4f/Provider/not_working/Chatxyz.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/Gpt6.py` & `g4f-0.3.1.3/g4f/Provider/not_working/Gpt6.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/GptChatly.py` & `g4f-0.3.1.3/g4f/Provider/not_working/GptChatly.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/GptForLove.py` & `g4f-0.3.1.3/g4f/Provider/not_working/GptForLove.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/GptGo.py` & `g4f-0.3.1.3/g4f/Provider/not_working/GptGo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/GptGod.py` & `g4f-0.3.1.3/g4f/Provider/not_working/GptGod.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/not_working/OnlineGpt.py` & `g4f-0.3.1.3/g4f/Provider/not_working/OnlineGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/README.md` & `g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/README.md`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js` & `g4f-0.3.1.3/g4f/Provider/npm/node_modules/crypto-js/crypto-js.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/npm/package-lock.json` & `g4f-0.3.1.3/g4f/Provider/npm/package-lock.json`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/openai/crypt.py` & `g4f-0.3.1.3/g4f/Provider/openai/crypt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/openai/har_file.py` & `g4f-0.3.1.3/g4f/Provider/openai/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/openai/proofofwork.py` & `g4f-0.3.1.3/g4f/Provider/openai/proofofwork.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/selenium/AItianhuSpace.py` & `g4f-0.3.1.3/g4f/Provider/selenium/AItianhuSpace.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/selenium/Bard.py` & `g4f-0.3.1.3/g4f/Provider/selenium/Bard.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/selenium/MyShell.py` & `g4f-0.3.1.3/g4f/Provider/selenium/MyShell.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/selenium/PerplexityAi.py` & `g4f-0.3.1.3/g4f/Provider/selenium/PerplexityAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/selenium/Phind.py` & `g4f-0.3.1.3/g4f/Provider/selenium/Phind.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/selenium/TalkAi.py` & `g4f-0.3.1.3/g4f/Provider/selenium/TalkAi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/unfinished/AiChatting.py` & `g4f-0.3.1.3/g4f/Provider/unfinished/AiChatting.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/unfinished/ChatAiGpt.py` & `g4f-0.3.1.3/g4f/Provider/unfinished/ChatAiGpt.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/unfinished/Komo.py` & `g4f-0.3.1.3/g4f/Provider/unfinished/Komo.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/unfinished/MikuChat.py` & `g4f-0.3.1.3/g4f/Provider/unfinished/MikuChat.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/Provider/you/har_file.py` & `g4f-0.3.1.3/g4f/Provider/you/har_file.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/__init__.py` & `g4f-0.3.1.3/g4f/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/api/__init__.py` & `g4f-0.3.1.3/g4f/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,18 @@
             }
             model_list = [{
                 'id': model_id,
                 'object': 'model',
                 'created': 0,
                 'owned_by': model.base_provider
             } for model_id, model in model_list.items()]
-            return JSONResponse(model_list)
+            return JSONResponse({
+                "object": "list",
+                "data": model_list,
+            })
 
         @self.app.get("/v1/models/{model_name}")
         async def model_info(model_name: str):
             try:
                 model_info = g4f.models.ModelUtils.convert[model_name]
                 return JSONResponse({
                     'id': model_name,
```

### Comparing `g4f-0.3.1.2/g4f/api/_logging.py` & `g4f-0.3.1.3/g4f/api/_logging.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/cli.py` & `g4f-0.3.1.3/g4f/cli.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/client/async_client.py` & `g4f-0.3.1.3/g4f/client/async_client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/client/client.py` & `g4f-0.3.1.3/g4f/client/client.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/client/helper.py` & `g4f-0.3.1.3/g4f/client/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/client/image_models.py` & `g4f-0.3.1.3/g4f/client/image_models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/client/service.py` & `g4f-0.3.1.3/g4f/client/service.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/client/stubs.py` & `g4f-0.3.1.3/g4f/stubs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from __future__ import annotations
 
 from typing import Union
 
 class Model():
     ...
 
@@ -99,8 +100,8 @@
     def __init__(self, url: str) -> None:
         self.url = url
 
 class ImagesResponse(Model):
     data: list[Image]
 
     def __init__(self, data: list) -> None:
-        self.data = data
+        self.data = data
```

### Comparing `g4f-0.3.1.2/g4f/client/types.py` & `g4f-0.3.1.3/g4f/client/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/cookies.py` & `g4f-0.3.1.3/g4f/cookies.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/errors.py` & `g4f-0.3.1.3/g4f/errors.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/__init__.py` & `g4f-0.3.1.3/g4f/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/index.html` & `g4f-0.3.1.3/g4f/gui/client/index.html`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/css/dracula.min.css` & `g4f-0.3.1.3/g4f/gui/client/static/css/dracula.min.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/css/style.css` & `g4f-0.3.1.3/g4f/gui/client/static/css/style.css`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-192x192.png` & `g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/img/android-chrome-512x512.png` & `g4f-0.3.1.3/g4f/gui/client/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/img/apple-touch-icon.png` & `g4f-0.3.1.3/g4f/gui/client/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/img/favicon-32x32.png` & `g4f-0.3.1.3/g4f/gui/client/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/img/gpt.png` & `g4f-0.3.1.3/g4f/gui/client/static/img/gpt.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/img/user.png` & `g4f-0.3.1.3/g4f/gui/client/static/img/user.png`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/js/chat.v1.js` & `g4f-0.3.1.3/g4f/gui/client/static/js/chat.v1.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/js/highlight.min.js` & `g4f-0.3.1.3/g4f/gui/client/static/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/js/highlightjs-copy.min.js` & `g4f-0.3.1.3/g4f/gui/client/static/js/highlightjs-copy.min.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/js/icons.js` & `g4f-0.3.1.3/g4f/gui/client/static/js/icons.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/630.index.js` & `g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/630.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/900.index.js` & `g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/900.index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/client/static/js/text_to_speech/index.js` & `g4f-0.3.1.3/g4f/gui/client/static/js/text_to_speech/index.js`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/server/android_gallery.py` & `g4f-0.3.1.3/g4f/gui/server/android_gallery.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/server/api.py` & `g4f-0.3.1.3/g4f/gui/server/api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/server/backend.py` & `g4f-0.3.1.3/g4f/gui/server/backend.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/server/config.py` & `g4f-0.3.1.3/g4f/gui/server/config.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/server/internet.py` & `g4f-0.3.1.3/g4f/gui/server/internet.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/server/js_api.py` & `g4f-0.3.1.3/g4f/gui/server/js_api.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/server/website.py` & `g4f-0.3.1.3/g4f/gui/server/website.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/gui/webview.py` & `g4f-0.3.1.3/g4f/gui/webview.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/image.py` & `g4f-0.3.1.3/g4f/image.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/local/__init__.py` & `g4f-0.3.1.3/g4f/local/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/locals/models.py` & `g4f-0.3.1.3/g4f/locals/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/locals/provider.py` & `g4f-0.3.1.3/g4f/locals/provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/models.py` & `g4f-0.3.1.3/g4f/models.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/providers/base_provider.py` & `g4f-0.3.1.3/g4f/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/providers/create_images.py` & `g4f-0.3.1.3/g4f/providers/create_images.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/providers/helper.py` & `g4f-0.3.1.3/g4f/providers/helper.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/providers/retry_provider.py` & `g4f-0.3.1.3/g4f/providers/retry_provider.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/providers/types.py` & `g4f-0.3.1.3/g4f/providers/types.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/requests/__init__.py` & `g4f-0.3.1.3/g4f/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/requests/aiohttp.py` & `g4f-0.3.1.3/g4f/requests/aiohttp.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/requests/curl_cffi.py` & `g4f-0.3.1.3/g4f/requests/curl_cffi.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/requests/defaults.py` & `g4f-0.3.1.3/g4f/requests/defaults.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/requests/raise_for_status.py` & `g4f-0.3.1.3/g4f/requests/raise_for_status.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/stubs.py` & `g4f-0.3.1.3/g4f/client/stubs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from __future__ import annotations
 
 from typing import Union
 
 class Model():
     ...
 
@@ -75,20 +74,22 @@
 
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
@@ -100,8 +101,8 @@
     def __init__(self, url: str) -> None:
         self.url = url
 
 class ImagesResponse(Model):
     data: list[Image]
 
     def __init__(self, data: list) -> None:
-        self.data = data
+        self.data = data
```

### Comparing `g4f-0.3.1.2/g4f/typing.py` & `g4f-0.3.1.3/g4f/typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 SHA256 = NewType('sha_256_hash', str)
 CreateResult = Iterator[str]
 AsyncResult = AsyncIterator[str]
-Messages = List[Dict[str, str]]
+Messages = List[Dict[str, Union[str,List[Dict[str,Union[str,Dict[str,str]]]]]]]
 Cookies = Dict[str, str]
 ImageType = Union[str, bytes, IO, Image, None]
 
 __all__ = [
     'Any',
     'AsyncGenerator',
     'Generator',
```

### Comparing `g4f-0.3.1.2/g4f/version.py` & `g4f-0.3.1.3/g4f/version.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f/webdriver.py` & `g4f-0.3.1.3/g4f/webdriver.py`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f.egg-info/PKG-INFO` & `g4f-0.3.1.3/g4f.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g4f
-Version: 0.3.1.2
+Version: 0.3.1.3
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
-Metadata-Version: 2.1 Name: g4f Version: 0.3.1.2 Summary: The official gpt4free
+Metadata-Version: 2.1 Name: g4f Version: 0.3.1.3 Summary: The official gpt4free
 repository | various collection of powerful language models Home-page: https://
 github.com/xtekky/gpt4free Author: Tekky Author-email:
 g4f.ai> Project-URL: Source Code, https://github.com/xtekky/gpt4free Project-
 URL: Bug Tracker, https://github.com/xtekky/gpt4free/issues Keywords:
 python,chatbot,reverse-engineering,openai,chatbots,gpt,language-model,gpt-
 3,gpt3,openai-api,gpt-4,gpt4,chatgpt,chatgpt-api,openai-chatgpt,chatgpt-
 free,chatgpt-4,chatgpt4,chatgpt4-api,free,free-gpt,gpt4free,g4f Classifier:
```

### Comparing `g4f-0.3.1.2/g4f.egg-info/SOURCES.txt` & `g4f-0.3.1.3/g4f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/g4f.egg-info/requires.txt` & `g4f-0.3.1.3/g4f.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `g4f-0.3.1.2/setup.py` & `g4f-0.3.1.3/setup.py`

 * *Files identical despite different names*

