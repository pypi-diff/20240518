# Comparing `tmp/unconscious-0.0.5.tar.gz` & `tmp/unconscious-0.0.6.tar.gz`

## Comparing `unconscious-0.0.5.tar` & `unconscious-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0      501       20      548 2024-05-17 03:03:43.000000 unconscious-0.0.5/unconscious-core/Cargo.toml
--rw-r--r--   0      501       20    11564 2024-05-18 18:23:21.000000 unconscious-0.0.5/unconscious-core/src/lib.rs
--rw-r--r--   0      501       20       94 2024-05-17 01:58:19.000000 unconscious-0.0.5/unconscious-core/src/main.rs
--rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 unconscious-0.0.5/unconscious/Cargo.toml
--rw-r--r--   0      501       20      807 2024-05-17 01:47:05.000000 unconscious-0.0.5/unconscious/.cargo/config.toml
--rw-r--r--   0      501       20      280 2024-05-15 04:49:11.000000 unconscious-0.0.5/unconscious/.env/pyvenv.cfg
--rw-r--r--   0      501       20     3526 2024-05-15 04:49:28.000000 unconscious-0.0.5/unconscious/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-05-15 04:49:28.000000 unconscious-0.0.5/unconscious/.gitignore
--rw-r--r--   0      501       20      151 2024-05-18 19:29:30.000000 unconscious-0.0.5/unconscious/Makefile
--rwxr-xr-x   0      501       20      114 2024-05-17 01:32:29.000000 unconscious-0.0.5/unconscious/custom-cargo-wrapper
--rw-r--r--   0      501       20      699 2024-05-16 23:54:53.000000 unconscious-0.0.5/unconscious/demo.py
--rw-r--r--   0      501       20      427 2024-05-18 18:51:37.000000 unconscious-0.0.5/unconscious/src/lib.rs
--rw-r--r--   0      501       20      737 2024-05-18 19:28:18.000000 unconscious-0.0.5/unconscious/unconscious/__init__.py
--rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.5/unconscious/unconscious/agent.py
--rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.5/unconscious/unconscious/client.py
--rw-r--r--   0      501       20    37586 2024-05-16 13:57:44.000000 unconscious-0.0.5/unconscious/Cargo.lock
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 unconscious-0.0.5/pyproject.toml
--rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.5/unconscious/client.py
--rw-r--r--   0      501       20      737 2024-05-18 19:28:18.000000 unconscious-0.0.5/unconscious/__init__.py
--rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.5/unconscious/agent.py
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 unconscious-0.0.5/PKG-INFO
+-rw-r--r--   0      501       20      548 2024-05-17 03:03:43.000000 unconscious-0.0.6/unconscious-core/Cargo.toml
+-rw-r--r--   0      501       20    11825 2024-05-18 19:59:45.000000 unconscious-0.0.6/unconscious-core/src/lib.rs
+-rw-r--r--   0      501       20       94 2024-05-17 01:58:19.000000 unconscious-0.0.6/unconscious-core/src/main.rs
+-rw-r--r--   0        0        0      429 1970-01-01 00:00:00.000000 unconscious-0.0.6/unconscious/Cargo.toml
+-rw-r--r--   0      501       20      807 2024-05-17 01:47:05.000000 unconscious-0.0.6/unconscious/.cargo/config.toml
+-rw-r--r--   0      501       20      280 2024-05-15 04:49:11.000000 unconscious-0.0.6/unconscious/.env/pyvenv.cfg
+-rw-r--r--   0      501       20     3526 2024-05-15 04:49:28.000000 unconscious-0.0.6/unconscious/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-05-15 04:49:28.000000 unconscious-0.0.6/unconscious/.gitignore
+-rw-r--r--   0      501       20      180 2024-05-18 20:00:18.000000 unconscious-0.0.6/unconscious/Makefile
+-rw-r--r--   0      501       20      699 2024-05-16 23:54:53.000000 unconscious-0.0.6/unconscious/demo.py
+-rw-r--r--   0      501       20      427 2024-05-18 18:51:37.000000 unconscious-0.0.6/unconscious/src/lib.rs
+-rw-r--r--   0      501       20      737 2024-05-18 19:28:18.000000 unconscious-0.0.6/unconscious/unconscious/__init__.py
+-rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.6/unconscious/unconscious/agent.py
+-rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.6/unconscious/unconscious/client.py
+-rw-r--r--   0      501       20    37586 2024-05-16 13:57:44.000000 unconscious-0.0.6/unconscious/Cargo.lock
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 unconscious-0.0.6/pyproject.toml
+-rw-r--r--   0      501       20     3863 2024-05-17 00:02:21.000000 unconscious-0.0.6/unconscious/client.py
+-rw-r--r--   0      501       20      737 2024-05-18 19:28:18.000000 unconscious-0.0.6/unconscious/__init__.py
+-rw-r--r--   0      501       20     2639 2024-05-17 00:02:16.000000 unconscious-0.0.6/unconscious/agent.py
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 unconscious-0.0.6/PKG-INFO
```

### Comparing `unconscious-0.0.5/unconscious-core/Cargo.toml` & `unconscious-0.0.6/unconscious-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious-core/src/lib.rs` & `unconscious-0.0.6/unconscious-core/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 use serde_derive::{Deserialize, Serialize};
 use serde_json::Value;
 use std::{convert::Infallible, net::SocketAddr, time::Duration};
 use tokio_stream::StreamExt as _;
 use tracing_subscriber::{layer::SubscriberExt, util::SubscriberInitExt};
 
 pub const DEFAULT_THREAD: &str = "k1";
+// static import of the html file
+pub static INDEX_HTML: &str = include_str!("../../static/index.html");
 
 pub async fn inner_main() {
     tracing_subscriber::registry()
         .with(
             tracing_subscriber::EnvFilter::try_from_default_env()
                 .unwrap_or_else(|_| "unconscious_core=debug".into()),
         )
@@ -68,28 +70,32 @@
         .await
         .unwrap();
     tracing::debug!("listening on {}", listener.local_addr().unwrap());
     axum::serve(listener, app).await.unwrap();
 }
 
 pub async fn index_page() -> Html<String> {
-    // get the path to the static file at runtime based on where the binary is
-    // rather than where its run from
-    let mut path = std::env::current_exe().unwrap();
-    path.pop();
-    path.pop();
-    path.pop();
-    path.push("static");
-    path.push("index.html");
+    let dev = std::env::var("DEV").is_ok();
+    if dev {
+        // get the path to the static file at runtime based on where the binary is
+        // rather than where its run from
+        let mut path = std::env::current_exe().unwrap();
+        path.pop();
+        path.pop();
+        path.pop();
+        path.push("static");
+        path.push("index.html");
 
-    // read the contents of the file at runtime
-    let file_contents = tokio::fs::read_to_string(path)
-        .await
-        .unwrap_or_else(|_| "<h1>Unconscious</h1>".to_string());
-    Html(file_contents)
+        // read the contents of the file at runtime
+        let file_contents = tokio::fs::read_to_string(path)
+            .await
+            .unwrap_or_else(|_| "<h1>Unconscious</h1>".to_string());
+        return Html(file_contents);
+    }
+    Html(INDEX_HTML.to_string())
 }
 
 type ConnectionPool = Pool<RedisConnectionManager>;
 
 #[derive(Deserialize, Debug)]
 struct Params {
     #[serde(default)]
```

### Comparing `unconscious-0.0.5/unconscious/.cargo/config.toml` & `unconscious-0.0.6/unconscious/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/.github/workflows/CI.yml` & `unconscious-0.0.6/unconscious/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/.gitignore` & `unconscious-0.0.6/unconscious/.gitignore`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/demo.py` & `unconscious-0.0.6/unconscious/demo.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/unconscious/__init__.py` & `unconscious-0.0.6/unconscious/unconscious/__init__.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/unconscious/agent.py` & `unconscious-0.0.6/unconscious/unconscious/agent.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/unconscious/client.py` & `unconscious-0.0.6/unconscious/unconscious/client.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/Cargo.lock` & `unconscious-0.0.6/unconscious/Cargo.lock`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/client.py` & `unconscious-0.0.6/unconscious/client.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/__init__.py` & `unconscious-0.0.6/unconscious/__init__.py`

 * *Files identical despite different names*

### Comparing `unconscious-0.0.5/unconscious/agent.py` & `unconscious-0.0.6/unconscious/agent.py`

 * *Files identical despite different names*

