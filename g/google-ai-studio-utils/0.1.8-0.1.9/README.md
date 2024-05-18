# Comparing `tmp/google_ai_studio_utils-0.1.8.tar.gz` & `tmp/google_ai_studio_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_ai_studio_utils-0.1.8.tar", max compression
+gzip compressed data, was "google_ai_studio_utils-0.1.9.tar", max compression
```

## Comparing `google_ai_studio_utils-0.1.8.tar` & `google_ai_studio_utils-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.8/README.md
--rw-r--r--   0        0        0      188 2024-04-17 01:59:04.520871 google_ai_studio_utils-0.1.8/google_ai_studio_utils/config.py
--rwxr-xr-x   0        0        0     2916 2024-04-15 17:01:31.595230 google_ai_studio_utils-0.1.8/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
--rwxr-xr-x   0        0        0     3145 2024-04-30 15:01:04.901844 google_ai_studio_utils-0.1.8/google_ai_studio_utils/google_ai_studio_conversation_python_to_html.py
--rw-r--r--   0        0        0     5305 2024-04-15 17:02:05.628767 google_ai_studio_utils-0.1.8/google_ai_studio_utils/templates/google-ai-studio-conversation.html
--rw-r--r--   0        0        0     5230 2024-04-30 15:18:47.363938 google_ai_studio_utils-0.1.8/google_ai_studio_utils/utils.py
--rw-r--r--   0        0        0      915 2024-04-30 15:19:20.828045 google_ai_studio_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-15 15:56:31.370705 google_ai_studio_utils-0.1.9/README.md
+-rw-r--r--   0        0        0      188 2024-04-17 01:59:04.520871 google_ai_studio_utils-0.1.9/google_ai_studio_utils/config.py
+-rwxr-xr-x   0        0        0     2916 2024-04-15 17:01:31.595230 google_ai_studio_utils-0.1.9/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py
+-rwxr-xr-x   0        0        0     3145 2024-04-30 15:01:04.901844 google_ai_studio_utils-0.1.9/google_ai_studio_utils/google_ai_studio_conversation_python_to_html.py
+-rw-r--r--   0        0        0     6041 2024-04-30 15:55:22.933256 google_ai_studio_utils-0.1.9/google_ai_studio_utils/templates/google-ai-studio-conversation.html
+-rw-r--r--   0        0        0     5452 2024-04-30 15:51:58.773779 google_ai_studio_utils-0.1.9/google_ai_studio_utils/utils.py
+-rw-r--r--   0        0        0      915 2024-04-30 15:55:51.545981 google_ai_studio_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 google_ai_studio_utils-0.1.9/PKG-INFO
```

### Comparing `google_ai_studio_utils-0.1.8/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py` & `google_ai_studio_utils-0.1.9/google_ai_studio_utils/google_ai_studio_conversation_csv_to_html.py`

 * *Files identical despite different names*

### Comparing `google_ai_studio_utils-0.1.8/google_ai_studio_utils/google_ai_studio_conversation_python_to_html.py` & `google_ai_studio_utils-0.1.9/google_ai_studio_utils/google_ai_studio_conversation_python_to_html.py`

 * *Files identical despite different names*

### Comparing `google_ai_studio_utils-0.1.8/google_ai_studio_utils/templates/google-ai-studio-conversation.html` & `google_ai_studio_utils-0.1.9/google_ai_studio_utils/templates/google-ai-studio-conversation.html`

 * *Files 7% similar despite different names*

```diff
@@ -130,32 +130,47 @@
         /* Adjust based on your line height */
     }
 </style>
 <script>document.addEventListener("DOMContentLoaded", function () {
         const contentDivs = document.querySelectorAll('.user-content, .model-content');
 
         contentDivs.forEach(div => {
+            let copyBtn = document.createElement('button');
+            copyBtn.innerHTML = '<i class="fa fa-copy"></i>'; // Use a copy icon from Font Awesome
+            copyBtn.onclick = function () {
+                let message = div.getAttribute('data-message');
+                navigator.clipboard.writeText(message).then(function () {
+                    console.log('Copying to clipboard was successful!');
+                }, function (err) {
+                    console.error('Could not copy text: ', err);
+                });
+            };
             // Create fold button
             let foldBtn = document.createElement('button');
             foldBtn.innerHTML = '<i class="fas fa-chevron-down"></i>'; // Default to 'unfold' icon
             foldBtn.onclick = function () {
                 toggleFold(div, foldBtn);
             };
 
             // Create wrap toggle button
 
             // Insert buttons before the div
             div.parentNode.insertBefore(foldBtn, div);
+            // insert a white space span
+            div.parentNode.insertBefore(document.createTextNode(' '), div);
+            div.parentNode.insertBefore(copyBtn, div);
 
             // Check if it's user-content and too long
             if (div.classList.contains('user-content') && isContentTooLong(div)) {
                 toggleFold(div, foldBtn);
             }
         });
     });
+        
+    
 
     function toggleFold(div, btn) {
         if (div.classList.contains('folded')) {
             div.classList.remove('folded');
             btn.innerHTML = '<i class="fas fa-chevron-down"></i>'; // Unfold icon
         } else {
             div.classList.add('folded');
```

### Comparing `google_ai_studio_utils-0.1.8/google_ai_studio_utils/utils.py` & `google_ai_studio_utils-0.1.9/google_ai_studio_utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,23 +94,27 @@
 
 def conversation_to_html(
     conversation: list[tuple[str, str]],
     font: str = "sans-serif",
     title: str = "Google AI Studio Exported Conversation",
 ) -> str:
     import markdown
+    import html
 
     html_template = google_ai_studio_html_template.read_text()
 
     content = ""
     for index, (role, message) in enumerate(conversation):
+        html_escaped_message = html.escape(message)
         if role.lower() == "Model".lower():
-            content += f'<a id="convo-item-{index}" class="anchor-button" href="#convo-item-{index}"># </a><div class="model-content">{markdown.markdown(message, extensions=['footnotes', 'meta', 'toc', 'admonition', 'fenced_code', 'tables'])}</div><hr>'
+            # model output (markdown)
+            content += f'<a id="convo-item-{index}"  class="anchor-button" href="#convo-item-{index}"># </a><div class="model-content" data-message="{html_escaped_message}">{markdown.markdown(message, extensions=['footnotes', 'meta', 'toc', 'admonition', 'fenced_code', 'tables'])}</div><hr>'
         else:
-            content += f'<a id="convo-item-{index}" class="anchor-button" href="#convo-item-{index}"># </a><div class="user-content"><pre>{message}</pre></div><hr>'
+            # user input (plain text)
+            content += f'<a id="convo-item-{index}"  class="anchor-button" href="#convo-item-{index}"># </a><div class="user-content" data-message="{html_escaped_message}"><pre>{message}</pre></div><hr>'
 
     return format_dunder_keys(html_template, content=content, font=font, title=title)
 
 
 def gist_create(p: PathLike) -> str:
     import subprocess
```

### Comparing `google_ai_studio_utils-0.1.8/pyproject.toml` & `google_ai_studio_utils-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "google-ai-studio-utils"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/google-ai-studio-utils"
 repository = "https://github.com/tddschn/google-ai-studio-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `google_ai_studio_utils-0.1.8/PKG-INFO` & `google_ai_studio_utils-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-studio-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/tddschn/google-ai-studio-utils
 License: MIT
 Keywords: chatgpt
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

