# Comparing `tmp/django_allauth_ui-0.2.2.tar.gz` & `tmp/django_allauth_ui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_allauth_ui-0.2.2.tar", max compression
+gzip compressed data, was "django_allauth_ui-0.3.0.tar", max compression
```

## Comparing `django_allauth_ui-0.2.2.tar` & `django_allauth_ui-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/LICENSE
--rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/__init__.py
--rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/apps.py
--rw-r--r--   0        0        0     4261 2023-12-20 16:13:58.510749 django_allauth_ui-0.2.2/allauth_ui/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.2.2/allauth_ui/static/allauth_ui/input.css
--rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.2.2/allauth_ui/static/allauth_ui/output.css
--rw-r--r--   0        0        0     1383 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/_button.html
--rw-r--r--   0        0        0      254 2023-10-23 20:51:46.098003 django_allauth_ui-0.2.2/allauth_ui/templates/account/_links.html
--rw-r--r--   0        0        0      224 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/_non_field_errors.html
--rw-r--r--   0        0        0      840 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/_render_form.html
--rw-r--r--   0        0        0      984 2023-01-29 13:57:46.486760 django_allauth_ui-0.2.2/allauth_ui/templates/account/base.html
--rw-r--r--   0        0        0     1001 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/email_confirm.html
--rw-r--r--   0        0        0     2090 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/login.html
--rw-r--r--   0        0        0      305 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/logout.html
--rw-r--r--   0        0        0      567 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/password_reset.html
--rw-r--r--   0        0        0     1163 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     1081 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      508 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      514 2023-12-20 16:13:56.382744 django_allauth_ui-0.2.2/allauth_ui/templates/account/signup.html
--rw-r--r--   0        0        0      605 2024-01-31 08:24:49.504001 django_allauth_ui-0.2.2/allauth_ui/templates/account/signup_closed.html
--rw-r--r--   0        0        0      765 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/account/verification_sent.html
--rw-r--r--   0        0        0      677 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0       33 2024-01-29 10:34:33.647135 django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/base.html
--rw-r--r--   0        0        0     1649 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1128 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/login.html
--rw-r--r--   0        0        0      686 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/signup.html
--rw-r--r--   0        0        0      774 2022-12-20 01:48:32.803185 django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      624 2022-11-06 12:22:33.884002 django_allauth_ui-0.2.2/allauth_ui/templatetags/allauth_ui.py
--rw-r--r--   0        0        0      916 2024-01-31 08:25:28.444001 django_allauth_ui-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 django_allauth_ui-0.2.2/setup.py
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 django_allauth_ui-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/LICENSE
+-rw-r--r--   0        0        0       22 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/__init__.py
+-rw-r--r--   0        0        0       94 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/apps.py
+-rw-r--r--   0        0        0     8374 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8352 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2022-12-20 01:16:52.519135 django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/input.css
+-rw-r--r--   0        0        0    35561 2022-12-20 01:53:25.418792 django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/output.css
+-rw-r--r--   0        0        0     1383 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/_button.html
+-rw-r--r--   0        0        0      254 2023-10-23 20:51:46.098003 django_allauth_ui-0.3.0/allauth_ui/templates/account/_links.html
+-rw-r--r--   0        0        0      224 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/_non_field_errors.html
+-rw-r--r--   0        0        0      840 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/_render_form.html
+-rw-r--r--   0        0        0      984 2023-01-29 13:57:46.486760 django_allauth_ui-0.3.0/allauth_ui/templates/account/base.html
+-rw-r--r--   0        0        0     1001 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     2226 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/login.html
+-rw-r--r--   0        0        0      392 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/logout.html
+-rw-r--r--   0        0        0      664 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset.html
+-rw-r--r--   0        0        0     1221 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     1150 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      508 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      595 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/account/signup.html
+-rw-r--r--   0        0        0      605 2024-01-31 08:24:49.504001 django_allauth_ui-0.3.0/allauth_ui/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      765 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      677 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0       33 2024-01-29 10:34:33.647135 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/base.html
+-rw-r--r--   0        0        0     1649 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1213 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      731 2024-05-18 21:09:02.615040 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0      774 2022-12-20 01:48:32.803185 django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      624 2022-11-06 12:22:33.884002 django_allauth_ui-0.3.0/allauth_ui/templatetags/allauth_ui.py
+-rw-r--r--   0        0        0      943 2024-05-18 21:09:30.733159 django_allauth_ui-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.0/setup.py
+-rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 django_allauth_ui-0.3.0/PKG-INFO
```

### Comparing `django_allauth_ui-0.2.2/LICENSE` & `django_allauth_ui-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/static/allauth_ui/input.css` & `django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/input.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/static/allauth_ui/output.css` & `django_allauth_ui-0.3.0/allauth_ui/static/allauth_ui/output.css`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/_button.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/_button.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/_render_form.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/_render_form.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/base.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/base.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/email_confirm.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/login.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/login.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "account/base.html" %}
-
+{% load i18n %}
 {% load widget_tweaks %}
 {% load account socialaccount %}
 
 {% block head_title %}
-Sign in
+  {% translate "Sign in" %}
 {% endblock %}
 
 {% block whitebox %}
 <h1 class="mb-5 text-3xl text-center">Sign in</h1>
 <form method="POST" action="{% url 'account_login' %}" class="flex flex-col items-center grow-0">
   {% csrf_token %}
 
@@ -28,35 +28,36 @@
       {{ error }}
     </span>
     {% endfor %}
     </div>
     {% endif %}
   {% endfor %}
 
-
-  {% include "account/_button.html" with text="Login" %}
+  {% translate "Login" as login_text %}
+  {% include "account/_button.html" with text=login_text %}
 
   <div class="flex justify-center mt-6 text-xs">
-    <a class="text-blue-400 hover:text-blue-500" href="{% url 'account_reset_password' %}">Forgot Password</a>
+    <a class="text-blue-400 hover:text-blue-500" href="{% url 'account_reset_password' %}">{% translate "Forgot Password" %}
+    </a>
     <span class="mx-2 text-gray-300">/</span>
-    <a class="text-blue-400 hover:text-blue-500" href="{% url 'account_signup' %}">Sign Up</a>
+    <a class="text-blue-400 hover:text-blue-500" href="{% url 'account_signup' %}">{% translate "Sign Up" %}</a>
   </div>
 
   {% if redirect_field_value %}
   <input type="hidden" name="{{ redirect_field_name }}" value="{{ redirect_field_value }}" />
   {% endif %}
 </form>
 {% get_providers as socialaccount_providers %}
 {% if socialaccount_providers %}
 <div class="flex items-center self-stretch justify-between pt-3 mt-3">
   <hr class="w-full">
   <span class="p-2 mb-1 text-gray-400">OR</span>
   <hr class="w-full">
 </div>
 
-<p class="text-xs text-center text-gray-500">Sign in with a third party</p>
+<p class="text-xs text-center text-gray-500">{% translate "Sign in with a third party" %}</p>
 
 {% include "socialaccount/snippets/provider_list.html" with process="login" %}
 {% endif %}
 
 {% include "socialaccount/snippets/login_extra.html" %}
 {% endblock %}
```

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/password_reset_done.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/login.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-{% extends "account/base.html" %}
+{% extends "socialaccount/base.html" %}
 
-{% block head_title %}Password Reset{% endblock %}
-
-{% block content %}
-<div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
-  <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg">
-  <h1 class="mb-8 text-3xl text-center">Reset email sent</h1>
-  <p class="flex items-center px-4 py-3 text-sm font-bold text-white bg-blue-500 rounded" role="alert">
-    <svg class="w-4 h-4 mr-2 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z"/></svg>
-    We have sent you an e-mail. Please contact us if you do not receive it within a few minutes.
+{% block whitebox %}
+<div class="flex items-center px-4 py-3 text-sm text-white bg-blue-500 rounded" role="alert">
+  <svg class="w-4 h-4 mr-2 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z"/></svg>
+  <p>
+    {% if process == "connect" %}
+    {% translate "You are about to connect a new third party account from" %} {{ provider.name }}.
+    {% else %}
+    {% translate "You are about to sign in using a third party account from" %} {{ provider.name }}.
+    {% endif %}
   </p>
-
-  {% include "account/_links.html" %}
-  </div>
 </div>
+<form method="POST" class="flex flex-col items-center justify-center pt-5 py-10">
+  {% csrf_token %}
+  {% translate "Continue" as continue_text %}
+  {% include "account/_button.html" with text=continue_text %}
+</form>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/password_reset_from_key.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_from_key.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends "account/base.html" %}
 
 {% load i18n %}
 
-{% block head_title %}Change Password{% endblock %}
+{% block head_title %}{% translate "Change Password" %}{% endblock %}
 
 {% block whitebox %}
 <h1 class="mb-5 text-3xl">{% if token_fail %}{% trans "Bad Token" %}{% else %}{% trans "Change Password" %}{% endif %}</h1>
 {% if token_fail %}
     <div class="px-4 py-3" role="alert">
       <strong class="font-bold">Invalid token!</strong>
       <span class="block text-black">
@@ -16,14 +16,15 @@
         <a class="text-blue-400 hover:text-blue-500" href="{{ passwd_reset_url }}">new password reset</a>.{% endblocktrans %}
       </span>
     </div>
 {% else %}
   {% if form %}
       <form method="POST" action="{{ action_url }}">
         {% include "account/_render_form.html" %}
-        {% include "account/_button.html" with text="Change password" %}
+        {% translate "Change password" as change_text %}
+        {% include "account/_button.html" with text=change_text %}
       </form>
   {% else %}
       <p>{% trans 'Your password is now changed.' %}</p>
   {% endif %}
 {% endif %}
 {% endblock %}
```

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/signup.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/signup.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,22 @@
-{% extends "account/base.html" %}
+{% extends "socialaccount/base.html" %}
 
-{% block head_title %}Sign up{% endblock %}
+{% load i18n %}
+
+{% block head_title %}{% trans "Sign Up" %}{% endblock %}
 
 {% block whitebox %}
-<h1 class="mb-5 text-3xl text-center">Sign up</h1>
-<form id="signup_form" method="post" action="{% url 'account_signup' %}" novalidate>
+<h1 class="mb-5 text-3xl text-center">{% trans "Sign Up" %}</h1>
+
+<p class="my-5">
+{% blocktrans with provider_name=account.get_provider.name site_name=site.name %}
+  You are about to use your {{provider_name}} account to login to
+  {{site_name}}. As a final step, please complete the following form:
+{% endblocktrans %}
+</p>
+
+<form class="signup" id="signup_form" method="post" action="{% url 'socialaccount_signup' %}">
   {% include "account/_render_form.html" %}
-  {% include "account/_button.html" with text="Sign up" %}
+  {% translate "Sign up" as signup_text %}
+  {% include "account/_button.html" with text=signup_text %}
 </form>
-<a class="self-center pt-8 text-xs text-blue-400 justify-self-center hover:text-blue-500" href="{{ login_url }}">Already have an account? Sign in.</a>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/signup_closed.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/account/verification_sent.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/authentication_error.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/connections.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/login.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/account/password_reset_done.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-{% extends "socialaccount/base.html" %}
+{% extends "account/base.html" %}
 
-{% block whitebox %}
-<div class="flex items-center px-4 py-3 text-sm text-white bg-blue-500 rounded" role="alert">
-  <svg class="w-4 h-4 mr-2 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z"/></svg>
-  <p>
-    {% if process == "connect" %}
-    You are about to connect a new third party account from {{ provider.name }}.
-    {% else %}
-    You are about to sign in using a third party account from {{ provider.name }}.
-    {% endif %}
+{% block head_title %}{% translate "Password Reset" %}{% endblock %}
+
+{% block content %}
+<div class="flex flex-col items-center justify-center w-screen h-screen text-gray-700 bg-gray-200">
+  <div class="flex flex-col items-center p-12 bg-white rounded shadow-lg">
+    <h1 class="mb-8 text-3xl text-center">{% translate "Reset email sent" %}</h1>
+  <p class="flex items-center px-4 py-3 text-sm font-bold text-white bg-blue-500 rounded" role="alert">
+    <svg class="w-4 h-4 mr-2 fill-current" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M12.432 0c1.34 0 2.01.912 2.01 1.957 0 1.305-1.164 2.512-2.679 2.512-1.269 0-2.009-.75-1.974-1.99C9.789 1.436 10.67 0 12.432 0zM8.309 20c-1.058 0-1.833-.652-1.093-3.524l1.214-5.092c.211-.814.246-1.141 0-1.141-.317 0-1.689.562-2.502 1.117l-.528-.88c2.572-2.186 5.531-3.467 6.801-3.467 1.057 0 1.233 1.273.705 3.23l-1.391 5.352c-.246.945-.141 1.271.106 1.271.317 0 1.357-.392 2.379-1.207l.6.814C12.098 19.02 9.365 20 8.309 20z"/></svg>
+      {% translate "We have sent you an e-mail. Please contact us if you do not receive it within a few minutes." %}
   </p>
+
+  {% include "account/_links.html" %}
+  </div>
 </div>
-<form method="POST" class="flex flex-col items-center justify-center pt-5 py-10">
-  {% csrf_token %}
-  {% include "account/_button.html" with text="Continue" %}
-</form>
 {% endblock %}
```

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templates/socialaccount/snippets/provider_list.html` & `django_allauth_ui-0.3.0/allauth_ui/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/allauth_ui/templatetags/allauth_ui.py` & `django_allauth_ui-0.3.0/allauth_ui/templatetags/allauth_ui.py`

 * *Files identical despite different names*

### Comparing `django_allauth_ui-0.2.2/pyproject.toml` & `django_allauth_ui-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django-allauth-ui"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 authors = ["Dani Hodovic <you@example.com>"]
 license = "MIT"
 packages = [
     { include = "allauth_ui" },
 ]
 include = ["allauth_ui/static/allauth_ui/output.css"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.2"
 django-widget-tweaks = "^1.4.12"
+django-rosetta = "^0.10.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "2.10.0"
 pytest-django = "4.1.0"
 black = "^23.3.0"
 mypy = "^1.3.0"
```

### Comparing `django_allauth_ui-0.2.2/setup.py` & `django_allauth_ui-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 
 packages = \
 ['allauth_ui', 'allauth_ui.templatetags']
 
 package_data = \
 {'': ['*'],
  'allauth_ui': ['locale/es/LC_MESSAGES/*',
+                'locale/fr/LC_MESSAGES/*',
                 'static/allauth_ui/*',
                 'templates/account/*',
                 'templates/socialaccount/*',
                 'templates/socialaccount/snippets/*']}
 
 install_requires = \
-['django-widget-tweaks>=1.4.12,<2.0.0']
+['django-rosetta>=0.10.0,<0.11.0', 'django-widget-tweaks>=1.4.12,<2.0.0']
 
 setup_kwargs = {
     'name': 'django-allauth-ui',
-    'version': '0.2.2',
+    'version': '0.3.0',
     'description': '',
     'long_description': 'None',
     'author': 'Dani Hodovic',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `django_allauth_ui-0.2.2/PKG-INFO` & `django_allauth_ui-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: django-allauth-ui
-Version: 0.2.2
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Dani Hodovic
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: django-rosetta (>=0.10.0,<0.11.0)
 Requires-Dist: django-widget-tweaks (>=1.4.12,<2.0.0)
```

