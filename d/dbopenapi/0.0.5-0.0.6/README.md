# Comparing `tmp/dbopenapi-0.0.5.tar.gz` & `tmp/dbopenapi-0.0.6.tar.gz`

## Comparing `dbopenapi-0.0.5.tar` & `dbopenapi-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/dbopenapi.pyproj
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/OpenApi.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/code_realtime_account.py
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/src/dbopenapi/tr_code_to_path.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/LICENSE
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/README.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dbopenapi-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/dbopenapi.pyproj
+-rw-r--r--   0        0        0    11448 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/src/dbopenapi/OpenApi.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/src/dbopenapi/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/src/dbopenapi/code_realtime_account.py
+-rw-r--r--   0        0        0    12427 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/src/dbopenapi/tr_code_to_path.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/README.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 dbopenapi-0.0.6/PKG-INFO
```

### Comparing `dbopenapi-0.0.5/dbopenapi.pyproj` & `dbopenapi-0.0.6/dbopenapi.pyproj`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.5/src/dbopenapi/OpenApi.py` & `dbopenapi-0.0.6/src/dbopenapi/OpenApi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ﻿import asyncio
-import aiohttp
 import json
+import aiohttp
 from dbopenapi.tr_code_to_path import tr_code_to_path
 from dbopenapi.code_realtime_account import code_realtime_account
 
-BASE_URL = "https://openapi.db-fi.com:8443"
-WSS_URL_REAL = "wss://openapi.db-fi.com:7070/websocket"
-WSS_URL_SIMULATION = "wss://openapi.db-fi.com:17070/websocket"
+BASE_URL = 'https://openapi.db-fi.com:8443'
+WSS_URL_REAL = 'wss://openapi.db-fi.com:7070'
+WSS_URL_SIMULATION = 'wss://openapi.db-fi.com:17070'
 
 #해외선물옵션
-WSS_URL_REAL_overseas_future = "wss://openapi.db-fi.com:7071/websocket"
+WSS_URL_GLOBAL = 'wss://openapi.db-fi.com:7071'
 
 class ResponseValue:
     def __init__(
         self,
         cont_yn: str,
         cont_key: str,
         body: dict,
@@ -21,276 +21,283 @@
         self.cont_yn = cont_yn
         self.cont_key = cont_key
         self.body = body
 
 class OpenApi:
     def __init__(self):
         super().__init__()
-        
-        self._access_token = '';
-        self.expires_in = 0;
-        self._http = None;
-        self._websocket = None;
-        self._connected:bool = False;
-        self._is_simulation:bool = False;
-        self._last_message:str = "";
-        self._mac_address : str|None = None;
+
+        self._access_token = ''
+        self.expires_in = 0
+        self._http = None
+        self._websocket = None
+        self._connected:bool = False
+        self._is_simulation:bool = False
+        self._last_message:str = ''
+        self._mac_address : str = ''
     
         # 이벤트 핸들러
-        self._on_message = lambda sender, msg: print(f"on_message: {msg}");
-        self._on_realtime = lambda sender, trcode, key, realtimedata: print(f"on_realtime: {trcode}, {key}, {realtimedata}")
-        self._is_async_on_message:bool = False;
-        self._is_async_on_realtime:bool = False;
+        self._on_message = lambda sender, msg: print(f'on_message: {msg}')
+        self._on_realtime = lambda sender, trcode, key, realtimedata: print(f'on_realtime: {trcode}, {key}, {realtimedata}')
+        self._is_async_on_message:bool = False
+        self._is_async_on_realtime:bool = False
 
     @property
     def connected(self) -> bool:
-        """로그인 연결상태.
+        '''로그인 연결상태.
         True: 연결됨, False: 연결안됨
 
         A readonly property.
-        """
+        '''
         return self._connected
     
     @property
     def is_simulation(self) -> bool:
-        """서버모드
+        '''서버모드
         True: 모의투자, False: 실투자
 
         A readonly property.
-        """
+        '''
         return self._is_simulation
 
     @property
     def last_message(self) -> str:
-        """last error message.
+        '''last error message.
 
         A readonly property.
-        """
+        '''
         return self._last_message
 
     @property
     def access_token(self) -> str:
-        """access_token 당일 재 로그인에 이용
-
-        A readonly property.
-        """
+        '''access_token 당일 재 로그인에 이용'''
         return self._access_token
 
     @property
     def mac_address(self) -> str:
-        """법인인 경우 필수 세팅"""
+        '''법인인 경우 필수 세팅'''
         return self._mac_address
 
     @mac_address.setter
     def mac_address(self, value:str) : self._mac_address = value
 
     @property
     def on_message(self) :
-        """메시지 수신 이벤트 핸들러
+        '''메시지 수신 이벤트 핸들러
         on_message(sender:OpenApi, msg:str)
-        """
+        '''
         return self._on_message
     
     @on_message.setter
-    def on_message(self, value) :
-        self._is_async_on_message = asyncio.iscoroutinefunction(value);
+    def on_message(self, value):
+        self._is_async_on_message = asyncio.iscoroutinefunction(value)
         self._on_message = value
 
     @property
     def on_realtime(self) :
-        """실시간 데이터 수신 이벤트 핸들러
+        '''실시간 데이터 수신 이벤트 핸들러
         on_realtime(sender:OpenApi, trcode:str, key:str, realtimedata:dict)
-        """
+        '''
         return self._on_realtime
     
     @on_realtime.setter
     def on_realtime(self, value) :
-        self._is_async_on_realtime = asyncio.iscoroutinefunction(value);
+        self._is_async_on_realtime = asyncio.iscoroutinefunction(value)
         self._on_realtime = value
     
     async def close(self) -> None:
-        """연결 종료"""
-        self._connected = False;
+        '''연결 종료'''
+        self._connected = False
         if self._websocket and not self._websocket.closed:
             await self._websocket.close()
         if self._http and not self._http.closed:
             await self._http.close()
 
     async def login(self, appkey:str, appsecretkey:str
                     ,*
-                    , wss_domain:str=None
-                    , access_token:str=None) -> bool:
+                    , is_simulation:bool=False
+                    , wss_domain:str=''
+                    , access_token:str='') -> bool:
         '''
-        로그인 요청
+        로그인 요청 (모의투자인 경우에는 is_simulation을 True로 설정, 해외선물옵션인 경우에는 wss_domain을 dbopenapi.WSS_URL_GLOBAL 로 설정)
         appkey: 앱키
         appsecretkey: 앱시크릿키
         *
-        wss_domain: 웹소켓 도메인(해외선물옵션인 경우에만 설정, wss://openapi.db-fi.com:7071 으로 설정)
+        is_simulation: 모의투자 여부(기본값: False)
+        wss_domain: 웹소켓 도메인(해외선물옵션인 경우에만 설정, dbopenapi.WSS_URL_GLOBAL 으로 설정)
         access_token: 토큰(기본값: ''), 토큰이 있는 경우에는 토큰을 사용하고, 없는 경우에는 새로 토큰을 가져옴
         return: True: 성공, False: 실패, 실패시 last_message에 실패사유가 저장됨
         '''
         if self._connected :
-            self._last_message = "aleady connected";
-            return True;
+            self._last_message = 'aleady connected'
+            return True
         
         timeout = aiohttp.ClientTimeout(total=10) # 10초 타임아웃
-        httpclient = aiohttp.ClientSession(timeout=timeout);
-        if access_token is None or access_token == '':
+        httpclient = aiohttp.ClientSession(timeout=timeout)
+        if access_token == '':
             # 토큰 가져오기
-            if appkey == "" or appsecretkey == "":
-                self._last_message = "appkey or appsecretkey is empty";
-                return False;
+            if appkey == '' or appsecretkey == '':
+                self._last_message = 'appkey or appsecretkey is empty'
+                return False
     
-            token_response = await httpclient.post(BASE_URL + "/oauth2/token"
+            token_response = await httpclient.post(BASE_URL + '/oauth2/token'
                         , data={'grant_type': 'client_credentials', 'appkey': appkey, 'appsecretkey': appsecretkey, 'scope': 'oob'}
-                        );
+                        )
             if token_response.status != 200:
-                await httpclient.close();
-                self._last_message = "Failed to retrieve authentication key.";
-                return False;
+                await httpclient.close()
+                self._last_message = 'Failed to retrieve authentication key.'
+                return False
     
             # 인증성공
-            response_data = await token_response.json();
-            access_token = response_data['access_token'];
-            self.expires_in = response_data['expires_in'];
+            response_data = await token_response.json()
+            access_token = response_data['access_token']
+            self.expires_in = response_data['expires_in']
         
-        httpclient.headers["Authorization"] = f"Bearer {access_token}";
-        httpclient.headers["Content-Type"] = "application/json; charset=UTF-8";
-        self._access_token = access_token;
+        httpclient.headers['Authorization'] = f'Bearer {access_token}'
+        httpclient.headers['Content-Type'] = 'application/json; charset=UTF-8'
+        self._access_token = access_token
         
-        self._http = httpclient;
-        self._connected = True;
+        self._http = httpclient
+        self._connected = True
         
         # 모의투자인지 실투자인지 구분한다.
-        CSPEQ00400 = dict();
-        response = await self.request("CSPEQ00400", CSPEQ00400);
-        if not response :
-            self._connected = False;
-            self._last_message = "Failed to require CSPEQ00400";
-            await httpclient.close();
-            return False;
-    
-        rsp_msg:str = response.body["rsp_msg"];
-        if rsp_msg.__contains__("모의투자"):
-            self._is_simulation = True;
+        # request = dict()
+        # response = await self.request('CSPEQ00400', request)
+        # if not response :
+        #     self._connected = False
+        #     self._last_message = 'Failed to require CSPEQ00400'
+        #     await httpclient.close()
+        #     return False
+    
+        # rsp_msg:str = response.body['rsp_msg']
+        # if rsp_msg.__contains__('모의투자'):
+        #     self._is_simulation = True
+
+        self._is_simulation = is_simulation
 
         # 웹소켓 연결
-        if not wss_domain:
-            wss_domain = WSS_URL_SIMULATION if self._is_simulation else WSS_URL_REAL;
-        self._connected = False;
+        if wss_domain == '':
+            wss_domain = WSS_URL_SIMULATION if self._is_simulation else WSS_URL_REAL
+        self._connected = False
         try:
-            websocket = await  httpclient.ws_connect(wss_domain)
-            self._connected = not websocket.closed;
+            websocket = await  httpclient.ws_connect(wss_domain + '/websocket')
+            self._connected = not websocket.closed
         except :
             pass
     
         if not self._connected:
-            await httpclient.close();
-            self._last_message = "websocket connection failed.";
-            return False;
+            await httpclient.close()
+            self._last_message = 'websocket connection failed.'
+            return False
     
-        self._websocket = websocket;
-        asyncio.create_task(self._websocket_listen());
+        self._websocket = websocket
+        asyncio.create_task(self._websocket_listen())
         
-        return True;
+        return True
 
     async def request(self, tr_cd:str, data:dict
                              ,*
-                             , path:str=None
-                             , cont_yn:str="N"
-                             , cont_key:str="0"
+                             , path:str=''
+                             , cont_yn:str='N'
+                             , cont_key:str=''
                              ) -> ResponseValue | None:
         '''
         TR데이터 요청
         tr_cd: TR코드
         data: 데이터
         return: 성공시 ResponseValue, 실패시 None, 실패시 last_message에 실패사유가 저장됨
         '''
-        self._last_message = "";
+        self._last_message = ''
         if not self._connected:
-            self._last_message = "Not connected";
-            return None;
+            self._last_message = 'Not connected'
+            return None
 
-        if not path:
+        if path == '':
             if not tr_code_to_path.__contains__(tr_cd):
-                self._last_message = "Not supported tr code";
-                return None;
-            path = tr_code_to_path[tr_cd];
-    
-        headers = dict();
-        headers["cont_yn"] = cont_yn;
-        headers["cont_key"] = cont_key;
-        if self._mac_address:
-            headers["mac_address"] = self._mac_address;
+                self._last_message = 'Not supported tr code'
+                return None
+            path = tr_code_to_path[tr_cd]
+    
+        headers = {
+            'cont_yn' : cont_yn,
+            'cont_key' : cont_key,
+            }
+        if self._mac_address != '':
+            headers['mac_address'] = self._mac_address
         
         try:
-            response = await self._http.post(BASE_URL + path, headers=headers, data=json.dumps(data));
+            response = await self._http.post(BASE_URL + path, headers=headers, data=json.dumps(data))
             if response.status != 200:
-                self._last_message = await response.json();
-                return None;
-            body = await response.json();
-            return ResponseValue(response.headers["cont_yn"], response.headers["cont_key"], body);
+                self._last_message = await response.json()
+                return None
+            body = await response.json()
+            return ResponseValue(response.headers['cont_yn'], response.headers['cont_key'], body)
         except Exception as e:
-            self._last_message = e;
+            self._last_message = f'exception: {e}'
 
-        return None;        
+        return None
 
     def add_realtime(self, tr_cd:str, tr_key:str) :
-        """실시간 데이터 요청
+        '''실시간 데이터 요청
         tr_cd: TR코드
         tr_key: TR키/종목코드
-        """
-        return self._realtime_request(tr_cd , tr_key, "3" if code_realtime_account.__contains__(tr_cd) else "1");
+        '''
+        return self._realtime_request(tr_cd , tr_key, '3' if code_realtime_account.__contains__(tr_cd) else '1')
 
     def remove_realtime(self, tr_cd:str, tr_key:str) :
-        """실시간 데이터 중지
+        '''실시간 데이터 중지
         tr_cd: TR코드
         tr_key: TR키/종목코드
-        """
-        return self._realtime_request(tr_cd, tr_key, "4" if code_realtime_account.__contains__(tr_cd) else "2");
+        '''
+        return self._realtime_request(tr_cd, tr_key, '4' if code_realtime_account.__contains__(tr_cd) else '2')
+
+    async def _realtime_request(self, tr_cd:str, tr_key:str, tr_type:str) -> bool:
+        if not self._connected:
+            self._last_message = 'Not connected'
+            return False
+        if self._websocket.closed:
+            self._last_message = 'websocket closed.'
+            return False
+        data = f'{{\"header\":{{\"token\":\"{self._access_token}\",\"tr_type\":\"{tr_type}\"}},\"body\":{{\"tr_cd\":\"{tr_cd}\",\"tr_key\":\"{tr_key}\"}}}}'
+        await self._websocket.send_str(data)
+        return True
 
     async def _websocket_listen(self):
         async for msg in self._websocket:
             if msg.type == aiohttp.WSMsgType.TEXT:
                 try:
-                    jsondata = json.loads(msg.data);
+                    jsondata = json.loads(msg.data)
                 except Exception as e:
-                    self._last_message = e;
-                    await self._inner_on_mesage(f"websocket exception. {e}");
-                    continue;
-                header = jsondata.get("header", None);
-                if header != None:
-                    tr_cd = header.get("tr_cd", None);
-                    rsp_msg = header.get("rsp_msg", None);
-                    if rsp_msg != None:
-                        self._last_message = ""
-                        tr_type = header.get("tr_type", None);
-                        await self._inner_on_mesage(f"{tr_cd}({tr_type}): {rsp_msg}");
-                    body = jsondata.get("body", None);
-                    tr_key = header.get("tr_key", None);
-                    if body != None:
+                    self._last_message = e
+                    await self._inner_on_mesage(f'websocket exception. {e}')
+                    continue
+                header = jsondata.get('header', None)
+                if header is not None:
+                    tr_cd = header.get('tr_cd', None)
+                    rsp_msg = header.get('rsp_msg', None)
+                    if rsp_msg is not None:
+                        self._last_message = ''
+                        tr_type = header.get('tr_type', None)
+                        await self._inner_on_mesage(f'{tr_cd}({tr_type}): {rsp_msg}')
+                    body = jsondata.get('body', None)
+                    tr_key = header.get('tr_key', None)
+                    if body is not None:
                         await self._inner_on_realtime(tr_cd, tr_key, body)
             elif msg.type == aiohttp.WSMsgType.CLOSED:
-                self._last_message = msg;
-                await self._inner_on_mesage(f"websocket closed. {msg}");
-                break;
+                self._last_message = msg
+                await self._inner_on_mesage(f'websocket closed. {msg}')
+                break
             elif msg.type == aiohttp.WSMsgType.ERROR:
-                self._last_message = msg;
-                await self._inner_on_mesage(f"websocket error. {msg}");
-
-    async def _realtime_request(self, tr_cd:str, tr_key:str, tr_type:str) -> bool:
-        if not self._connected: return False;
-        data = f"{{\"header\":{{\"token\":\"{self._access_token}\",\"tr_type\":\"{tr_type}\"}},\"body\":{{\"tr_cd\":\"{tr_cd}\",\"tr_key\":\"{tr_key}\"}}}}";
-        await self._websocket.send_str(data);
-        return True;
+                self._last_message = msg
+                await self._inner_on_mesage(f'websocket error. {msg}')
 
     async def _inner_on_mesage(self, msg:str):
         if self._is_async_on_message:
-            await self._on_message(self, msg);
+            await self._on_message(self, msg)
         else:
-            self._on_message(self, msg);
+            self._on_message(self, msg)
 
     async def _inner_on_realtime(self, trcode:str, key:str, realtimedata):
         if self._is_async_on_realtime:
-            await self._on_realtime(self, trcode, key, realtimedata);
+            await self._on_realtime(self, trcode, key, realtimedata)
         else:
-            self._on_realtime(self, trcode, key, realtimedata);
+            self._on_realtime(self, trcode, key, realtimedata)
```

### Comparing `dbopenapi-0.0.5/src/dbopenapi/tr_code_to_path.py` & `dbopenapi-0.0.6/src/dbopenapi/tr_code_to_path.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,174 +1,158 @@
 ﻿tr_code_to_path:dict = {
-            
     # 국내주식주문
-    "CSPAT00600" : "/api/v1/trading/kr-stock/order", # 주식종합주문
-    "CSPAT00700" : "/api/v1/trading/kr-stock/order-revision", # 주식정정주문
-    "CSPAT00800" : "/api/v1/trading/kr-stock/order-cancel", # 주식취소주문
-    "CSPAQ04800" : "/api/v1/trading/kr-stock/inquiry/transaction-history", # 체결/미체결조회
-    "CSPBQ00100" : "/api/v1/trading/kr-stock/inquiry/able-orderqty", # 주식주문가능수량조회
-    "CSPAQ03420" : "/api/v1/trading/kr-stock/inquiry/balance", # 주식잔고조회
-    "CDPCQ00100" : "/api/v1/trading/kr-stock/inquiry/acnt-deposit", # 계좌예수금조회
-    "CSPEQ00400" : "/api/v1/trading/kr-stock/inquiry/daliy-trade-report", # 일자별매매내역 ...
-    "FOCCQ10800" : "api/v1/trading/kr-stock/inquiry/rdterm-ernrate", # 임의기간수익률집계
-    "CSPAQ07800" : "/api/v1/trading/kr-stock/inquiry/stock-ernrate", # 종목별수익률조회
-    "CSPAQ00600" : "/api/v1/trading/kr-stock/inquiry/able-crdlimit", # 계좌별신용한도조회
-    "CSPAQ09400" : "/api/v1/trading/kr-stock/inquiry/able-crdrepayment", # 신용상환가능총수량조회
-    
+    'CSPAT00600' : '/api/v1/trading/kr-stock/order', # 주식종합주문
+    'CSPAT00700' : '/api/v1/trading/kr-stock/order-revision', # 주식정정주문
+    'CSPAT00800' : '/api/v1/trading/kr-stock/order-cancel', # 주식취소주문
+    'CSPAQ04800' : '/api/v1/trading/kr-stock/inquiry/transaction-history', # 체결/미체결조회
+    'CSPBQ00100' : '/api/v1/trading/kr-stock/inquiry/able-orderqty', # 주식주문가능수량조회
+    'CSPAQ03420' : '/api/v1/trading/kr-stock/inquiry/balance', # 주식잔고조회
+    'CDPCQ00100' : '/api/v1/trading/kr-stock/inquiry/acnt-deposit', # 계좌예수금조회
+    'CSPEQ00400' : '/api/v1/trading/kr-stock/inquiry/daliy-trade-report', # 일자별매매내역 ...
+    'FOCCQ10800' : 'api/v1/trading/kr-stock/inquiry/rdterm-ernrate', # 임의기간수익률집계
+    'CSPAQ07800' : '/api/v1/trading/kr-stock/inquiry/stock-ernrate', # 종목별수익률조회
+    'CSPAQ00600' : '/api/v1/trading/kr-stock/inquiry/able-crdlimit', # 계좌별신용한도조회
+    'CSPAQ09400' : '/api/v1/trading/kr-stock/inquiry/able-crdrepayment', # 신용상환가능총수량조회
     # 국내주식시세
-    "JCODES" : "/api/v1/quote/kr-stock/inquiry/stock-ticker", # 주식종목 조회
-    "WCODES" : "/api/v1/quote/kr-stock/inquiry/elw-ticker", # ELW 종목 조회
-    "PRICE" : "/api/v1/quote/kr-stock/inquiry/price", # 현재가조회
-    "HOGA" : "/api/v1/quote/kr-stock/inquiry/orderbook", # 호가조회
-    "CONCLUSION" : "/api/v1/quote/kr-stock/inquiry/hour-price", # 시간대별체결조회
-    "DAYTRADE" : "/api/v1/quote/kr-stock/inquiry/daily-price", # 일별체결조회
-    "RANKLIST" : "/api/v1/quote/kr-stock/inquiry/rank-list", # 주식조건상승하락조회
-    
+    'JCODES' : '/api/v1/quote/kr-stock/inquiry/stock-ticker', # 주식종목 조회
+    'WCODES' : '/api/v1/quote/kr-stock/inquiry/elw-ticker', # ELW 종목 조회
+    'PRICE' : '/api/v1/quote/kr-stock/inquiry/price', # 현재가조회
+    'HOGA' : '/api/v1/quote/kr-stock/inquiry/orderbook', # 호가조회
+    'CONCLUSION' : '/api/v1/quote/kr-stock/inquiry/hour-price', # 시간대별체결조회
+    'DAYTRADE' : '/api/v1/quote/kr-stock/inquiry/daily-price', # 일별체결조회
+    'RANKLIST' : '/api/v1/quote/kr-stock/inquiry/rank-list', # 주식조건상승하락조회
     # 국내주식시세(실시간)
-    "IS1" : "/websocket", # [실시간]주식주문체결
-    "IS0" : "/websocket", # [실시간]주식주문접수
-    "S01" : "/websocket", # [실시간]주식호가
-    "S00" : "/websocket", # [실시간]주식체결가
-    "W01" : "/websocket", # [실시간]ELW호가
-    "W00" : "/websocket", # [실시간]ELW체결
-    "U00" : "/websocket", # [실시간]업종지수체결가
-    "U03" : "/websocket", # [실시간]업종지수등락
-    "U05" : "/websocket", # [실시간]업종별투자자
-    
+    'IS1' : '/websocket', # [실시간]주식주문체결
+    'IS0' : '/websocket', # [실시간]주식주문접수
+    'S01' : '/websocket', # [실시간]주식호가
+    'S00' : '/websocket', # [실시간]주식체결가
+    'W01' : '/websocket', # [실시간]ELW호가
+    'W00' : '/websocket', # [실시간]ELW체결
+    'U00' : '/websocket', # [실시간]업종지수체결가
+    'U03' : '/websocket', # [실시간]업종지수등락
+    'U05' : '/websocket', # [실시간]업종별투자자
     # 국내선물옵션주문
-    "CFOAT00100" : "/api/v1/trading/kr-futureoption/order", # 선물옵션 주문
-    "CFOAT00200" : "/api/v1/trading/kr-futureoption/order-revision", # 선물옵션 정정주문
-    "CFOAT00300" : "/api/v1/trading/kr-futureoption/order-cancel", # 선물옵션 취소주문
-    "CFOAQ04000" : "/api/v1/trading/kr-futureoption/inquiry/transaction-history", # 선물옵션 체결조회
-    "CFOAQ42400" : "/api/v1/trading/kr-futureoption/inquiry/able-orderqty", # 선물옵션 주문가능수량
-    "CFOAQ02500" : "/api/v1/trading/kr-futureoption/inquiry/balance", # 선물옵션 잔고조회
-    "CFOAQ50100" : "/api/v1/trading/kr-futureoption/inquiry/balance-evalstatus", # 선물옵션 잔고_평가현황조회
-    "CFOAQ02600" : "/api/v1/trading/kr-futureoption/inquiry/day-rlzpnl", # 선물옵션 당일실현손익
-    "CFOEQ11100" : "/api/v1/trading/kr-futureoption/inquiry/deposit-detail", # 선물옵션 가정산예탁금 상세
-    "CFOHT00100" : "/api/v1/trading/night-futureoption/order", # 선물옵션 주문 (야간)
-    "CFOHT00200" : "/api/v1/trading/night-futureoption/order-revision", # 선물옵션 정정주문 (야간)
-    "CFOHT00300" : "/api/v1/trading/night-futureoption/order-cancel", # 선물옵션 취소주문 (야간)
-    "CFOHQ04000" : "/api/v1/trading/night-futureoption/inquiry/cmedt", # 선물옵션 체결조회 (야간)
-    "CFOHQ02500" : "/api/v1/trading/night-futureoption/inquiry/balance", # 선물옵션 잔고조회 (야간)
-    
+    'CFOAT00100' : '/api/v1/trading/kr-futureoption/order', # 선물옵션 주문
+    'CFOAT00200' : '/api/v1/trading/kr-futureoption/order-revision', # 선물옵션 정정주문
+    'CFOAT00300' : '/api/v1/trading/kr-futureoption/order-cancel', # 선물옵션 취소주문
+    'CFOAQ04000' : '/api/v1/trading/kr-futureoption/inquiry/transaction-history', # 선물옵션 체결조회
+    'CFOAQ42400' : '/api/v1/trading/kr-futureoption/inquiry/able-orderqty', # 선물옵션 주문가능수량
+    'CFOAQ02500' : '/api/v1/trading/kr-futureoption/inquiry/balance', # 선물옵션 잔고조회
+    'CFOAQ50100' : '/api/v1/trading/kr-futureoption/inquiry/balance-evalstatus', # 선물옵션 잔고_평가현황조회
+    'CFOAQ02600' : '/api/v1/trading/kr-futureoption/inquiry/day-rlzpnl', # 선물옵션 당일실현손익
+    'CFOEQ11100' : '/api/v1/trading/kr-futureoption/inquiry/deposit-detail', # 선물옵션 가정산예탁금 상세
+    'CFOHT00100' : '/api/v1/trading/night-futureoption/order', # 선물옵션 주문 (야간)
+    'CFOHT00200' : '/api/v1/trading/night-futureoption/order-revision', # 선물옵션 정정주문 (야간)
+    'CFOHT00300' : '/api/v1/trading/night-futureoption/order-cancel', # 선물옵션 취소주문 (야간)
+    'CFOHQ04000' : '/api/v1/trading/night-futureoption/inquiry/cmedt', # 선물옵션 체결조회 (야간)
+    'CFOHQ02500' : '/api/v1/trading/night-futureoption/inquiry/balance', # 선물옵션 잔고조회 (야간)
     # 국내선물옵션시세
-    "FCODES" : "/api/v1/quote/kr-futureoption/inquiry/future-ticker", # 선물종목 조회
-    "OCODES" : "/api/v1/quote/kr-futureoption/inquiry/option-ticker", # 옵션종목 조회
-    "FPRICE" : "/api/v1/quote/kr-futureoption/inquiry/price", # 현재가조회 ...............
-    "FHOGA" : "/api/v1/quote/kr-futureoption/inquiry/orderbook", # 호가조회 ...............
-    "FDAYTRADE" : "/api/v1/quote/kr-futureoption/inquiry/daily-price", # 일별체결조회 ...............
-    "FCONCLUSION" : "/api/v1/quote/kr-futureoption/inquiry/hour-price", # 시간대별체결조회 ...............
-    
+    'FCODES' : '/api/v1/quote/kr-futureoption/inquiry/future-ticker', # 선물종목 조회
+    'OCODES' : '/api/v1/quote/kr-futureoption/inquiry/option-ticker', # 옵션종목 조회
+    'FPRICE' : '/api/v1/quote/kr-futureoption/inquiry/price', # 현재가조회 ...............
+    'FHOGA' : '/api/v1/quote/kr-futureoption/inquiry/orderbook', # 호가조회 ...............
+    'FDAYTRADE' : '/api/v1/quote/kr-futureoption/inquiry/daily-price', # 일별체결조회 ...............
+    'FCONCLUSION' : '/api/v1/quote/kr-futureoption/inquiry/hour-price', # 시간대별체결조회 ...............
     # 국내선물옵션시세(실시간)
-    "IF0" : "/websocket", # [실시간]선물옵션주문체결
-    "F01" : "/websocket", # [실시간]지수선물호가
-    "F00" : "/websocket", # [실시간]지수선물체결
-    "F91" : "/websocket", # [실시간]미니지수선물호가
-    "F90" : "/websocket", # [실시간]미니지수선물체결
-    "F71" : "/websocket", # [실시간]섹터지수선물호가
-    "F70" : "/websocket", # [실시간]섹터지수선물체결
-    "F21" : "/websocket", # [실시간]주식선물호가
-    "F20" : "/websocket", # [실시간]주식선물체결
-    "F11" : "/websocket", # [실시간]상품선물호가
-    "F10" : "/websocket", # [실시간]상품선물체결
-    "O01" : "/websocket", # [실시간]지수옵션호가
-    "O00" : "/websocket", # [실시간]지수옵션체결
-    "O21" : "/websocket", # [실시간]주식옵션호가
-    "O20" : "/websocket", # [실시간]주식옵션체결
-    "O91" : "/websocket", # [실시간]미니지수옵션호가
-    "O90" : "/websocket", # [실시간]미니지수옵션체결
-    "OB1" : "/websocket", # [실시간]K200지수위클리옵션호가
-    "OB0" : "/websocket", # [실시간]K200지수위클리옵션체결
-    "OA1" : "/websocket", # [실시간]KOSDAQ150옵션호가
-    "OA0" : "/websocket", # [실시간]KOSDAQ150옵션체결
-    "F40" : "/websocket", # [실시간]선물체결(야간)
-    "F41" : "/websocket", # [실시간]선물호가(야간)
-    "O30" : "/websocket", # [실시간]옵션체결(야간)
-    "O31" : "/websocket", # [실시간]옵션호가(야간)
-    
+    'IF0' : '/websocket', # [실시간]선물옵션주문체결
+    'F01' : '/websocket', # [실시간]지수선물호가
+    'F00' : '/websocket', # [실시간]지수선물체결
+    'F91' : '/websocket', # [실시간]미니지수선물호가
+    'F90' : '/websocket', # [실시간]미니지수선물체결
+    'F71' : '/websocket', # [실시간]섹터지수선물호가
+    'F70' : '/websocket', # [실시간]섹터지수선물체결
+    'F21' : '/websocket', # [실시간]주식선물호가
+    'F20' : '/websocket', # [실시간]주식선물체결
+    'F11' : '/websocket', # [실시간]상품선물호가
+    'F10' : '/websocket', # [실시간]상품선물체결
+    'O01' : '/websocket', # [실시간]지수옵션호가
+    'O00' : '/websocket', # [실시간]지수옵션체결
+    'O21' : '/websocket', # [실시간]주식옵션호가
+    'O20' : '/websocket', # [실시간]주식옵션체결
+    'O91' : '/websocket', # [실시간]미니지수옵션호가
+    'O90' : '/websocket', # [실시간]미니지수옵션체결
+    'OB1' : '/websocket', # [실시간]K200지수위클리옵션호가
+    'OB0' : '/websocket', # [실시간]K200지수위클리옵션체결
+    'OA1' : '/websocket', # [실시간]KOSDAQ150옵션호가
+    'OA0' : '/websocket', # [실시간]KOSDAQ150옵션체결
+    'F40' : '/websocket', # [실시간]선물체결(야간)
+    'F41' : '/websocket', # [실시간]선물호가(야간)
+    'O30' : '/websocket', # [실시간]옵션체결(야간)
+    'O31' : '/websocket', # [실시간]옵션호가(야간)
     # 국내주식/선물차트
-    "CHARTTICK" : "/api/v1/quote/kr-chart/tick", # 틱차트조회
-    "CHARTMIN" : "/api/v1/quote/kr-chart/min", # 분차트조회
-    "CHARTDAY" : "/api/v1/quote/kr-chart/day", # 일차트조회
-    "CHARTWEEK" : "/api/v1/quote/kr-chart/week", # 주차트조회
-    "CHARTMONTH" : "/api/v1/quote/kr-chart/month", # 월차트조회
-    
+    'CHARTTICK' : '/api/v1/quote/kr-chart/tick', # 틱차트조회
+    'CHARTMIN' : '/api/v1/quote/kr-chart/min', # 분차트조회
+    'CHARTDAY' : '/api/v1/quote/kr-chart/day', # 일차트조회
+    'CHARTWEEK' : '/api/v1/quote/kr-chart/week', # 주차트조회
+    'CHARTMONTH' : '/api/v1/quote/kr-chart/month', # 월차트조회
     # 해외주식주문
-    "CAZCT00100" : "/api/v1/trading/overseas-stock/order", # 해외주식 주문
-    "CAZCQ00100" : "/api/v1/trading/overseas-stock/inquiry/transaction-history", # 해외주식 체결내역조회
-    "CAZCQ00400" : "/api/v1/trading/overseas-stock/inquiry/balance-margin", # 해외주식 잔고/증거금 조회
-    "CAZCQ00200" : "/api/v1/trading/overseas-stock/inquiry/trading-history", # 해외주식 매매내역 조회
-    "CAZCQ01600" : "/api/v1/trading/overseas-stock/inquiry/trade-history", # 해외주식 거래내역 조회
-    "CAZCQ01300" : "/api/v1/trading/overseas-stock/inquiry/able-orderqty", # 해외주식 주문가능금액 조회
-    "CAZCQ00300" : "/api/v1/trading/overseas-stock/inquiry/day-rlzpnl", # 해외주식 실현손익 조회
-    "CAZCQ01400" : "/api/v1/trading/overseas-stock/inquiry/deposit-detail", # 해외주식 예수금상세
-    "CAZCQ03400" : "/api/v1/trading/overseas-stock/inquiry/avg-pur-price", # 해외주식 평균매입단가 조회
-
+    'CAZCT00100' : '/api/v1/trading/overseas-stock/order', # 해외주식 주문
+    'CAZCQ00100' : '/api/v1/trading/overseas-stock/inquiry/transaction-history', # 해외주식 체결내역조회
+    'CAZCQ00400' : '/api/v1/trading/overseas-stock/inquiry/balance-margin', # 해외주식 잔고/증거금 조회
+    'CAZCQ00200' : '/api/v1/trading/overseas-stock/inquiry/trading-history', # 해외주식 매매내역 조회
+    'CAZCQ01600' : '/api/v1/trading/overseas-stock/inquiry/trade-history', # 해외주식 거래내역 조회
+    'CAZCQ01300' : '/api/v1/trading/overseas-stock/inquiry/able-orderqty', # 해외주식 주문가능금액 조회
+    'CAZCQ00300' : '/api/v1/trading/overseas-stock/inquiry/day-rlzpnl', # 해외주식 실현손익 조회
+    'CAZCQ01400' : '/api/v1/trading/overseas-stock/inquiry/deposit-detail', # 해외주식 예수금상세
+    'CAZCQ03400' : '/api/v1/trading/overseas-stock/inquiry/avg-pur-price', # 해외주식 평균매입단가 조회
     # 해외주식시세
-    "FSTKCODES" : "/api/v1/quote/overseas-stock/inquiry/stock-ticker", # 해외주식 종목조회
-    "FSTKPRICE" : "/api/v1/quote/overseas-stock/inquiry/price", # 해외주식 현재가조회
-    "FSTKHOGA" : "/api/v1/quote/overseas-stock/inquiry/orderbook", # 해외주식 호가조회
-    "FSTKCONCLUSION" : "/api/v1/quote/overseas-stock/inquiry/hour-price", # 해외주식 시간대별체결조회
-    "FSTKCHARTTICK" : "/api/v1/quote/overseas-stock/chart/tick", # 해외주식 틱차트조회
-    "FSTKCHARTMIN" : "/api/v1/quote/overseas-stock/chart/min", # 해외주식 분차트조회
-    "FSTKCHARTDAY" : "/api/v1/quote/overseas-stock/chart/day", # 해외주식 일차트조회
-    "FSTKCHARTWEEK" : "/api/v1/quote/overseas-stock/chart/week", # 해외주식 주차트조회
-    "FSTKCHARTMONTH" : "/api/v1/quote/overseas-stock/chart/month", # 해외주식 월차트조회
-    
+    'FSTKCODES' : '/api/v1/quote/overseas-stock/inquiry/stock-ticker', # 해외주식 종목조회
+    'FSTKPRICE' : '/api/v1/quote/overseas-stock/inquiry/price', # 해외주식 현재가조회
+    'FSTKHOGA' : '/api/v1/quote/overseas-stock/inquiry/orderbook', # 해외주식 호가조회
+    'FSTKCONCLUSION' : '/api/v1/quote/overseas-stock/inquiry/hour-price', # 해외주식 시간대별체결조회
+    'FSTKCHARTTICK' : '/api/v1/quote/overseas-stock/chart/tick', # 해외주식 틱차트조회
+    'FSTKCHARTMIN' : '/api/v1/quote/overseas-stock/chart/min', # 해외주식 분차트조회
+    'FSTKCHARTDAY' : '/api/v1/quote/overseas-stock/chart/day', # 해외주식 일차트조회
+    'FSTKCHARTWEEK' : '/api/v1/quote/overseas-stock/chart/week', # 해외주식 주차트조회
+    'FSTKCHARTMONTH' : '/api/v1/quote/overseas-stock/chart/month', # 해외주식 월차트조회
     # 해외주식시세(실시간)
-    "IS2" : "/websocket", # [실시간]해외주식 주문체결
-    "V60" : "/websocket", # [실시간]해외주식 체결가
-    "V61" : "/websocket", # [실시간]해외주식 호가
-    "V10" : "/websocket", # [실시간]해외주식 지연체결가
-    "V11" : "/websocket", # [실시간]해외주식 지연호가
-    
+    'IS2' : '/websocket', # [실시간]해외주식 주문체결
+    'V60' : '/websocket', # [실시간]해외주식 체결가
+    'V61' : '/websocket', # [실시간]해외주식 호가
+    'V10' : '/websocket', # [실시간]해외주식 지연체결가
+    'V11' : '/websocket', # [실시간]해외주식 지연호가
     # 해외선물옵션주문
-    "ph700101o" : "/api/v1/trading/overseas-futureoption/order", # 주문
-    "ph700201o" : "/api/v1/trading/overseas-futureoption/order-revision", # 정정/취소주문
-    "ph710201o" : "/api/v1/trading/overseas-futureoption/inquiry/able-orderqty", # 주문가능수량조회
-    "ph800404o" : "/api/v1/trading/overseas-futureoption/inquiry/product-margin", # 상품별증거금조회
-    "ph020101o" : "/api/v1/trading/overseas-futureoption/inquiry/order-history", # 주문내역조회
-    "ph020301o" : "/api/v1/trading/overseas-futureoption/inquiry/transaction-history", # 체결내역조회
-    "ph020201o" : "/api/v1/trading/overseas-futureoption/inquiry/untransaction-history", # 미체결내역조회
-    "ph020401o" : "/api/v1/trading/overseas-futureoption/inquiry/open-interest", # 미결제 약정 조회
-    "ph131101o" : "/api/v1/trading/overseas-futureoption/inquiry/daily-open-interest", # 일별 미결제 약정내역
-    "ph131601o" : "/api/v1/trading/overseas-futureoption/inquiry/balance", # 예탁잔고현황
-    "ph135102o" : "/api/v1/trading/overseas-futureoption/inquiry/term-trade-history", # 기간별 거래내역 조회
-
+    'ph700101o' : '/api/v1/trading/overseas-futureoption/order', # 주문
+    'ph700201o' : '/api/v1/trading/overseas-futureoption/order-revision', # 정정/취소주문
+    'ph710201o' : '/api/v1/trading/overseas-futureoption/inquiry/able-orderqty', # 주문가능수량조회
+    'ph800404o' : '/api/v1/trading/overseas-futureoption/inquiry/product-margin', # 상품별증거금조회
+    'ph020101o' : '/api/v1/trading/overseas-futureoption/inquiry/order-history', # 주문내역조회
+    'ph020301o' : '/api/v1/trading/overseas-futureoption/inquiry/transaction-history', # 체결내역조회
+    'ph020201o' : '/api/v1/trading/overseas-futureoption/inquiry/untransaction-history', # 미체결내역조회
+    'ph020401o' : '/api/v1/trading/overseas-futureoption/inquiry/open-interest', # 미결제 약정 조회
+    'ph131101o' : '/api/v1/trading/overseas-futureoption/inquiry/daily-open-interest', # 일별 미결제 약정내역
+    'ph131601o' : '/api/v1/trading/overseas-futureoption/inquiry/balance', # 예탁잔고현황
+    'ph131501o' : '/api/v1/trading/overseas-futureoption/inquiry/deposit', # 예탁자산현황
+    'ph135102o' : '/api/v1/trading/overseas-futureoption/inquiry/term-trade-history', # 기간별 거래내역 조회
     # 해외선물옵션시세
-    "pibo7042" : "/api/v1/quote/overseas-futureoption/inquiry/orderbook-price", # 호가 & 현재가 조회
-    "pibo7044" : "/api/v1/quote/overseas-futureoption/inquiry/daily-price", # 일자별 시세추이
-    "pibg7301" : "/api/v1/quote/overseas-futureoption/future-chart/tick", # 해외선물 틱차트조회
-    "pibg7302" : "/api/v1/quote/overseas-futureoption/future-chart/min", # 해외선물 분차트조회
-    "pibg7303" : "/api/v1/quote/overseas-futureoption/future-chart/dwmonth", # 해외선물 일주월차트조회
-    "pibg7401" : "/api/v1/quote/overseas-futureoption/option-chart/tick", # 해외옵션 틱차트조회
-    "pibg7402" : "/api/v1/quote/overseas-futureoption/option-chart/min", # 해외옵션 분차트조회
-    "pibg7403" : "/api/v1/quote/overseas-futureoption/option-chart/dwmonth", # 해외옵션 일주월차트조회
-    
+    'pibo7042' : '/api/v1/quote/overseas-futureoption/inquiry/orderbook-price', # 호가 & 현재가 조회
+    'pibo7044' : '/api/v1/quote/overseas-futureoption/inquiry/daily-price', # 일자별 시세추이
+    'pibg7301' : '/api/v1/quote/overseas-futureoption/future-chart/tick', # 해외선물 틱차트조회
+    'pibg7302' : '/api/v1/quote/overseas-futureoption/future-chart/min', # 해외선물 분차트조회
+    'pibg7303' : '/api/v1/quote/overseas-futureoption/future-chart/dwmonth', # 해외선물 일주월차트조회
+    'pibg7401' : '/api/v1/quote/overseas-futureoption/option-chart/tick', # 해외옵션 틱차트조회
+    'pibg7402' : '/api/v1/quote/overseas-futureoption/option-chart/min', # 해외옵션 분차트조회
+    'pibg7403' : '/api/v1/quote/overseas-futureoption/option-chart/dwmonth', # 해외옵션 일주월차트조회
     # 해외선물옵션시세(실시간)
-    "O" : "/websocket", # [실시간]주문체결
-    "P" : "/websocket", # [실시간]잔고
-    "L01" : "/websocket", # [실시간]해외선물호가
-    "K01" : "/websocket", # [실시간]해외선물시세
-    "K02" : "/websocket", # [실시간]해외옵션시세
-    "L02" : "/websocket", # [실시간]해외옵션호가
-    
+    'O' : '/websocket', # [실시간]주문체결
+    'P' : '/websocket', # [실시간]잔고
+    'L01' : '/websocket', # [실시간]해외선물호가
+    'K01' : '/websocket', # [실시간]해외선물시세
+    'K02' : '/websocket', # [실시간]해외옵션시세
+    'L02' : '/websocket', # [실시간]해외옵션호가
     # 장내채권주문
-    "CSPAT02000" : "/api/v1/trading/krx-bond/order", # 채권주문
-    "CSPAT02100" : "/api/v1/trading/krx-bond/order-revision", # 채권정정주문
-    "CSPAT02200" : "/api/v1/trading/krx-bond/order-cancel", # 채권취소주문
-    "CSPAQ05700" : "/api/v1/trading/krx-bond/inquiry/transaction-history", # 채권주문체결조회
-    "CSPAQ01200" : "/api/v1/trading/krx-bond/inquiry/balance", # 채권잔고조회
-    "CSPAQ07900" : "/api/v1/trading/krx-bond/inquiry/balance-evalstatus", # 채권잔고평가조회
-
+    'CSPAT02000' : '/api/v1/trading/krx-bond/order', # 채권주문
+    'CSPAT02100' : '/api/v1/trading/krx-bond/order-revision', # 채권정정주문
+    'CSPAT02200' : '/api/v1/trading/krx-bond/order-cancel', # 채권취소주문
+    'CSPAQ05700' : '/api/v1/trading/krx-bond/inquiry/transaction-history', # 채권주문체결조회
+    'CSPAQ01200' : '/api/v1/trading/krx-bond/inquiry/balance', # 채권잔고조회
+    'CSPAQ07900' : '/api/v1/trading/krx-bond/inquiry/balance-evalstatus', # 채권잔고평가조회
     # 장내채권시세
-    "BO_SEARCH" : "/api/v1/quote/krx-bond/search", # 장내채권 상세검색
-    "BO_SISE" : "/api/v1/quote/krx-bond/inquiry/price", # 장내채권 현재가조회
-    "BO_HOGA" : "/api/v1/quote/krx-bond/inquiry/orderbook", # 장내채권 호가조회
-
+    'BO_SEARCH' : '/api/v1/quote/krx-bond/search', # 장내채권 상세검색
+    'BO_SISE' : '/api/v1/quote/krx-bond/inquiry/price', # 장내채권 현재가조회
+    'BO_HOGA' : '/api/v1/quote/krx-bond/inquiry/orderbook', # 장내채권 호가조회
     #장내채권시세(실시간)
-    "B00" : "/websocket", # [실시간]일반채권체결
-    "B01" : "/websocket", # [실시간]일반채권호가
-    "B10" : "/websocket", # [실시간]소액채권체결
-    "B11" : "/websocket", # [실시간]소액채권호가
-    
-}
+    'B00' : '/websocket', # [실시간]일반채권체결
+    'B01' : '/websocket', # [실시간]일반채권호가
+    'B10' : '/websocket', # [실시간]소액채권체결
+    'B11' : '/websocket', # [실시간]소액채권호가
+    }
```

### Comparing `dbopenapi-0.0.5/.gitignore` & `dbopenapi-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.5/LICENSE` & `dbopenapi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dbopenapi-0.0.5/pyproject.toml` & `dbopenapi-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbopenapi"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="teranum", email="teranum@gmail.com" },
 ]
 description = "package for db openapi"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dbopenapi-0.0.5/PKG-INFO` & `dbopenapi-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dbopenapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: package for db openapi
 Project-URL: Homepage, https://github.com/teranum/python-packages/tree/master/dbopenapi
 Project-URL: Issues, https://github.com/teranum/python-packages/issues
 Author-email: teranum <teranum@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,17 +32,35 @@
 ```python
 import asyncio
 import dbopenapi
 from app_keys import appkey, appsecretkey # app_keys.py 파일에 appkey, appsecretkey 변수를 정의하고 사용하세요
 
 async def main():
     api=dbopenapi.OpenApi()
-    if not await api.login(appkey, appsecretkey): return print(f"연결실패: {api.last_message}")
-    print("연결성공, 접속서버: " + ("모의투자" if api.is_simulation else "실투자"))
     
-    ... # 다른 작업 수행
+    logined:bool = False
+    logined = await api.login(appkey, appsecretkey)
+    
+    # 옵션1: 당일 발급받은 access_token 이 있는 경우, access_token 으로 로그인
+    # logined = await api.login('', '', access_token=saved__access_token)
+    
+    # 옵션2: 모의투자 일 경우 is_simulation 옵션을 True 로 설정
+    # logined = await api.login(appkey, appsecretkey, is_simulation=True)
+    
+    # 옵션3: 해외선물옵션인 경우 wss_domain 옵션을 dbopenapi.WSS_URL_GLOBAL 로 설정
+    # logined = await api.login(appkey, appsecretkey, wss_domain=dbopenapi.WSS_URL_GLOBAL)
 
+    if not logined:
+        print(f'연결실패: {api.last_message}')
+        return
+    
+    print('연결성공, 접속서버: ' + ('모의투자' if api.is_simulation else '실투자'))
+    
+    # 발급된 access_token 출력
+    print('access_token: ', api.access_token)
+    
+    ... # 다른 작업 수행
     await api.close()
 
 asyncio.run(main())
 ```
```

