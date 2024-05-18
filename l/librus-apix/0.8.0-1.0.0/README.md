# Comparing `tmp/librus_apix-0.8.0.tar.gz` & `tmp/librus_apix-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-0.8.0.tar", last modified: Fri May 17 18:04:02 2024, max compression
+gzip compressed data, was "librus_apix-1.0.0.tar", last modified: Sat May 18 20:21:14 2024, max compression
```

## Comparing `librus_apix-0.8.0.tar` & `librus_apix-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:04:02.138646 librus_apix-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 18:03:59.000000 librus_apix-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-17 18:04:02.138646 librus_apix-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-17 18:03:59.000000 librus_apix-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:04:02.138646 librus_apix-0.8.0/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/get_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-17 18:03:59.000000 librus_apix-0.8.0/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:04:02.138646 librus_apix-0.8.0/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-17 18:04:02.000000 librus_apix-0.8.0/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-17 18:04:02.000000 librus_apix-0.8.0/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:04:02.000000 librus_apix-0.8.0/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 18:04:02.000000 librus_apix-0.8.0/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 18:04:02.000000 librus_apix-0.8.0/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-17 18:03:59.000000 librus_apix-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-17 18:04:02.138646 librus_apix-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:03:59.000000 librus_apix-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:21:14.008468 librus_apix-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-18 20:21:10.000000 librus_apix-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 20:21:14.008468 librus_apix-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-18 20:21:10.000000 librus_apix-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:21:14.008468 librus_apix-1.0.0/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-18 20:21:10.000000 librus_apix-1.0.0/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:21:14.008468 librus_apix-1.0.0/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-18 20:21:13.000000 librus_apix-1.0.0/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-18 20:21:10.000000 librus_apix-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-18 20:21:14.008468 librus_apix-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:21:10.000000 librus_apix-1.0.0/setup.py
```

### Comparing `librus_apix-0.8.0/LICENSE` & `librus_apix-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-0.8.0/README.md` & `librus_apix-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,141 +1,151 @@
 <p align="center">
   <img src="https://github.com/RustySnek/librus-apix/blob/main/logo.png" alt="librus-apix logo"/>
 </p>
 
 # Librus Synergia web scraper.
+### Be sure to visit the [documentation](https://rustysnek.github.io/librus-apix/).
 
 
-> [!IMPORTANT]  
-> It's advised to [run all tests](#running-tests) before trying everything out.  Some schools have different librus setups which may cause errors/warnings  If you find any open an issue or contribute with a PR
-
 ## Installation
 
 ```sh
 pip install librus-apix
 ```
 
+> [!IMPORTANT]  
+> It's advised to [run all tests](#running-tests) before trying everything out.  Some schools have different librus setups which may cause errors/warnings  If you find any open an issue or contribute with a PR
+
+
 ## Running tests
 ### First, follow the [steps to clone the repo and install librus-apix locally](#working-on-the-project), then install pytest.
 ```bash
-  pip install pytest
+pip install pytest
 ```
 ### Run the tests
   #### [Retrieve your token key](#save-and-load-token) and test on actual data  
   
   ```bash
-    pytest --token {output of token.API_Key}
+  pytest --token {output of token.API_Key}
   ```
   
   #### [Dev] Test using a mock server
   - For developing purposes I've created a [simple mock html server](https://github.com/RustySnek/librus-apix-mock)
 
     ```bash
-      # generate all html pages and run server
-      python scripts/generate_all.py
-      python server.py
-      # now unless you've changed the server.py default port you should be good to go and run
-      pytest
-      # if you did change the port, you have to edit the tests/conftest.py file accordingly
+    # generate all html pages and run server
+    python scripts/generate_all.py
+    python server.py
+    # now unless you've changed the server.py default port you should be good to go and run
+    pytest
+    # if you did change the port, you have to edit the tests/conftest.py file accordingly
     ```
 
 # Quick Start
 
-## Getting the Token
+## Setting up client
 ```py
-from librus_apix.get_token import get_token
+from librus_apix.client import Client, Token, new_client
 
-token = get_token("Username", "Password")
+# create a new client with empty Token()
+client: Client = new_client()
+# update the token
+_token: Token = client.get_token("username", "password")
+# now you can pass your client to librus-apix functions
 ```
 ### Save and Load token
 ```py
-from librus_apix.get_token import get_token, Token
+from librus_apix.client import Token, Client, new_client
 
-token = get_token("Username", "Password")
-
-token_key = token.API_Key
-# you can store this key and later load it into Token class like this:
-token = Token(token_key)
+key = client.token.API_Key
 
+# you can store this key and later load it in ways like this:
+## Load directly into token object
+token = Token(API_Key=token_key)
+client: Client = new_client(token=token)
+## or put it into existing client
+client.token = token
+## or into empty token
+client.token.API_Key = key
 
 ```
 ### Getting the Math grades
 
 ```py
 from librus_apix.grades import get_grades
 
-grades, average_grades, descriptive_grades = get_grades(token)
+grades, average_grades, descriptive_grades = get_grades(client)
 
 for semester in grades:
   for mark in semester["Mathematics"]:
       print(mark.grade)
 for semester in descriptive_grades:
   for mark in semester["Emotional development"]:
       print(mark.grade)
 ```
 
 ### Getting the Announcements
 ```py
 from librus_apix.announcements import get_announcements
 
-announcements = get_announcements(token)
+announcements = get_announcements(client)
 
 for a in announcements:
   print(a.description)
 
 ```
 
 ### Getting the attendance
 ```py
 from librus_apix.attendance import get_attendance
 
-first_semester, second_semester = get_attendance(token)
+first_semester, second_semester = get_attendance(client)
 
 for attendance in first_semester:
   print(attendance.symbol, attendance.date)
 
 ```
 
 ### Getting the attendance frequency
 ```py
 from librus_apix.attendance import get_attendance_frequency
 
-first, second, overall = get_attendance_frequency(token)
+first, second, overall = get_attendance_frequency(client)
 print(f"{first*100}%")
 
 ```
 
 ### Getting the Homework
 ```py
 from librus_apix.homework import get_homework, homework_detail
 
 # date from-to up to 1 month 
 date_from = '2023-03-02'
 date_to = '2023-03-30'
 
-homework = get_homework(token, date_from, date_to)
+homework = get_homework(client, date_from, date_to)
 
 for h in homework:
   print(h.lesson, h.completion_date)
   href = h.href
-  details = homework_detail(token, href)
+  details = homework_detail(client, href)
   print(details)
 
 ```
 
 ### Sending Messages
 ```py
 from librus_apix.messages import recipient_groups, get_recipients, send_message
 
-groups = recipient_groups(token)
-recipients = get_recipients(token, groups[0])
+groups = recipient_groups(client)
+recipients = get_recipients(client, groups[0])
 my_recipient = recipients["John Brown"]
 my_second_recipient = recipients["Barbara Brown"]
 
-sent = send_message(token,
+sent = send_message(client,
                    "Message Title",
                    "Message\n content",
                    "teachers",
                    [my_recipient, my_second_recipient]
 )
 if sent == True:
   print("Sent!")
@@ -143,70 +153,68 @@
   print("Error sending a message!")
 ```
 
 ### Getting the Messages
 ```py
 from librus_apix.messages import get_recieved, message_content
 
-messages = get_recieved(token, page=1)
+messages = get_recieved(client, page=1)
 for message in messages:
   print(message.title)
   href = message.href
-  print(message_content(token, href))
+  print(message_content(client, href))
 
 ```
 
 ### Getting the Schedule
 
 ```py
 from librus_apix.schedule import get_schedule, schedule_detail
 month = '2'
 year = '2023'
-schedule = get_schedule(token, month, year)
+schedule = get_schedule(client, month, year)
 for day in schedule:
   for event in schedule[day]:
     print(event.title)
     prefix, href = event.href.split('/')
-    details = schedule_detail(token, prefix, href)
+    details = schedule_detail(client, prefix, href)
     print(details)
 
 ```
 
 ### Getting the Timetable
 
 ```py
 from datetime import datetime
 from librus_apix.timetable import get_timetable
 
 monday_date = '2023-04-3'
 monday_datetime = datetime.strptime(monday_date, '%Y-%m-%d')
-timetable = get_timetable(token, monday_datetime)
+timetable = get_timetable(client, monday_datetime)
 for weekday in timetable:
   for period in timetable[weekday]:
     print(period.subject, period.teacher_and_classroom)
 
 ```
 
 
 ### Getting the lucky number
 ```py
 from librus_apix.student_information import student_information
 
-info = student_information(token)
+info = student_information(client)
 print(info.lucky_number)
 ```
 
 ### Adding a proxy
 ```py
 # Proxy can be added with
-token = get_token(u, p, proxy={"https": "http://my-proxy.xyz"})
-# or
-token.proxy = {"https": "http://my-proxy.xyz"}
+client = new_client(proxy={"https": "http://my-proxy.xyz"})
 # or
-token = Token(token_key, proxy={"https": "http://my-proxy.xyz"})
+client.proxy = {"https": "http://my-proxy.xyz"}
 ```
 
 ## Working On The Project
 
 ```sh
 git clone https://github.com/RustySnek/librus-apix
 cd librus-apix
```

### Comparing `librus_apix-0.8.0/librus_apix.egg-info/SOURCES.txt` & `librus_apix-1.0.0/librus_apix.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 librus_apix/__init__.py
 librus_apix/announcements.py
 librus_apix/attendance.py
+librus_apix/client.py
 librus_apix/completed_lessons.py
 librus_apix/exceptions.py
-librus_apix/get_token.py
 librus_apix/grades.py
 librus_apix/helpers.py
 librus_apix/homework.py
 librus_apix/messages.py
 librus_apix/schedule.py
 librus_apix/student_information.py
 librus_apix/timetable.py
```

### Comparing `librus_apix-0.8.0/setup.cfg` & `librus_apix-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v0.8.0
+version = v1.0.0
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

