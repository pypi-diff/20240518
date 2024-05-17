# Comparing `tmp/tweepy_authlib-1.4.1.tar.gz` & `tmp/tweepy_authlib-1.5.0.tar.gz`

## Comparing `tweepy_authlib-1.4.1.tar` & `tweepy_authlib-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/.editorconfig
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/.env.example
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/License.txt
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/example_json.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/example_pickle.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/tests/test_main.py
--rw-r--r--   0        0        0    34058 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/tweepy_authlib/CookieSessionUserHandler.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/tweepy_authlib/__about__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/tweepy_authlib/__init__.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/.gitignore
--rw-r--r--   0        0        0    16153 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/Readme.md
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    17378 2020-02-02 00:00:00.000000 tweepy_authlib-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/.editorconfig
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/.env.example
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/License.txt
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/example_json.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/example_pickle.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/tests/test_main.py
+-rw-r--r--   0        0        0    34626 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/tweepy_authlib/CookieSessionUserHandler.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/tweepy_authlib/__about__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/tweepy_authlib/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/.gitignore
+-rw-r--r--   0        0        0    16906 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/Readme.md
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18131 2020-02-02 00:00:00.000000 tweepy_authlib-1.5.0/PKG-INFO
```

### Comparing `tweepy_authlib-1.4.1/License.txt` & `tweepy_authlib-1.5.0/License.txt`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.4.1/example_json.py` & `tweepy_authlib-1.5.0/example_json.py`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.4.1/example_pickle.py` & `tweepy_authlib-1.5.0/example_pickle.py`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.4.1/tests/test_main.py` & `tweepy_authlib-1.5.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         CookieSessionUserHandler(screen_name='elonmusk', password='')
 
 def test_04():
     with pytest.raises(tweepy.BadRequest, match=r'.*399 - アカウントが見つかりません。.*'):
         CookieSessionUserHandler(screen_name='not__found__user', password='password')
 
 def test_05():
-    with pytest.raises(tweepy.BadRequest, match=r'.*366 - Required input \'LoginEnterAlternateIdentifierSubtask\' not provided\..*'):
+    with pytest.raises(tweepy.BadRequest, match=r'.*399 - パスワードが正しくありません。.*'):
         CookieSessionUserHandler(screen_name='elonmusk', password='password')
 
 def test_06():
 
     # 環境変数に TWITTER_SCREEN_NAME と TWITTER_PASSWORD が設定されている場合のみ実行
     if 'TWITTER_SCREEN_NAME' in os.environ and 'TWITTER_PASSWORD' in os.environ:
         print('=' * terminal_size)
```

### Comparing `tweepy_authlib-1.4.1/tweepy_authlib/CookieSessionUserHandler.py` & `tweepy_authlib-1.5.0/tweepy_authlib/CookieSessionUserHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     認証フローは2023年2月現在の Twitter Web App (Chrome Desktop) の挙動に極力合わせたもの
     requests.auth.AuthBase を継承しているので、tweepy.API の auth パラメーターに渡すことができる
 
     ref: https://github.com/mikf/gallery-dl/blob/master/gallery_dl/extractor/twitter.py
     ref: https://github.com/fa0311/TwitterFrontendFlow/blob/master/TwitterFrontendFlow/TwitterFrontendFlow.py
     """
 
-    # User-Agent と Sec-CH-UA を Chrome 124 に偽装
-    USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36'
-    SEC_CH_UA = '"Chromium";v="124", "Google Chrome";v="124", "Not-A.Brand";v="99"'
+    # User-Agent と Sec-CH-UA を Chrome 125 に偽装
+    USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36'
+    SEC_CH_UA = '"Chromium";v="125", "Google Chrome";v="125", "Not-A.Brand";v="99"'
 
     # Twitter Web App (GraphQL API) の Bearer トークン
     TWITTER_WEB_APP_BEARER_TOKEN = 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA'
 
     # 旧 TweetDeck (Twitter API v1.1) の Bearer トークン
     TWEETDECK_BEARER_TOKEN = 'Bearer AAAAAAAAAAAAAAAAAAAAAFQODgEAAAAAVHTp76lzh3rFzcHbmHVvQxYYpTw%3DckAlMINMjmCwxUcaXbAN4XqJVdgMJaHqNOFgPMK0zN1qLqLQCF'
 
@@ -87,43 +87,43 @@
             'upgrade-insecure-requests': '1',
             'user-agent': self.USER_AGENT,
         }
 
         # JavaScript 取得時の HTTP リクエストヘッダー
         self._js_headers = self._html_headers.copy()
         self._js_headers['accept'] = '*/*'
-        self._js_headers['referer'] = 'https://twitter.com/'
+        self._js_headers['referer'] = 'https://x.com/'
         self._js_headers['sec-fetch-dest'] = 'script'
         self._js_headers['sec-fetch-mode'] = 'no-cors'
         del self._js_headers['sec-fetch-user']
 
         # 認証フロー API アクセス時の HTTP リクエストヘッダー
         self._auth_flow_api_headers = {
             'accept': '*/*',
             'accept-encoding': 'gzip, deflate, br',
             'accept-language': 'ja',
             'authorization': self.TWITTER_WEB_APP_BEARER_TOKEN,
             'content-type': 'application/json',
-            'origin': 'https://twitter.com',
-            'referer': 'https://twitter.com/',
+            'origin': 'https://x.com',
+            'referer': 'https://x.com/',
             'sec-ch-ua': self.SEC_CH_UA,
             'sec-ch-ua-mobile': '?0',
             'sec-ch-ua-platform': '"Windows"',
             'sec-fetch-dest': 'empty',
             'sec-fetch-mode': 'cors',
             'sec-fetch-site': 'same-site',
             'user-agent': self.USER_AGENT,
             'x-csrf-token': None,  # ここは後でセットする
             'x-guest-token': None,  # ここは後でセットする
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'ja',
         }
 
         # GraphQL API (Twitter Web App API) アクセス時の HTTP リクエストヘッダー
-        ## GraphQL API は https://twitter.com/i/api/graphql/ 配下にあり同一ドメインのため、referer は意図的に省略している
+        ## GraphQL API は https://x.com/i/api/graphql/ 配下にあり同一ドメインのため、origin と referer は意図的に省略している
         self._graphql_api_headers = {
             'accept': '*/*',
             'accept-encoding': 'gzip, deflate, br',
             'accept-language': 'ja',
             'authorization': self.TWITTER_WEB_APP_BEARER_TOKEN,
             'content-type': 'application/json',
             'sec-ch-ua': self.SEC_CH_UA,
@@ -171,15 +171,15 @@
         if csrf_token:
             self._auth_flow_api_headers['x-csrf-token'] = csrf_token
             self._graphql_api_headers['x-csrf-token'] = csrf_token
 
         # セッションのヘッダーを GraphQL API 用のものに差し替える
         ## 以前は旧 TweetDeck API 用ヘッダーに差し替えていたが、旧 TweetDeck が完全廃止されたことで
         ## 逆に怪しまれる可能性があるため GraphQL API 用ヘッダーに変更した
-        ## cross_origin=True を指定して、twitter.com から api.twitter.com にクロスオリジンリクエストを送信した際のヘッダーを模倣する
+        ## cross_origin=True を指定して、x.com から api.x.com にクロスオリジンリクエストを送信した際のヘッダーを模倣する
         self._session.headers.clear()
         self._session.headers.update(self.get_graphql_api_headers(cross_origin=True))
 
 
     def __call__(self, request: PreparedRequest) -> PreparedRequest:
         """
         requests ライブラリからリクエスト開始時に呼び出されるフック
@@ -194,33 +194,38 @@
         # リクエストヘッダーを認証用セッションのものに差し替える
         # content-type を上書きしないよう、content-type を控えておいてから差し替える
         content_type = request.headers.get('content-type', None)
         request.headers.update(self._session.headers)  # type: ignore
         if content_type is not None:
             request.headers['content-type'] = content_type  # 元の content-type に戻す
 
+        # リクエストがまだ *.twitter.com に対して行われている場合は、*.x.com に差し替える
+        ## サードパーティー向け API は互換性のため引き続き api.twitter.com でアクセスできるはずだが、
+        ## tweepy-authlib でアクセスしている API は内部 API のため、api.twitter.com のままアクセスしていると怪しまれる可能性がある
+        assert request.url is not None
+        request.url = request.url.replace('twitter.com/', 'x.com/')
+
         # Twitter API v1.1 の一部 API には旧 TweetDeck 用の Bearer トークンでないとアクセスできないため、
         # 該当の API のみ旧 TweetDeck 用の Bearer トークンに差し替える
         # それ以外の API ではそのまま Twitter Web App の Bearer トークンを使い続けることで、不審判定される可能性を下げる
         ## OldTweetDeck の interception.js に記載の API のうち、明示的に PUBLIC_TOKEN[1] が設定されている API が対象
-        ## ref: https://raw.githubusercontent.com/dimdenGD/OldTweetDeck/main/src/interception.js
+        ## ref: https://github.com/dimdenGD/OldTweetDeck/blob/main/src/interception.js
         TWEETDECK_BEARER_TOKEN_REQUIRED_APIS = [
             '/1.1/statuses/home_timeline.json',
             '/1.1/lists/statuses.json',
             '/1.1/activity/about_me.json',
             '/1.1/statuses/mentions_timeline.json',
             '/1.1/favorites/',
             '/1.1/collections/',
         ]
-        assert request.url is not None
         if any(api_url in request.url for api_url in TWEETDECK_BEARER_TOKEN_REQUIRED_APIS):
             request.headers['authorization'] = self.TWEETDECK_BEARER_TOKEN
 
-        # upload.twitter.com 以下の API のみ、Twitter Web App の挙動に合わせいくつかのヘッダーを削除する
-        if 'upload.twitter.com' in request.url:
+        # upload.twitter.com or upload.x.com 以下の API のみ、Twitter Web App の挙動に合わせいくつかのヘッダーを削除する
+        if 'upload.twitter.com' in request.url or 'upload.x.com' in request.url:
             request.headers.pop('x-client-transaction-id', None)  # 未実装だが将来的に実装した時のため
             request.headers.pop('x-twitter-active-user', None)
             request.headers.pop('x-twitter-client-language', None)
 
         # Cookie を認証用セッションのものに差し替える
         request._cookies.update(self._session.cookies)  # type: ignore
         cookie_header = ''
@@ -276,31 +281,31 @@
 
 
     def get_graphql_api_headers(self, cross_origin: bool = False) -> Dict[str, str]:
         """
         GraphQL API (Twitter Web App API) アクセス用の HTTP リクエストヘッダーを取得する
         このリクエストヘッダーを使い独自に API リクエストを行う際は、
         必ず x-csrf-token ヘッダーの値を常に Cookie 内の "ct0" と一致させるように実装しなければならない
-        Twitter API v1.1 に使う場合は cross_origin=True を指定すること (api.twitter.com が twitter.com から見て cross-origin になるため)
-        逆に GraphQL API に使う場合は cross_origin=False でなければならない (GraphQL API は twitter.com から見て same-origin になるため)
+        Twitter API v1.1 に使う場合は cross_origin=True を指定すること (api.x.com が x.com から見て cross-origin になるため)
+        逆に GraphQL API に使う場合は cross_origin=False でなければならない (GraphQL API は x.com から見て same-origin になるため)
 
         Args:
-            cross_origin (bool, optional): 返すヘッダーを twitter.com 以外のオリジンに送信するかどうか. Defaults to False.
+            cross_origin (bool, optional): 返すヘッダーを x.com 以外のオリジンに送信するかどうか. Defaults to False.
 
         Returns:
             Dict[str, str]: GraphQL API (Twitter Web App API) アクセス用の HTTP リクエストヘッダー
         """
 
         headers = self._graphql_api_headers.copy()
 
         # クロスオリジン用に origin と referer を追加
-        # Twitter Web App から api.twitter.com にクロスオリジンリクエストを送信する際のヘッダーを模倣する
+        # Twitter Web App から api.x.com にクロスオリジンリクエストを送信する際のヘッダーを模倣する
         if cross_origin is True:
-            headers['origin'] = 'https://twitter.com'
-            headers['referer'] = 'https://twitter.com/'
+            headers['origin'] = 'https://x.com'
+            headers['referer'] = 'https://x.com/'
 
         return headers
 
 
     def logout(self) -> None:
         """
         ログアウト処理を行い、Twitter からセッションを切断する
@@ -315,16 +320,16 @@
         # ログアウト API 専用ヘッダー
         ## self._graphql_api_headers と基本共通で、content-type だけ application/x-www-form-urlencoded に変更
         logout_headers = self._graphql_api_headers.copy()
         logout_headers['content-type'] = 'application/x-www-form-urlencoded'
 
         # ログアウト API にログアウトすることを伝える
         ## この API を実行すると、サーバー側でセッションが切断され、今まで持っていたほとんどの Cookie が消去される
-        logout_api_response = self._session.post('https://api.twitter.com/1.1/account/logout.json', headers=logout_headers, data={
-            'redirectAfterLogout': 'https://twitter.com/account/switch',
+        logout_api_response = self._session.post('https://api.x.com/1.1/account/logout.json', headers=logout_headers, data={
+            'redirectAfterLogout': 'https://x.com/account/switch',
         })
         if logout_api_response.status_code != 200:
             raise self._get_tweepy_exception(logout_api_response)
 
         # 基本固定値のようなので不要だが、念のためステータスチェック
         try:
             status = logout_api_response.json()['status']
@@ -341,15 +346,15 @@
         Args:
             response (requests.Response): レスポンス
         """
 
         csrf_token = response.cookies.get('ct0')
         if csrf_token:
             if self._session.cookies.get('ct0') != csrf_token:
-                self._session.cookies.set('ct0', csrf_token, domain='.twitter.com')
+                self._session.cookies.set('ct0', csrf_token, domain='.x.com')
             self._auth_flow_api_headers['x-csrf-token'] = csrf_token
             self._graphql_api_headers['x-csrf-token'] = csrf_token
             self._session.headers['x-csrf-token'] = csrf_token
 
 
     def _get_tweepy_exception(self, response: requests.Response) -> tweepy.TweepyException:
         """
@@ -404,28 +409,28 @@
         # HTTP ヘッダーは基本的に認証用セッションのものを使う
         headers = self._auth_flow_api_headers.copy()
         headers.pop('x-csrf-token')
         headers.pop('x-guest-token')
 
         # API からゲストトークンを取得する
         # ref: https://github.com/fa0311/TwitterFrontendFlow/blob/master/TwitterFrontendFlow/TwitterFrontendFlow.py#L26-L36
-        guest_token_response = self._session.post('https://api.twitter.com/1.1/guest/activate.json', headers=headers)
+        guest_token_response = self._session.post('https://api.x.com/1.1/guest/activate.json', headers=headers)
         if guest_token_response.status_code != 200:
             raise self._get_tweepy_exception(guest_token_response)
         try:
             guest_token = guest_token_response.json()['guest_token']
         except:
             raise tweepy.TweepyException('Failed to get guest token')
 
         return guest_token
 
 
     def _get_ui_metrics(self, js_inst: str) -> Dict[str, Any]:
         """
-        https://twitter.com/i/js_inst?c_name=ui_metrics から出力される難読化された JavaScript から ui_metrics を取得する
+        https://x.com/i/js_inst?c_name=ui_metrics から出力される難読化された JavaScript から ui_metrics を取得する
         ref: https://github.com/hfthair/TweetScraper/blob/master/TweetScraper/spiders/following.py#L50-L94
 
         Args:
             js_inst (str): 難読化された JavaScript
 
         Returns:
             dict[str, Any]: 取得された ui_metrics
@@ -520,45 +525,45 @@
                 if response.status_code < 400:
                     return data['flow_token']
             raise self._get_tweepy_exception(response)
 
         # Cookie をクリア
         self._session.cookies.clear()
 
-        # 一度 https://twitter.com/ にアクセスして Cookie をセットさせる
+        # 一度 https://x.com/ にアクセスして Cookie をセットさせる
         ## 取得した HTML はゲストトークンを取得するために使う
-        html_response = self._session.get('https://twitter.com/i/flow/login', headers=self._html_headers)
+        html_response = self._session.get('https://x.com/i/flow/login', headers=self._html_headers)
         if html_response.status_code != 200:
             raise self._get_tweepy_exception(html_response)
 
         # CSRF トークンを生成し、"ct0" としてセッションの Cookie に保存
         ## 同時に認証フロー API 用の HTTP リクエストヘッダーにもセット ("ct0" と "x-csrf-token" は同じ値になる)
         csrf_token = self._generate_csrf_token()
-        self._session.cookies.set('ct0', csrf_token, domain='.twitter.com')
+        self._session.cookies.set('ct0', csrf_token, domain='.x.com')
         self._auth_flow_api_headers['x-csrf-token'] = csrf_token
 
         # まだ取得できていない場合のみ、ゲストトークンを取得し、"gt" としてセッションの Cookie に保存
         if self._session.cookies.get('gt', default=None) is None:
             guest_token = self._get_guest_token()
-            self._session.cookies.set('gt', guest_token, domain='.twitter.com')
+            self._session.cookies.set('gt', guest_token, domain='.x.com')
 
         ## ゲストトークンを認証フロー API 用の HTTP リクエストヘッダーにもセット ("gt" と "x-guest-token" は同じ値になる)
         self._auth_flow_api_headers['x-guest-token'] = self._session.cookies.get('gt')
 
         # これ以降は基本認証フロー API へのアクセスしか行わないので、セッションのヘッダーを認証フロー API 用のものに差し替える
         self._session.headers.clear()
         self._session.headers.update(self._auth_flow_api_headers)
 
         # 極力公式の Twitter Web App に偽装するためのダミーリクエスト
-        self._session.get('https://api.twitter.com/1.1/hashflags.json')
+        self._session.get('https://api.x.com/1.1/hashflags.json')
 
-        # https://api.twitter.com/1.1/onboarding/task.json?task=login に POST して認証フローを開始
+        # https://api.x.com/1.1/onboarding/task.json?task=login に POST して認証フローを開始
         ## 認証フローを開始するには、Cookie に "ct0" と "gt" がセットされている必要がある
-        ## 2024年4月時点の Twitter Web App が送信する JSON パラメータを模倣している
-        flow_01_response = self._session.post('https://api.twitter.com/1.1/onboarding/task.json?flow_name=login', json={
+        ## 2024年5月時点の Twitter Web App が送信する JSON パラメータを模倣している
+        flow_01_response = self._session.post('https://api.x.com/1.1/onboarding/task.json?flow_name=login', json={
             'input_flow_data': {
                 'flow_context': {
                     'debug_overrides': {},
                     'start_location': {
                         'location': 'manual_link',
                     }
                 }
@@ -607,23 +612,25 @@
                 'web_modal': 1,
             }
         })
         if flow_01_response.status_code != 200:
             raise self._get_tweepy_exception(flow_01_response)
 
         # js_inst (難読化された JavaScript で、これの実行結果を認証フローに送信する必要があるらしい) を取得
-        js_inst_response = self._session.get('https://twitter.com/i/js_inst?c_name=ui_metrics', headers=self._js_headers)
+        ## 2024/05/18 時点の Twitter Web App では js_inst のみ x.com ではなく twitter.com から取得されているが、
+        ## 将来的なことを考慮しあえて x.com から取得している
+        js_inst_response = self._session.get('https://x.com/i/js_inst?c_name=ui_metrics', headers=self._js_headers)
         if js_inst_response.status_code != 200:
             raise tweepy.TweepyException('Failed to get js_inst')
 
         # js_inst の JavaScript を実行し、ui_metrics オブジェクトを取得
         ui_metrics = self._get_ui_metrics(js_inst_response.text)
 
         # 取得した ui_metrics を認証フローに送信
-        flow_02_response = self._session.post('https://api.twitter.com/1.1/onboarding/task.json', json={
+        flow_02_response = self._session.post('https://api.x.com/1.1/onboarding/task.json', json={
             'flow_token': get_flow_token(flow_01_response),
             'subtask_inputs': [
                 {
                     'subtask_id': 'LoginJsInstrumentationSubtask',
                     'js_instrumentation': {
                         'response': json.dumps(ui_metrics),
                         'link': 'next_link',
@@ -631,21 +638,21 @@
                 },
             ]
         })
         if flow_02_response.status_code != 200:
             raise self._get_tweepy_exception(flow_02_response)
 
         # 極力公式の Twitter Web App に偽装するためのダミーリクエスト
-        self._session.post('https://api.twitter.com/1.1/onboarding/sso_init.json', json={'provider': 'apple'})
+        self._session.post('https://api.x.com/1.1/onboarding/sso_init.json', json={'provider': 'apple'})
 
         # 怪しまれないように、2秒～4秒の間にランダムな時間待機
         time.sleep(random.uniform(2.0, 4.0))
 
         # スクリーンネームを認証フローに送信
-        flow_03_response = self._session.post('https://api.twitter.com/1.1/onboarding/task.json', json={
+        flow_03_response = self._session.post('https://api.x.com/1.1/onboarding/task.json', json={
             'flow_token': get_flow_token(flow_02_response),
             'subtask_inputs': [
                 {
                     'subtask_id': 'LoginEnterUserIdentifierSSO',
                     'settings_list': {
                         'setting_responses': [
                             {
@@ -665,15 +672,15 @@
         if flow_03_response.status_code != 200:
             raise self._get_tweepy_exception(flow_03_response)
 
         # 怪しまれないように、2秒～4秒の間にランダムな時間待機
         time.sleep(random.uniform(2.0, 4.0))
 
         # パスワードを認証フローに送信
-        flow_04_response = self._session.post('https://api.twitter.com/1.1/onboarding/task.json', json={
+        flow_04_response = self._session.post('https://api.x.com/1.1/onboarding/task.json', json={
             'flow_token': get_flow_token(flow_03_response),
             'subtask_inputs': [
                 {
                     'subtask_id': 'LoginEnterPassword',
                     'enter_password': {
                         'password': self.password,
                         'link': 'next_link',
@@ -686,15 +693,15 @@
 
         # ログイン失敗
         if flow_04_response.json()['status'] != 'success':
             raise tweepy.TweepyException(f'Failed to login (status: {flow_04_response.json()["status"]})')
 
         # 最後におまじないを認証フローに送信 (アカウント重複チェック…？)
         ## このリクエストで、Cookie に auth_token がセットされる
-        flow_05_response = self._session.post('https://api.twitter.com/1.1/onboarding/task.json', json={
+        flow_05_response = self._session.post('https://api.x.com/1.1/onboarding/task.json', json={
             'flow_token': get_flow_token(flow_04_response),
             'subtask_inputs': [
                 {
                     'subtask_id': 'AccountDuplicationCheck',
                     'check_logged_in_account': {
                         'link': 'AccountDuplicationCheck_false',
                     }
@@ -703,15 +710,15 @@
         })
         if flow_05_response.status_code != 200:
             raise self._get_tweepy_exception(flow_05_response)
 
         # 最後の最後にファイナライズを行う
         ## たぶんなくても動くけど、念のため
         ## このタイミングで Cookie の "ct0" 値 (CSRF トークン) がクライアント側で生成したものから、サーバー側で生成したものに更新される
-        flow_06_response = self._session.post('https://api.twitter.com/1.1/onboarding/task.json', json={
+        flow_06_response = self._session.post('https://api.x.com/1.1/onboarding/task.json', json={
             'flow_token': get_flow_token(flow_05_response),
             'subtask_inputs': [],
         })
         if flow_06_response.status_code != 200:
             raise self._get_tweepy_exception(flow_06_response)
 
         # ここまで来たら、ログインに成功しているはず
```

### Comparing `tweepy_authlib-1.4.1/.gitignore` & `tweepy_authlib-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.4.1/Readme.md` & `tweepy_authlib-1.5.0/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,22 @@
 > 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、参考になれば幸いです。  
 > また現時点で廃止されていない API を利用したサンプルコードが [example_json.py](example_json.py) と [example_pickle.py](example_pickle.py) にありますので、そちらもご一読ください。
 
 > [!NOTE]  
 > **tweepy-authlib v1.4.1 以降では、より厳密に Twitter Web App からの HTTP リクエストに偽装したり、一部の Twitter API v1.1 に再びアクセスできるようになるなど、様々な改善が行われています！**  
 > 凍結やアカウントロックのリスクを下げるためにも、最新版の tweepy-authlib の利用をおすすめします。
 
+> [!IMPORTANT]
+> **tweepy-authlib v1.5.0 にて、twitter.com の x.com への移行に対応しました。**  
+> 2024/05/18 時点では api.twitter.com でも引き続きアクセスできますが、不審がられるリスクが上がるうえ、いつまでアクセスできるかも不透明なためです。
+> これにより、`CookieSessionUserHandler.get_graphql_api_headers()` で返される Origin / Referer ヘッダーの値が `twitter.com` から `x.com` に変更されています。  
+> GraphQL API クライアントを自作されている場合は、更新と同時に GraphQL API クライアントのアクセス先 URL を `twitter.com/i/api/graphql` から `x.com/i/api/graphql` に変更することを推奨します。
+
 > [!IMPORTANT]  
-> 2024/04/30 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
+> 2024/05/18 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
 > [js2py](https://github.com/PiotrDabkowski/Js2Py) の Python 3.12 対応が完了するまで、Python 3.11 以下での利用をおすすめします。
 
 -----
 
 **Table of Contents**
 
 - [tweepy-authlib](#tweepy-authlib)
```

### Comparing `tweepy_authlib-1.4.1/pyproject.toml` & `tweepy_authlib-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tweepy_authlib-1.4.1/PKG-INFO` & `tweepy_authlib-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tweepy-authlib
-Version: 1.4.1
+Version: 1.5.0
 Summary: Twitter Web App (Web 版公式クライアント) の内部 API を使い、Tweepy でスクリーンネームとパスワードで認証するためのライブラリ
 Project-URL: Documentation, https://github.com/tsukumijima/tweepy-authlib
 Project-URL: Issues, https://github.com/tsukumijima/tweepy-authlib/issues
 Project-URL: Source, https://github.com/tsukumijima/tweepy-authlib
 Author: tsukumi
 License-Expression: MIT
 Keywords: Library,Tweepy,Twitter
@@ -49,16 +49,22 @@
 > 私が [KonomiTV](https://github.com/tsukumijima/KonomiTV) 向けに開発した GraphQL API クライアントの実装が [こちら](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/utils/TwitterGraphQLAPI.py) ([使用例](https://github.com/tsukumijima/KonomiTV/blob/master/server/app/routers/TwitterRouter.py)) にありますので、参考になれば幸いです。  
 > また現時点で廃止されていない API を利用したサンプルコードが [example_json.py](example_json.py) と [example_pickle.py](example_pickle.py) にありますので、そちらもご一読ください。
 
 > [!NOTE]  
 > **tweepy-authlib v1.4.1 以降では、より厳密に Twitter Web App からの HTTP リクエストに偽装したり、一部の Twitter API v1.1 に再びアクセスできるようになるなど、様々な改善が行われています！**  
 > 凍結やアカウントロックのリスクを下げるためにも、最新版の tweepy-authlib の利用をおすすめします。
 
+> [!IMPORTANT]
+> **tweepy-authlib v1.5.0 にて、twitter.com の x.com への移行に対応しました。**  
+> 2024/05/18 時点では api.twitter.com でも引き続きアクセスできますが、不審がられるリスクが上がるうえ、いつまでアクセスできるかも不透明なためです。
+> これにより、`CookieSessionUserHandler.get_graphql_api_headers()` で返される Origin / Referer ヘッダーの値が `twitter.com` から `x.com` に変更されています。  
+> GraphQL API クライアントを自作されている場合は、更新と同時に GraphQL API クライアントのアクセス先 URL を `twitter.com/i/api/graphql` から `x.com/i/api/graphql` に変更することを推奨します。
+
 > [!IMPORTANT]  
-> 2024/04/30 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
+> 2024/05/18 時点では [tweepy-authlib が依存する js2py が Python 3.12 に対応していない](https://github.com/tsukumijima/tweepy-authlib/issues/5) ため、tweepy-authlib は Python 3.12 以降では動作しません。  
 > [js2py](https://github.com/PiotrDabkowski/Js2Py) の Python 3.12 対応が完了するまで、Python 3.11 以下での利用をおすすめします。
 
 -----
 
 **Table of Contents**
 
 - [tweepy-authlib](#tweepy-authlib)
```

