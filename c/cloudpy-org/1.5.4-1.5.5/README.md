# Comparing `tmp/cloudpy_org-1.5.4.tar.gz` & `tmp/cloudpy_org-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.5.4.tar", last modified: Thu May 16 20:45:49 2024, max compression
+gzip compressed data, was "dist\cloudpy_org-1.5.5.tar", last modified: Fri May 17 07:48:25 2024, max compression
```

## Comparing `cloudpy_org-1.5.4.tar` & `cloudpy_org-1.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 20:45:49.624537 cloudpy_org-1.5.4/
--rw-rw-rw-   0        0        0      935 2024-05-16 20:45:49.623994 cloudpy_org-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 20:45:49.439348 cloudpy_org-1.5.4/cloudpy_org/
--rw-rw-rw-   0        0        0     3240 2024-05-16 20:39:34.000000 cloudpy_org-1.5.4/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    32752 2024-05-16 20:39:43.000000 cloudpy_org-1.5.4/cloudpy_org/aws.py
--rw-rw-rw-   0        0        0    80029 2024-05-16 20:39:48.000000 cloudpy_org-1.5.4/cloudpy_org/client_usage.py
--rw-rw-rw-   0        0        0    13614 2024-05-16 20:39:53.000000 cloudpy_org-1.5.4/cloudpy_org/docs.py
--rw-rw-rw-   0        0        0     3924 2024-05-01 08:43:26.000000 cloudpy_org-1.5.4/cloudpy_org/imgedit.py
--rw-rw-rw-   0        0        0    51895 2024-05-16 20:40:00.000000 cloudpy_org-1.5.4/cloudpy_org/tools.py
--rw-rw-rw-   0        0        0     4998 2024-05-16 20:40:17.000000 cloudpy_org-1.5.4/cloudpy_org/web.py
--rw-rw-rw-   0        0        0    10189 2024-05-16 20:40:06.000000 cloudpy_org-1.5.4/cloudpy_org/web_client_usage.py
-drwxrwxrwx   0        0        0        0 2024-05-16 20:45:49.594975 cloudpy_org-1.5.4/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      935 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-05-16 20:45:48.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-16 20:45:47.000000 cloudpy_org-1.5.4/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 20:45:49.625038 cloudpy_org-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1352 2024-05-16 20:45:19.000000 cloudpy_org-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:48:25.486212 cloudpy_org-1.5.5/
+-rw-rw-rw-   0        0        0      935 2024-05-17 07:48:25.485643 cloudpy_org-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 07:48:25.299564 cloudpy_org-1.5.5/cloudpy_org/
+-rw-rw-rw-   0        0        0     3240 2024-05-17 07:44:06.000000 cloudpy_org-1.5.5/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    32752 2024-05-16 20:39:43.000000 cloudpy_org-1.5.5/cloudpy_org/aws.py
+-rw-rw-rw-   0        0        0    81879 2024-05-17 07:43:54.000000 cloudpy_org-1.5.5/cloudpy_org/client_usage.py
+-rw-rw-rw-   0        0        0    13614 2024-05-16 20:39:53.000000 cloudpy_org-1.5.5/cloudpy_org/docs.py
+-rw-rw-rw-   0        0        0     3924 2024-05-01 08:43:26.000000 cloudpy_org-1.5.5/cloudpy_org/imgedit.py
+-rw-rw-rw-   0        0        0    51895 2024-05-16 20:40:00.000000 cloudpy_org-1.5.5/cloudpy_org/tools.py
+-rw-rw-rw-   0        0        0     4998 2024-05-16 20:40:17.000000 cloudpy_org-1.5.5/cloudpy_org/web.py
+-rw-rw-rw-   0        0        0    10189 2024-05-16 20:40:06.000000 cloudpy_org-1.5.5/cloudpy_org/web_client_usage.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:48:25.462885 cloudpy_org-1.5.5/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      935 2024-05-17 07:48:24.000000 cloudpy_org-1.5.5/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-17 07:48:25.000000 cloudpy_org-1.5.5/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:48:24.000000 cloudpy_org-1.5.5/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-05-17 07:48:24.000000 cloudpy_org-1.5.5/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 07:48:24.000000 cloudpy_org-1.5.5/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 07:48:25.486714 cloudpy_org-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2024-05-17 07:48:05.000000 cloudpy_org-1.5.5/setup.py
```

### Comparing `cloudpy_org-1.5.4/PKG-INFO` & `cloudpy_org-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.5.4
+Version: 1.5.5
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.4/cloudpy_org/__init__.py` & `cloudpy_org-1.5.5/cloudpy_org/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'eu-west-1': {'long_name': 'Europe (Ireland)', 'code': 'euw1'},
  'eu-west-2': {'long_name': 'Europe (London)', 'code': 'euw2'},
  'eu-west-3': {'long_name': 'Europe (Paris)', 'code': 'euw3'},
  'eu-north-1': {'long_name': 'Europe (Stockholm)', 'code': 'eun1'},
  'sa-east-1': {'long_name': 'South America (São Paulo)', 'code': 'sae1'}}
 subscription_url = 'https://www.cloudpy.org'
 msh = 'secure'
-cloudpy_org_version='1.5.4'
+cloudpy_org_version='1.5.5'
 gsep = {'user_email_sep': '-0-', '@': '-1-', '.': '-2-'}
 from cloudpy_org.tools import processing_tools,unique_id
 from cloudpy_org.docs import auto_document,convert_jupiter_notebook_to_html,documentation_from_folder
 from cloudpy_org.aws import aws_framework_manager,aws_framework_manager_client,gen_aws_auth_token,gen_new_service_token,configure_aws,get_my_aws_service_token,authenticate_with_token,delete_biscuit,co_token_auth
 from cloudpy_org.web import flask_website
 from cloudpy_org.imgedit import colors
 from cloudpy_org.client_usage import cloudpy_org_aws_framework_client
```

### Comparing `cloudpy_org-1.5.4/cloudpy_org/aws.py` & `cloudpy_org-1.5.5/cloudpy_org/aws.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.4/cloudpy_org/client_usage.py` & `cloudpy_org-1.5.5/cloudpy_org/client_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #___________________________________________________
 k = 'select'
 this_dict[k] = {}
 this_dict[k]['html'] = """
 <br>
 <label class="sensation">@label_title</label>
 <br>
-<select k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation inx" onchange="temp_input(this,'@k','');" onload="">
+<select action_id="@action_id" action_item="@action_item" k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation inx" onchange="temp_input(this,'@k','');" onload="">
 @options
 </select>
 <br>
 """.replace('@k',k)
 this_dict[k]['object'] = "<option>@object</option>"
 this_dict[k]['params'] = ['@id','@label_title','@options']
 #___________________________________________________
@@ -46,15 +46,15 @@
 @options
 </a>
 </div>
 <br>
 """.replace('@k',k)
 this_dict[k]['object'] = """&nbsp;&nbsp;&nbsp;
 <span style="padding-right:10px;">
-<input k="@k" obj="@object" enter_key='@enter_key' labelkey="@label_title" type="radio" name="radio_@id" id="@id_@n" onchecked="temp_input(this,'@k','@object');" onload="">
+<input action_id="@action_id" action_item="@action_item" k="@k" obj="@object" enter_key='@enter_key' labelkey="@label_title" type="radio" name="radio_@id" id="@id_@n" onchecked="temp_input(this,'@k','@object');" onload="">
 <label for="@id_@n" class ="sensation">@object</label>
 </span>
 """.replace('@k',k)
 this_dict[k]['params'] = ['@id','@label_title','@option_1','@option_2']
 #___________________________________________________
 k = 'radios_vertical'
 this_dict[k] = {}
@@ -68,82 +68,82 @@
 @options
 </a>
 </div>
 <br>
 """.replace('@k',k)
 this_dict[k]['object'] = """&nbsp;&nbsp;&nbsp;
 <div style="padding-right:10px;">
-<input k="@k" obj="@object" labelkey="@label_title" type="radio" name="radio_@id" id="@id_@n" onchecked="temp_input(this,'@k','@object');" onload="">
+<input action_id="@action_id" action_item="@action_item" k="@k" obj="@object" labelkey="@label_title" type="radio" name="radio_@id" id="@id_@n" onchecked="temp_input(this,'@k','@object');" onload="">
 <label for="@id_@n" class ="sensation">@object</label>
 </div>
 """.replace('@k',k)
 this_dict[k]['params'] = ['@id','@label_title','@option_1','@option_2']
 #___________________________________________________
 k = 'text_input'
 this_dict[k] = {}
 this_dict[k]['html'] = """
 <br>
 <label class="sensation" for="@id">@label_title</label>
 <br>
-<input k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation" us="@us" type="text" value="@text_content" style="border-bottom-width:1px;" oninput="temp_input(this,'@k','');" onload="">
+<input action_id="@action_id" action_item="@action_item" k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation" us="@us" type="text" value="@text_content" style="border-bottom-width:1px;" oninput="temp_input(this,'@k','');" onload="">
 <br>
 """.replace('@k',k)
 this_dict[k]['params'] = ['@id','@label_title','@text_content']
 #___________________________________________________
 k = 'pwd_input'
 this_dict[k] = {}
 this_dict[k]['html'] = """
 <br>
 <label class="sensation" for="@id">@label_title</label>
 <br>
-<input k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation" type="password" autocomplete="off" cpw="@cpw" cpwconf="@cpwconf" value="@text_content" style="border-bottom-width:1px;" oninput="temp_input(this,'@k','');" onload="">
+<input action_id="@action_id" action_item="@action_item" k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation" type="password" autocomplete="off" cpw="@cpw" cpwconf="@cpwconf" value="@text_content" style="border-bottom-width:1px;" oninput="temp_input(this,'@k','');" onload="">
 <br>
 """.replace('@k',k)
 this_dict[k]['params'] = ['@id','@label_title','@text_content']
 #___________________________________________________
 k = 'btn_input'
 this_dict[k] = {}
 this_dict[k]['html'] = """
 <br>
 <br>
 <br>
 <a class="sensation" id="@id_label" style="display:none;font-size:16px;color:gray;"><a/>
-<button id="@id" class="submitrequest" event_type='@event_type' style="width:100%;" onclick="temp_input(this,'@k','');" onload="">@label_title</button>
+<button action_id="@action_id" action_item="@action_item" id="@id" class="submitrequest" event_type='@event_type' style="width:100%;" onclick="temp_input(this,'@k','');" onload="">@label_title</button>
 <br>
 """.replace('@k',k)
 this_dict[k]['params'] = ['@id','@label_title','@text_content']
 #___________________________________________________
 k = 'text_area'
 this_dict[k] = {}
 this_dict[k]['html'] = """
 <br>
 <label class="sensation" for="@id">@label_title</label>
 <br>
-<textarea k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation inx" rows="@rowsnum" oninput="temp_input(this,'@k','');" onload="">@text_content</textarea>
+<textarea action_id="@action_id" action_item="@action_item" k="@k" obj="" enter_key='@enter_key' labelkey="@label_title" id="@id" class="sensation inx" rows="@rowsnum" oninput="temp_input(this,'@k','');" onload="">@text_content</textarea>
 <br>
 """.replace('@k',k)
 this_dict[k]['params'] = ['@id','@label_title','@rowsnum']
 #___________________________________________________
 k = 'acc_checkboxes'
 this_dict[k] = {}
 this_dict[k]['html'] = """
 <br>
-<div class='accordion' id='acc_@id'>
+<div action_id="@action_id" action_item="@action_item" class='accordion' id='acc_@id'>
 <div class="accordion-item" style="font-size:14px;">
 <h2 class="accordion-header" id="@id">
 <button class="accordion-button collapsed sensation" style="font-size:14px;padding:7px;" type="button" data-bs-toggle="collapse" 
 data-bs-target="#collapse_@id" aria-expanded="false" aria-controls="collapseOne">
 @label_title
 <a id="@id_counter_container" style="position:absolute;left:@counter_leftpx;color:#252F3E;display:none;"><span id="@id_counter" 
 style="padding-right:10px;">0</span><span>selected</span></a>
 </button>
 </h2>
 <div id="collapse_@id" class="accordion-collapse collapse" aria-labelledby="@id" 
 data-bs-parent="#acc_@id" style="">
-<div class="accordion-body">
+<div id='acc_@id_body' class="accordion-body">
 @options
 </div></div></div>
 </div>
 <br>
 """.replace('@k',k)
 this_dict[k]['object'] = """<div style="padding:7px;"><input labelkey="@label_title" type="checkbox" id="@id_checkbox_@n" onclick="temp_input(this,'@k','');service_counter(this,'@id');" onload=""><label class="sensation" for="@id_checkbox_@n">@object</label></div>
 """.replace('@k',k)
@@ -389,36 +389,53 @@
                     ,menu_font_color=menu_font_color
                 )
         
         rslt = rslt.replace('@items',items)
         return rslt.replace('\n','')
         
     #___________________________________________________
-    def create_input(self,input_type:str,label_title:str,options:list=[],text_content:str='',rowsnum:int=3,section_size:int=3,event_type:str='save',us:str='no',cpw:str='no',cpwconf:str='no',enter_key:str='no'):
+    def create_input(self
+                     ,input_type:str
+                     ,label_title:str
+                     ,options:list=[]
+                     ,text_content:str=''
+                     ,rowsnum:int=3
+                     ,section_size:int=3
+                     ,event_type:str='save'
+                     ,us:str='no'
+                     ,cpw:str='no'
+                     ,cpwconf:str='no'
+                     ,enter_key:str='no'
+                     ,action_id:str=''
+                     ,action_item:str=''):
         counter_left = (section_size-1)*120 + 20
         a = self.pt.camel_to_snake(label_title)[0:12].replace('?','').replace('.','_').replace(',','')
         this_id = a[0:6] + a[::-1][0:6][::-1]
         this_id = this_id.replace("'","").replace('"','')
         rslt = self.main_dict['inputs'][input_type]['html']\
         .replace('@id',this_id)\
         .replace('@label_title',label_title)\
         .replace('@us',us)\
         .replace('@cpwconf',cpwconf)\
         .replace('@cpw',cpw)\
-        .replace('@enter_key',enter_key)
+        .replace('@enter_key',enter_key)\
+        .replace('@action_id',action_id)\
+        .replace('@action_item',action_item)
         if input_type in ['select','radios_horizontal','radios_vertical','acc_checkboxes']:
             opti = ''
             obj = self.main_dict['inputs'][input_type]['object']
             n = 0
             for this_option in options:
                 n+=1
                 opti += obj.replace('@object',this_option)\
                 .replace('@n',str(n))\
                 .replace('@id',this_id)\
-                .replace('@label_title',label_title)
+                .replace('@label_title',label_title)\
+                .replace('@action_id',action_id)\
+                .replace('@action_item',action_item)
             rslt = rslt.replace('@options',opti).replace('@counter_left',str(counter_left))
         elif input_type in['text_input','pwd_input','text_area']:
             rslt = rslt.replace('@text_content',text_content)
             if input_type == 'text_area':
                 rslt = rslt.replace('@rowsnum',str(rowsnum))
         elif input_type in ['btn_input']:
             rslt = rslt.replace('@event_type',event_type)
@@ -439,14 +456,21 @@
             editvisibility = 'hidden'
             if 'edit_enabled' in set(ts.keys()):
                 if len(ts['section_title']) > 0 and ts['edit_enabled'].lower().replace(' ','') == 'yes':
                     editvisibility = 'visible'
             section = section.replace('@editvisibility',editvisibility)
             content = ""
             for j in inputs:
+                action_id = ''
+                if 'action_id' in set(j.keys()):
+                    action_id=j['action_id'].lower().replace(' ','')
+                action_item= ''
+                if 'action_item' in set(j.keys()):
+                    action_item=j['action_item'].lower().replace(' ','')
+                
                 if 'custom_content' in set(j.keys()):
                     content += j['custom_content']
                 elif j['input_type'] in ['text_input','pwd_input','text_area']:
                     enter_key = 'no'
                     if 'enter_key' in set(j.keys()):
                         enter_key = j['enter_key'].lower().replace(' ','')
                             
@@ -457,26 +481,30 @@
                         rowsnum = j['rowsnum']
                         content += self.create_input(
                             input_type=j['input_type']
                             ,label_title=j['label_title']
                             ,text_content=text_content
                             ,rowsnum=rowsnum
                             ,section_size=section_size
-                            ,enter_key=enter_key)
+                            ,enter_key=enter_key
+                            ,action_id=action_id
+                            ,action_item=action_item)
                     elif j['input_type'] == 'text_input':
                         us = 'no'
                         if 'us' in set(j.keys()):
                             us=j['us'].lower().replace(' ','')
                         content += self.create_input(
                             input_type=j['input_type']
                             ,label_title=j['label_title']
                             ,text_content=text_content
                             ,section_size=section_size
                             ,us=us
                             ,enter_key=enter_key
+                            ,action_id=action_id
+                            ,action_item=action_item
                         )
                     elif j['input_type'] == 'pwd_input':
                         cpw = 'no'
                         if 'cpw' in set(j.keys()):
                             cpw=j['cpw'].lower().replace(' ','')
                         cpwconf = 'no'
                         if 'cpwconf' in set(j.keys()):
@@ -485,40 +513,48 @@
                             input_type=j['input_type']
                             ,label_title=j['label_title']
                             ,text_content=text_content
                             ,section_size=section_size
                             ,cpw=cpw
                             ,cpwconf=cpwconf
                             ,enter_key=enter_key
+                            ,action_id=action_id
+                            ,action_item=action_item
                         )
                     else:
                         content += self.create_input(
                             input_type=j['input_type']
                             ,label_title=j['label_title']
                             ,text_content=text_content
-                            ,section_size=section_size)
+                            ,section_size=section_size
+                            ,action_id=action_id
+                            ,action_item=action_item)
                 elif j['input_type'] in ['btn_input']:
                     event_type = None
                     if 'event_type' in set(j.keys()):
                         event_type=j['event_type']
                     content += self.create_input(
                         input_type=j['input_type']
                         ,label_title=j['label_title']
                         ,section_size=section_size
                         ,event_type=str(event_type)
+                        ,action_id=action_id
+                        ,action_item=action_item
                     )
                 else:
                     options = []
                     if 'options' in set(j.keys()):
                         options=j['options']
                     content += self.create_input(
                         input_type=j['input_type']
                         ,label_title=j['label_title']
                         ,options=options
                         ,section_size=section_size
+                        ,action_id=action_id
+                        ,action_item=action_item
                     )
             sections += section.replace('@content',content)
         
         complete_form = '<div id="main_row" class="row">@sections</div>'
         complete_form =complete_form.replace('@sections',sections)
         dynamic_form_keys = set(dynamic_form.keys())
         if 'body_style' in dynamic_form_keys and dynamic_form['body_style'].lower().replace(' ','') != 'default':
```

### Comparing `cloudpy_org-1.5.4/cloudpy_org/docs.py` & `cloudpy_org-1.5.5/cloudpy_org/docs.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.4/cloudpy_org/imgedit.py` & `cloudpy_org-1.5.5/cloudpy_org/imgedit.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.4/cloudpy_org/tools.py` & `cloudpy_org-1.5.5/cloudpy_org/tools.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.4/cloudpy_org/web.py` & `cloudpy_org-1.5.5/cloudpy_org/web.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.4/cloudpy_org/web_client_usage.py` & `cloudpy_org-1.5.5/cloudpy_org/web_client_usage.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.5.4/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.5.5/cloudpy_org.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.5.4
+Version: 1.5.5
 Summary: Cloud data pipeline organization and automation library. Includes AWS framework manager API.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.5.4/setup.py` & `cloudpy_org-1.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.5.4",
+    version="1.5.5",
     description="Cloud data pipeline organization and automation library. Includes AWS framework manager API.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

