# Comparing `tmp/zibuyu_LLM-0.1.9-py3-none-any.whl.zip` & `tmp/zibuyu_LLM-2.1.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,23 @@
-Zip file size: 67284 bytes, number of entries: 18
+Zip file size: 79335 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat      305 b- defN 24-May-11 08:41 zibuyu_llm_api/__init__.py
--rw-rw-rw-  2.0 fat    31879 b- defN 24-May-11 08:41 zibuyu_llm_api/minmax_api.py
--rw-rw-rw-  2.0 fat      735 b- defN 24-May-11 08:46 zibuyu_llm_web/__init__.py
+-rw-rw-rw-  2.0 fat    30976 b- defN 24-May-16 04:34 zibuyu_llm_api/minmax_api.py
+-rw-rw-rw-  2.0 fat      909 b- defN 24-May-17 16:06 zibuyu_llm_web/__init__.py
 -rw-rw-rw-  2.0 fat     7376 b- defN 24-May-11 14:22 zibuyu_llm_web/baichuan.py
--rw-rw-rw-  2.0 fat     7104 b- defN 24-May-12 05:31 zibuyu_llm_web/base.py
--rw-rw-rw-  2.0 fat    14789 b- defN 24-May-11 14:25 zibuyu_llm_web/deepseek.py
--rw-rw-rw-  2.0 fat      732 b- defN 24-May-11 08:49 zibuyu_llm_web/errors.py
--rw-rw-rw-  2.0 fat     9962 b- defN 24-May-11 14:22 zibuyu_llm_web/kimi.py
--rw-rw-rw-  2.0 fat    37747 b- defN 24-May-12 02:39 zibuyu_llm_web/minmax.py
+-rw-rw-rw-  2.0 fat     8509 b- defN 24-May-17 16:48 zibuyu_llm_web/base.py
+-rw-rw-rw-  2.0 fat    15556 b- defN 24-May-17 16:17 zibuyu_llm_web/deepseek.py
+-rw-rw-rw-  2.0 fat     2783 b- defN 24-May-17 13:53 zibuyu_llm_web/emohaa.py
+-rw-rw-rw-  2.0 fat      807 b- defN 24-May-12 10:11 zibuyu_llm_web/errors.py
+-rw-rw-rw-  2.0 fat    11202 b- defN 24-May-16 01:36 zibuyu_llm_web/kimi.py
+-rw-rw-rw-  2.0 fat    11531 b- defN 24-May-17 16:17 zibuyu_llm_web/metaso.py
+-rw-rw-rw-  2.0 fat    44926 b- defN 24-May-18 09:38 zibuyu_llm_web/minmax.py
 -rw-rw-rw-  2.0 fat    37730 b- defN 24-May-11 13:49 zibuyu_llm_web/qwen.py
--rw-rw-rw-  2.0 fat     5308 b- defN 24-May-12 03:43 zibuyu_llm_web/types.py
--rw-rw-rw-  2.0 fat     8118 b- defN 24-May-11 08:37 zibuyu_llm_web/wanxiang.py
--rw-rw-rw-  2.0 fat    14705 b- defN 24-May-11 14:25 zibuyu_llm_web/xinchen.py
--rw-rw-rw-  2.0 fat    55663 b- defN 24-May-12 05:50 zibuyu_llm_web/xunfei.py
--rw-rw-rw-  2.0 fat     1621 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       30 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1455 b- defN 24-May-12 05:51 zibuyu_LLM-0.1.9.dist-info/RECORD
-18 files, 235351 bytes uncompressed, 64926 bytes compressed:  72.4%
+-rw-rw-rw-  2.0 fat    14134 b- defN 24-May-18 12:42 zibuyu_llm_web/step_chat.py
+-rw-rw-rw-  2.0 fat     5355 b- defN 24-May-18 09:50 zibuyu_llm_web/types.py
+-rw-rw-rw-  2.0 fat     8097 b- defN 24-May-17 14:20 zibuyu_llm_web/wanxiang.py
+-rw-rw-rw-  2.0 fat    14705 b- defN 24-May-17 14:20 zibuyu_llm_web/xinchen.py
+-rw-rw-rw-  2.0 fat    62458 b- defN 24-May-16 05:13 zibuyu_llm_web/xunfei.py
+-rw-rw-rw-  2.0 fat     1739 b- defN 24-May-18 12:44 zibuyu_LLM-2.1.19.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 12:44 zibuyu_LLM-2.1.19.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       30 b- defN 24-May-18 12:44 zibuyu_LLM-2.1.19.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1708 b- defN 24-May-18 12:44 zibuyu_LLM-2.1.19.dist-info/RECORD
+21 files, 280928 bytes uncompressed, 76591 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -12,44 +12,53 @@
 
 Filename: zibuyu_llm_web/base.py
 Comment: 
 
 Filename: zibuyu_llm_web/deepseek.py
 Comment: 
 
+Filename: zibuyu_llm_web/emohaa.py
+Comment: 
+
 Filename: zibuyu_llm_web/errors.py
 Comment: 
 
 Filename: zibuyu_llm_web/kimi.py
 Comment: 
 
+Filename: zibuyu_llm_web/metaso.py
+Comment: 
+
 Filename: zibuyu_llm_web/minmax.py
 Comment: 
 
 Filename: zibuyu_llm_web/qwen.py
 Comment: 
 
+Filename: zibuyu_llm_web/step_chat.py
+Comment: 
+
 Filename: zibuyu_llm_web/types.py
 Comment: 
 
 Filename: zibuyu_llm_web/wanxiang.py
 Comment: 
 
 Filename: zibuyu_llm_web/xinchen.py
 Comment: 
 
 Filename: zibuyu_llm_web/xunfei.py
 Comment: 
 
-Filename: zibuyu_LLM-0.1.9.dist-info/METADATA
+Filename: zibuyu_LLM-2.1.19.dist-info/METADATA
 Comment: 
 
-Filename: zibuyu_LLM-0.1.9.dist-info/WHEEL
+Filename: zibuyu_LLM-2.1.19.dist-info/WHEEL
 Comment: 
 
-Filename: zibuyu_LLM-0.1.9.dist-info/top_level.txt
+Filename: zibuyu_LLM-2.1.19.dist-info/top_level.txt
 Comment: 
 
-Filename: zibuyu_LLM-0.1.9.dist-info/RECORD
+Filename: zibuyu_LLM-2.1.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zibuyu_llm_api/minmax_api.py

```diff
@@ -218,40 +218,42 @@
                 if response.status != 200 or "json" in response.headers["Content-Type"]:
                     print("调用失败！", f"状态码为：【{response.status_code}】")
                     print(response.text)
                     return False
                 with open(file_path, "wb") as f:
                     f.write(await response.content.read())
 
-    async def async_text2voice(self, text: str,
-                               file_path: str,
-                               pitch: int = 0,
-                               vol: float = 2.0,
-                               speed: float = 1.0,
-                               output_format: str = 'mp3',
-                               voice_id: str = 'male-qn-qingse',
-                               model: str = 'speech-02',
-                               char_to_pitch: list[str] = None,
-                               timber_weights: list[dict] = None,
-                               ):
+    async def async_text2voice(
+            self, text: str,
+            file_path: str,
+            pitch: int = 0,
+            vol: float = 2.0,
+            speed: float = 1.0,
+            output_format: str = 'mp3',
+            voice_id: str = 'male-qn-qingse',
+            model: str = 'speech-02',
+            char_to_pitch: list[str] = None,
+            timber_weights: list[dict] = None,
+    ):
 
         data = self.check_request_data(text, pitch, vol, speed, output_format, voice_id, model,
                                        char_to_pitch, timber_weights)
         return await self._async_text2voice(file_path, data)
 
-    async def _text2voice_list(self, text_list: list[str],
-                               file_path_list: list[str],
-                               pitch: int = 0,
-                               vol: float = 2.0,
-                               speed: float = 1.0,
-                               output_format: str = 'mp3',
-                               voice_id: str = 'male-qn-qingse',
-                               model: str = 'speech-02',
-                               char_to_pitch: list[str] = None,
-                               timber_weights: list[dict] = None):
+    async def _text2voice_list(
+            self, text_list: list[str],
+            file_path_list: list[str],
+            pitch: int = 0,
+            vol: float = 2.0,
+            speed: float = 1.0,
+            output_format: str = 'mp3',
+            voice_id: str = 'male-qn-qingse',
+            model: str = 'speech-02',
+            char_to_pitch: list[str] = None,
+            timber_weights: list[dict] = None):
 
         if len(text_list) != len(file_path_list):
             raise ValueError(f'输入的文本和文件路径数量不匹配！')
 
         task_list = []
         for text, file_path in zip(text_list, file_path_list):
             task = asyncio.create_task(
@@ -263,24 +265,25 @@
         while True:
 
             if all([task.done() for task in task_list]):
                 return True
             else:
                 await asyncio.sleep(0.2)
 
-    def text2voice_list(self, text_list: list[str],
-                        file_path_list: list[str],
-                        pitch: int = 0,
-                        vol: float = 2.0,
-                        speed: float = 1.0,
-                        output_format: str = 'mp3',
-                        voice_id: str = 'male-qn-qingse',
-                        model: str = 'speech-02',
-                        char_to_pitch: list[str] = None,
-                        timber_weights: list[dict] = None):
+    def text2voice_list(
+            self, text_list: list[str],
+            file_path_list: list[str],
+            pitch: int = 0,
+            vol: float = 2.0,
+            speed: float = 1.0,
+            output_format: str = 'mp3',
+            voice_id: str = 'male-qn-qingse',
+            model: str = 'speech-02',
+            char_to_pitch: list[str] = None,
+            timber_weights: list[dict] = None):
 
         """
         异步合成多个语音
         :param text_list: 需合成的文本列表
         :param file_path_list: 合成语音的存放路径，列表个数需与text_list一致
         :param pitch:
         :param vol:
@@ -316,24 +319,25 @@
             print("调用失败！", f"状态码为：【{response.status_code}】")
             print(response.text)
             return False
         with open(file_path, "wb") as f:
             f.write(response.content)
         return True
 
-    def text2voice(self, text: str,
-                   file_path: str,
-                   pitch: int = 0,
-                   vol: float = 2.0,
-                   speed: float = 1.0,
-                   output_format: str = 'mp3',
-                   voice_id: str = 'male-qn-qingse',
-                   model: str = 'speech-02',
-                   char_to_pitch: list[str] = None,
-                   timber_weights: list[dict] = None, ):
+    def text2voice(
+            self, text: str,
+            file_path: str,
+            pitch: int = 0,
+            vol: float = 2.0,
+            speed: float = 1.0,
+            output_format: str = 'mp3',
+            voice_id: str = 'male-qn-qingse',
+            model: str = 'speech-02',
+            char_to_pitch: list[str] = None,
+            timber_weights: list[dict] = None, ):
         """
         文本转语音
         :param text: 文本
         :param file_path: 音频路径
         :param pitch: 音调大小，范围[-12, 12]，0为原音色输出，取值需为整数
         :param vol: 音量大小，范围(0, 10]，取值越大，音量越高
         :param speed: 语速大小，范围[0.5, 2]，取值越大，语速越高
@@ -357,25 +361,26 @@
 
         payload = {}
 
         response = requests.request("GET", url, headers=self.headers, data=payload)
 
         print(response.text)
 
-    def text2voice_async(self, text_file_path: str,
-                         pitch: int = 0,
-                         vol: float = 2.0,
-                         speed: float = 1.0,
-                         audio_sample_rate: Literal[16000, 24000, 32000] = 32000,
-                         bitrate: Literal[32000, 64000, 128000] = 128000,
-                         output_format: str = 'mp3',
-                         voice_id: str = 'male-qn-qingse',
-                         char_to_pitch: list[str] = None,
-                         timber_weights: list[dict] = None,
-                         ):
+    def text2voice_async(
+            self, text_file_path: str,
+            pitch: int = 0,
+            vol: float = 2.0,
+            speed: float = 1.0,
+            audio_sample_rate: Literal[16000, 24000, 32000] = 32000,
+            bitrate: Literal[32000, 64000, 128000] = 128000,
+            output_format: str = 'mp3',
+            voice_id: str = 'male-qn-qingse',
+            char_to_pitch: list[str] = None,
+            timber_weights: list[dict] = None,
+    ):
         """
         文本转语音，超长文本版，最高支持1000万字符。仅支持speech-01
         :param text_file_path: 长度限制<10000000字符，格式为zip。打包上传，包里应只包含txt或json文件（压缩包内为同一格式文件），
             json文件会有三个字段，["title", "content", "extra"]，分别表示标题，正文，作者。
             json里会有三个字段，["title", "content", "extra"]，分别是标题，正文，作者的话，
             需要产出三份结果，一共9个文件放在一个文件夹里。如果某字段不存在，或者内容为空，则不生成相应文件。
         :param pitch: 音调大小，范围[-12, 12]，0为原音色输出，取值需为整数
@@ -401,27 +406,28 @@
 
         result = requests.post(self.text2text_large_url, headers=self.headers, json=data)
 
         print(result.text)
         with open(text_file_path.replace('.zip', '(任务记录).txt'), mode='w', encoding='utf-8') as f:
             f.write(result.text)
 
-    def text2voice_long_text(self, text: str,
-                             file_path: str,
-                             pitch: int = 0,
-                             vol: float = 2.0,
-                             speed: float = 1.0,
-                             audio_sample_rate: Literal[16000, 24000, 32000] = 32000,
-                             bitrate: Literal[32000, 64000, 128000] = 128000,
-                             output_format: str = 'mp3',
-                             voice_id: str = 'male-qn-qingse',
-                             model: str = 'speech-02',
-                             char_to_pitch: list[str] = None,
-                             timber_weights: list[dict] = None,
-                             ):
+    def text2voice_long_text(
+            self, text: str,
+            file_path: str,
+            pitch: int = 0,
+            vol: float = 2.0,
+            speed: float = 1.0,
+            audio_sample_rate: Literal[16000, 24000, 32000] = 32000,
+            bitrate: Literal[32000, 64000, 128000] = 128000,
+            output_format: str = 'mp3',
+            voice_id: str = 'male-qn-qingse',
+            model: str = 'speech-02',
+            char_to_pitch: list[str] = None,
+            timber_weights: list[dict] = None,
+    ):
         """
         文本转语音，长文本版，长度限制<50000字符
         :param text: 文本
         :param file_path: 音频路径
         :param pitch: 音调大小，范围[-12, 12]，0为原音色输出，取值需为整数
         :param vol: 音量大小，范围(0, 10]，取值越大，音量越高
         :param speed: 语速大小，范围[0.5, 2]，取值越大，语速越高
@@ -493,21 +499,22 @@
         if not isinstance(value, float):
             raise TypeError(f'top_p参数类型错误，应为float！')
         if not 0 < value <= 1:
             raise ValueError(f'top_p参数范围错误，应为(0,1]！')
         self.top_p = value
         return self.top_p
 
-    def check_params(self,
-                     prompt: str = "",
-                     model: str = "abab5.5s-chat",
-                     tokens_to_generate: int = 1024,
-                     temperature: float = 0.9,
-                     top_p: float = 0.9,
-                     stream: bool = False, ) -> dict:
+    def check_params(
+            self,
+            prompt: str = "",
+            model: str = "abab5.5s-chat",
+            tokens_to_generate: int = 1024,
+            temperature: float = 0.9,
+            top_p: float = 0.9,
+            stream: bool = False, ) -> dict:
         """
         检查输入的各个参数是否符合要求
         :param stream:
         :param prompt:
         :param model:
         :param tokens_to_generate:
         :param temperature:
@@ -535,24 +542,25 @@
         }
 
         if prompt:
             payload['prompt'] = prompt
 
         return payload
 
-    def ask_normal(self, question: str,
-                   prompt: str = "",
-                   stream: bool = False,
-                   model: str = "abab5.5s-chat",
-                   tokens_to_generate: int = 1024,
-                   temperature: float = 0.9,
-                   top_p: float = 0.9,
-                   messages: list[MessageNormal] = None,
-                   callback_func=None,
-                   ) -> str:
+    def ask_normal(
+            self, question: str,
+            prompt: str = "",
+            stream: bool = False,
+            model: str = "abab5.5s-chat",
+            tokens_to_generate: int = 1024,
+            temperature: float = 0.9,
+            top_p: float = 0.9,
+            messages: list[MessageNormal] = None,
+            callback_func=None,
+    ) -> str:
         """
         文本生成普通接口，基于自然语言交互的文本生成能力接口
         不包含功能支持，比如：多人对话、对话示例，支持集合搜索引擎、调用自定义函数、限制返回格式等。
         :param question: 提问的文本
         :param prompt: prompt，不提供时将使用内置prompt
         :param stream: 是否流式输出
         :param model: 大模型的版本
```

## zibuyu_llm_web/__init__.py

```diff
@@ -14,23 +14,31 @@
 from .xinchen import XinChenWeb
 from .xunfei import XunFeiWeb
 from .kimi import KimiWeb
 from .minmax import MinMaxWeb
 from .deepseek import DeepSeekWeb
 from .baichuan import BaiChuanWeb
 from .wanxiang import WanXiangWeb
+from .metaso import MetaSoWeb
+from .emohaa import EmohaaWeb
+from .base import LLMBase, END_SIGNAL
 from . import errors
 from . import types
 
-
 __all__ = [
-    'QwenWeb',
-    'XinChenWeb',
-    'XunFeiWeb',
+    'LLMBase',
+    'END_SIGNAL',
+
+    'BaiChuanWeb',
+    'DeepSeekWeb',
+    'EmohaaWeb',
     'KimiWeb',
+    'MetaSoWeb',
     'MinMaxWeb',
-    'DeepSeekWeb',
-    'BaiChuanWeb',
+    'QwenWeb',
     'WanXiangWeb',
+    'XinChenWeb',
+    'XunFeiWeb',
+
     'errors',
     'types'
 ]
```

## zibuyu_llm_web/base.py

```diff
@@ -11,16 +11,20 @@
 各类AI平台的逆向，均需继承LLMBase类：
     - 定义类变量 model_name ；用于存放错误信息时，区分不同平台
     - 定义 ask 方法；该实现AI文本交互，如果cookie过期，需抛出NeedLoginError错误；
     - 流式输出时，最后需返回结束符号 END_SIGNAL；
     - 在子类的初始化方法中，调用super().__init__()之前，必须先传入自己的logger，否则将新建logger；
 --------------------------------------------
 """
-
+import base64
+import json
+import re
 import os
+from typing import Union, Optional
+
 import urllib3
 import logging
 import datetime
 
 import requests
 from fake_useragent import UserAgent
 
@@ -198,7 +202,44 @@
         )
 
         file_handler.setLevel(logging.DEBUG)
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
 
         return logger
+
+    @staticmethod
+    def is_valid_cn_phone(phone_number: Union[str, int]) -> bool:
+        """检查输入的国内手机号码是否正确"""
+
+        pattern = r'^1[3-9]\d{9}$'
+        return bool(re.match(pattern, phone_number))
+
+    @staticmethod
+    def is_valid_email(email):
+        """检查输入的邮箱地址是否正确"""
+
+        pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
+        return bool(re.match(pattern, email))
+
+    @staticmethod
+    def add_padding_to_base64(s):
+        """为base64字符串添加缺失的=号"""
+
+        missing_padding = 4 - (len(s) % 4)
+        if missing_padding == 4:
+            return s  # 已经是4的倍数，不需要添加填充
+        return s + '=' * missing_padding  # 添加缺失的填充字符
+
+    def parse_jwt_token(self, token_str: str) -> Optional[dict]:
+        """解析JWT Token，获取载荷部分信息 """
+
+        try:
+
+            first_data = token_str.split('.')[1]
+            padded_payload = self.add_padding_to_base64(first_data)
+            data = json.loads(base64.b64decode(padded_payload).decode())
+
+            self.logger.info(f"解析JWT Token成功：【{data}】")
+            return data
+        except:
+            self.logger.error(f"解析JWT Token失败：【{token_str}】")
```

## zibuyu_llm_web/deepseek.py

```diff
@@ -10,18 +10,17 @@
 
 已完全逆向，注册、登录、自动管理Token。
 
 该平台的邮箱注册仅支持海外IP
 --------------------------------------------
 """
 
+import re
 import json
 import logging
-import re
-from typing import Optional
 
 from .base import LLMBase
 from .types import AiAnswer
 from .errors import NeedLoginError
 
 # 在发送手机或邮件验证码时，需要携带这个参数；该参数目前为固定值
 TURNSTILE_TOKEN = '0.m0l729JxhJEkMRTF3KmaamhsRl0HLUZUVJgQcwaMzJsEHhpZ1YGHhSCPZwP9yWV2N_-rUdwI4P8A5Xm1Kl4ZLxCtFRA5je-3TJhcPkUinVuJwIzBvIah1DILaSEhNo-Ws89CX0TORBX9birCRNY6t3e6Fmsgxvo60mrtmRTkpd5k8jDyRweAqXiILJBkK_EzwwOq9pWHD_HEJjQ5KiId-8FcN18_m3UGUrUQXAQLOMTxqcs9g9tIjseyM81mB-C7HOHrdXhfQqiYX-wdiLa4NqqHgbiZUwP4d_IWWgloS9EAdLtJQQoiMPUjI5gkAGOmtNCFX3RcAQca4jsfod8DzTcYmCd03HJMZsXNr7A8dFegaLxzxWu9-I6TdTMfjaCI-Wzra1KN4BiSP_eWEK_Uz8hYzO3Ohj_Nonm3EpGnABeplDzqiteRunXESzatMv_4.aJXkGwUBtqKoVH0R5DFm3Q.656f25ad10112a3a66a6b5f8a480daedb469eb74c98722855441b164bbdad82c'
@@ -77,27 +76,33 @@
             'Priority': "u=1, i",
             "Sec-Ch-Ua": '"Chromium";v="124", "Google Chrome";v="124", "Not-A.Brand";v="99"',
             "Sec-Ch-Ua-Mobile": "?0",
             "Sec-Ch-Ua-Platform": '"Windows"',
             "User-Agent": self.user_agent,
         }
 
-        self.single_answer_obj: Optional[AiAnswer] = None
-        self.__single_answer: str = ''
-        self.__single_padding: str = ''
+        self.single_answer_obj: AiAnswer = AiAnswer()
+        self.__single_answer: str = ''  # 单次交互的回复内容
+        self.__single_padding: str = ''  # 单次交互的padding内容
 
     @property
     def token(self):
 
         if self._token:
             return self._token
         self.login()
         return self._token
 
     def __ask(self, question: str, model: str, callback_func=None):
+        """
+        :param question: 问题
+        :param model: 模型(通用助手或代码助手)
+        :param callback_func: 回调函数
+        :return:
+        """
 
         uri = '/api/v0/chat/completions'
 
         headers = self.__headers.copy()
         headers['Authorization'] = f'Bearer {self.token}'
         headers['Content-Type'] = 'application/json'
         headers['Referer'] = 'https://chat.deepseek.com/'
@@ -156,18 +161,16 @@
                         callback_func(self.end_signal)
                     except:
                         self.logger.error(f'回调函数【{callback_func.__name__}】执行失败', exc_info=True)
 
             if self.__single_padding:
                 self.__single_answer += self.__single_padding
 
-        self.single_answer_obj = AiAnswer(
-            content=self.__single_answer,
-            is_success=True,
-        )
+        self.single_answer_obj.content = self.__single_answer
+        self.single_answer_obj.is_success = True
 
         return self.single_answer_obj
 
     def __get_history(self, model: str, referer: str) -> dict:
         uri = '/api/v0/chat/history'
 
         params = {
@@ -208,15 +211,16 @@
             data = {
                 "email": "",
                 "mobile": self.account_phone,
                 "password": self.password,
                 "area_code": "+86"
             }
         else:
-            raise Exception('未传入账号信息【手机号或邮箱】')
+            self.logger.error('未传入账号信息【手机号或邮箱】，停止登录')
+            return False
 
         headers = self.__headers.copy()
 
         headers['Content-Type'] = 'application/json'
 
         try:
             response = self.request_session.post(
@@ -274,28 +278,49 @@
     def ask_code(self, question: str, callback_func=None) -> AiAnswer:
         """
         代码助手
         :param question:
         :param callback_func:
         :return:
         """
-
         model = "deepseek_code"
-        return self.__ask(question, model, callback_func=callback_func)
+
+        for i in range(3):
+
+            try:
+                return self.__ask(question, model, callback_func=callback_func)
+            except:
+                self.logger.error(f'ask_code方法请求失败！', exc_info=True)
+                self.logger.info(f'尝试重新登录，后再发送请求。')
+
+                if not self.login():
+                    self.logger.error(f'重新登录失败')
+                    return self.single_answer_obj
 
     def ask(self, question: str, callback_func=None) -> AiAnswer:
         """
         通用助手
         :param question:
         :param callback_func:
         :return:
         """
 
         model = "deepseek_chat"
-        return self.__ask(question, model, callback_func=callback_func)
+
+        for i in range(3):
+
+            try:
+                return self.__ask(question, model, callback_func=callback_func)
+            except:
+                self.logger.error(f'ask方法请求失败！', exc_info=True)
+                self.logger.info(f'尝试重新登录，后再发送请求。')
+
+                if not self.login():
+                    self.logger.error(f'重新登录失败')
+                    return self.single_answer_obj
 
     def get_chat_history(self):
         """
         获取通用助手聊天记录
         :return:
         """
 
@@ -311,14 +336,16 @@
         """
 
         model = "deepseek_code"
         referer = 'https://chat.deepseek.com/coder'
         data = self.__get_history(model, referer)
         return data
 
+    # #################### 注册相关 ####################
+
     def get_register_header(self):
         """获取注册相关请求时所需的请求头"""
 
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json'
         headers['Referer'] = 'https://chat.deepseek.com/sign_up'
         headers['Origin'] = 'https://chat.deepseek.com'
@@ -363,16 +390,16 @@
             "locale": "zh_CN",
             "turnstile_token": TURNSTILE_TOKEN,
         }
         return self.send_code(uri=uri, data=data)
 
     def send_phone_code(self, phone: str):
 
-        if not self.is_valid_phone_number(phone):
-            self.logger.error(f'手机号格式错误，请检查手机号格式')
+        if not self.is_valid_cn_phone(phone):
+            self.logger.error(f'输入号码【{phone}】不是合法的手机号')
             return False
 
         uri = '/api/v0/users/create_sms_verification_code'
 
         data = {
             "mobile_phone_number": phone,
             "locale": "zh_CN",
@@ -438,17 +465,17 @@
         通过手机号注册
         :param phone: 手机号
         :param code: 手机验证码
         :param password: 密码
         :return: 注册成功时，返回token
         """
 
-        if not self.is_valid_phone_number(phone):
-            self.logger.error(f'手机号格式错误，请检查手机号格式')
-            return
+        if not self.is_valid_cn_phone(phone):
+            self.logger.error(f'输入号码【{phone}】不是合法的国内手机号')
+            return False
 
         uri = '/api/v0/users/register_by_mobile'
 
         data = {
             "locale": "zh_CN",
             "region": "CN",
             "payload": {
@@ -457,17 +484,7 @@
                 "sms_verification_code": code,
                 "audit_json_str": "{\"reasons\":[2,1]}",
                 "password": password or 'ilovedeepseek'
             }
         }
 
         return self.register(uri=uri, data=data)
-
-    @staticmethod
-    def is_valid_phone_number(phone_number):
-        pattern = r'^1[3-9]\d{9}$'
-        return bool(re.match(pattern, phone_number))
-
-    @staticmethod
-    def is_valid_email(email):
-        pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
-        return bool(re.match(pattern, email))
```

## zibuyu_llm_web/errors.py

```diff
@@ -29,7 +29,11 @@
 
 class APIConnectionError(Exception):
     message = "网络连接错误"
 
 
 class SpiderHasToChangeError(Exception):
     message = "网页出现新逻辑，爬虫需要更换"
+
+
+class UnexpectResponseError(Exception):
+    message = "响应异常"
```

## zibuyu_llm_web/kimi.py

```diff
@@ -12,25 +12,24 @@
 
 refresh_token获取方法：
     1. 在官网聊天界面登录后；
     2. 打开开发者模式，在终端输入：window.localStorage.getItem('refresh_token')
 --------------------------------------------
 """
 
+import os
 import json
 import logging
-import os
 from json import JSONDecodeError
-from typing import Optional
 
 import requests
 
+from .base import LLMBase
 from .errors import NeedLoginError
 from .types import ReferenceLink, AiAnswer
-from .base import LLMBase
 
 # 一个用于测试的token，随时可能失效
 TEST_TOKEN = 'eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJ1c2VyLWNlbnRlciIsImV4cCI6MTcyMjQzMTE3MiwiaWF0IjoxNzE0NjU1MTcyLCJqdGkiOiJjb3BvdmgydWw3MjI3dHFodWZoZyIsInR5cCI6InJlZnJlc2giLCJzdWIiOiJjbmc0cDgxa3FxNGg3cDY5dm1nZyIsInNwYWNlX2lkIjoiY24xcGF1bzNyMDdhcmRnNnM0aTAiLCJhYnN0cmFjdF91c2VyX2lkIjoiY24xcGF1bzNyMDdhcmRnNnM0aGcifQ.0zOu2bYYB4OdBtQTFRX5Vo-6hHQC6eqZRX1a3Z40rSGdM2vNQvtHXXFhbcISt_bu6J1vI8aDXlxIB68WbWRQRQ'
 
 
 class KimiWeb(LLMBase):
     """
@@ -42,14 +41,19 @@
 
     def __init__(
             self,
             refresh_token: str = None,
             logger_obj: logging.Logger = None,
             error_dir: str = None
     ):
+        """
+        :param refresh_token: 登录后获取的refresh_token
+        :param logger_obj: 日志对象
+        :param error_dir: 错误日志保存目录
+        """
 
         if not refresh_token:
             self.refresh_token = TEST_TOKEN
         else:
             self.refresh_token = refresh_token
 
         self.logger = logger_obj
@@ -73,23 +77,20 @@
             "sec-fetch-site": "same-origin"
         }
 
         self._chat_id: str = ''
         self.group_id: str = ''
 
         self.single_answer: str = ''
-        self.single_answer_obj: Optional[AiAnswer] = None
+        self.single_answer_obj: AiAnswer = AiAnswer()
 
         self.single_answer_url_list: list = []
 
     def get_new_token(self):
-        """
-        获取新的token
-        :return:
-        """
+        """ 刷新token """
 
         uri = "/api/auth/token/refresh"
 
         headers = self.headers.copy()
         headers['authorization'] = 'Bearer ' + self.refresh_token
 
         response = self.request_session.get(
@@ -106,35 +107,34 @@
         self._access_token = response.json()['access_token']
         self.refresh_token = response.json()['refresh_token']
 
         return self._access_token
 
     @property
     def access_token(self):
+
         if self._access_token:
             return self._access_token
 
         return self.get_new_token()
 
     @property
     def kimi_cookies(self):
         return 'Bearer ' + self.access_token
 
     @property
     def chat_id(self):
+        """ 获取聊天id，Kimi对于会话窗口的管理，是将chat_id嵌入到URL中的 """
         if self._chat_id:
             return self._chat_id
 
         return self.get_chat_id()
 
     def get_chat_id(self):
-        """
-        获取聊天id
-        :return:
-        """
+        """ 获取聊天id """
 
         url = "https://kimi.moonshot.cn/api/chat"
 
         headers = self.headers.copy()
         headers['authorization'] = self.kimi_cookies
 
         data = {
@@ -150,46 +150,54 @@
                 return self._chat_id
         except:
             self.logger.error(f'获取聊天id失败')
 
     def ask(
             self,
             question: str,
+            search_model: bool = True,
             chat_id: str = None,
-            kimiplus_id: str = None,
-            callback_func=None
+            kimi_plus_id: str = None,
+            callback_func=None,
+            perfect_prompt: bool = False
     ) -> AiAnswer:
         """
-        提问
+        向AI提问。
+        Kimi官方提供了一个提示词专家，如果perfect_prompt为真，将自动使用该助手。
         :param question: 向AI交互的文本
+        :param search_model: 是否开启联网搜索
         :param chat_id: 保证上下文
-        :param kimiplus_id: Kimi助手id
+        :param kimi_plus_id: Kimi助手id
         :param callback_func: 回调函数
+        :param perfect_prompt: 是否是优化提示词
         :return:
         """
 
         # 如果用户传入了chat_id，则使用用户的chat_id
         if chat_id:
             self._chat_id = chat_id
 
+        if not kimi_plus_id and perfect_prompt:
+            kimi_plus_id = 'conpg00t7lagbbsfqkq0'
+
         # 如果用户没有传入chat_id，则新建，kimi的通讯必须要有chat_id
         if not self.chat_id:
             self.logger.error(f'chat_id为空，通讯失败')
-            return ''
+            return AiAnswer()
 
         data = {
             "messages": [
                 {
                     "role": "user",
                     "content": question
                 }
             ],
-            "refs": [],
-            "use_search": True,
-            'kimiplus_id': kimiplus_id if kimiplus_id else 'kimi'
+            "refs": [],  # TODO 上传文档时，在这里添加文档id
+            "use_search": search_model,
+            'kimiplus_id': kimi_plus_id if kimi_plus_id else 'kimi'
         }
 
         uri = '/api/chat/' + str(self.chat_id) + '/completion/stream'
 
         headers = self.headers.copy()
         headers['authorization'] = self.kimi_cookies
 
@@ -198,15 +206,15 @@
             json=data,
             headers=headers,
             stream=True
         )
 
         if response.status_code != 200:
             self.logger.error(f'AI交互请求失败，状态码：{response.status_code}')
-            return ''
+            return AiAnswer()
 
         for line in response.iter_lines():
 
             if not line:
                 continue
 
             try:
@@ -224,51 +232,61 @@
             json_data = json.loads(line[6:])
             event = json_data['event']
 
             if event == 'ping':  # 测试连通性，无意义
                 continue
             elif event == 'resp':  # 第一次回复，主要返回请求确认信息
                 self.group_id = json_data['group_id']
-            elif event == 'req':  # 未知
+            elif event == 'req':  # 第一次回复，主要返回请求确认信息
                 pass
-            elif event == 'cmpl':
+            elif event == 'cmpl':  # 流式输出回复
                 padding = json_data['text']
 
                 if callable(callback_func):
-                    callback_func(padding)
+                    try:
+                        callback_func(padding)
+                    except:
+                        self.logger.error(f'回调函数执行失败')
 
                 self.single_answer += padding
             elif event == 'ref_docs':
                 pass
             elif event == 'search_plus':
                 msg_type = json_data['msg']['type']
+                # 等待搜索全部完成
                 if msg_type != 'done':
                     continue
 
                 url_list = json_data['msg']['url_list']
 
                 for uri_item in url_list:
                     obj = ReferenceLink(**uri_item)
                     self.single_answer_url_list.append(obj)
 
             elif event == 'all_done':
                 if callable(callback_func):
-                    callback_func(self.end_signal)
+                    try:
+                        callback_func(self.end_signal)
+                    except:
+                        self.logger.error(f'回调函数执行失败')
 
         # 封装回答
-        self.single_answer_obj = AiAnswer(
-            is_success=True,
-            content=self.single_answer,
-            conversation_id=self.chat_id,
-            reference_link_list=self.single_answer_url_list
-        )
+        self.single_answer_obj.is_success = True
+        self.single_answer_obj.content = self.single_answer
+        self.single_answer_obj.conversation_id = self.chat_id
+        self.single_answer_obj.reference_link_list = self.single_answer_url_list
 
         return self.single_answer_obj
 
     def send_sms_code(self, phone: str) -> bool:
+        """
+        发送验证码。与login方法配合实现登录
+        :param phone: 手机号
+        :return: 成功时返回True, 失败时返回False
+        """
 
         if len(phone) != 11:
             self.logger.error(f'目前仅支持国内手机，手机号格式错误')
             return False
 
         uri = '/api/user/sms/verify-code'
```

## zibuyu_llm_web/minmax.py

```diff
@@ -2,28 +2,42 @@
 
 """
 --------------------------------------------
 project: zibuyu_LLM
 author: 子不语
 date: 2024/5/4
 contact: 【公众号】思维兵工厂
-description: 海螺问问Web逆向
+description: 海螺问问Web逆向。
+
+该平台使用是在请求头中通过Token（JWT）进行鉴权的；cookies无关鉴权。
+
+JWT的载荷部分:
+
+{
+  "exp": 1718232417,
+  "user": {
+    "id": "242935160332279815",
+    "name": "小螺帽9815",
+    "avatar": "https://cdn.yingshi-ai.com/prod/user_avatar/1706267544389820801-173194570668965896oversize.png",
+    "deviceID": "242935159979966466",
+    "isAnonymous": false
+  }
+}
 --------------------------------------------
 """
-import base64
+
 import os
 import re
 import uuid
 import time
 import json
 import hashlib
 import logging
 import asyncio
-import traceback
-from typing import Dict, Optional
+from typing import Dict, Optional, Literal, Union
 from urllib.parse import urlencode, quote_plus
 
 import aiohttp
 import requests
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from .base import LLMBase
@@ -36,45 +50,95 @@
     MinMax Web
     """
 
     model_name = 'MinMax'
 
     base_host = 'https://hailuoai.com'
 
+    # 配音音色信息
+    voice_info_dict = {
+        'male-botong': {'voiceID': 'male-botong', 'voiceName': '思远'},
+        'Podcast_girl': {'voiceID': 'Podcast_girl', 'voiceName': '心悦'},
+        'boyan_new_hailuo': {'voiceID': 'boyan_new_hailuo', 'voiceName': '子轩'},
+        'female-shaonv': {'voiceID': 'female-shaonv', 'voiceName': '灵儿'},
+        'YaeMiko_hailuo': {'voiceID': 'YaeMiko_hailuo', 'voiceName': '语嫣'},
+        'xiaoyi_mix_hailuo': {'voiceID': 'xiaoyi_mix_hailuo', 'voiceName': '少泽'},
+        'xiaomo_sft': {'voiceID': 'xiaomo_sft', 'voiceName': '芷溪'},
+        'cove_test2_hailuo': {'voiceID': 'cove_test2_hailuo', 'voiceName': '浩翔（英文）'},
+        'scarlett_hailuo': {'voiceID': 'scarlett_hailuo', 'voiceName': '雅涵（英文）'},
+        'Leishen2_hailuo': {'voiceID': 'Leishen2_hailuo', 'voiceName': '模仿雷电将军'},
+        'Zhongli_hailuo': {'voiceID': 'Zhongli_hailuo', 'voiceName': '模仿钟离'},
+        'Paimeng_hailuo': {'voiceID': 'Paimeng_hailuo', 'voiceName': '模仿派蒙'},
+        'keli_hailuo': {'voiceID': 'keli_hailuo', 'voiceName': '模仿可莉'},
+        'Hutao_hailuo': {'voiceID': 'Hutao_hailuo', 'voiceName': '模仿胡桃'},
+        'Xionger_hailuo': {'voiceID': 'Xionger_hailuo', 'voiceName': '模仿熊二'},
+        'Haimian_hailuo': {'voiceID': 'Haimian_hailuo', 'voiceName': '模仿海绵宝宝'},
+        'Robot_hunter_hailuo': {'voiceID': 'Robot_hunter_hailuo', 'voiceName': '模仿变形金刚'},
+        'Linzhiling_hailuo': {'voiceID': 'Linzhiling_hailuo', 'voiceName': '小玲玲'},
+        'huafei_hailuo': {'voiceID': 'huafei_hailuo', 'voiceName': '拽妃'},
+        'lingfeng_hailuo': {'voiceID': 'lingfeng_hailuo', 'voiceName': '东北er'},
+        'male_dongbei_hailuo': {'voiceID': 'male_dongbei_hailuo', 'voiceName': '老铁'},
+        'Beijing_hailuo': {'voiceID': 'Beijing_hailuo', 'voiceName': '北京er'},
+        'JayChou_hailuo': {'voiceID': 'JayChou_hailuo', 'voiceName': 'JayJay'},
+        'Daniel_hailuo': {'voiceID': 'Daniel_hailuo', 'voiceName': '潇然'},
+        'Bingjiao_zongcai_hailuo': {'voiceID': 'Bingjiao_zongcai_hailuo', 'voiceName': '沉韵'},
+        'female-yaoyao-hd': {'voiceID': 'female-yaoyao-hd', 'voiceName': '瑶瑶'},
+        'murong_sft': {'voiceID': 'murong_sft', 'voiceName': '晨曦'},
+        'shangshen_sft': {'voiceID': 'shangshen_sft', 'voiceName': '沐珊'},
+        'kongchen_sft': {'voiceID': 'kongchen_sft', 'voiceName': '祁辰'},
+        'shenteng2_hailuo': {'voiceID': 'shenteng2_hailuo', 'voiceName': '夏洛特'},
+        'Guodegang_hailuo': {'voiceID': 'Guodegang_hailuo', 'voiceName': '郭嘚嘚'},
+        'yueyue_hailuo': {'voiceID': 'yueyue_hailuo', 'voiceName': '小月月'}
+    }
+
     def __init__(
             self,
             login_phone: str = None,
             token_str: str = None,
+            request_uuid: str = '',
+            request_device_id: str = '',
+            device_info_expire: Union[int, str] = '',
             logger_obj: logging.Logger = None,
             error_dir: str = None
     ):
+        """
+        :param login_phone: 登录手机号
+        :param token_str: Token字符串
+        :param request_uuid: 标记请求的uuid，目前无验证，后续可能验证
+        :param request_device_id: 请求时的设备ID，目前无验证，后续可能验证
+        :param device_info_expire: 设备ID过期时间
+        :param logger_obj: 日志对象
+        :param error_dir: 错误日志保存目录
+        """
 
         self.logger = logger_obj
         self.login_phone = login_phone
         self.error_dir = error_dir
         self.token_str = token_str
 
         super().__init__()
 
         self.chat_id: str = ''  # 会话ID
-        self.user_msg_id: str = ''  # 用户所发送的消息的id
-        self.system_msg_id: str = ''  # 系统回复的消息的id
+        self.user_msg_id: str = ''  # 用户所发送的消息的id，目前无作用
+        self.system_msg_id: str = ''  # 系统回复的消息的id，主要用于获取音频
 
-        self.__single_uuid: str = ''  # 单次会话标识ID
-        self.__user_id: str = ''  # 用户标识ID
-        self.__device_id: str = ''  # 设备标识ID
-        self.__device_info_expire: int = 0  # 设备ID过期时间
+        self.__user_id: str = ''  # 用户标识ID，作用未知
+        self.__single_uuid: str = request_uuid  # 单次会话标识ID
+        self.__device_id: str = request_device_id  # 设备标识ID
 
-        self.__voice_info_dict: Optional[dict] = None
+        try:
+            self.__device_info_expire: int = int(device_info_expire)  # 设备ID过期时间
+        except:
+            self.__device_info_expire: int = 0
 
         # 语音相关_请求参数
         self.__voice_user_data = {
             'msgID': "",  # 消息ID
             'timbre': "",  # 配音音色
-            'device_platform': "zibuyu_llm_web",
+            'device_platform': "web",
             'app_id': "3001",
             'uuid': '',  # uuid，待填充
             'device_id': '',  # 设备ID，待填充
             'version_code': "21200",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
@@ -85,19 +149,19 @@
             'screen_width': 1920,
             'screen_height': 1080,
             'unix': '',  # 时间戳，待填充
         }
 
         # 公用请求参数
         self.__user_data = {
-            'device_platform': "zibuyu_llm_web",
+            'device_platform': "web",
             'app_id': "3001",
             'uuid': '',  # uuid，待填充
             'device_id': '',  # 设备ID，待填充
-            'version_code': "21200",
+            'version_code': "21300",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
             'device_memory': 8,
             'cpu_core_num': 8,
             'browser_language': "zh-CN",
             'browser_platform': "Win32",
@@ -111,40 +175,68 @@
             'Accept': "*/*",
             "Accept-Encoding": "gzip, deflate, br, zstd",
             "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
             "Cache-Control": "no-cache",
             'Origin': "https://hailuoai.com",
             'Pragma': "no-cache",
             'Priority': "u=1, i",
+
             "Sec-Ch-Ua": '"Chromium";v="124", "Google Chrome";v="124", "Not-A.Brand";v="99"',
             "Sec-Ch-Ua-Mobile": "?0",
             "Sec-Ch-Ua-Platform": '"Windows"',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-origin',
+
             "User-Agent": super().user_agent,
             "Token": self.token_str,
         }
 
+        self.is_anonymous: bool = True  # 是否是匿名用户；默认为匿名用户
         self.single_answer: str = ''
-        self.single_answer_obj: Optional[AiAnswer] = None
+        self.single_answer_obj: AiAnswer = AiAnswer()
         self.single_padding: str = ''  # 流式输出时，每次接收到的回答中的增量部分
-        self.single_answer_audio_url_list: list = []  # 单次回复时，音频文件的url列表
+        self.single_answer_audio_url_list: Optional[list] = None  # 单次回复时，音频文件的url列表
+
+        if self.token_str:
+            self.logger.info(f'实例化时传入Token_str，开始解析')
+            self.parse_token_str()
+        elif self.anonymity_login():
+            self.logger.info(f'未传入Token，进行匿名登录，成功获取token_str')
+        else:
+            self.logger.error(f'未传入Token，且匿名登录失败')
+
+    @property
+    def voice_list(self):
+        """ 获取所有支持的音色列表 """
+
+        for k, v in self.voice_info_dict.items():
+            print(v['voiceName'])
+
+        return self.voice_info_dict
 
     @property
     def device_id(self):
         """ 获取设备id，该值存在有效期 """
 
-        now = int(time.time())
+        now = int(time.time()) * 1000
 
         if self.__device_id and self.__device_info_expire > now:
             return self.__device_id
 
         self.update_device_id()
 
         return self.__device_id
 
     @property
+    def device_info_expire(self):
+        """ 获取设备id的过期时间 """
+        return self.__device_info_expire
+
+    @property
     def user_id(self):
         """ 获取user_id """
 
         if self.__user_id:
             return self.__user_id
 
         self.update_device_id()
@@ -156,184 +248,14 @@
         """ 海螺平台未登录也可访问，通过此uuid来唯一标识用户 """
 
         if self.__single_uuid:
             return self.__single_uuid
         self.__single_uuid = str(uuid.uuid4())
         return self.__single_uuid
 
-    @property
-    def voice_info_dict(self):
-        """ 获取语音列表 """
-
-        if self.__voice_info_dict:
-            return self.__voice_info_dict
-        self.__voice_info_dict = {
-            "male-botong": {
-                "voiceID": "male-botong",
-                "voiceName": "思远",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/male-botongccf85929-b9c6-40a3-a66d-8ae734e8fe0c.mp3"
-            },
-            "Podcast_girl": {
-                "voiceID": "Podcast_girl",
-                "voiceName": "心悦",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Podcast_girl9e3c80b6-4f23-4af2-8578-4204161eabd5.mp3"
-            },
-            "boyan_new_hailuo": {
-                "voiceID": "boyan_new_hailuo",
-                "voiceName": "子轩",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/boyan_new_hailuo70102124-b4dd-4fe3-8d6e-b57d44f01a90.mp3"
-            },
-            "female-shaonv": {
-                "voiceID": "female-shaonv",
-                "voiceName": "灵儿",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/female-shaonv9c5a5aa5-d527-4b8a-adce-d25e911d2fed.mp3"
-            },
-            "YaeMiko_hailuo": {
-                "voiceID": "YaeMiko_hailuo",
-                "voiceName": "语嫣",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/YaeMiko_hailuo7384790c-d84b-4c59-9a31-be1a1fe40361.mp3"
-            },
-            "xiaoyi_mix_hailuo": {
-                "voiceID": "xiaoyi_mix_hailuo",
-                "voiceName": "少泽",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/xiaoyi_mix_hailuoe47a2c39-fef1-49df-b5b7-7734ab195969.mp3"
-            },
-            "xiaomo_sft": {
-                "voiceID": "xiaomo_sft",
-                "voiceName": "芷溪",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/xiaomo_sfta8bb210d-b35a-46d2-9bcd-46f286c0527c.mp3"
-            },
-            "cove_test2_hailuo": {
-                "voiceID": "cove_test2_hailuo",
-                "voiceName": "浩翔（英文）",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/cove_test2_hailuob22985f3-277c-442d-bf9c-f28a773ce50d.mp3"
-            },
-            "scarlett_hailuo": {
-                "voiceID": "scarlett_hailuo",
-                "voiceName": "雅涵（英文）",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/scarlett_hailuo97649559-1373-4ea8-86dd-b7cfb4aeb029.mp3"
-            },
-            "Leishen2_hailuo": {
-                "voiceID": "Leishen2_hailuo",
-                "voiceName": "模仿雷电将军",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Leishen2_hailuo27ae6370-589e-459f-878d-b6a43c326729.mp3"
-            },
-            "Zhongli_hailuo": {
-                "voiceID": "Zhongli_hailuo",
-                "voiceName": "模仿钟离",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Zhongli_hailuo98dad06d-4e23-49e7-8094-c530c4c05fa5.mp3"
-            },
-            "Paimeng_hailuo": {
-                "voiceID": "Paimeng_hailuo",
-                "voiceName": "模仿派蒙",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Paimeng_hailuo9bda8f9f-3b85-4c76-8c63-cb481980c534.mp3"
-            },
-            "keli_hailuo": {
-                "voiceID": "keli_hailuo",
-                "voiceName": "模仿可莉",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/keli_hailuoeb6d70b9-572b-4a15-a1fa-b139a47780ce.mp3"
-            },
-            "Hutao_hailuo": {
-                "voiceID": "Hutao_hailuo",
-                "voiceName": "模仿胡桃",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Hutao_hailuo6c655b82-3c7c-4232-9bdf-64069039dcf5.mp3"
-            },
-            "Xionger_hailuo": {
-                "voiceID": "Xionger_hailuo",
-                "voiceName": "模仿熊二",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Xionger_hailuo4ae3b6b6-a833-45c4-b8d4-659d4a4ca003.mp3"
-            },
-            "Haimian_hailuo": {
-                "voiceID": "Haimian_hailuo",
-                "voiceName": "模仿海绵宝宝",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Haimian_hailuo3afd8572-99e2-420a-bea0-63dd85ffb37f.mp3"
-            },
-            "Robot_hunter_hailuo": {
-                "voiceID": "Robot_hunter_hailuo",
-                "voiceName": "模仿变形金刚",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Robot_hunter_hailuo38ac6dbf-7941-4498-9ed7-5b4bb94c7650.mp3"
-            },
-            "Linzhiling_hailuo": {
-                "voiceID": "Linzhiling_hailuo",
-                "voiceName": "小玲玲",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Linzhiling_hailuo0db5aad6-5c2f-46f5-871f-4f9197a270b1.mp3"
-            },
-            "huafei_hailuo": {
-                "voiceID": "huafei_hailuo",
-                "voiceName": "拽妃",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/huafei_hailuoe4d1c4b1-2ea1-4538-b4a7-d97bd68d4915.mp3"
-            },
-            "lingfeng_hailuo": {
-                "voiceID": "lingfeng_hailuo",
-                "voiceName": "东北er",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/lingfeng_hailuo044e3100-ec23-435b-8b74-aa1d4ae450c3.mp3"
-            },
-            "male_dongbei_hailuo": {
-                "voiceID": "male_dongbei_hailuo",
-                "voiceName": "老铁",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/male_dongbei_hailuo67361485-a4e7-41cc-8592-989667d4c747.mp3"
-            },
-            "Beijing_hailuo": {
-                "voiceID": "Beijing_hailuo",
-                "voiceName": "北京er",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Beijing_hailuoa16df4af-7107-43d7-adb5-30ee80016509.mp3"
-            },
-            "JayChou_hailuo": {
-                "voiceID": "JayChou_hailuo",
-                "voiceName": "JayJay",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/JayChou_hailuo654d0644-addf-44f1-8fbc-984d60c519b5.mp3"
-            },
-            "Daniel_hailuo": {
-                "voiceID": "Daniel_hailuo",
-                "voiceName": "潇然",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Daniel_hailuod259f6db-4522-4f1f-8310-d7cbf361d08a.mp3"
-            },
-            "Bingjiao_zongcai_hailuo": {
-                "voiceID": "Bingjiao_zongcai_hailuo",
-                "voiceName": "沉韵",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Bingjiao_zongcai_hailuo924dca88-c6a4-49c6-be19-0c9a30c836c3.mp3"
-            },
-            "female-yaoyao-hd": {
-                "voiceID": "female-yaoyao-hd",
-                "voiceName": "瑶瑶",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/female-yaoyao-hdca94aef9-4321-4b3e-a655-8bf0f7d729f2.mp3"
-            },
-            "murong_sft": {
-                "voiceID": "murong_sft",
-                "voiceName": "晨曦",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/murong_sft714a221f-30fc-4d1b-9942-d4824f296b9c.mp3"
-            },
-            "shangshen_sft": {
-                "voiceID": "shangshen_sft",
-                "voiceName": "沐珊",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/shangshen_sft6ba79922-6a38-4150-bbd0-0570a571f7af.mp3"
-            },
-            "kongchen_sft": {
-                "voiceID": "kongchen_sft",
-                "voiceName": "祁辰",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/kongchen_sft3d025ed0-d041-4620-8cd7-f3d09723d275.mp3"
-            },
-            "shenteng2_hailuo": {
-                "voiceID": "shenteng2_hailuo",
-                "voiceName": "夏洛特",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/shenteng2_hailuo3922d48b-1edb-4e7e-baa7-bed0131bf20a.mp3"
-            },
-            "Guodegang_hailuo": {
-                "voiceID": "Guodegang_hailuo",
-                "voiceName": "郭嘚嘚",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/Guodegang_hailuocba5a5aa-781b-4e0b-96e7-070f0e4e97fb.mp3"
-            },
-            "yueyue_hailuo": {
-                "voiceID": "yueyue_hailuo",
-                "voiceName": "小月月",
-                "previewAudioUrl": "https://cdn.yingshi-ai.com/audio/example/yueyue_hailuoa518c725-1be1-456f-8274-be18de1c4f34.mp3"
-            }
-        }
-        return self.__voice_info_dict
-
     @staticmethod
     def md5(value, is_bytes=False):
         """
         md5加密
         :param value: 需要加密的值
         :param is_bytes: 是否已经是二进制数据
         :return:
@@ -360,68 +282,264 @@
 
     @staticmethod
     def get_timestamp():
         """ 获取时间戳 """
 
         return str(int(time.time()) * 1000)
 
-    def update_device_id(self):
+    def parse_token_str(self) -> bool:
+        """海螺使用的Token是JWT格式，可以解析后获取基本信息"""
+
+        if not self.token_str:
+            return False
+
+        try:
+
+            data = self.parse_jwt_token(self.token_str)
+
+            device_id = data.get('user', {}).get('deviceID', '')
+            self.is_anonymous = data.get('user', {}).get('isAnonymous', True)
+            self.__device_id = device_id
+            self.logger.info(f'成功解析JWT\n\n设备ID：【{device_id}】\n用户类型：isAnonymous【{self.is_anonymous}】\n')
+            return True
+        except:
+            self.logger.error(f'解析JWT失败', exc_info=True)
+            return False
+
+    def renew_token_str(self) -> bool:
+        """
+        更新token_str的有效期：一般40天后过期
+        :return: 成功时返回True，失败返回False
+        """
+
+        uri = '/v1/api/user/renewal'
+        unix = self.get_timestamp()
+
+        user_data = self.__user_data.copy()
+        user_data['device_id'] = self.device_id
+        user_data['uuid'] = self.single_uuid
+        user_data['unix'] = unix
+
+        headers = self.__headers.copy()
+
+        yy = self.get_yy(
+            uri=uri,
+            unix=unix,
+            data=user_data,
+            user_data=user_data,
+            jsonfy=True,
+        )
+
+        headers["Yy"] = yy
+        try:
+            response = self.request_session.post(
+                self.base_host + uri,
+                headers=headers,
+                json=user_data
+            )
+
+            resp_data = response.json()
+            request_status = resp_data.get('statusInfo', {}).get('code', )
+            if request_status != 200:
+                self.logger.error(f'token_str更新失败，错误码：{request_status}')
+                return False
+
+            token = resp_data.get('data', {}).get('token')
+            if not token:
+                self.logger.error(f'token_str更新失败，token为空')
+                return False
+
+            self.token_str = token
+        except:
+            self.logger.error(f'token_str更新失败', exc_info=True)
+            return False
+
+    def anonymity_login(self) -> bool:
+        """ 匿名登录，获取token_str """
+
+        uri = '/v1/api/user/login/phone'
+
+        unix = self.get_timestamp()
+
+        user_data = self.__user_data.copy()
+        user_data['device_id'] = self.device_id
+        user_data['uuid'] = self.single_uuid
+        user_data['unix'] = unix
+
+        headers = self.__headers.copy()
+
+        data = {
+            "loginType": "3",
+            "adInfo": {}
+        }
+
+        yy = self.get_yy(
+            uri=uri,
+            unix=unix,
+            data=data,
+            user_data=user_data,
+            jsonfy=True,
+        )
+
+        headers["Yy"] = yy
+        headers["server_version"] = ''
+
+        query_str = self.build_query_string(user_data)
+
+        response = self.request_session.post(
+            self.base_host + uri + f'?{query_str}',
+            headers=headers,
+            json=data
+        )
+
+        resp_data = response.json()
+
+        token_str = resp_data.get('data', {}).get('token')
+        device_id = resp_data.get('data', {}).get('deviceID')
+        user_id = resp_data.get('data', {}).get('userID')
+
+        if token_str:
+            self.chat_id = None
+
+            self.token_str = token_str
+            self.__headers['Token'] = token_str
+            self.__device_id = device_id
+            self.__user_id = user_id
+            self.__device_info_expire = (int(time.time()) + 10800) * 1000
+
+            self.logger.info(f'成功获取到token_str：{token_str}')
+            return True
+
+        return False
+
+    def post(
+            self,
+            url: str,
+            headers: dict,
+            data: dict,
+            stream: bool = False,
+            multipart_encode: bool = False,
+    ) -> Optional[requests.Response]:
+        """
+        发送post请求，如果失败，则重新登录后再尝试，尝试两次
+        :param url: 请求url
+        :param headers: 请求头
+        :param data: 请求体
+        :param stream: 是否流式传输
+        :param multipart_encode: 是否使用multipart/form-data格式
+        :return:
+        """
+
+        for i in range(3):
+
+            if multipart_encode:
+                self.logger.info(f"使用multipart/form-data格式发送POST请求")
+
+                multipart_data = MultipartEncoder(data)
+                headers["Content-Type"] = multipart_data.content_type
+                headers["Token"] = self.token_str
+                response = self.request_session.post(
+                    url,
+                    headers=headers,
+                    data=multipart_data,
+                    stream=stream
+                )
+            else:
+                self.logger.info(f"使用json格式发送POST请求")
+
+                headers["Token"] = self.token_str
+                response = self.request_session.post(
+                    url,
+                    headers=headers,
+                    data=data,
+                    stream=stream
+                )
+
+            if response.status_code == 200:
+                self.logger.info(f"POST请求成功")
+                return response
+
+            self.logger.error(f"POST请求失败，状态码：{response.status_code}")
+            self.logger.error(f"POST请求失败，响应内容：{response.text}")
+
+            if not self.is_anonymous:
+                self.logger.info(f"并非匿名用户，不进行自动登录")
+                return
+
+            result = self.re_login_by_anonymous(data)
+            if not result:
+                self.logger.error(f"重新匿名登录失败，不再尝试发送POST请求")
+                return
+            self.logger.info(f"重新匿名登录成功，即将重新发送请求")
+
+        self.logger.error(f"请求3次仍然失败，退出")
+
+    def get(self, url: str, headers: dict, params: dict, stream: bool = False) -> Optional[requests.Response]:
+        pass
+
+    def update_device_id(
+            self,
+            request_uuid: str = None,
+            request_device_id: str = None,
+    ):
         """ 更新设备id """
 
-        path = self.base_host + "/v1/api/user/device/register"
+        uri = "/v1/api/user/device/register"
+
+        unix = self.get_timestamp()
+
+        user_data = self.__user_data.copy()
+
+        user_data['uuid'] = request_uuid or self.single_uuid
+        user_data['device_id'] = request_device_id or self.__device_id
+        data = {"uuid": request_uuid or self.single_uuid}
+
+        user_data['unix'] = unix
+
+        headers = self.__headers.copy()
+
+        yy = self.get_yy(
+            user_data=user_data,
+            uri=uri,
+            data=data,
+            unix=unix,
+            jsonfy=True
+        )
 
-        data = self.__user_data.copy()
+        headers["Yy"] = yy
 
-        data['uuid'] = self.single_uuid
+        query_str = self.build_query_string(user_data)
+        response = self.request_session.post(
+            self.base_host + uri + f'?{query_str}',
+            json=data,
+            headers=headers
+        )
 
-        response = requests.post(path, json=data, headers=self.__headers)
         resp_json = response.json()
+
         status_code = resp_json.get('statusInfo', {}).get('code')
 
         if status_code != 0:
             self.logger.error(f'获取设备信息出错')
             self.logger.info(f'响应数据: {resp_json}')
             raise RequestsError(resp_json)
 
         self.__device_id = resp_json.get('data', {}).get('deviceIDStr')
         self.__user_id = resp_json.get('data', {}).get('userID')
 
         if self.__device_id:
             self.logger.info(f'成功更新设备ID: 【{self.__device_id}】')
 
-            now = int(time.time())
-            self.__device_info_expire = now + 10800
+            self.__device_info_expire = (int(time.time()) + 10800) * 1000
 
             self.logger.info(f'成功更新设备过期时间: 【{self.__device_info_expire}】')
 
         if self.__user_id:
             self.logger.info(f'成功更新用户ID: 【{self.__user_id}】')
 
-        # 响应数据示例
-        """
-        {'data':
-                 {
-                  'deviceID': 242986651646619650,
-                  'deviceIDStr': '242986651646619650',
-                  'userID': '2Y62maaVyPGK',
-                  'realUserID': '242986651696951305'
-                  },
-             'statusInfo':
-                 {
-                  'code': 0,
-                  'httpCode': 0,
-                  'message': '成功',
-                  'serviceTime': 1714788676,
-                  'requestID': '7e353b60-8462-4488-ae36-42bd62428e5b',
-                  'debugInfo': '',
-                  'serverAlert': 0
-                  }
-             }
-        """
-
     def get_yy(
             self,
             uri,
             unix: str,
             user_data: dict,
             data: dict = None,
             jsonfy: bool = False,
@@ -445,20 +563,17 @@
         elif is_file:
             # 计算chatID的MD5哈希
             chat_id_hash = self.md5(data['chatID'])
 
             # 计算characterID的MD5哈希
             character_id_hash = self.md5(data['characterID'])
 
-            play_speed_level_hash = self.md5(data['playSpeedLevel'])
-
-            file_hash = self.md5(data['voiceBytes'], is_bytes=True)
+            file_hash = self.md5(data['voiceBytes'][:1024], is_bytes=True)
 
-            # data_json = chat_id_hash + file_hash + character_id_hash + play_speed_level_hash
-            data_json = character_id_hash + file_hash + chat_id_hash + play_speed_level_hash
+            data_json = character_id_hash + chat_id_hash + file_hash
 
         else:
 
             # 计算characterID的MD5哈希
             character_id_hash = self.md5(data['characterID'])
 
             # 移除msgContent中的换行符并计算MD5哈希
@@ -475,57 +590,93 @@
 
         full_uri = f"{uri}{uri.find('?') != -1 and '&' or '?'}{query_str}"
 
         yy = self.md5(f"{quote_plus(full_uri)}_{data_json}{self.md5(unix)}ooui")
 
         return yy
 
+    def check_request_info(
+            self, request_uuid: str = None,
+            request_device_id: str = None,
+            device_info_expire: Union[int, str] = 0,
+    ) -> bool:
+
+        """MinMax似乎并不检查请求时携带的device_id；但这里仍然带上"""
+
+        if not request_uuid or not request_device_id or not device_info_expire:
+            return False
+
+        if not isinstance(device_info_expire, int):
+            try:
+                device_info_expire = int(device_info_expire)
+            except:
+                device_info_expire = 0
+
+        now = int(time.time()) * 1000
+
+        if device_info_expire < now:
+            return False
+
+        self.__device_info_expire = device_info_expire
+        self.__device_id = request_device_id
+        self.__single_uuid = request_uuid
+        return True
+
     def ask(
             self,
             question: str,
             chat_id: str = None,
             callback_func=None,
             character_id: str = '1',
-            search_mode: str = '0',
-            audio_output_dir: str = '',
+            search_mode: Literal['0', '1'] = '0',
+            audio_output_dir: str = None,
             voice_id: str = 'male-botong',
+            request_uuid: str = None,
+            request_device_id: str = None,
+            device_info_expire: Union[int, str] = None,
     ) -> AiAnswer:
         """
         提问
         :param question: 问题
         :param chat_id: 会话ID
         :param callback_func: 回调函数，处理每一次回答的增量文本
         :param character_id: 角色id，目前固定为1
         :param search_mode: 搜索模式：1表示关闭；0表示开启
         :param audio_output_dir: 音频文件输出目录；不为空时将在AI交互之后生成音频
         :param voice_id: 配音音色ID
-        :return:
+        :param request_uuid: 配音音色ID
+        :param request_device_id: 配音音色ID
+        :param device_info_expire: 配音音色ID
+        :return: AiAnswer
         """
 
         if search_mode not in ['0', '1']:
             raise ValueError("search_mode参数错误，请传入0或1")
 
-        self.chat_id = chat_id
+        self.check_request_info(request_uuid, request_device_id, device_info_expire)
+
+        if chat_id:
+            self.logger.info(f'使用传入的会话ID: 【{chat_id}】')
+            self.chat_id = chat_id
 
         uri = "/v4/api/chat/msg"
 
         unix = self.get_timestamp()
 
         # 1. 处理请求参数
         user_data = self.__user_data.copy()
+
         user_data["uuid"] = self.single_uuid
         user_data["device_id"] = self.device_id
         user_data["unix"] = unix
 
         # 2. 处理请求体数据
         headers = self.__headers.copy()
-
-        headers[
-            "Referer"] = f'https://hailuoai.com/?chat={self.chat_id}' if self.chat_id else 'https://hailuoai.com/'
-
+        referer = f'https://hailuoai.com/?chat={self.chat_id}' if self.chat_id else 'https://hailuoai.com/'
+        headers["Referer"] = referer
         headers["Accept"] = 'text/event-stream'
 
         data = {
             "characterID": character_id,
             "msgContent": question,
             "chatID": self.chat_id if self.chat_id else '0',  # 为0时将新建对话
             "searchMode": search_mode,
@@ -536,35 +687,85 @@
             uri=uri,
             data=data,
             unix=unix
         )
 
         headers["Yy"] = yy
 
-        # 3. 将data转换为FormData格式
-        multipart_data = MultipartEncoder(data)
-        headers['Content-Type'] = multipart_data.content_type
-
-        # 4. 发起请求
         query_str = self.build_query_string(user_data)
-        response = requests.post(
-            self.base_host + uri + f'?{query_str}',
-            headers=headers,
-            data=multipart_data,
-            stream=True
-        )
 
+        for i in range(3):
+
+            try:
+                response = self.post(
+                    self.base_host + uri + f'?{query_str}',
+                    headers=headers,
+                    data=data,
+                    stream=True,
+                    multipart_encode=True,
+                )
+
+                # 请求失败，返回空对象
+                if not response:
+                    return AiAnswer()
+
+                self.parse_ask_result(
+                    response=response,
+                    callback_func=callback_func,
+                    audio_output_dir=audio_output_dir,
+                    voice_id=voice_id
+                )
+
+                return self.single_answer_obj
+            except NeedLoginError:
+
+                if not self.is_anonymous:
+                    self.logger.info('该用户并非匿名用户，不进行自动登录')
+                    return AiAnswer()
+
+                result = self.re_login_by_anonymous(data)
+                if not result:
+                    self.logger.error(f"重新匿名登录失败，AI回答获取失败，返回空对象")
+                    return AiAnswer()
+
+        self.logger.error(f"多次获取AI回答都失败，返回空对象")
+        return AiAnswer()
+
+    def re_login_by_anonymous(self, data: dict) -> bool:
+        """重新进行匿名登录"""
+
+        self.logger.info(f"尝试重新匿名登录...")
+        result = self.anonymity_login()
+
+        if not result:
+            self.logger.error(f"重新匿名登录失败")
+            return False
+
+        self.logger.info(f"重新匿名登录成功")
+        self.__headers["Token"] = self.token_str
+
+        # 匿名登录后，就没法保持原来的会话了
+        if 'chatID' in data:
+            data['chatID'] = '0'
+            self.chat_id = None
+            self.logger.info(f"原会话ID失效，已清除")
+
+        return True
+
+    def parse_ask_result(
+            self,
+            response: requests.Response,
+            callback_func,
+            audio_output_dir,
+            voice_id
+    ):
         index = 0
         pending = ""
         event = ""
 
-        if response.status_code != 200:
-            self.logger.error(f"请求失败，状态码：{response.status_code}")
-            raise NeedLoginError('请检查Token是否过期')
-
         for chunk in response.iter_lines():
 
             if not chunk:
                 continue
 
             index += 1
             chunk = chunk.decode("utf-8")
@@ -585,124 +786,119 @@
             # Incomplete chunk
             if not pending.endswith("}"):
                 self.logger.debug("The chunk is incomplete.")
                 continue
 
             self.logger.debug(f"The chunk is complete.")
 
-            try:
-
-                # Remove the 'data:' prefix, convert JSON to dict
-                pending = pending[5:]
-                resp_json = json.loads(pending)
-                pending = ""
-
-                message_type = resp_json.get('type')
-                status_code = resp_json.get('statusInfo', {}).get('code')
-                error_message = resp_json.get('statusInfo', {}).get('message')
-
-                if status_code != 0:
-                    self.logger.error(f"请求失败，状态码：{status_code}，消息：{error_message}")
-                    continue
-
-                if event == "send_result" and message_type == 1:
-                    self.handle_send_result(resp_json)
-                    continue
-                elif event == "message_result" and message_type == 2:
-                    self.handle_message_result(resp_json, callback_func)
-                    continue
-                elif event == "follow_up_question_result" and message_type == 4:
-                    self.handle_follow_up_question_result(resp_json)
-                    continue
-                else:
-                    self.logger.error(f"MinMax响应出现未知数据，可能需要重新逆向，数据类型：{event}")
-                    self.logger.info(f"MinMax响应数据：{pending}")
-
-            except Exception:
-
-                request_url = self.base_host + uri
-
-                request_data = json.dumps(data)
-                request_response = pending
-                traceback_info = f"\n--- Error Log Entry ---\n{traceback.format_exc()}\n--- End of Entry ---\n"
-
-                all_data = (f"请求URL：\n{request_url}\n\n"
-                            f"请求头数据：\n{headers}\n\n"
-                            f"请求体数据：\n{request_data}\n\n"
-                            f"回信数据：\n{request_response}\n\n"
-                            f"调用栈信息：\n{traceback_info}")
+            # Remove the 'data:' prefix, convert JSON to dict
+            pending = pending[5:]
+            resp_json = json.loads(pending)
+            pending = ""
+
+            message_type = resp_json.get('type')
+            status_code = resp_json.get('statusInfo', {}).get('code')
+            error_message = resp_json.get('statusInfo', {}).get('message')
 
-                file_path = self.save_bad_request_data('MinMax交互-出现未知错误', all_data)
+            if status_code == 0:
+                pass
+            else:
+                self.logger.error(f"解析请求数据时发送错误，状态码：【{status_code}】，消息：【{error_message}】")
+                raise NeedLoginError('error_message')
 
-                self.logger.error(f"MinMax交互-出现未知错误，相关数据已写入【{file_path}】", exc_info=True)
+            if event == "send_result" and message_type == 1:
+                self.handle_send_result(resp_json)
+                continue
+            elif event == "message_result" and message_type == 2:
+                self.handle_message_result(resp_json, callback_func)
                 continue
+            elif event == "follow_up_question_result" and message_type == 4:
+                self.handle_follow_up_question_result(resp_json)
+                continue
+            else:
+                self.logger.error(f"MinMax响应出现未知数据，可能需要重新逆向，数据类型：{event}")
+                self.logger.info(f"MinMax响应数据：{pending}")
 
         # 检查是否收到任何响应
         if index == 0:
             self.logger.error("MinMax请求没有收到任何响应")
 
         if audio_output_dir:
+            self.logger.info(f"接收到音频存放路径【{audio_output_dir}】，MinMax音频获取中...")
+
             audio_path_list = self.download_audios(output_dir=audio_output_dir, voice_id=voice_id)
 
             if not audio_path_list:
                 self.logger.error("MinMax音频获取失败")
                 return self.single_answer_obj
 
             self.logger.info(f"已将文本转为音频，存放到【{audio_output_dir}】，共计{len(audio_path_list)}条音频")
 
-            self.single_answer_obj.audio_url_list = audio_path_list
+            self.single_answer_obj.audio_path_list = audio_path_list
             return self.single_answer_obj
-
-        return self.single_answer_obj
+        self.logger.info(f'没有接收到音频存放路径，无需处理音频回复')
 
     def handle_follow_up_question_result(self, data: dict):
         """服务端返回最后总结信息"""
 
         self.single_answer = data.get('data', {}).get('messageResult', {}).get('content')
 
         reference_link_list = data.get('data', {}).get('extra', {}).get('netSearchStatus', {}).get('linkDetail', [])
 
-        answer_obj = AiAnswer(
-            is_success=True,
-            content=self.single_answer,
-            conversation_id=self.chat_id,
-            reference_link_list=[ReferenceLink(
-                title=item['detail'],
-                url=item['url'],
-            ) for item in reference_link_list]
-        )
-
-        self.single_answer_obj = answer_obj
+        self.single_answer_obj.is_success = True
+        self.single_answer_obj.content = self.single_answer
+        self.single_answer_obj.conversation_id = self.chat_id
+        self.single_answer_obj.reference_link_list = [ReferenceLink(
+            title=item['detail'],
+            url=item['url'],
+        ) for item in reference_link_list]
 
     def handle_message_result(self, data: dict, callback_func: callable = None):
         """服务端返回响应文本"""
 
         content = data.get('data', {}).get('messageResult', {}).get('content')
         self.single_padding = content.replace(self.single_answer, '')
         self.single_answer = content
 
-        if callback_func:
+        if callable(callback_func):
             try:
                 callback_func(self.single_padding)
             except:
                 self.logger.error("回调函数执行失败")
 
+        is_end = data.get('data', {}).get('messageResult', {}).get('isEnd')
+
+        if is_end == 0:
+            self.single_answer_obj.is_success = True
+            self.single_answer_obj.content = self.single_answer
+            self.single_answer_obj.conversation_id = self.chat_id
+
+        if is_end == 0 and callable(callback_func):
+            try:
+                callback_func(self.end_signal)
+            except:
+                self.logger.error("回调函数执行失败")
+
     def handle_send_result(self, data: dict):
         """服务端接收到用户文本，返回chatID等信息"""
 
         self.user_msg_id = data.get('data', {}).get('sendResult', {}).get('userMsgID')
         self.chat_id = data.get('data', {}).get('sendResult', {}).get('chatID')
         self.system_msg_id = data.get('data', {}).get('sendResult', {}).get('systemMsgID')
 
     def __get_voice_url(self, msg_id: str = None, voice_id: str = 'male-botong'):
 
         uri = "/v1/api/chat/msg_tts"
 
+        self.logger.info(f"语音ID：【{voice_id}】")
+
         if voice_id not in self.voice_info_dict:
-            raise ValueError("语音ID不存在")
+            self.logger.error(f"输入的语音ID不存在，使用默认值【{voice_id}】")
+            voice_id = 'male-botong'
+            # raise ValueError("语音ID不存在")
 
         msg_id = msg_id or self.system_msg_id
 
         if not msg_id:
             raise ValueError("msg_id不能为空")
 
         # 1. 处理请求参数
@@ -758,18 +954,18 @@
             if response.status == 200:
                 with open(file_name, 'wb') as f:
                     while True:
                         chunk = await response.content.read(1024)
                         if not chunk:
                             break
                         f.write(chunk)
-                self.logger.info(f"{file_name} downloaded successfully.")
+                self.logger.info(f"【{file_name}】 downloaded successfully.")
                 # print(f"{file_name} downloaded successfully.")
             else:
-                self.logger.error(f"Failed to download {file_name}. Status code: {response.status}")
+                self.logger.error(f"Failed to download 【{file_name}】. Status code: {response.status}")
                 # print(f"Failed to download {file_name}. Status code: {response.status}")
 
     async def __download_all_audios(self, audio_urls, output_dir):
         """ 并发下载所有音频 """
 
         async with aiohttp.ClientSession() as session:
             tasks = []
@@ -812,85 +1008,25 @@
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         asyncio.run(self.__download_all_audios(audio_url_list, output_dir))
 
         return [f"{output_dir}/audio_{index}.mp3" for index, url in enumerate(audio_url_list)]
 
-    def voice2voice(
-            self,
-            audio_path: str
-    ):
-        """
-        语音输入 + 语音输出 【未完成】
-        :param audio_path: 音频文件路径
-        :return:
-        """
-
-        if not os.path.exists(audio_path):
-            self.logger.error("音频文件不存在")
-            return
-
-        uri = "/v1/api/chat/phone_msg"
-
-        unix = self.get_timestamp()
-
-        # 1. 处理请求参数
-        user_data = self.__user_data.copy()
-        user_data["uuid"] = self.single_uuid
-        user_data["device_id"] = self.device_id
-        user_data["unix"] = unix
-
-        with open(audio_path, 'rb') as f:
-            voice_bytes = f.read()
-
-        data = {
-            "chatID": self.chat_id if self.chat_id else '0',  # 为0时将新建对话
-            "voiceBytes": voice_bytes,
-            # "voiceBytes": base64.b64encode(voice_bytes),
-            "characterID": '1',
-            "playSpeedLevel": '1',
-        }
-
-        yy = self.get_yy(user_data=user_data, uri=uri, unix=unix, is_file=True, data=data)
-        headers = self.__headers.copy()
-        headers[
-            "Referer"] = f'https://hailuoai.com/?chat={self.chat_id}' if self.chat_id else 'https://hailuoai.com/'
-
-        headers["Accept"] = 'text/event-stream'
-        headers["Yy"] = yy
-
-        # 3. 将data转换为FormData格式
-        multipart_data = MultipartEncoder(data)
-        headers['Content-Type'] = multipart_data.content_type
-
-        response = self.request_session.post(
-            url=self.base_host + uri,
-            headers=headers,
-            data=multipart_data
-        )
-
-        print(response.status_code)
-        print(response.text)
-
-        if response.status_code != 200:
-            self.logger.error(f"MinMax音频交互失败，响应数据：{response.text}")
-            return
-
-        for line in response.iter_lines():
-            line = line.decode('utf-8')
-            print(line)
-
     def send_sms_code(self, phone_num: str) -> bool:
         """
         发送验证码
         :param phone_num: 手机号码
-        :return: bool
+        :return: 成功时返回True，失败时返回False
         """
 
+        if not self.is_valid_cn_phone(phone_num):
+            self.logger.error(f'输入号码【{phone_num}】不是合法的国内手机号')
+            return False
+
         uri = '/v1/api/user/login/sms/send'
 
         unix = self.get_timestamp()
 
         # 1. 处理请求参数
         user_data = self.__user_data.copy()
         user_data["unix"] = unix
@@ -928,15 +1064,15 @@
 
     def login(
             self,
             phone: str,
             sms_code: str,
     ) -> bool:
         """
-        登录
+        账号登录
         :param phone: 手机号
         :param sms_code: 手机验证码
         :return: 登录成功时返回获取到的Token
         """
 
         if len(sms_code) != 6:
             self.logger.error(f"验证码长度错误")
@@ -987,35 +1123,169 @@
             self.token_str = token
             return True
 
         except:
             self.logger.error(f"登录失败")
             return False
 
+    def update_voice_config(self, voice_id: str = 'female-shaonv') -> bool:
+        """
+        更新语音配置
+        :param voice_id: 语音ID
+        :return: 成功时返回True；失败时返回False
+        """
+
+        if voice_id not in self.voice_info_dict:
+            self.logger.error(f"输入的语音ID错误")
+            return False
+
+        uri = '/v1/api/chat/update_robot_custom_config'
+
+        data = {
+            "robotID": "1",
+            "config": {
+                "robotVoiceID": voice_id
+            }
+        }
+
+        unix = self.get_timestamp()
+
+        user_data = self.__user_data.copy()
+        user_data["unix"] = unix
+        user_data['device_id'] = self.device_id
+        user_data['uuid'] = self.single_uuid
+
+        yy = self.get_yy(
+            uri=uri,
+            unix=unix,
+            user_data=user_data,
+            data=data,
+            jsonfy=True,
+        )
+
+        headers = self.__headers.copy()
+        headers['Accept'] = 'application/json, text/plain, */*'
+        headers['Referer'] = 'https://hailuoai.com/'
+        headers['Accept-Language'] = 'zh-CN,zh;q=0.9'
+        headers['Content-Type'] = 'application/json'
+        headers['Yy'] = yy
+
+        query_str = self.build_query_string(user_data)
+
+        response = self.request_session.post(
+            url=self.base_host + uri + f'?{query_str}',
+            headers=headers,
+            # json=data,  # 纪念此处一个大坑。requests在进行json序列化时，并不会自动去除换行空格之类的东西，但海螺会验证。
+            data=json.dumps(data).replace(' ', '').replace('\r', '').replace('\n', ''),
+        )
+
+        try:
+            resp_data = response.json()
+
+            code = resp_data.get('statusInfo', {}).get('code')
+            if code == 0:
+                self.logger.info(f"更新语音配置成功")
+                return True
+
+            self.logger.error(f"更新语音配置失败")
+            return False
+
+        except:
+            self.logger.error(f"更新语音配置时出现位置错误", exc_info=True)
+            return False
+
+    # ######################## 未完成 ########################
+
+    def voice2voice(self, audio_path: str):
+        """
+        【未完成】语音输入 + 语音输出
+        :param audio_path: 音频文件路径
+        :return:
+        """
+
+        if not os.path.exists(audio_path):
+            self.logger.error("音频文件不存在")
+            return
+
+        uri = "/v1/api/chat/phone_msg"
+
+        unix = self.get_timestamp()
+
+        # 1. 处理请求参数
+        user_data = self.__user_data.copy()
+        user_data["uuid"] = self.single_uuid
+        user_data["device_id"] = self.device_id
+        user_data["unix"] = unix
+
+        with open(audio_path, 'rb') as f:
+            voice_bytes = f.read()
+
+        data = {
+            "chatID": self.chat_id if self.chat_id else '0',  # 为0时将新建对话
+            "voiceBytes": voice_bytes,
+            "characterID": '1',
+            "playSpeedLevel": '1',
+        }
+
+        yy = self.get_yy(user_data=user_data, uri=uri, unix=unix, is_file=True, data=data)
+
+        headers = self.__headers.copy()
+
+        headers["Referer"] = 'https://hailuoai.com/'
+        headers["Accept"] = 'text/event-stream'
+        headers["Yy"] = yy
+
+        # 3. 将data转换为FormData格式
+        multipart_data = MultipartEncoder(data)
+        headers['Content-Type'] = multipart_data.content_type
+
+        query_str = self.build_query_string(user_data)
+
+        response = self.request_session.post(
+            url=self.base_host + uri + f'?{query_str}',
+            headers=headers,
+            data=multipart_data,
+        )
+
+        print(response.status_code)
+
+        if response.status_code != 200:
+            self.logger.error(f"MinMax音频交互失败，响应数据：{response.content}")
+            return
+
+        for line in response.iter_lines():
+            line = line.decode('utf-8')
+            print(line)
+
     def test(self):
-        unix = '1715264091000'
+        unix = '1715851530000'
 
         user_data = {
-            'msgID': 244977956405796869,
-            'timbre': "male-botong",
-            'device_platform': "zibuyu_llm_web",
+            'device_platform': "web",
             'app_id': "3001",
-            'uuid': '7c251825-9626-4e8a-81df-d8a3cbf58c50',  # uuid，待填充
-            'device_id': '244976245380423685',  # 设备ID，待填充
-            'version_code': "21200",
+            'uuid': '533a6e83-07c1-4d79-882c-604e1c56ba92',  # uuid，待填充
+            'device_id': '247444514620280836',  # 设备ID，待填充
+            'version_code': "21300",
             'os_name': "Windows",
             'browser_name': "chrome",
             'server_version': "101",
             'device_memory': 8,
             'cpu_core_num': 8,
             'browser_language': "zh-CN",
             'browser_platform': "Win32",
             'screen_width': 1920,
             'screen_height': 1080,
             'unix': unix,  # 时间戳，待填充
         }
 
-        data = {}
+        data = {"robotID": "1", "config": {"robotVoiceID": "boyan_new_hailuo"}}
 
-        uri = '/v1/api/chat/msg_tts'
-        yy = self.get_yy(user_data=user_data, uri=uri, data=data, unix=unix, jsonfy=True)
+        uri = '/v1/api/chat/update_robot_custom_config'
+
+        yy = self.get_yy(
+            uri=uri,
+            unix=unix,
+            user_data=user_data,
+            data=data,
+            jsonfy=True,
+        )
         print(yy)
```

## zibuyu_llm_web/types.py

```diff
@@ -18,14 +18,16 @@
 
 @dataclass
 class ReferenceLink:
     """回复中的相关链接"""
 
     title: str
     url: str
+    index: int = 0
+    description: str = ''
 
 
 @dataclass
 class AiAnswer:
     """AI回复"""
 
     content: str = ''
```

## zibuyu_llm_web/wanxiang.py

```diff
@@ -27,19 +27,21 @@
     WanXiangWeb：通义万相web端
     """
 
     model_name = 'WanXiang'
 
     api_base: str = "https://wanx.aliyun.com/wanx"
 
-    def __init__(self,
-                 cookies_str: str = None,
-                 cookies_dict: dict = None,
-                 logger_obj: logging.Logger = None,
-                 error_dir: str = None):
+    def __init__(
+            self,
+            cookies_str: str = None,
+            cookies_dict: dict = None,
+            logger_obj: logging.Logger = None,
+            error_dir: str = None
+    ):
         """
         QwenWeb初始化
         :param cookies_str: cookies字符串
         :param cookies_dict: cookies字典
         :param logger_obj: 日志记录对象
         :param error_dir: 错误请求记录的保存目录，当出现请求失败时，会将关于该请求的URL、请求参数、响应数据整理成文件，存放于此目录
         """
@@ -84,17 +86,20 @@
         """
         获取风格列表
         """
 
         for style in self.style_list.keys():
             print(style)
 
-    def _get_task_id(self, prompt: str,
-                     resolution: Literal["1024*1024", "1280*720", "720*1280"] = "1024*1024",
-                     style: str = "默认", ):
+    def _get_task_id(
+            self,
+            prompt: str,
+            resolution: Literal["1024*1024", "1280*720", "720*1280"] = "1024*1024",
+            style: str = "默认",
+    ):
         """
         提交会话任务，获取任务id
         :param prompt: (str)图片描述
         :param resolution: (str, optional)分辨率. Defaults to "1024*1024", 支持："1280*720", "720*1280"
         :param style: (str)图片风格
         :return: task_id (str)
         """
@@ -163,20 +168,22 @@
             file_path = self.save_bad_request_data('获取最新任务id-出现错误', all_data)
             self.logger.error(f"获取最新任务id出现错误，相关数据已写入【{file_path}】")
             raise RequestsError("functon [generate_image] got an unexpected response.")
 
         latest_id = resp.json()['data'][0]['id']
         return latest_id
 
-    def generate_image(self,
-                       prompt: str,
-                       resolution: Literal["1024*1024", "1280*720", "720*1280"] = "1024*1024",
-                       style: Literal[
-                           "水彩", "油画", "中国风", "扁平插画", "二次元", "素描", "3D卡通", "默认"] = "默认",
-                       total_timeout=120) -> list[WanXianImage]:
+    def generate_image(
+            self,
+            prompt: str,
+            resolution: Literal["1024*1024", "1280*720", "720*1280"] = "1024*1024",
+            style: Literal[
+                "水彩", "油画", "中国风", "扁平插画", "二次元", "素描", "3D卡通", "默认"] = "默认",
+            total_timeout=120
+    ) -> list[WanXianImage]:
         """
         文生图功能主入口，根据描述词生成图片
         :param prompt: (str)图片描述
         :param resolution: (str, optional)分辨率. Defaults to "1024*1024", 支持："1280*720", "720*1280"
         :param style: (str)图片风格
         :param total_timeout: 最长等待时间
         :return:
```

## zibuyu_llm_web/xinchen.py

```diff
@@ -22,19 +22,21 @@
 from .errors import NeedLoginError
 from .types import XincChatHistory, XincChatContent, XincMessageIssuer, XincCharacterInfo, XincCharacter, AiAnswer
 
 
 class XinChenWeb(LLMBase):
     model_name = 'XinChen'
 
-    def __init__(self,
-                 cookies_str: str = None,
-                 cookies_dict: dict = None,
-                 logger_obj: logging.Logger = None,
-                 error_dir: str = None):
+    def __init__(
+            self,
+            cookies_str: str = None,
+            cookies_dict: dict = None,
+            logger_obj: logging.Logger = None,
+            error_dir: str = None
+    ):
         """
         QwenWeb初始化
         :param cookies_str: cookies字符串
         :param cookies_dict: cookies字典
         :param logger_obj: 日志记录对象
         :param error_dir: 错误请求记录的保存目录，当出现请求失败时，会将关于该请求的URL、请求参数、响应数据整理成文件，存放于此目录
         """
```

## zibuyu_llm_web/xunfei.py

```diff
@@ -2,46 +2,47 @@
 
 """
 --------------------------------------------
 project: zibuyu_LLM
 author: 子不语
 date: 2024/5/10
 contact: 【公众号】思维兵工厂
-description: 
+description: 讯飞星火Web端。
+
+但出现因Token失效而导致的访问失败，会自动尝试重新登录。
 --------------------------------------------
 """
 
-from typing import List, Optional
+from typing import Optional, Union
 from pathlib import Path
 import logging
 import base64
 import random
+import uuid
 import time
 import json
 import sys
 import io
 import re
 
 from PIL import Image
 import numpy as np
 import requests
 import ddddocr
 import execjs
 
 from .base import LLMBase
 from .types import AiAnswer
-from .errors import LoginFailError, APIConnectionError, NeedLoginError
+from .errors import LoginFailError, NeedLoginError, UnexpectResponseError
 
 BASE_DIR = Path(__file__).parent
 STATIC_DIR = BASE_DIR / 'static_data'
 if not STATIC_DIR.exists():
     STATIC_DIR.mkdir(parents=True)
 
-JS_FILE_PATH = STATIC_DIR / 'generate_w.js'
-
 
 class GTrace(object):
     def __init__(self):
         self.__pos_x = []
         self.__pos_y = []
         self.__pos_z = []
 
@@ -172,30 +173,30 @@
         for idx in range(len(x)):
             result.append([int(x[idx]), int(y[idx]), int(z[idx])])
 
         return int(_distance), result
 
 
 class WebLogin(object):
-    """
-    该类用于讯飞网页版登录，获取登录token
-    """
+    """该类用于讯飞网页版登录，获取登录token"""
 
     def __init__(
             self,
             account_name: str,
             password: str,
             logger: logging.Logger = None,
+            generate_w_js_file_path: str = None,
     ):
         """
 
         :param account_name: 账号
         :param password: 密码
         """
 
+        self.generate_w_js_file_path = generate_w_js_file_path
         self.account_name = account_name
         self.password = password
         self.logger = logger or logging.getLogger(__name__)
 
         self.gt = ''
         self.challenge = ''
         self.c = ''
@@ -612,15 +613,15 @@
 
     def generate_w(self, target_bytes, background_bytes):
 
         res = self.get_slice_res(target_bytes, background_bytes)
         self.logger.info(f'【generate_w】识别结果：{res}')
 
         # 读取slide.js执行get_w()方法
-        with open(JS_FILE_PATH, 'r', encoding='utf-8') as f:
+        with open(self.generate_w_js_file_path, 'r', encoding='utf-8') as f:
             js = f.read()
 
         ctx = execjs.compile(js)
 
         gtrace = GTrace()
 
         # -10，图片不是从头部开始的
@@ -774,14 +775,18 @@
         self.logger.info(f'【get_cookie】请求响应数据：{response.text}')
 
         for k, v in self.session.cookies.items():
             print(f'{k}: {v}')
 
     def run(self):
 
+        if not self.generate_w_js_file_path:
+            print('缺少js解密文件')
+            return
+
         self.if_captcha()
         print(f"第一次请求，if_captcha")
 
         print('-'.center(50, '-'))
 
         self.get_gt_and_challenge()
         print(f"第二次请求，获取gt和challenge")
@@ -834,15 +839,20 @@
         self.login()
         print('-'.center(50, '-'))
 
         if self.sso_session_id:
             print(f"第十一次请求，获取cookie")
             self.get_cookie()
 
-    def get_session_id(self):
+    def get_session_id(self, generate_w_js_file_path: str = None):
+
+        self.generate_w_js_file_path = generate_w_js_file_path
+
+        if not self.generate_w_js_file_path:
+            raise Exception('缺少js解密文件')
 
         for i in range(3):
 
             self.if_captcha()
 
             self.get_gt_and_challenge()
 
@@ -876,37 +886,49 @@
 
 class XunFeiWeb(LLMBase):
     model_name = 'XunFeiWeb'
     base_url = 'https://xinghuo.xfyun.cn'
 
     def __init__(
             self,
+            cookie: str = None,
             account: str = None,
             password: str = None,
-            cookie: str = None,
+            error_dir: str = None,
             sso_session_id: str = None,
             logger_obj: logging.Logger = None,
-            error_dir: str = None,
+            generate_w_js_file_path: str = None,
             *args,
             **kwargs
     ):
+        """
+        :param generate_w_js_file_path: js解密文件
+        :param account: 账号
+        :param password: 密码
+        :param cookie: cookie
+        :param sso_session_id: ssoSessionId
+        :param logger_obj: 日志对象
+        :param error_dir: 错误保存目录
+        """
+
         self.logger = logger_obj
         self.account = account
         self.password = password
         self.cookie = cookie
         self._sso_session_id = sso_session_id
         self._account_id: str = ''
         self.__gt_token = ''
         self.error_dir = error_dir
+        self.generate_w_js_file_path = generate_w_js_file_path
 
         super().__init__()
         self.request_session.cookies.update(self.cookies_dict)
 
         if self._sso_session_id:
-            self.request_session.cookies.set('ssoSessionId', self._sso_session_id)
+            self.request_session.cookies.update({'ssoSessionId': self._sso_session_id})
 
         self.__headers = {
             'Accept': "*/*",
             "Accept-Encoding": "gzip, deflate, br, zstd",
             "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
 
             "Cache-Control": "no-cache",
@@ -925,25 +947,27 @@
         self.chat_id: str = ''
         self.single_answer: str = ''
         self.single_answer_obj: Optional[AiAnswer] = None
         self.single_answer_padding: str = ''
 
     @property
     def account_id(self) -> str:
+        """ 获取cookie中的账号id """
 
         if self._account_id:
             return self._account_id
 
         result = self.login()
         if result:
             return self._account_id
         raise LoginFailError(f'{self.model_name} login failed')
 
     @property
     def sso_session_id(self) -> str:
+        """ 获取ssoSessionId """
 
         if self._sso_session_id:
             return self._sso_session_id
 
         result = self.login()
         if result:
             return self._sso_session_id
@@ -960,96 +984,163 @@
     def decode(text):
         try:
             decoded_data = base64.b64decode(text).decode('utf-8')
             return decoded_data
         except Exception as e:
             return ''
 
+    def check_response_status(self, response: requests.Response, jsonfy: bool, function_name: str = None):
+
+        result = {
+            'is_success': True,
+            'response': response,
+            'continue': True
+        }
+
+        if response.status_code == 200:
+            if jsonfy:
+                result['response'] = self.parse_data(response, function_name=function_name)
+
+        elif response.status_code == 401:
+            self.logger.error(f'The response status_code is 401, need to login again.')
+
+            self.logger.info('即将尝试重新登录...')
+            login_result = self.login()
+            if login_result:
+                self.logger.info('重新登录成功，即将重新请求...')
+                result['is_success'] = False
+
+            self.logger.error('重新登录失败，即将退出程序...')
+            result['continue'] = False
+
+        else:
+            self.logger.error(f'【{self.model_name}】 get failed, status_code: 【{response.status_code}】')
+            result['continue'] = False
+
+        return result
+
     def get(
             self,
             url: str,
             headers: dict = None,
             params: Optional[dict] = None,
-    ) -> Optional[requests.Response]:
+            function_name: str = None,
+            jsonfy: bool = False,
+    ) -> Optional[Union[requests.Response, dict]]:
 
         for i in range(3):
             try:
                 if not headers:
                     headers = self.__headers
+
                 response = self.request_session.get(
                     url,
                     headers=headers,
                     params=params,
                     verify=False,
                 )
 
-                if response.status_code == 200:
-                    return response
+                check_result = self.check_response_status(response, jsonfy=jsonfy, function_name=function_name)
+
+                if check_result['is_success']:
+                    return check_result['response']
+                elif check_result['continue']:
+                    continue
                 else:
-                    self.logger.error(f'【{self.model_name}】 get failed, status_code: 【{response.status_code}】')
+                    return
+
+            except NeedLoginError:
+
+                self.logger.info('即将尝试重新登录...')
+                result = self.login()
+
+                # 如果成功重新登录，则重新请求
+                if result:
+                    self.logger.info('重新登录成功，即将重新请求...')
+                    continue
+
+                # 如果登录失败，则跳出循环，直接返回
+                self.logger.error('重新登录失败，即将退出程序...')
+                break
+            except UnexpectResponseError:
+                # TODO 这里暂时留空，后续补充
+                pass
+
             except:
                 self.logger.error(f'【{self.model_name}】 get request got an unexpected error.', exc_info=True)
-        raise APIConnectionError(f'【{self.model_name}】 get request failed. URL: 【{url}】')
 
     def post(
             self,
             url: str,
             headers: dict = None,
             params: Optional[dict] = None,
-            json: Optional[dict] = None,
+            _json: Optional[dict] = None,
             data: [dict, str] = None,
-            stream=False
-    ) -> Optional[requests.Response]:
+            stream=False,
+            function_name: str = None,
+            jsonfy: bool = False,
+    ) -> Optional[Union[requests.Response, dict]]:
 
         # 防止网络错误，设置重试次数
         for i in range(3):
 
             try:
                 if not headers:
                     headers = self.__headers
 
                 response = self.request_session.post(
                     url,
                     headers=headers,
                     params=params,
-                    json=json,
+                    json=_json,
                     data=data,
                     stream=stream,
                     verify=False
                 )
 
-                if response.status_code == 200:
-                    return response
-                elif response.status_code == 401:
-                    self.logger.error(f'【{self.model_name}】 post failed, status_code: 【{response.status_code}】')
-                    self.logger.info('即将尝试重新登录...')
-                    result = self.login()
-                    if result:
-                        self.logger.info('重新登录成功，即将重新请求...')
-                        continue
-                    self.logger.error('重新登录失败，即将退出程序...')
-                    break
+                check_result = self.check_response_status(response, jsonfy=jsonfy, function_name=function_name)
+
+                if check_result['is_success']:
+                    return check_result['response']
+                elif check_result['continue']:
+                    continue
                 else:
-                    self.logger.error(f'【{self.model_name}】 post failed, status_code: 【{response.status_code}】')
+                    return
+
+            except NeedLoginError:
+
+                self.logger.info('即将尝试重新登录...')
+                result = self.login()
+
+                # 如果成功重新登录，则重新请求
+                if result:
+                    self.logger.info('重新登录成功，即将重新请求...')
+                    continue
+
+                # 如果登录失败，则跳出循环，直接返回
+                self.logger.error('重新登录失败，即将退出程序...')
+                break
+            except UnexpectResponseError:
+                # TODO 这里暂时留空，后续补充
+                self.logger.error('出现了预期外的回应数据...')
             except:
                 self.logger.error(f'【{self.model_name}】 post request got an unexpected error.', exc_info=True)
 
-        raise APIConnectionError(f'【{self.model_name}】 post request failed. URL: 【{url}】')
-
     def login(self) -> bool:
         """登录新方法，添加极验滑块的逆向"""
 
         try:
             handler = WebLogin(
                 account_name=self.account,
                 password=self.password,
             )
-            session_id = handler.get_session_id()
+            session_id = handler.get_session_id(self.generate_w_js_file_path)
 
             if session_id:
+                self.request_session.cookies.update({'ssoSessionId': session_id})
                 self.request_session.headers.update({'Cookie': f'ssoSessionId={session_id}'})
                 self._sso_session_id = session_id
                 return True
         except:
             self.logger.error(f'【{self.model_name}】 login failed', exc_info=True)
 
         return False
@@ -1078,137 +1169,156 @@
                 self.logger.error(
                     f'【{self.model_name}】 login failed, code: 【{code}】, message: 【{resp_json.get("desc")}】')
                 return False
 
             self.logger.info(f'【{self.model_name}】 login success')
 
             self._sso_session_id = data['ssoSessionId']
-            self.request_session.cookies.set('ssoSessionId', data['ssoSessionId'])
-            self.request_session.cookies.set('account_id', data['account_id'])
+            self._account_id = data['account_id']
+            self.request_session.cookies.update({'ssoSessionId': data['ssoSessionId']})
+            self.request_session.cookies.update({'account_id': data['account_id']})
 
             return True
         except:
             self.logger.error(f'【{self.model_name}】 login request got an unexpected error.', exc_info=True)
             return False
 
-    def get_chat_list(self) -> List[dict]:
+    def get_chat_list(self) -> dict:
         """获取会话列表"""
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/chat-list'
 
-        response = self.get(url=url)
-        return self.parse_data(response.json(), 'get_chat_list')
+        return self.get(url=url, function_name='get_chat_list', jsonfy=True)
 
     def get_prompt_list(self) -> dict:
         """
         获取提示列表
         :return：提示列表
         """
 
         url = self.base_url + '/iflygpt/u/prompt/getPromptList'
 
-        response = self.get(url)
-        return self.parse_data(response.json(), 'get_prompt_list')
+        return self.get(url=url, function_name='get_prompt_list', jsonfy=True)
 
     def get_chat_history(self, chat_id: [int, str]) -> dict:
         """
         获取会话记录
         :param chat_id：会话 ID
         :return：会话记录
         """
 
         url = self.base_url + f'/iflygpt/u/chat_history/all/{chat_id}'
 
-        response = self.get(url)
-
-        return self.parse_data(response.json(), 'get_chat_history')
+        data = self.get(url=url, function_name='get_chat_history', jsonfy=True)
+        return data.get('data', {})
 
-    def create_new_chat(self, bot_id: str = None) -> str:
+    def create_new_chat(self, chat_name: str = None, bot_id: str = None) -> str:
         """
         创建新的会话，注意，在新的会话窗口未被使用前，重复创建返回的chat_id是一样的
-        :return：chat_id
+        :return：成功时返回新建的chat_id；失败时返回空字符串
         """
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/create-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
 
         if bot_id:
             data = json.dumps({"botId": bot_id})
         else:
             data = "{}"
 
-        response = self.post(url=url, headers=headers, data=data)
-        data = self.parse_data(response.json(), 'create_new_chat')
-        chat_id = data.get('id')
+        data = self.post(url=url, headers=headers, data=data, function_name='create_new_chat', jsonfy=True)
+
+        if not data:
+            return ''
+
+        chat_id = data.get('data', {}).get('id')
 
         if chat_id:
+
+            if chat_name:
+                self.rename_chat(chat_id, chat_name)
+
             self.chat_id = chat_id
             return chat_id
 
-    def rename_chat(self, chat_id: int, name: str) -> bool:
+    def rename_chat(self, chat_id: int, chat_name: str) -> dict:
         """
         重命名会话
         :param chat_id：会话 ID
-        :param name：新的会话名
+        :param chat_name：新的会话名
         :return：bool
         """
 
+        # 名称长度存在限制，截取前15个字符
+        chat_name = chat_name[:15]
+
         url = self.base_url + '/iflygpt/u/chat-list/v1/rename-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
 
-        _json = {'chatListId': chat_id, 'chatListName': name}
+        _json = {'chatListId': chat_id, 'chatListName': chat_name}
 
-        response = self.post(url=url, headers=headers, json=_json)
-        return self.parse_data(response.json(), 'rename_chat') or False
+        return self.post(url=url, headers=headers, _json=_json, function_name='rename_chat', jsonfy=True)
 
-    def delete_chat(self, chat_id: int) -> bool:
+    def delete_chat(self, chat_id: int) -> dict:
         """
         删除会话
         :param chat_id：会话 ID
         :return：bool
         """
 
         url = self.base_url + '/iflygpt/u/chat-list/v1/del-chat-list'
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json;charset=UTF-8'
         _json = {'chatListId': chat_id}
 
-        response = self.post(url=url, headers=headers, json=_json)
-        return self.parse_data(response.json(), 'delete_chat') or False
+        return self.post(url=url, headers=headers, _json=_json, function_name='delete_chat', jsonfy=True)
 
     def get_chat_sid(self, chat_id: str) -> str:
         """
         通过会话id获取最新的机器人消息的sid；
         该值与chat_id一起确保了会话的上下文记忆
         新会话没有消息时，返回空字符串；
         """
 
         try:
             history_list = self.get_chat_history(chat_id)
             return history_list[-1]["historyList"][-1]["sid"]
         except:
             self.logger.error(f'【{self.model_name}】 get_chat_sid failed, chat_id: 【{chat_id}】')
 
-    def parse_data(self, resp_json, function_name):
+    def parse_data(self, response: Optional[requests.Response], function_name: str = None) -> dict:
+
+        if not response:
+            self.logger.error(f'【{self.model_name}】 search_bot failed.')
+            return {}
 
+        resp_json = response.json()
         code = resp_json.get('code')
         if code != 0:
             self.logger.error(
                 f'【{self.model_name}】 {function_name} failed, code: 【{code}】, message: 【{resp_json.get("desc")}】')
 
+            # 判断是否需要重新登录：80000错误表示token过期，需要重新登录
             if code == 80000:
-                raise NeedLoginError(
-                    f'【{self.model_name}】 {function_name} failed!\n\ncode: 【{code}】, message: 【{resp_json.get("desc")}】')
-
-            raise Exception(
-                f'【{self.model_name}】 {function_name} got an unexpected error.\n\ncode: 【{code}】, message: 【{resp_json.get("desc")}】')
+                msg = (f'【{self.model_name}】 {function_name} failed! Need re-login!\n\n'
+                       f'code: 【{code}】, message: 【{resp_json.get("desc")}】')
+                self.logger.error(msg)
+
+                raise NeedLoginError(msg)
+
+            # 非预期响应
+            msg = (f'【{self.model_name}】 {function_name} got an unexpected response.\n\n'
+                   f'code: 【{code}】, message: 【{resp_json.get("desc")}】\n\n'
+                   f'full data: 【{response.text}】\n\n')
+            self.logger.error(msg)
+            raise UnexpectResponseError(msg)
 
-        return resp_json.get('data')
+        return resp_json
 
     def ask(
             self,
             question: str,
             gt_token: str = None,
             chat_id: str = None,
             callback_func=None,
@@ -1251,15 +1361,15 @@
             'sid': self.get_chat_sid(chat_id),
             'GtToken': gt_token or self.gt_token,
             'clientType': client_type
         }
 
         response = self.post(url=url, headers=headers, data=data, stream=True)
 
-        if response.status_code != 200:
+        if not response:
             self.logger.error(f'【{self.model_name}】 ask failed, status_code: 【{response.status_code}】')
             return AiAnswer()
 
         self.single_answer = ''
         for line in response.iter_lines():
 
             if not line:
@@ -1271,15 +1381,16 @@
             if missing_padding != 0:
                 encoded_data += b'=' * (4 - missing_padding)
 
             if self.decode(encoded_data) != 'zw':
                 answer = self.decode(encoded_data).replace('\n\n', '\n')
 
                 if answer.startswith('```') and answer.endswith('```'):
-                    answer = '【任务执行中】'
+                    answer = ''
+                    # answer = '【任务执行中】'
 
                 self.single_answer_padding = answer
 
                 # 执行回调函数，如果有的话
                 if callable(callback_func):
                     try:
                         self.logger.debug(f"执行回调函数：内容【{answer}】")
@@ -1303,42 +1414,42 @@
             content=self.single_answer,
             is_success=True,
             conversation_id=chat_id,
         )
 
         return self.single_answer_obj
 
-    def search_bot(self, bot_name: str):
+    def search_bot(self, bot_name: str) -> dict:
         """根据名称搜索助手"""
 
         url = self.base_url + '/iflygpt/bot/search'
 
         data = {
             "searchValue": bot_name,
             "pageIndex": 1,
             "pageSize": 45,
             "botType": ""
         }
 
-        response = self.post(url=url, json=data)
-        return self.parse_data(response.json(), 'search_bot')
+        return self.post(url=url, _json=data, function_name='search_bot', jsonfy=True)
 
     def reset_bot(self, bot_id: str, chat_id: str):
         """
         【待完成】
         助手2.0重置话题
         """
         url = 'https://xinghuo.xfyun.cn/iflygpt/u/bot/v2/restart'
 
         params = {
             'botId': bot_id,
             'chatId': chat_id
         }
 
-        response = self.get(url=url, params=params)
+        response = self.get(url=url, params=params, function_name='reset_bot')
+
         return response.text
 
     def get_gt_token(self):
         """
         【待完成】
         对于gt_token，经分析是极验的风控，定时将旧的gt_token更换
         但讯飞似乎并没有进行验证
@@ -1360,7 +1471,75 @@
         headers = self.__headers.copy()
         headers['Content-Type'] = 'application/json'
         headers['AppID'] = 'ihuqg3dmuzcr2kmghumvivsk7c3l4joe'
         headers['Host'] = 'riskct.geetest.com'
 
         response = requests.post(url=url, json=data, verify=False, headers=headers)
         print(response.text)
+
+
+class XunFeiVoice(LLMBase):
+    model_name = 'XunFeiVoice'
+    base_url = 'https://xinghuo.xfyun.cn'
+
+    def __init__(
+            self,
+            cookie: str = None,
+            account: str = None,
+            password: str = None,
+            error_dir: str = None,
+            sso_session_id: str = None,
+            logger_obj: logging.Logger = None,
+            generate_w_js_file_path: str = None,
+            uid: str = None,
+    ):
+
+        if not uid:
+            uid = uuid.uuid4().hex
+        self.uid = uid
+
+        self.logger = logger_obj
+        self.account = account
+        self.password = password
+        self.cookie = cookie
+        self._sso_session_id = sso_session_id
+        self._account_id: str = ''
+        self.__gt_token = ''
+        self.error_dir = error_dir
+        self.generate_w_js_file_path = generate_w_js_file_path
+
+        super().__init__()
+
+        self.request_session.cookies.update(self.cookies_dict)
+
+        if self._sso_session_id:
+            self.request_session.cookies.update({'ssoSessionId': self._sso_session_id})
+
+        self.__tts_sign_header = {
+            'Accept': 'application/json, text/plain, */*',
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Accept-Language': 'zh-CN,zh;q=0.9',
+            'Connection': 'keep-alive',
+            # 'Cookie': self.cookie,
+            'Origin': 'https://xinghuo.xfyun.cn',
+            'Referer': 'https://xinghuo.xfyun.cn/desk',
+            'sec-ch-ua': '"Chromium";v="112", "Google Chrome";v="112", "Not:A-Brand";v="99"',
+            'sec-ch-ua-mobile': '?1',
+            'sec-ch-ua-platform': '"Windows"',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-origin',
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36'
+        }
+
+        # ################################# 文本转语音相关 #################################
+
+        self.app_id: str = ''
+
+        self.tts_receive_data: dict = {}  # 流式传送，用来接收语音数据
+        self.tts_audio_file_path: str = ''  # 语音文件保存路径
+        self.tts_text: str = ''  # 语音文本内容
+        self.tts_voice_choice: str = 'x4_lingxiaoqi'  # 音色选择
+        self.tts_url_expires: int = 0  # 语音合成url过期时间
+        self.tts_authorization: str = ''  # 语音合成授权
+        self.__tts_wss_url: str = ''  # 语音合成url，300秒内有效
+        self.__is_tts_websocket_open: bool = False  # 语音合成websocket是否开启
```

## Comparing `zibuyu_LLM-0.1.9.dist-info/METADATA` & `zibuyu_LLM-2.1.19.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zibuyu-LLM
-Version: 0.1.9
+Version: 2.1.19
 Summary: 子不语个人工具包-LLM
 Author: 子不语
 License: MIT
 Keywords: LLM,zibuyu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -34,29 +34,34 @@
 - 深度求索（DeepSeek）
 - 月之暗面（Kimi）
 - 海螺问问（MinMax）
 - 通义千问（Qwen）
 - 通义星辰（XinChen)
 - 通义万相（XinXiang）
 - 讯飞星火（Spark）
+- 聆心智能（Emohaa）
+- 秘塔搜索（Metaso）
+- 阶跃星辰（StepChat）
 
 # 版本记录
 
-`0.1.9`：讯飞星火部分添加自动鉴权
+`2.1.19`：新增阶跃星辰
 
-`0.0.9`：修复由于类型注解引起的版本不兼容问题
+`1.1.19`：新增聆心智能与秘塔搜索
 
-`0.0.8`：修复由于类型注解引起的版本不兼容问题
+`0.1.16`：海螺问问添加鉴权出错重试机制
 
-`0.0.7`：统一各模型交互输出类型
+`0.1.12`：讯飞星火添加请求出错重试机制
 
-`0.0.6`：修改讯飞星火调用的传值
+`0.1.11`：修改讯飞星火请求出错判断
 
-`0.0.5`：增加error与types模块
+`0.1.10`：修改bug
 
-`0.0.4`：修复导包路径问题
+`0.1.9`：讯飞星火部分添加自动鉴权
+
+`0.0.9`：修复由于类型注解引起的版本不兼容问题
 
 `0.0.3`：修复导包路径问题
 
 `0.0.2`：无变化，增加Readme文件
 
 `0.0.1`：第一次上传
```

## Comparing `zibuyu_LLM-0.1.9.dist-info/RECORD` & `zibuyu_LLM-2.1.19.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 zibuyu_llm_api/__init__.py,sha256=Ox3V8_X8l52LqJ_ATAWv0xpxBZxq5o1xn16TcEvSUl4,305
-zibuyu_llm_api/minmax_api.py,sha256=6gZMHkmSfwsmbFtjkJF2W9uUX35zmdk1vLwIlcUuOJo,31879
-zibuyu_llm_web/__init__.py,sha256=1YEBJuq9b5XG8jUOtgdrMNDiSiHZ9_OCT6PxH_xDoiY,735
+zibuyu_llm_api/minmax_api.py,sha256=86tA4Fey-WsUoKziwT7WM8X-6UVGYEftleJ2xnDLz5Q,30976
+zibuyu_llm_web/__init__.py,sha256=cxqRec1toutUxIA0Mc8Zx3lpjlqSxDFuVV3783IRtXU,909
 zibuyu_llm_web/baichuan.py,sha256=lFq8jX7VwTBqB9EP31-H1Zj-WIiDWD4JScVMiq9yxUA,7376
-zibuyu_llm_web/base.py,sha256=C2BF_5tdCYt4XzWiWpQBlA3Gc3HfQS7suDl5yOVwGCU,7104
-zibuyu_llm_web/deepseek.py,sha256=b7buJU59WMri4qqulb_T2HuBEqsTtkoulI9M4aPRzpc,14789
-zibuyu_llm_web/errors.py,sha256=Vib55tBOR1goqM7ddmx51TbJ8vKEXOCJEqcbvjTNaWw,732
-zibuyu_llm_web/kimi.py,sha256=kWj7tUqTOyFsbe60bFhg6dcNdzNKtDQ0kAIxEvSFvdU,9962
-zibuyu_llm_web/minmax.py,sha256=TUbX4Dzn3JP9vNYdYdeYzcZIJgBK-tySdypHQF12URc,37747
+zibuyu_llm_web/base.py,sha256=UKcYa2l84I92qXfN3ClSjf-ypzhNXlnOr6F9465Zny8,8509
+zibuyu_llm_web/deepseek.py,sha256=iIPPhYATkZjgNazjiKU7z_89EOev6uuNocnC1HYIgZg,15556
+zibuyu_llm_web/emohaa.py,sha256=EhhI08tlDYPmhytBe6lvuPE4miEzBRxemp85Kekx-0w,2783
+zibuyu_llm_web/errors.py,sha256=EPjEXZJTWyhUz-LLnTra7Rg6Qu2EjpdYog2_QE-iEs8,807
+zibuyu_llm_web/kimi.py,sha256=zw36tKtv89J3W_i4U3rCY5GIZpeC1IraE1oRv_GcJ48,11202
+zibuyu_llm_web/metaso.py,sha256=3lrjs9J4OfJae-awk9iJkrw88ZD0Ynul-UkUv6oZ6QY,11531
+zibuyu_llm_web/minmax.py,sha256=g-BFdG2PLM_zL6meb-ah34wP84NP89L8x4OKw9nLRI8,44926
 zibuyu_llm_web/qwen.py,sha256=ja3fyFtY6bQmjCWNtcOtgMIRt6RSgtuYmNxDCQBk5oU,37730
-zibuyu_llm_web/types.py,sha256=a_kIEwO3gK8tHgHqfYOi7ug2qNK9s54PDjEdm1Z5ZKg,5308
-zibuyu_llm_web/wanxiang.py,sha256=YU9R42VaxWlY7gpcT_qAkguSqhCfDuK19-lpWaWgRDA,8118
-zibuyu_llm_web/xinchen.py,sha256=PTkPhh-S8gsWr6ULAvJV2E2kwBtO95lKohyxQiGA_hE,14705
-zibuyu_llm_web/xunfei.py,sha256=3PtnE7Tv9Hs1r4AAUfPkGXnVmJIlEWB28h1JQ1_1sPo,55663
-zibuyu_LLM-0.1.9.dist-info/METADATA,sha256=4RikLUzMc_jtRXXy8MfEQ7W0a5aPZkASb55eRVJqOYU,1621
-zibuyu_LLM-0.1.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-zibuyu_LLM-0.1.9.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
-zibuyu_LLM-0.1.9.dist-info/RECORD,,
+zibuyu_llm_web/step_chat.py,sha256=miDqwEP-6f-wzaFEKVQfd-vfYDwtWbcA5t2QVK9UkeU,14134
+zibuyu_llm_web/types.py,sha256=OHHCYjl66Zl8V_NBxoYKHEIidwjxtj_k89I6sx9PHIw,5355
+zibuyu_llm_web/wanxiang.py,sha256=SRGH5iCrHg9zzr9GRhyjF8UulPrwwwYAEkgeEg6aazU,8097
+zibuyu_llm_web/xinchen.py,sha256=gY0YGYLSaChNSjemSnKPgHGd58jx3HllGKYpaJoJse0,14705
+zibuyu_llm_web/xunfei.py,sha256=qDB4mxLincaYG35sJfKFW9G8fFACM5IC2Lb6Xua8wfE,62458
+zibuyu_LLM-2.1.19.dist-info/METADATA,sha256=SIYciduaJwi803JyD3vVEEDbgjkOXiaamK1dbb6Mb3c,1739
+zibuyu_LLM-2.1.19.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+zibuyu_LLM-2.1.19.dist-info/top_level.txt,sha256=QF6FI2Tcc78mYBpfy15YWDU-j16KK_2WqGF-3kj8Jew,30
+zibuyu_LLM-2.1.19.dist-info/RECORD,,
```

