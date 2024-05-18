# Comparing `tmp/django-appointment-3.4.1.tar.gz` & `tmp/django_appointment-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-appointment-3.4.1.tar", last modified: Sun Mar 31 00:31:21 2024, max compression
+gzip compressed data, was "django_appointment-3.5.0.tar", last modified: Sat May 18 17:38:35 2024, max compression
```

## Comparing `django-appointment-3.4.1.tar` & `django_appointment-3.5.0.tar`

### file list

```diff
@@ -1,140 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.033220 django-appointment-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-03-31 00:31:13.000000 django-appointment-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-31 00:31:13.000000 django-appointment-3.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-03-31 00:31:21.033220 django-appointment-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13831 2024-03-31 00:31:13.000000 django-appointment-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.013220 django-appointment-3.4.1/appointment/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.013220 django-appointment-3.4.1/appointment/email_sender/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/email_sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/email_sender/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/logger_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/messages_.py
--rw-r--r--   0 runner    (1001) docker     (127)    33146 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    26938 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.009220 django-appointment-3.4.1/appointment/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.013220 django-appointment-3.4.1/appointment/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.017220 django-appointment-3.4.1/appointment/static/css/app_admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/admin.css
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/btn.css
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/days_off.css
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/display_appointment.css
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/service.css
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/staff_member.css
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/user_profile.css
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/app_admin/working_hours.css
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/appointments.css
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/appt-common.css
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/thank_you.css
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/css/verification_code.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.017220 django-appointment-3.4.1/appointment/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)   119329 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/img/email_hd_bg.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.017220 django-appointment-3.4.1/appointment/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.017220 django-appointment-3.4.1/appointment/static/js/app_admin/
--rw-r--r--   0 runner    (1001) docker     (127)    32207 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/js/app_admin/staff_index.js
--rw-r--r--   0 runner    (1001) docker     (127)    15128 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/js/appointments.js
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/js/js-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.017220 django-appointment-3.4.1/appointment/static/js/modal/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/js/modal/error_modal.js
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/static/js/modal/show_modal.js
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.009220 django-appointment-3.4.1/appointment/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.021220 django-appointment-3.4.1/appointment/templates/administration/
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/display_appointment.html
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/email_change_verification_code.html
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/manage_day_off.html
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/manage_service.html
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/manage_staff_member.html
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/manage_staff_personal_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/manage_working_hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/service_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    16059 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/staff_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/staff_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    15890 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/administration/user_profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.021220 django-appointment-3.4.1/appointment/templates/appointment/
--rw-r--r--   0 runner    (1001) docker     (127)     8711 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/appointment/appointments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/appointment/enter_verification_code.html
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/appointment/rescheduling_thank_you.html
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/appointment/set_password.html
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/appointment/thank_you.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.021220 django-appointment-3.4.1/appointment/templates/base_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.021220 django-appointment-3.4.1/appointment/templates/email_sender/
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/email_sender/admin_new_appointment_email.html
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/email_sender/reminder_email.html
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/email_sender/reschedule_email.html
--rw-r--r--   0 runner    (1001) docker     (127)    12661 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/email_sender/thank_you_email.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.021220 django-appointment-3.4.1/appointment/templates/error_pages/
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/error_pages/304_already_submitted.html
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/error_pages/403_forbidden.html
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/error_pages/403_forbidden_rescheduling.html
--rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/error_pages/404_not_found.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.021220 django-appointment-3.4.1/appointment/templates/modal/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/modal/confirm_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/modal/error_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/templates/modal/event_details_modal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.025220 django-appointment-3.4.1/appointment/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.025220 django-appointment-3.4.1/appointment/tests/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/base/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.025220 django-appointment-3.4.1/appointment/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/mixins/base_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.029220 django-appointment-3.4.1/appointment/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_appointment_reschedule_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    12656 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_appointment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_appointment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_day_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_email_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_password_reset_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_payment_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_staff_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/models/test_model_working_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/test_availability_slot.py
--rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55826 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.029220 django-appointment-3.4.1/appointment/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18916 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/utils/test_date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    54957 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/utils/test_db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/utils/test_email_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/utils/test_json_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/utils/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/tests/utils/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.029220 django-appointment-3.4.1/appointment/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    26879 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/email_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/json_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/utils/view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28598 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    23688 2024-03-31 00:31:13.000000 django-appointment-3.4.1/appointment/views_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 00:31:21.033220 django-appointment-3.4.1/django_appointment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-03-31 00:31:20.000000 django-appointment-3.4.1/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-03-31 00:31:20.000000 django-appointment-3.4.1/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 00:31:20.000000 django-appointment-3.4.1/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-31 00:31:20.000000 django-appointment-3.4.1/django_appointment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-31 00:31:20.000000 django-appointment-3.4.1/django_appointment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-31 00:31:13.000000 django-appointment-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-31 00:31:13.000000 django-appointment-3.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-31 00:31:21.033220 django-appointment-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-31 00:31:13.000000 django-appointment-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.897058 django_appointment-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-18 17:38:24.000000 django_appointment-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-18 17:38:24.000000 django_appointment-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-18 17:38:35.897058 django_appointment-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-05-18 17:38:24.000000 django_appointment-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.881058 django_appointment-3.5.0/appointment/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.881058 django_appointment-3.5.0/appointment/email_sender/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/email_sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/email_sender/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/messages_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27021 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.873058 django_appointment-3.5.0/appointment/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.881058 django_appointment-3.5.0/appointment/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.881058 django_appointment-3.5.0/appointment/static/css/app_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/admin.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/btn.css
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/days_off.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/display_appointment.css
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/service.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/staff_member.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/user_profile.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/app_admin/working_hours.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/appointments.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/appt-common.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/thank_you.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/css/verification_code.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.885058 django_appointment-3.5.0/appointment/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   119329 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/img/email_hd_bg.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.885058 django_appointment-3.5.0/appointment/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.885058 django_appointment-3.5.0/appointment/static/js/app_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    32693 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/js/app_admin/staff_index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15136 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/js/appointments.js
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/js/js-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.885058 django_appointment-3.5.0/appointment/static/js/modal/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/js/modal/error_modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/static/js/modal/show_modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.873058 django_appointment-3.5.0/appointment/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.885058 django_appointment-3.5.0/appointment/templates/administration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/display_appointment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/email_change_verification_code.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/manage_day_off.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/manage_service.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/manage_staff_member.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/manage_staff_personal_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/manage_working_hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/service_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/staff_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/staff_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/administration/user_profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.889058 django_appointment-3.5.0/appointment/templates/appointment/
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/appointment/enter_verification_code.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/appointment/rescheduling_thank_you.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/appointment/set_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/appointment/thank_you.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.889058 django_appointment-3.5.0/appointment/templates/base_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.889058 django_appointment-3.5.0/appointment/templates/email_sender/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/email_sender/admin_new_appointment_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/email_sender/reminder_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/email_sender/reschedule_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/email_sender/thank_you_email.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.889058 django_appointment-3.5.0/appointment/templates/error_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/error_pages/304_already_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/error_pages/403_forbidden.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/error_pages/403_forbidden_rescheduling.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/error_pages/404_not_found.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.889058 django_appointment-3.5.0/appointment/templates/modal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/modal/confirm_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/modal/error_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/templates/modal/event_details_modal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.889058 django_appointment-3.5.0/appointment/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.893058 django_appointment-3.5.0/appointment/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/base/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.893058 django_appointment-3.5.0/appointment/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/mixins/base_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.893058 django_appointment-3.5.0/appointment/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_appointment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_appointment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_appointment_reschedule_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_day_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_email_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_password_reset_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_payment_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_staff_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/models/test_working_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56524 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.893058 django_appointment-3.5.0/appointment/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51195 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_email_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_json_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_staff_member_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/tests/utils/test_view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.897058 django_appointment-3.5.0/appointment/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26916 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/email_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/json_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/utils/view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27965 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24130 2024-05-18 17:38:24.000000 django_appointment-3.5.0/appointment/views_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:38:35.897058 django_appointment-3.5.0/django_appointment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-18 17:38:35.000000 django_appointment-3.5.0/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-18 17:38:35.000000 django_appointment-3.5.0/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:38:35.000000 django_appointment-3.5.0/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-18 17:38:35.000000 django_appointment-3.5.0/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 17:38:35.000000 django_appointment-3.5.0/django_appointment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-18 17:38:24.000000 django_appointment-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-18 17:38:24.000000 django_appointment-3.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-18 17:38:35.897058 django_appointment-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-18 17:38:24.000000 django_appointment-3.5.0/setup.py
```

### Comparing `django-appointment-3.4.1/LICENSE` & `django_appointment-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/MANIFEST.in` & `django_appointment-3.5.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/PKG-INFO` & `django_appointment-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 3.4.1
+Version: 3.5.0
 Summary: Managing appointment scheduling with customizable slots, staff features, and conflict handling.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
-Author-email: adamspd.developer@gmail.com
+Author-email: django-appt@adamspierredavid.com
 License: Apache License 2.0
 Project-URL: Author's Website, https://adamspierredavid.com/
-Project-URL: Package's Website, https://django-appt.adamspierredavid.com/
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Package's demo Website, https://django-appt.adamspierredavid.com/
+Project-URL: Documentation, https://django-appt-doc.adamspierredavid.com/overview.html
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -37,15 +38,14 @@
 
 ![Tests](https://github.com/adamspd/django-appointment/actions/workflows/tests.yml/badge.svg)
 ![Published on PyPi](https://github.com/adamspd/django-appointment/actions/workflows/publish.yml/badge.svg)
 [![Doc](https://github.com/adamspd/django-appointment-doc/actions/workflows/build-docs.yml/badge.svg)](https://django-appt-doc.adamspierredavid.com/overview.html)
 [![Current Release Version](https://img.shields.io/github/release/adamspd/django-appointment.svg?style=flat-square&logo=github)](https://github.com/adamspd/django-appointment/releases)
 [![pypi Version](https://img.shields.io/pypi/v/django-appointment.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/django-appointment/)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/django-appointment?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/django-appointment/)
-[![codecov](https://codecov.io/gh/adamspd/django-appointment/branch/main/graph/badge.svg?token=ZQZQZQZQZQ)](https://codecov.io/gh/adamspd/django-appointment)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/commits/main)
 [![GitHub last commit](https://img.shields.io/github/last-commit/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/commit/main)
 [![GitHub issues](https://img.shields.io/github/issues/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/pulls)
 [![GitHub contributors](https://img.shields.io/github/contributors/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/graphs/contributors)
 [![GitHub stars](https://img.shields.io/github/stars/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/stargazers)
@@ -331,15 +331,14 @@
 ## Security policy 🔒
 
 Please refer to the [security policy](https://github.com/adamspd/django-appointment/tree/main/SECURITY.md) for more
 information.
 
 ## Notes 📝⚠️
 
-I'm working on a testing website for the application
-that is not fully functional yet, no hard feelings. But you can check it out
-at [https://django-appt.adamspierredavid.com/](https://django-appt.adamspierredavid.com/). Ideas are welcome here since
-I'm blocked on a few points.
+I'm working on a testing website for the application that is not fully functional yet, no hard feelings. Before using it, 
+it's important to me that you read the terms of use, only then you can use it if you agree to them. The demo website is located
+at [https://django-appt.adamspierredavid.com/](https://django-appt.adamspierredavid.com/terms-and-conditions/). Ideas are welcome.
 
 ## About the Author
 
 Adams Pierre David - [Website](https://adamspierredavid.com/)
```

### Comparing `django-appointment-3.4.1/README.md` & `django_appointment-3.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 ![Tests](https://github.com/adamspd/django-appointment/actions/workflows/tests.yml/badge.svg)
 ![Published on PyPi](https://github.com/adamspd/django-appointment/actions/workflows/publish.yml/badge.svg)
 [![Doc](https://github.com/adamspd/django-appointment-doc/actions/workflows/build-docs.yml/badge.svg)](https://django-appt-doc.adamspierredavid.com/overview.html)
 [![Current Release Version](https://img.shields.io/github/release/adamspd/django-appointment.svg?style=flat-square&logo=github)](https://github.com/adamspd/django-appointment/releases)
 [![pypi Version](https://img.shields.io/pypi/v/django-appointment.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/django-appointment/)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/django-appointment?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/django-appointment/)
-[![codecov](https://codecov.io/gh/adamspd/django-appointment/branch/main/graph/badge.svg?token=ZQZQZQZQZQ)](https://codecov.io/gh/adamspd/django-appointment)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/commits/main)
 [![GitHub last commit](https://img.shields.io/github/last-commit/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/commit/main)
 [![GitHub issues](https://img.shields.io/github/issues/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/pulls)
 [![GitHub contributors](https://img.shields.io/github/contributors/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/graphs/contributors)
 [![GitHub stars](https://img.shields.io/github/stars/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/stargazers)
@@ -296,15 +295,14 @@
 ## Security policy 🔒
 
 Please refer to the [security policy](https://github.com/adamspd/django-appointment/tree/main/SECURITY.md) for more
 information.
 
 ## Notes 📝⚠️
 
-I'm working on a testing website for the application
-that is not fully functional yet, no hard feelings. But you can check it out
-at [https://django-appt.adamspierredavid.com/](https://django-appt.adamspierredavid.com/). Ideas are welcome here since
-I'm blocked on a few points.
+I'm working on a testing website for the application that is not fully functional yet, no hard feelings. Before using it, 
+it's important to me that you read the terms of use, only then you can use it if you agree to them. The demo website is located
+at [https://django-appt.adamspierredavid.com/](https://django-appt.adamspierredavid.com/terms-and-conditions/). Ideas are welcome.
 
 ## About the Author
 
 Adams Pierre David - [Website](https://adamspierredavid.com/)
```

### Comparing `django-appointment-3.4.1/appointment/admin.py` & `django_appointment-3.5.0/appointment/admin.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/decorators.py` & `django_appointment-3.5.0/appointment/decorators.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/email_sender/email_sender.py` & `django_appointment-3.5.0/appointment/email_sender/email_sender.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/forms.py` & `django_appointment-3.5.0/appointment/forms.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 from phonenumber_field.widgets import PhoneNumberPrefixWidget
 
 from .models import (
     Appointment, AppointmentRequest, AppointmentRescheduleHistory, DayOff, Service, StaffMember,
     WorkingHours
 )
 from .utils.db_helpers import get_user_model
+from .utils.validators import not_in_the_past
+
+
+class SlotForm(forms.Form):
+    selected_date = forms.DateField(validators=[not_in_the_past])
+    staff_member = forms.ModelChoiceField(StaffMember.objects.all(), error_messages={'invalid_choice': 'Staff member does not exist'})
 
 
 class AppointmentRequestForm(forms.ModelForm):
     class Meta:
         model = AppointmentRequest
         fields = ('date', 'start_time', 'end_time', 'service', 'staff_member')
 
@@ -60,14 +66,19 @@
         self.fields['additional_info'].widget.attrs.update(
             {
                 'class': 'form-control',
                 'placeholder': 'I would like to be contacted by phone.'
             })
 
 
+class ClientDataForm(forms.Form):
+    name = forms.CharField(max_length=50, widget=forms.TextInput(attrs={'class': 'form-control'}))
+    email = forms.EmailField(widget=forms.EmailInput(attrs={'class': 'form-control'}))
+
+
 class PersonalInformationForm(forms.Form):
     # first_name, last_name, email
     first_name = forms.CharField(max_length=50, widget=forms.TextInput(attrs={'class': 'form-control'}))
     last_name = forms.CharField(max_length=50, widget=forms.TextInput(attrs={'class': 'form-control'}))
     email = forms.EmailField(widget=forms.EmailInput(attrs={'class': 'form-control'}))
 
     def __init__(self, *args, **kwargs):
@@ -113,14 +124,54 @@
                 'placeholder': _('Example value: 15, 30, 45, 60... (in minutes)')
             }),
             'work_on_saturday': forms.CheckboxInput(attrs={'class': 'form-check-input'}),
             'work_on_sunday': forms.CheckboxInput(attrs={'class': 'form-check-input'}),
         }
 
 
+class StaffMemberForm(forms.ModelForm):
+    class Meta:
+        model = StaffMember
+        fields = ['user', 'services_offered', 'slot_duration', 'lead_time', 'finish_time',
+                  'appointment_buffer_time', 'work_on_saturday', 'work_on_sunday']
+        widgets = {
+            'user': forms.Select(attrs={'class': 'form-control'}),
+            'service_offered': forms.Select(attrs={'class': 'form-control'}),
+            'slot_duration': forms.NumberInput(attrs={
+                'class': 'form-control',
+                'placeholder': _('Example value: 30, 60, 90, 120... (in minutes)')
+            }),
+            'lead_time': forms.TimeInput(attrs={
+                'class': 'form-control',
+                'placeholder': _('Example value: 08:00:00, 09:00:00... (24-hour format)')
+            }),
+            'finish_time': forms.TimeInput(attrs={
+                'class': 'form-control',
+                'placeholder': _('Example value: 17:00:00, 18:00:00... (24-hour format)')
+            }),
+            'appointment_buffer_time': forms.NumberInput(attrs={
+                'class': 'form-control',
+                'placeholder': _('Example value: 15, 30, 45, 60... (in minutes)')
+            }),
+            'work_on_saturday': forms.CheckboxInput(attrs={'class': 'form-check-input'}),
+            'work_on_sunday': forms.CheckboxInput(attrs={'class': 'form-check-input'}),
+        }
+
+    def __init__(self, *args, **kwargs):
+        super(StaffMemberForm, self).__init__(*args, **kwargs)
+        # Exclude users who are already staff members
+        existing_staff_user_ids = StaffMember.objects.values_list('user', flat=True)
+        # Filter queryset for user field to include only superusers or users not already staff members
+        self.fields['user'].queryset = get_user_model().objects.filter(
+            is_superuser=True
+        ).exclude(id__in=existing_staff_user_ids) | get_user_model().objects.exclude(
+            id__in=existing_staff_user_ids
+        )
+
+
 class StaffDaysOffForm(forms.ModelForm):
     class Meta:
         model = DayOff
         fields = ['start_date', 'end_date', 'description']
         widgets = {
             'start_date': forms.DateInput(attrs={'class': 'datepicker'}),
             'end_date': forms.DateInput(attrs={'class': 'datepicker'}),
```

### Comparing `django-appointment-3.4.1/appointment/messages_.py` & `django_appointment-3.5.0/appointment/messages_.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/models.py` & `django_appointment-3.5.0/appointment/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Since: 1.0.0
 """
 import colorsys
 import datetime
 import random
 import string
 import uuid
+from decimal import Decimal, InvalidOperation
 
 from babel.numbers import get_currency_symbol
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.core.validators import MaxLengthValidator, MinLengthValidator, MinValueValidator
 from django.db import models
 from django.urls import reverse
@@ -63,15 +64,15 @@
     Author: Adams Pierre David
     Version: 1.1.0
     Since: 1.0.0
     """
     name = models.CharField(max_length=100, blank=False)
     description = models.TextField(blank=True, null=True)
     duration = models.DurationField(validators=[MinValueValidator(datetime.timedelta(seconds=1))])
-    price = models.DecimalField(max_digits=6, decimal_places=2, validators=[MinValueValidator(0)])
+    price = models.DecimalField(max_digits=8, decimal_places=2, validators=[MinValueValidator(0)])
     down_payment = models.DecimalField(max_digits=6, decimal_places=2, default=0, validators=[MinValueValidator(0)])
     image = models.ImageField(upload_to='services/', blank=True, null=True)
     currency = models.CharField(max_length=3, default='USD', validators=[MaxLengthValidator(3), MinLengthValidator(3)])
     background_color = models.CharField(max_length=50, null=True, blank=True, default=generate_rgb_color)
     reschedule_limit = models.PositiveIntegerField(
         default=0,
         help_text=_("Maximum number of times an appointment can be rescheduled.")
@@ -209,15 +210,17 @@
     def works_on_both_weekends_day(self):
         return self.work_on_saturday and self.work_on_sunday
 
     def get_staff_member_name(self):
         if hasattr(self.user, 'get_full_name') and callable(getattr(self.user, 'get_full_name')):
             name = self.user.get_full_name()
         else:
-            name = self.user.first_name
+            name = f"{self.user.first_name} {self.user.last_name}".strip()
+        if not name:
+            name = self.user.username
         return name
 
     def get_staff_member_first_name(self):
         return self.user.first_name
 
     def get_non_working_days(self):
         non_working_days = []
@@ -431,15 +434,15 @@
     appointment_request = models.OneToOneField(AppointmentRequest, on_delete=models.CASCADE)
     phone = PhoneNumberField(blank=True)
     address = models.CharField(max_length=255, blank=True, null=True, default="",
                                help_text=_("Does not have to be specific, just the city and the state"))
     want_reminder = models.BooleanField(default=False)
     additional_info = models.TextField(blank=True, null=True)
     paid = models.BooleanField(default=False)
-    amount_to_pay = models.DecimalField(max_digits=6, decimal_places=2, blank=True, null=True)
+    amount_to_pay = models.DecimalField(max_digits=10, decimal_places=2, blank=True, null=True)
     id_request = models.CharField(max_length=100, blank=True, null=True)
 
     # meta datas
     created_at = models.DateTimeField(auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True)
 
     def __str__(self):
@@ -592,15 +595,15 @@
 
     def is_owner(self, staff_user_id):
         return self.appointment_request.staff_member.user.id == staff_user_id
 
     def to_dict(self):
         return {
             "id": self.id,
-            "client_name": self.client.get_full_name(),
+            "client_name": self.get_client_name(),
             "client_email": self.client.email,
             "start_time": self.appointment_request.start_time.strftime('%Y-%m-%d %H:%M'),
             "end_time": self.appointment_request.end_time.strftime('%Y-%m-%d %H:%M'),
             "service_name": self.appointment_request.service.name,
             "address": self.address,
             "want_reminder": self.want_reminder,
             "additional_info": self.additional_info,
@@ -660,14 +663,18 @@
 
     def clean(self):
         if Config.objects.exists() and not self.pk:
             raise ValidationError(_("You can only create one Config object"))
         if self.lead_time is not None and self.finish_time is not None:
             if self.lead_time >= self.finish_time:
                 raise ValidationError(_("Lead time must be before finish time"))
+        if self.appointment_buffer_time is not None and self.appointment_buffer_time < 0:
+            raise ValidationError(_("Appointment buffer time cannot be negative"))
+        if self.slot_duration is not None and self.slot_duration <= 0:
+            raise ValidationError(_("Slot duration must be greater than 0"))
 
     def save(self, *args, **kwargs):
         self.clean()
         self.pk = 1
         super(Config, self).save(*args, **kwargs)
 
     def delete(self, *args, **kwargs):
```

### Comparing `django-appointment-3.4.1/appointment/services.py` & `django_appointment-3.5.0/appointment/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -557,14 +557,16 @@
             return None, False, get_error_message_in_form(form=form)
     except Exception as e:
         return None, False, str(e)
 
 
 def create_new_appointment(data, request):
     service = Service.objects.get(id=data.get("service_id"))
+    print(f"service id {data.get('service_id')}")
+    print(f"Service: {service}")
     staff_id = data.get("staff_id")
     if staff_id:
         staff_member = StaffMember.objects.get(id=staff_id)
     else:
         staff_member = StaffMember.objects.get(user=request.user)
 
     # Convert date and start time strings to datetime objects
```

### Comparing `django-appointment-3.4.1/appointment/settings.py` & `django_appointment-3.5.0/appointment/settings.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/app_admin/admin.css` & `django_appointment-3.5.0/appointment/static/css/app_admin/admin.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/app_admin/btn.css` & `django_appointment-3.5.0/appointment/static/css/app_admin/btn.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/app_admin/days_off.css` & `django_appointment-3.5.0/appointment/static/css/app_admin/days_off.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/app_admin/display_appointment.css` & `django_appointment-3.5.0/appointment/static/css/app_admin/display_appointment.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/app_admin/service.css` & `django_appointment-3.5.0/appointment/static/css/app_admin/service.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/app_admin/user_profile.css` & `django_appointment-3.5.0/appointment/static/css/app_admin/user_profile.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/app_admin/working_hours.css` & `django_appointment-3.5.0/appointment/static/css/app_admin/working_hours.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/appointments-user-details.css` & `django_appointment-3.5.0/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/appt-common.css` & `django_appointment-3.5.0/appointment/static/css/appt-common.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/thank_you.css` & `django_appointment-3.5.0/appointment/static/css/thank_you.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/css/verification_code.css` & `django_appointment-3.5.0/appointment/static/css/verification_code.css`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/img/email_hd_bg.jpg` & `django_appointment-3.5.0/appointment/static/img/email_hd_bg.jpg`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/js/app_admin/staff_index.js` & `django_appointment-3.5.0/appointment/static/js/app_admin/staff_index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -600,14 +600,17 @@
 }
 
 async function showCreateAppointmentModal(defaultStartTime, formattedDate) {
     const servicesDropdown = await populateServices(null, false);
     let staffDropdown = null;
     if (isUserSuperUser) {
         staffDropdown = await populateStaffMembers(null, false);
+        staffDropdown.id = "staffSelect";
+        staffDropdown.disabled = false; // Enable dropdown
+        attachEventListenersToDropdown(); // Attach event listener
     }
     servicesDropdown.id = "serviceSelect";
     servicesDropdown.disabled = false; // Enable dropdown
 
     document.getElementById('eventModalBody').innerHTML = prepareCreateAppointmentModalContent(servicesDropdown, staffDropdown, defaultStartTime, formattedDate);
 
     adjustCreateAppointmentModalButtons();
@@ -674,14 +677,15 @@
     const appointment = await getAppointmentData(eventId, isCreatingMode, defaultStartTime);
     if (!appointment) return;
 
     const servicesDropdown = await getServiceDropdown(appointment.service_id, isEditMode);
     let staffDropdown = null;
     if (isUserSuperUser) {
         staffDropdown = await getStaffDropdown(appointment.staff_id, isEditMode);
+        attachEventListenersToDropdown(); // Attach event listener
     }
 
     document.getElementById('eventModalBody').innerHTML = generateModalContent(appointment, servicesDropdown, isEditMode, staffDropdown);
     adjustModalButtonsVisibility(isEditMode, isCreatingMode);
     $('#eventDetailsModal').modal('show');
 }
 
@@ -779,22 +783,34 @@
 
 }
 
 // Collect form data from modal
 function collectFormDataFromModal(modal) {
     const inputs = modal.querySelectorAll("input");
     const serviceId = modal.querySelector("#serviceSelect").value;
-    const staffId = modal.querySelector("#staffSelect").value;
+    let staffId = null;
+
+    if (isUserSuperUser) {
+        // If the user is a superuser, get the staff ID from the dropdown
+        const staffDropdown = modal.querySelector("#staffSelect");
+        if (staffDropdown) {
+            staffId = staffDropdown.value;
+        }
+    }
+
     const data = {
         isCreating: AppState.isCreating,
         service_id: serviceId,
-        staff_id: staffId,
         appointment_id: AppState.eventIdSelected
     };
 
+    if (staffId) {
+        data.staff_id = staffId;
+    }
+
     inputs.forEach(input => {
         if (input.name !== "date") {
             let key = input.name.replace(/([A-Z])/g, '_$1').toLowerCase();
             data[key] = input.value;
         }
     });
```

### Comparing `django-appointment-3.4.1/appointment/static/js/appointments.js` & `django_appointment-3.5.0/appointment/static/js/appointments.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -247,15 +247,15 @@
         // Optionally disable the "submit" button here
         $('.btn-submit-appointment').attr('disabled', 'disabled');
         return; // Exit the function early
     }
 
     let ajaxData = {
         'selected_date': selectedDate,
-        'staff_id': staffId,
+        'staff_member': staffId,
     };
     fetchNonWorkingDays(staffId, function(nonWorkingDays) {
         // Check if nonWorkingDays is an array
         if (Array.isArray(nonWorkingDays)) {
             // Update the FullCalendar configuration
             // calendar.setOption('hiddenDays', nonWorkingDays);
         } else {
@@ -341,15 +341,15 @@
 
 function requestNextAvailableSlot(serviceId) {
     const requestNextAvailableSlotURL = requestNextAvailableSlotURLTemplate.replace('0', serviceId);
     if (staffId === null) {
         return;
     }
     let ajaxData = {
-        'staff_id': staffId,
+        'staff_member': staffId,
     };
     $.ajax({
         url: requestNextAvailableSlotURL,
         data: ajaxData,
         dataType: 'json',
         success: function(data) {
             // If there's an error, just log it and return
```

### Comparing `django-appointment-3.4.1/appointment/static/js/modal/error_modal.js` & `django_appointment-3.5.0/appointment/static/js/modal/error_modal.js`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/static/js/modal/show_modal.js` & `django_appointment-3.5.0/appointment/static/js/modal/show_modal.js`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/tasks.py` & `django_appointment-3.5.0/appointment/tasks.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/administration/display_appointment.html` & `django_appointment-3.5.0/appointment/templates/administration/display_appointment.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/administration/email_change_verification_code.html` & `django_appointment-3.5.0/appointment/templates/administration/email_change_verification_code.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/administration/manage_day_off.html` & `django_appointment-3.5.0/appointment/templates/administration/manage_day_off.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/administration/manage_service.html` & `django_appointment-3.5.0/appointment/templates/administration/manage_service.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/administration/manage_staff_member.html` & `django_appointment-3.5.0/appointment/templates/administration/manage_staff_member.html`

 * *Files 17% similar despite different names*

```diff
@@ -6,42 +6,59 @@
     <link rel="stylesheet" type="text/css" href="{% static 'css/app_admin/staff_member.css' %}"/>
 {% endblock %}
 
 {% block body %}
     <section class="content content-wrapper">
         <div class="staff-form-wrapper">
             <div class="staff-form-content">
-                <h2>{% trans 'Staff Appointment Information' %}</h2>
+                <h3>{% trans 'Staff Appointment Information' %}</h3>
                 <form method="post">
                     {% csrf_token %}
+                    {% if form.user %}
+                        <div class="form-group">
+                            {{ form.user.label_tag }}
+                            {{ form.user.errors }}
+                            {{ form.user }}
+                        </div>
+                        <div class="user-not-found">
+                            <small>
+                                {% translate 'User not found' %} ? <a href="{% url 'appointment:add_staff_member_personal_info' %}">{% translate 'Create staff member manually' %}</a>
+                            </small>
+                        </div>
+                    {% endif %}
 
                     <div class="form-group">
                         {{ form.services_offered.label_tag }}
                         {{ form.services_offered.errors }}
                         {{ form.services_offered }}
+                        <br><small>{% trans 'Hold down “Control”, or “Command” on a Mac, to select more than one.' %}</small>
                     </div>
 
                     <div class="form-group">
-                        {{ form.slot_duration.label_tag }}
+                        {{ form.slot_duration.label_tag }} 
                         {{ form.slot_duration }}
+                        <small>{{ form.slot_duration.help_text }}</small>
                     </div>
 
                     <div class="form-group">
                         {{ form.lead_time.label_tag }}
                         {{ form.lead_time }}
+                        <small>{{ form.lead_time.help_text }}</small>
                     </div>
 
                     <div class="form-group">
                         {{ form.finish_time.label_tag }}
                         {{ form.finish_time }}
+                        <small>{{ form.finish_time.help_text }}</small>
                     </div>
 
                     <div class="form-group">
                         {{ form.appointment_buffer_time.label_tag }}
                         {{ form.appointment_buffer_time }}
+                        <small>{{ form.appointment_buffer_time.help_text }}</small>
                     </div>
 
                     <div class="form-check">
                         {{ form.work_on_saturday }}
                         {{ form.work_on_saturday.label_tag }}
                     </div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,18 +1,28 @@
 {% extends BASE_TEMPLATE %} {% load i18n %} {% load static %} {% block
 customCSS %}
 {% endblock %} {% block body %}
-********** {{%% ttrraannss ''SSttaaffff AAppppooiinnttmmeenntt IInnffoorrmmaattiioonn'' %%}} **********
-{% csrf_token %}
+******** {{%% ttrraannss ''SSttaaffff AAppppooiinnttmmeenntt IInnffoorrmmaattiioonn'' %%}} ********
+{% csrf_token %} {% if form.user %}
+{{ form.user.label_tag }} {{ form.user.errors }} {{ form.user }}
+{% translate 'User not found' %} ? _{_%_ _t_r_a_n_s_l_a_t_e_ _'_C_r_e_a_t_e_ _s_t_a_f_f_ _m_e_m_b_e_r_ _m_a_n_u_a_l_l_y_'
+_%_}
+{% endif %}
 {{ form.services_offered.label_tag }} {{ form.services_offered.errors }} {
 { form.services_offered }}
-{{ form.slot_duration.label_tag }} {{ form.slot_duration }}
-{{ form.lead_time.label_tag }} {{ form.lead_time }}
-{{ form.finish_time.label_tag }} {{ form.finish_time }}
+{% trans 'Hold down âControlâ, or âCommandâ on a Mac, to select more
+than one.' %}
+{{ form.slot_duration.label_tag }} {{ form.slot_duration }} {
+{ form.slot_duration.help_text }}
+{{ form.lead_time.label_tag }} {{ form.lead_time }} {{ form.lead_time.help_text
+}}
+{{ form.finish_time.label_tag }} {{ form.finish_time }} {
+{ form.finish_time.help_text }}
 {{ form.appointment_buffer_time.label_tag }} {{ form.appointment_buffer_time }}
+{{ form.appointment_buffer_time.help_text }}
 {{ form.work_on_saturday }} {{ form.work_on_saturday.label_tag }}
 {{ form.work_on_sunday }} {{ form.work_on_sunday.label_tag }}
 {% trans 'Save' %}
 {% if messages %} {% for message in messages %}
 {{ message }}
 {% endfor %} {% endif %}
 {% endblock %} {% block customJS %}
```

### Comparing `django-appointment-3.4.1/appointment/templates/administration/manage_staff_personal_info.html` & `django_appointment-3.5.0/appointment/templates/administration/manage_staff_personal_info.html`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     <link rel="stylesheet" type="text/css" href="{% static 'css/app_admin/staff_member.css' %}"/>
 {% endblock %}
 
 {% block body %}
     <section class="content content-wrapper">
         <div class="staff-form-wrapper">
             <div class="staff-form-content">
-                <h2>{% trans 'Staff Personal Information' %}</h2>
+                <h3>{% trans 'Staff Personal Information' %}</h3>
                 <form id="updatePersonalInfoForm" method="post" action="">
                     {% csrf_token %}
 
                     <div class="form-group">
                         {{ form.first_name.label_tag }}
                         {{ form.first_name }}
                     </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends BASE_TEMPLATE %} {% load i18n %} {% load static %} {% block
 customCSS %}
 {% endblock %} {% block body %}
-********** {{%% ttrraannss ''SSttaaffff PPeerrssoonnaall IInnffoorrmmaattiioonn'' %%}} **********
+******** {{%% ttrraannss ''SSttaaffff PPeerrssoonnaall IInnffoorrmmaattiioonn'' %%}} ********
 {% csrf_token %}
 {{ form.first_name.label_tag }} {{ form.first_name }}
 {{ form.last_name.label_tag }} {{ form.last_name }}
 {{ form.email.label_tag }} {{ form.email }}
 {{ btn_text }}
 {% if messages %} {% for message in messages %}
 {{ message }}
```

### Comparing `django-appointment-3.4.1/appointment/templates/administration/manage_working_hours.html` & `django_appointment-3.5.0/appointment/templates/administration/manage_working_hours.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/administration/service_list.html` & `django_appointment-3.5.0/appointment/templates/administration/service_list.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/administration/staff_index.html` & `django_appointment-3.5.0/appointment/templates/administration/staff_index.html`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
     <script src="{% static 'js/modal/show_modal.js' %}"></script>
     <script src="{% static 'js/js-utils.js' %}"></script>
 
     <script>
         function createCommonInputFields(appointment, servicesDropdown, isEditMode, defaultStartTime, staffDropdown) {
             const startTimeValue = isEditMode ? moment(appointment.start_time).format('HH:mm:ss') : defaultStartTime;
             const disabledAttribute = isEditMode ? '' : 'disabled';
-            
+
             let superuserInputField = '';
             if (isUserSuperUser) {
                 superuserInputField = `
                     <div class="flex-container-appt">
                     <label>{% trans 'Staff Member' %}:</label>
                     ${staffDropdown.outerHTML}
                     </div>
```

### Comparing `django-appointment-3.4.1/appointment/templates/administration/staff_list.html` & `django_appointment-3.5.0/appointment/templates/administration/staff_list.html`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 <div class="section-header">
                     <h2 class="section-header-itm">{% trans 'Staff Members' %}</h2>
                     <div class="buttons-container section-header-itm">
                         <a href="{{ btn_staff_me_link }}"
                            class="modify-btn button-color-purple">
                             {{ btn_staff_me }}
                         </a>
-                        <a href="{% url 'appointment:add_staff_member_personal_info' %}"
+                        <a href="{% url 'appointment:add_staff_member_info' %}"
                            class="modify-btn button-color-green">
                             <i class="fas fa-add"></i>
                         </a>
                     </div>
                 </div>
                 <div class="responsive-table-container">
                     <table>
@@ -39,16 +39,16 @@
                             <th>{% trans 'Email' %}</th>
                             <th>{% trans 'Details' %}</th>
                         </tr>
                         </thead>
                         <tbody>
                         {% for staff_member in staff_members %}
                             <tr>
-                                <td>{{ staff_member.user.first_name }} {{ staff_member.user.last_name }}</td>
-                                <td>{{ staff_member.user.email }}</td>
+                                <td>{{ staff_member.get_staff_member_name }}</td>
+                                <td>{{ staff_member.user.email|default:"N/A" }}</td>
                                 <td>
                                     <a href="{% url 'appointment:user_profile' staff_member.user.id %}"
                                        class="modify-btn button-color-blue">{% trans 'View Profile' %}</a>
                                     <a href="{% url 'appointment:remove_staff_member' staff_member.user.id %}"
                                        class="modify-btn button-color-red">{% trans 'Remove' %}</a>
                                 </td>
                             </tr>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 {% extends BASE_TEMPLATE %} {% load i18n %} {% load static %} {% block
 customCSS %}
 {% endblock %} {% block title %} Staff Members List {% endblock %} {% block
 description %} {% trans 'List of all staff members' %}. {% endblock %} {% block
 body %}
 ********** {{%% ttrraannss ''SSttaaffff MMeemmbbeerrss'' %%}} **********
 _{_{_ _b_t_n___s_t_a_f_f___m_e_ _}_}
-{{%% ttrraannss ''NNaammee'' %%}}           {{%% ttrraannss ''EEmmaaiill'' %%}}       {{%% ttrraannss ''DDeettaaiillss'' %%}}
-{
-{
-staff_member.user.first_name {                         _{_%_ _t_r_a_n_s_ _'_V_i_e_w_ _P_r_o_f_i_l_e_'
-}} {                         { staff_member.user.email _%_} _{_%_ _t_r_a_n_s_ _'_R_e_m_o_v_e_'_ _%_}
-{                            }}
-staff_member.user.last_name
-}}
+                                                                    {{%% ttrraannss
+{{%% ttrraannss ''NNaammee'' %%}}                 {{%% ttrraannss ''EEmmaaiill'' %%}}              ''DDeettaaiillss''
+                                                                    %%}}
+{                                  {                                _{_%_ _t_r_a_n_s
+{                                  {                                _'_V_i_e_w
+staff_member.get_staff_member_name staff_member.user.email|default: _P_r_o_f_i_l_e_'_ _%_}
+}}                                 "N/A" }}                         _{_%_ _t_r_a_n_s
+                                                                    _'_R_e_m_o_v_e_'_ _%_}
 {% trans 'No staff members found' %}.
 {% if messages %} {% for message in messages %}
 {{ message }}
 {% endfor %} {% endif %}
 {% endblock %} {% block customJS %}
 {% endblock %}
```

### Comparing `django-appointment-3.4.1/appointment/templates/administration/user_profile.html` & `django_appointment-3.5.0/appointment/templates/administration/user_profile.html`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
             <section class="profile-section">
                 {% translate "Confirm Deletion" as modal_title %}
                 {% translate "Delete" as delete_btn_modal %}
 
                 <h2>{% trans 'Personal Information' %}</h2>
                 <!-- Display fields from PersonalInformationForm -->
                 <div class="section-content">
-                    <p><strong>{% trans 'First name' %}:</strong> {{ user.first_name }}</p>
-                    <p><strong>{% trans 'Last name' %}:</strong> {{ user.last_name }}</p>
-                    <p><strong>{% trans 'Email' %}:</strong> {{ user.email }}</p>
+                    <p><strong>{% trans 'First name' %}:</strong> {{ user.first_name|default:user.username }}</p>
+                    <p><strong>{% trans 'Last name' %}:</strong> {{ user.last_name|default:"N/A" }}</p>
+                    <p><strong>{% trans 'Email' %}:</strong> {{ user.email|default:"N/A" }}</p>
                 </div>
                 <a href="{% url 'appointment:update_user_info' user.id %}"
                    class="section-content-button modify-btn button-color-blue">
                     <i class="fas fa-pen"></i>
                 </a>
             </section>
 
@@ -238,15 +238,15 @@
                             <th>{% trans 'Down payment' %}</th>
                         </tr>
                         </thead>
                         <tbody>
                         {% for service in services_offered %}
                             <tr>
                                 <td>{{ service.name }}</td>
-                                <td>{{ service.description }}</td>
+                                <td>{{ service.description|default:"N/A" }}</td>
                                 <td>{{ service.get_duration }}</td>
                                 <td>{{ service.get_price_text }}</td>
                                 <td>{{ service.get_down_payment_text }}</td>
                             </tr>
                         {% empty %}
                             <tr>
                                 <td colspan="5">{% trans 'No service offered yet' %}.</td>
```

#### html2text {}

```diff
@@ -4,17 +4,17 @@
 description %} {{ page_description }} {% endblock %} {% block body %}
 {% if messages %} {% for message in messages %}
 {{ message }}
 {% endfor %} {% endif %}
 {% translate "Confirm Deletion" as modal_title %} {% translate "Delete" as
 delete_btn_modal %}
 ********** {{%% ttrraannss ''PPeerrssoonnaall IInnffoorrmmaattiioonn'' %%}} **********
-{{%% ttrraannss ''FFiirrsstt nnaammee'' %%}}:: {{ user.first_name }}
-{{%% ttrraannss ''LLaasstt nnaammee'' %%}}:: {{ user.last_name }}
-{{%% ttrraannss ''EEmmaaiill'' %%}}:: {{ user.email }}
+{{%% ttrraannss ''FFiirrsstt nnaammee'' %%}}:: {{ user.first_name|default:user.username }}
+{{%% ttrraannss ''LLaasstt nnaammee'' %%}}:: {{ user.last_name|default:"N/A" }}
+{{%% ttrraannss ''EEmmaaiill'' %%}}:: {{ user.email|default:"N/A" }}
 ********** {{%% ttrraannss ''AAppppooiinnttmmeenntt IInnffoorrmmaattiioonn'' %%}} **********
 {{ service_msg }} {% if staff_member %}
 {{%% ttrraannss ''SSlloott dduurraattiioonn'' %%}}:: {{ staff_member.get_slot_duration_text }}
 {{%% ttrraannss ''GGeenneerraall ssttaarrtt ttiimmee'' %%}}:: {{ staff_member.get_lead_time }}
 {{%% ttrraannss ''GGeenneerraall eenndd ttiimmee'' %%}}:: {{ staff_member.get_finish_time }}
 {{%% ttrraannss ''WWeeeekkeenndd ddaayyss yyoouu wwoorrkk'' %%}}:: {
 { staff_member.get_weekend_days_worked_text }}
@@ -58,16 +58,16 @@
                                                                                            else %} {%
                                                                                            endif %}
 {% trans 'No working hours have been set' %}.
 ********** {{%% ttrraannss ''SSeerrvviiccee OOffffeerreedd'' %%}} **********
 {% if not superuser %} {% trans "To add/modify a new service, make a request to
 an admin." %} {% trans "Changes made in one service will change it for every
 staff member." %} {% endif %}
-{{%% ttrraannss     {{%% ttrraannss            {{%% ttrraannss ''DDuurraattiioonn''  {{%% ttrraannss ''PPrriiccee'' %%}}    {{%% ttrraannss ''DDoowwnn ppaayymmeenntt'' %%}}
-''NNaammee'' %%}}    ''DDeessccrriippttiioonn'' %%}}    %%}}
-{            {                   {                    {                      {
-{            {                   {                    {                      {
-service.name service.description service.get_duration service.get_price_text service.get_down_payment_text
-}}           }}                  }}                   }}                     }}
+{{%% ttrraannss     {{%% ttrraannss ''DDeessccrriippttiioonn'' %%}}    {{%% ttrraannss ''DDuurraattiioonn''  {{%% ttrraannss ''PPrriiccee'' %%}}    {{%% ttrraannss ''DDoowwnn ppaayymmeenntt'' %%}}
+''NNaammee'' %%}}                                 %%}}
+{            {                            {                    {                      {
+{            {                            {                    {                      {
+service.name service.description|default: service.get_duration service.get_price_text service.get_down_payment_text
+}}           "N/A" }}                     }}                   }}                     }}
 {% trans 'No service offered yet' %}.
 {% include 'modal/confirm_modal.html' %} {% endblock %} {% block customJS %}
 {% endblock %}
```

### Comparing `django-appointment-3.4.1/appointment/templates/appointment/appointment_client_information.html` & `django_appointment-3.5.0/appointment/templates/appointment/appointment_client_information.html`

 * *Files 4% similar despite different names*

```diff
@@ -40,22 +40,19 @@
                             <div class="already-have-account">
                                 <div>
                                     {% trans 'Already have an account?' %}
                                     <a href="#">{% trans 'Log in' %}</a> {% trans 'for faster booking.' %}
                                 </div>
                             </div>
                             <div class="name-email">
-                                <label for="name" class="name">{% trans "Full Name" %} *<br>
-                                    <input type="text" placeholder="John DOE" id="name" class="client-name"
-                                           maxlength="100" minlength="3" required name="name">
+                                <label for="{{ form.name.id_for_label }}" class="name">{% trans "Full Name" %} *<br>
+                                    {{ client_data_form.name }}
                                 </label>
-                                <label for="email" class="email">{% trans "Email" %} *<br>
-                                    <input type="email" placeholder="john.doe@email.com" id="email"
-                                           class="client-email" name="email"
-                                           maxlength="100" required>
+                                <label for="{{ form.email.id_for_label }}" class="email">{% trans "Email" %} *<br>
+                                    {{ client_data_form.email }}
                                 </label>
                             </div>
                             <div class="receive-email">
                                 <label for="{{ form.want_reminder.id_for_label }}">
                                     {{ form.want_reminder }}
                                     {% trans "I want to receive an EMAIL reminder 24 hours before this session starts" %}
                                 </label>
```

### Comparing `django-appointment-3.4.1/appointment/templates/appointment/appointments.html` & `django_appointment-3.5.0/appointment/templates/appointment/appointments.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/appointment/default_thank_you.html` & `django_appointment-3.5.0/appointment/templates/appointment/default_thank_you.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/appointment/enter_verification_code.html` & `django_appointment-3.5.0/appointment/templates/appointment/enter_verification_code.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/appointment/rescheduling_thank_you.html` & `django_appointment-3.5.0/appointment/templates/appointment/rescheduling_thank_you.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/appointment/set_password.html` & `django_appointment-3.5.0/appointment/templates/appointment/set_password.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/appointment/thank_you.html` & `django_appointment-3.5.0/appointment/templates/appointment/thank_you.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/base_templates/base.html` & `django_appointment-3.5.0/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/email_sender/admin_new_appointment_email.html` & `django_appointment-3.5.0/appointment/templates/email_sender/admin_new_appointment_email.html`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     <div class="appointment-details">
         <p><strong>{% translate 'Client Name' %}:</strong> {{ client_name }}</p>
         <p><strong>{% translate 'Service Requested' %}:</strong> {{ appointment.get_service_name }}</p>
         <p><strong>{% translate 'Appointment Date' %}:</strong> {{ appointment.appointment_request.date }}</p>
         <p><strong>{% translate 'Time' %}:</strong> {{ appointment.appointment_request.start_time }}
             - {{ appointment.appointment_request.end_time }}</p>
-        <p><strong>{% translate 'Contact Details' %}:</strong> {{ appointment.phone }} | {{ client_email }}</p>
+        <p><strong>{% translate 'Contact Details' %}:</strong> {{ appointment.phone }} | {{ appointment.client.email }}</p>
         <p><strong>{% translate 'Additional Info' %}:</strong> {{ appointment.additional_info|default:"N/A" }}</p>
     </div>
 
     <p>{% translate 'Please review the appointment request and take the necessary action.' %}</p>
 
     <div class="footer">
         <p>{% translate 'This is an automated message. Please do not reply directly to this email.' %}</p>
```

#### html2text {}

```diff
@@ -4,14 +4,15 @@
 {% translate 'You have received a new appointment request. Here are the
 details:' %}
 {{%% ttrraannssllaattee ''CClliieenntt NNaammee'' %%}}:: {{ client_name }}
 {{%% ttrraannssllaattee ''SSeerrvviiccee RReeqquueesstteedd'' %%}}:: {{ appointment.get_service_name }}
 {{%% ttrraannssllaattee ''AAppppooiinnttmmeenntt DDaattee'' %%}}:: {{ appointment.appointment_request.date }}
 {{%% ttrraannssllaattee ''TTiimmee'' %%}}:: {{ appointment.appointment_request.start_time }} - {
 { appointment.appointment_request.end_time }}
-{{%% ttrraannssllaattee ''CCoonnttaacctt DDeettaaiillss'' %%}}:: {{ appointment.phone }} | {{ client_email }}
+{{%% ttrraannssllaattee ''CCoonnttaacctt DDeettaaiillss'' %%}}:: {{ appointment.phone }} | {
+{ appointment.client.email }}
 {{%% ttrraannssllaattee ''AAddddiittiioonnaall IInnffoo'' %%}}:: {{ appointment.additional_info|default:"N/A"
 }}
 {% translate 'Please review the appointment request and take the necessary
 action.' %}
 {% translate 'This is an automated message. Please do not reply directly to
 this email.' %}
```

### Comparing `django-appointment-3.4.1/appointment/templates/email_sender/reminder_email.html` & `django_appointment-3.5.0/appointment/templates/email_sender/reminder_email.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/email_sender/reschedule_email.html` & `django_appointment-3.5.0/appointment/templates/email_sender/reschedule_email.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/email_sender/thank_you_email.html` & `django_appointment-3.5.0/appointment/templates/email_sender/thank_you_email.html`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
                         <tr>
                     {% endif %}
                 </tr>
                     <tr>
                         <td align="left" valign="top"
                             style="font-family: Open Sans, Helvetica, Arial, sans-serif; padding-top: 0;">
                             <h3>{% trans "Account Information" %}</h3>
-                            <div style="color: #000000; font-size: 14px; line-height: 24px; margin-top: -30px !important;">
+                            <div style="color: #000000; font-size: 14px; line-height: 24px;">
                                 <ul>
                                     {% for key, value in account_details.items %}
                                         <li>{{ key }}: {{ value }}</li>
                                     {% endfor %}
                                 </ul>
                             </div>
 
@@ -207,15 +207,15 @@
                     </tr>
                 {% endif %}
                 {% if more_details %}
                     <tr>
                         <td align="left" valign="top"
                             style="font-family: Open Sans, Helvetica, Arial, sans-serif; padding-top: 0;">
                             <h3>{% trans "Appointment Details" %}</h3>
-                            <div style="color: #000000; font-size: 14px; line-height: 24px; margin-top: -30px !important;">
+                            <div style="color: #000000; font-size: 14px; line-height: 24px;">
                                 <ul>
                                     {% for key, value in more_details.items %}
                                         <li>{{ key }}: {{ value }}</li>
                                     {% endfor %}
                                 </ul>
                             </div>
```

### Comparing `django-appointment-3.4.1/appointment/templates/error_pages/304_already_submitted.html` & `django_appointment-3.5.0/appointment/templates/error_pages/304_already_submitted.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/error_pages/403_forbidden.html` & `django_appointment-3.5.0/appointment/templates/error_pages/403_forbidden.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/error_pages/403_forbidden_rescheduling.html` & `django_appointment-3.5.0/appointment/templates/error_pages/403_forbidden_rescheduling.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/error_pages/404_not_found.html` & `django_appointment-3.5.0/appointment/templates/error_pages/404_not_found.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/modal/confirm_modal.html` & `django_appointment-3.5.0/appointment/templates/modal/confirm_modal.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/modal/error_modal.html` & `django_appointment-3.5.0/appointment/templates/modal/error_modal.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/templates/modal/event_details_modal.html` & `django_appointment-3.5.0/appointment/templates/modal/event_details_modal.html`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/tests/base/base_test.py` & `django_appointment-3.5.0/appointment/tests/test_tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,52 @@
-from datetime import timedelta
+# test_tasks.py
+# Path: appointment/tests/test_tasks.py
 
-from django.test import TestCase
+from unittest.mock import patch
 
-from appointment.tests.mixins.base_mixin import (
-    AppointmentMixin, AppointmentRequestMixin, AppointmentRescheduleHistoryMixin, ServiceMixin, StaffMemberMixin,
-    UserMixin
-)
-
-
-class BaseTest(TestCase, UserMixin, StaffMemberMixin, ServiceMixin, AppointmentRequestMixin, AppointmentMixin,
-               AppointmentRescheduleHistoryMixin):
-    def setUp(self):
-        # Users
-        self.user1 = self.create_user_(email="tester1@gmail.com", username="tester1")
-        self.user2 = self.create_user_(first_name="Tester2", email="tester2@gmail.com", username="tester2")
-        self.client1 = self.create_user_(first_name="Client1", email="client1@gmail.com", username="client1")
-        self.client2 = self.create_user_(first_name="Client2", email="client2@gmail.com", username="client2")
-
-        # Services
-        self.service1 = self.create_service_()
-        self.service2 = self.create_service_(name="Service 2")
-
-        # Staff Members
-        self.staff_member1 = self.create_staff_member_(user=self.user1, service=self.service1)
-        self.staff_member2 = self.create_staff_member_(user=self.user2, service=self.service2)
-
-    def create_appt_request_for_sm1(self, **kwargs):
-        """Create an appointment request for staff_member1."""
-        return self.create_appointment_request_(service=self.service1, staff_member=self.staff_member1, **kwargs)
-
-    def create_appt_request_for_sm2(self, **kwargs):
-        """Create an appointment request for staff_member2."""
-        return self.create_appointment_request_(service=self.service2, staff_member=self.staff_member2, **kwargs)
-
-    def create_appointment_for_user1(self, appointment_request=None):
-        if not appointment_request:
-            appointment_request = self.create_appt_request_for_sm1()
-        return self.create_appointment_(user=self.client1, appointment_request=appointment_request)
-
-    def create_appointment_for_user2(self, appointment_request=None):
-        if not appointment_request:
-            appointment_request = self.create_appt_request_for_sm2()
-        return self.create_appointment_(user=self.client2, appointment_request=appointment_request)
-
-    def create_appointment_reschedule_for_user1(self, appointment_request=None, reason_for_rescheduling="Reason"):
-        if not appointment_request:
-            appointment_request = self.create_appt_request_for_sm1()
-        date_ = appointment_request.date + timedelta(days=1)
-        return self.create_reschedule_history_(
-            appointment_request=appointment_request,
-            date_=date_,
-            start_time=appointment_request.start_time,
-            end_time=appointment_request.end_time,
-            staff_member=appointment_request.staff_member,
-            reason_for_rescheduling=reason_for_rescheduling,
+from django.utils.translation import gettext as _
+
+from appointment.tasks import send_email_reminder
+from appointment.tests.base.base_test import BaseTest
+
+
+class SendEmailReminderTest(BaseTest):
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    @patch('appointment.tasks.send_email')
+    @patch('appointment.tasks.notify_admin')
+    def test_send_email_reminder(self, mock_notify_admin, mock_send_email):
+        # Use BaseTest setup to create an appointment
+        appointment_request = self.create_appt_request_for_sm1()
+        appointment = self.create_appt_for_sm1(appointment_request=appointment_request)
+
+        # Extract necessary data for the test
+        to_email = appointment.client.email
+        first_name = appointment.client.first_name
+        appointment_id = appointment.id
+
+        # Call the function under test
+        send_email_reminder(to_email, first_name, "", appointment_id)
+
+        # Verify send_email was called with correct parameters
+        mock_send_email.assert_called_once_with(
+            recipient_list=[to_email],
+            subject=_("Reminder: Upcoming Appointment"),
+            template_url='email_sender/reminder_email.html',
+            context={'first_name': first_name, 'appointment': appointment, 'reschedule_link': "",
+                     'recipient_type': 'admin'}
+        )
+
+        # Verify notify_admin was called with correct parameters
+        mock_notify_admin.assert_called_once_with(
+            subject=_("Admin Reminder: Upcoming Appointment"),
+            template_url='email_sender/reminder_email.html',
+            context={'first_name': first_name, 'appointment': appointment, 'reschedule_link': "",
+                     'recipient_type': 'admin'}
         )
```

### Comparing `django-appointment-3.4.1/appointment/tests/mixins/base_mixin.py` & `django_appointment-3.5.0/appointment/tests/mixins/base_mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 
 
 class UserMixin:
     def __init__(self):
         pass
 
     @classmethod
-    def create_user_(cls, first_name="Tester", email="testemail@gmail.com", username="test_user",
-                     password="Kfdqi3!?n"):
-        user_model = get_user_model()
-        return user_model.objects.create_user(
+    def create_user_(cls, first_name="Janet", email="janet.fraiser@django-appointment.com", username="janet.fraiser",
+                     password="G0a'uld$Emp1re"):
+        return get_user_model().objects.create_user(
             first_name=first_name,
             email=email,
             username=username,
             password=password
         )
 
 
 class ServiceMixin:
     def __init__(self):
         pass
 
     @classmethod
-    def create_service_(cls, name="Test Service", duration=timedelta(hours=1), price=100):
+    def create_service_(cls, name="Quantum Mirror Assessment", duration=timedelta(hours=1), price=50000,
+                        description="Assess the Quantum Mirror"):
         return Service.objects.create(
             name=name,
             duration=duration,
-            price=price
+            price=price,
+            description=description
         )
 
 
 class StaffMemberMixin:
     def __init__(self):
         pass
 
@@ -57,36 +58,45 @@
             date=date_,
             start_time=start_time,
             end_time=end_time,
             service=service,
             staff_member=staff_member
         )
 
+    @classmethod
+    def clean_appt_request_for_user_(cls, user):
+        AppointmentRequest.objects.filter(staff_member__user=user).delete()
+
 
 class AppointmentMixin:
     def __init__(self):
         pass
 
     @classmethod
-    def create_appointment_(cls, user, appointment_request, phone="1234567890", address="Some City, Some State"):
+    def create_appointment_(cls, user, appointment_request, phone="+12392340543",
+                            address="Stargate Command, Cheyenne Mountain Complex, Colorado Springs, CO"):
         return Appointment.objects.create(
             client=user,
             appointment_request=appointment_request,
             phone=phone,
             address=address
         )
 
+    @classmethod
+    def clean_appointment_for_user_(cls, user):
+        Appointment.objects.filter(client=user).delete()
+
 
 class AppointmentRescheduleHistoryMixin:
     def __init__(self):
         pass
 
     @classmethod
     def create_reschedule_history_(cls, appointment_request, date_, start_time, end_time, staff_member,
-                                   reason_for_rescheduling=""):
+                                   reason_for_rescheduling="Zat'nik'tel Discharge"):
         return AppointmentRescheduleHistory.objects.create(
             appointment_request=appointment_request,
             date=date_,
             start_time=start_time,
             end_time=end_time,
             staff_member=staff_member,
             reason_for_rescheduling=reason_for_rescheduling
```

### Comparing `django-appointment-3.4.1/appointment/tests/models/test_model_appointment.py` & `django_appointment-3.5.0/appointment/tests/models/test_appointment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,249 +1,115 @@
+from copy import deepcopy
 from datetime import datetime, time, timedelta
 
 from django.core.exceptions import ValidationError
-from django.db import IntegrityError
 from django.utils import timezone
+from django.utils.translation import gettext as _
 
 from appointment.models import Appointment, DayOff, WorkingHours
 from appointment.tests.base.base_test import BaseTest
 from appointment.utils.date_time import get_weekday_num
 
 
-class AppointmentModelTestCase(BaseTest):
+class AppointmentCreationTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
-        super().setUp()
+        self.address = 'Stargate Command, Cheyenne Mountain Complex, Colorado Springs, CO'
         self.ar = self.create_appt_request_for_sm1()
-        self.appointment = self.create_appointment_for_user1(appointment_request=self.ar)
-
-    # Test appointment creation
-    def test_appointment_creation(self):
-        """Test if an appointment can be created."""
-        appointment = Appointment.objects.get(appointment_request=self.ar)
-        self.assertIsNotNone(appointment)
-        self.assertEqual(appointment.client, self.client1)
-        self.assertEqual(appointment.phone, "1234567890")
-        self.assertEqual(appointment.address, "Some City, Some State")
+        self.appointment = self.create_appt_for_sm1(appointment_request=self.ar)
+        self.client_ = self.users['client1']
+        self.expected_end_time = datetime.combine(self.ar.date, self.ar.end_time)
+        self.expected_service_name = 'Stargate Activation'
+        self.expected_service_price = 100000
+        self.expected_start_time = datetime.combine(self.ar.date, self.ar.start_time)
+        self.phone = '+12392340543'
+        return super().setUp()
+
+    def tearDown(self):
+        self.appointment.delete()
+        return super().tearDown()
+
+    def test_default_attributes_on_creation(self):
+        """Test default attributes when an appointment is created."""
+        self.assertIsNotNone(self.appointment)
+        self.assertIsNotNone(self.appointment.created_at)
+        self.assertIsNotNone(self.appointment.updated_at)
+        self.assertIsNotNone(self.appointment.get_appointment_id_request())
+        self.assertIsNone(self.appointment.additional_info)
+        self.assertEqual(self.appointment.client, self.users['client1'])
+        self.assertEqual(self.appointment.phone, self.phone)
+        self.assertEqual(self.appointment.address, self.address)
+        self.assertFalse(self.appointment.want_reminder)
 
-    # Test str representation
     def test_str_representation(self):
         """Test if an appointment's string representation is correct."""
-        expected_str = f"{self.client1} - {self.ar.start_time.strftime('%Y-%m-%d %H:%M')} to " \
+        expected_str = f"{self.client_} - {self.ar.start_time.strftime('%Y-%m-%d %H:%M')} to " \
                        f"{self.ar.end_time.strftime('%Y-%m-%d %H:%M')}"
         self.assertEqual(str(self.appointment), expected_str)
 
-    # Test start time
-    def test_get_start_time(self):
-        """Test if an appointment's start time is correct."""
-        expected_start_time = datetime.combine(self.ar.date,
-                                               self.ar.start_time)
-        self.assertEqual(self.appointment.get_start_time(), expected_start_time)
-
-    # Test end time
-    def test_get_end_time(self):
-        """Test if an appointment's end time is correct."""
-        expected_end_time = datetime.combine(self.ar.date,
-                                             self.ar.end_time)
-        self.assertEqual(self.appointment.get_end_time(), expected_end_time)
-
-    # Test service name retrieval
-    def test_get_service_name(self):
-        """Test if an appointment's service name is correct."""
-        self.assertEqual(self.appointment.get_service_name(), "Test Service")
-
-    # Test service price retrieval
-    def test_get_service_price(self):
-        """Test if an appointment's service price is correct."""
-        self.assertEqual(self.appointment.get_service_price(), 100)
-
-    # Test phone retrieval
-    def test_get_phone(self):
-        """Test if an appointment's phone number is correct."""
-        self.assertEqual(self.appointment.phone, "1234567890")
-
-    # Test address retrieval
-    def test_get_address(self):
-        """Test if an appointment's address is correct."""
-        self.assertEqual(self.appointment.address, "Some City, Some State")
-
-    # Test reminder retrieval
-    def test_get_want_reminder(self):
-        """Test if an appointment's reminder status is correct."""
-        self.assertFalse(self.appointment.want_reminder)
-
-    # Test additional info retrieval
-    def test_get_additional_info(self):
-        """Test if an appointment's additional info is correct."""
-        self.assertIsNone(self.appointment.additional_info)
-
-    # Test paid status retrieval
-    def test_is_paid(self):
-        """Test if an appointment's paid status is correct."""
-        self.assertFalse(self.appointment.is_paid())
-
-    def test_is_paid_text(self):
-        """Test if an appointment's paid status is correct."""
-        self.assertEqual(self.appointment.is_paid_text(), "No")
-
-    # Test appointment amount to pay
-    def test_get_appointment_amount_to_pay(self):
-        """Test if an appointment's amount to pay is correct."""
-        self.assertEqual(self.appointment.get_appointment_amount_to_pay(), 100)
-
-    # Test appointment currency retrieval
-    def test_get_appointment_currency(self):
-        """Test if an appointment's currency is correct."""
-        self.assertEqual(self.appointment.get_appointment_currency(), "USD")
-
-    # Test appointment ID request retrieval
-    def test_get_appointment_id_request(self):
-        """Test if an appointment's ID request is correct."""
-        self.assertIsNotNone(self.appointment.get_appointment_id_request())
-
-    # Test created at retrieval
-    def test_created_at(self):
-        """Test if an appointment's created at date is correct."""
-        self.assertIsNotNone(self.appointment.created_at)
-
-    # Test updated at retrieval
-    def test_updated_at(self):
-        """Test if an appointment's updated at date is correct."""
-        self.assertIsNotNone(self.appointment.updated_at)
-
-    # Test paid status setting
-    def test_set_appointment_paid_status(self):
-        """Test if an appointment's paid status can be set."""
-        self.appointment.set_appointment_paid_status(True)
-        self.assertTrue(self.appointment.is_paid())
-        self.appointment.set_appointment_paid_status(False)
-        self.assertFalse(self.appointment.is_paid())
-
-    # Test invalid phone number
-    def test_invalid_phone(self):
-        """Test that an appointment cannot be created with an invalid phone number."""
-        self.appointment.phone = "1234"  # Invalid phone number
-        with self.assertRaises(ValidationError):
-            self.appointment.full_clean()
-
-    # Test service down payment retrieval
-    def test_get_service_down_payment(self):
-        """Test if an appointment's service down payment is correct."""
+    def test_appointment_getters(self):
+        """Test getter methods for appointment details."""
+        self.assertEqual(self.appointment.get_start_time(), self.expected_start_time)
+        self.assertEqual(self.appointment.get_end_time(), self.expected_end_time)
+        self.assertEqual(self.appointment.get_service_name(), self.expected_service_name)
+        self.assertEqual(self.appointment.get_service_price(), self.expected_service_price)
+        self.assertEqual(self.appointment.is_paid_text(), _('No'))
+        self.assertEqual(self.appointment.get_appointment_amount_to_pay(), self.expected_service_price)
         self.assertEqual(self.appointment.get_service_down_payment(), self.service1.get_down_payment())
-
-    # Test service description retrieval
-    def test_service_description(self):
-        """Test if an appointment's service description is correct."""
         self.assertEqual(self.appointment.get_service_description(), self.service1.description)
-
-    # Test appointment date retrieval
-    def test_get_appointment_date(self):
-        """Test if an appointment's date is correct."""
         self.assertEqual(self.appointment.get_appointment_date(), self.ar.date)
-
-    # Test save function with down payment type
-    def test_save_with_down_payment(self):
-        """Test if an appointment can be saved with a down payment."""
-        self.ar.payment_type = 'down'
-        self.ar.save()
-        self.appointment.save()
-        self.assertEqual(self.appointment.get_service_down_payment(), self.service1.get_down_payment())
-
-    def test_appointment_without_appointment_request(self):
-        """Test that an appointment cannot be created without an appointment request."""
-        with self.assertRaises(ValidationError):  # Assuming model validation prevents this
-            Appointment.objects.create(client=self.client1)
-
-    def test_appointment_without_client(self):
-        """Test that an appointment cannot be created without a client."""
-        with self.assertRaises(IntegrityError):  # Assuming model validation prevents this
-            Appointment.objects.create(appointment_request=self.ar)
-
-    def test_appointment_amount_to_pay_calculation(self):
-        """
-        Test if an appointment's amount_to_pay field is correctly calculated based on the associated AppointmentRequest.
-        """
+        self.assertEqual(self.appointment.get_service_duration(), "1 hour")
+        self.assertEqual(self.appointment.get_appointment_currency(), "USD")
         self.assertEqual(self.appointment.get_appointment_amount_to_pay(), self.ar.get_service_price())
-
-    def test_update_appointment_paid_status(self):
-        """Simulate appointment's paid status being updated."""
-        self.appointment.set_appointment_paid_status(True)
-        self.assertTrue(self.appointment.is_paid())
-        self.appointment.set_appointment_paid_status(False)
+        self.assertEqual(self.appointment.get_service_img_url(), "")
+        self.assertEqual(self.appointment.get_staff_member_name(), self.staff_member1.get_staff_member_name())
+        self.assertTrue(self.appointment.service_is_paid())
         self.assertFalse(self.appointment.is_paid())
 
-    def test_appointment_rescheduling(self):
-        """Simulate appointment rescheduling by changing the appointment date and times."""
-        new_date = self.ar.date + timedelta(days=1)
-        new_start_time = time(10, 0)
-        new_end_time = time(11, 0)
-        self.ar.date = new_date
-        self.ar.start_time = new_start_time
-        self.ar.end_time = new_end_time
-        self.ar.save()
-
-        self.assertEqual(self.appointment.get_date(), new_date)
-        self.assertEqual(self.appointment.get_start_time().time(), new_start_time)
-        self.assertEqual(self.appointment.get_end_time().time(), new_end_time)
-
-    def test_create_appointment_without_required_fields(self):
-        """Test that an appointment cannot be created without the required fields."""
-        with self.assertRaises(ValidationError):
-            Appointment.objects.create()
-
-    def test_get_service_duration(self):
-        """Test if an appointment's service duration is correct."""
-        self.assertEqual(self.appointment.get_service_duration(), "1 hour")
-
-    def test_appt_to_dict(self):
+    def test_conversion_to_dict(self):
         response = {
             'id': 1,
-            'client_name': 'Client1',
-            'client_email': 'client1@gmail.com',
+            'client_name': self.client_.first_name,
+            'client_email': self.client_.email,
             'start_time': '1900-01-01 09:00',
             'end_time': '1900-01-01 10:00',
-            'service_name': 'Test Service',
-            'address': 'Some City, Some State',
+            'service_name': self.expected_service_name,
+            'address': self.address,
             'want_reminder': False,
             'additional_info': None,
             'paid': False,
-            'amount_to_pay': 100,
+            'amount_to_pay': self.expected_service_price,
         }
         actual_response = self.appointment.to_dict()
         actual_response.pop('id_request', None)
         self.assertEqual(actual_response, response)
 
-    def test_get_staff_member_name_with_staff_member(self):
-        """Test if you get_staff_member_name method returns the correct name when a staff member is associated."""
-        expected_name = self.staff_member1.get_staff_member_name()
-        actual_name = self.appointment.get_staff_member_name()
-        self.assertEqual(actual_name, expected_name)
-
-    def test_get_staff_member_name_without_staff_member(self):
-        """Test if you get_staff_member_name method returns an empty string when no staff member is associated."""
-        self.appointment.appointment_request.staff_member = None
-        self.appointment.appointment_request.save()
-        self.assertEqual(self.appointment.get_staff_member_name(), "")
-
-    def test_get_service_img_url_no_image(self):
-        """Service should handle cases where no image is provided gracefully."""
-        self.assertEqual(self.appointment.get_service_img_url(), "")
-
 
 class AppointmentValidDateTestCase(BaseTest):
     def setUp(self):
         super().setUp()
         self.weekday = "Monday"  # Example weekday
         self.weekday_num = get_weekday_num(self.weekday)
-        WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=self.weekday_num,
-                                    start_time=time(9, 0),
-                                    end_time=time(17, 0))
+        self.wh = WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=self.weekday_num,
+                                              start_time=time(9, 0), end_time=time(17, 0))
         self.appt_date = timezone.now().date() + timedelta(days=(self.weekday_num - timezone.now().weekday()) % 7)
         self.start_time = timezone.now().replace(hour=10, minute=0, second=0, microsecond=0)
         self.current_appointment_id = None
 
+    def tearDown(self):
+        self.wh.delete()
+        return super().tearDown()
+
     def test_staff_member_works_on_given_day(self):
         is_valid, message = Appointment.is_valid_date(self.appt_date, self.start_time, self.staff_member1,
                                                       self.current_appointment_id, self.weekday)
         self.assertTrue(is_valid)
 
     def test_staff_member_does_not_work_on_given_day(self):
         non_working_day = "Sunday"
@@ -263,7 +129,96 @@
 
     def test_staff_member_has_day_off(self):
         DayOff.objects.create(staff_member=self.staff_member1, start_date=self.appt_date, end_date=self.appt_date)
         is_valid, message = Appointment.is_valid_date(self.appt_date, self.start_time, self.staff_member1,
                                                       self.current_appointment_id, self.weekday)
         self.assertFalse(is_valid)
         self.assertIn("has a day off on this date", message)
+
+
+class AppointmentValidationTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        self.tomorrow = timezone.now().date() + timedelta(days=1)
+        self.ar = self.create_appointment_request_(service=self.service2, staff_member=self.staff_member2,
+                                                   date_=self.tomorrow)
+        self.appointment = self.create_appt_for_sm2(appointment_request=self.ar)
+        self.client_ = self.users['client1']
+        return super().setUp()
+
+    def tearDown(self):
+        self.appointment.delete()
+        return super().tearDown()
+
+    def test_invalid_phone_number(self):
+        """Test that an appointment cannot be created with an invalid phone number."""
+        self.appointment.phone = "1234"  # Invalid phone number
+        with self.assertRaises(ValidationError):
+            self.appointment.full_clean()
+
+    def test_set_paid_status(self):
+        """Test if an appointment's paid status can be set."""
+        appointment = deepcopy(self.appointment)
+        appointment.set_appointment_paid_status(True)
+        self.assertTrue(appointment.is_paid())
+        appointment.set_appointment_paid_status(False)
+        self.assertFalse(appointment.is_paid())
+
+    def test_save_with_down_payment(self):
+        """Test if an appointment can be saved with a down payment."""
+        ar = self.create_appointment_request_(service=self.service2, staff_member=self.staff_member2,
+                                              date_=self.tomorrow)
+        appointment = self.create_appt_for_sm2(appointment_request=ar)
+        ar.payment_type = 'down'
+        ar.save()
+        appointment.save()
+        self.assertEqual(appointment.get_service_down_payment(), self.service2.get_down_payment())
+
+    def test_creation_without_appointment_request(self):
+        """Test that an appointment cannot be created without an appointment request."""
+        with self.assertRaises(ValidationError):  # Assuming model validation prevents this
+            Appointment.objects.create(client=self.client_)
+
+    def test_creation_without_client(self):
+        """Test that an appointment can be created without a client."""
+        ar = self.create_appointment_request_(service=self.service2, staff_member=self.staff_member2,
+                                              date_=self.tomorrow)
+        appt = Appointment.objects.create(appointment_request=ar)
+        self.assertIsNone(appt.client)
+
+    def test_creation_without_required_fields(self):
+        """Test that an appointment cannot be created without the required fields."""
+        with self.assertRaises(ValidationError):
+            Appointment.objects.create()
+
+    def test_get_staff_member_name_without_staff_member(self):
+        """Test if you get_staff_member_name method returns an empty string when no staff member is associated."""
+        ar = self.create_appointment_request_(service=self.service2, staff_member=self.staff_member2,
+                                              date_=self.tomorrow)
+        appointment = self.create_appt_for_sm2(appointment_request=ar)
+        appointment.appointment_request.staff_member = None
+        appointment.appointment_request.save()
+        self.assertEqual(appointment.get_staff_member_name(), "")
+
+    def test_rescheduling(self):
+        """Simulate appointment rescheduling by changing the appointment date and times."""
+        ar = self.create_appointment_request_(service=self.service2, staff_member=self.staff_member2,
+                                              date_=self.tomorrow)
+        appointment = self.create_appt_for_sm2(appointment_request=ar)
+        new_date = ar.date + timedelta(days=1)
+        new_start_time = time(10, 0)
+        new_end_time = time(11, 0)
+        ar.date = new_date
+        ar.start_time = new_start_time
+        ar.end_time = new_end_time
+        ar.save()
+
+        self.assertEqual(appointment.get_date(), new_date)
+        self.assertEqual(appointment.get_start_time().time(), new_start_time)
+        self.assertEqual(appointment.get_end_time().time(), new_end_time)
```

### Comparing `django-appointment-3.4.1/appointment/tests/models/test_model_appointment_request.py` & `django_appointment-3.5.0/appointment/tests/models/test_appointment_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,168 +1,182 @@
-import datetime
-from datetime import date, time, timedelta
+from copy import deepcopy
+from datetime import date, datetime, time, timedelta
 
 from django.core.exceptions import ValidationError
+from django.utils import timezone
 
 from appointment.tests.base.base_test import BaseTest
 
 
-class AppointmentRequestModelTestCase(BaseTest):
-    def setUp(self):
-        super().setUp()
-        self.ar = self.create_appointment_request_(self.service1, self.staff_member1)
-        self.today = date.today()
+class AppointmentRequestCreationAndBasicAttributesTests(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        return super().setUpTestData()
+
+    @classmethod
+    def tearDownClass(cls):
+        return super().tearDownClass()
+
+    def setUp(self) -> None:
+        self.ar = self.create_appt_request_for_sm1()
+        return super().setUp()
+
+    def tearDown(self):
+        self.ar.delete()
+        super().tearDown()
 
-    def test_appointment_request_creation(self):
-        """Test if an appointment request can be created."""
+    def test_default_attributes_on_creation(self):
         self.assertIsNotNone(self.ar)
+        self.assertEqual(self.ar.service, self.service1)
+        self.assertEqual(self.ar.staff_member, self.staff_member1)
         self.assertEqual(self.ar.start_time, time(9, 0))
         self.assertEqual(self.ar.end_time, time(10, 0))
-
-    def test_service_name_retrieval(self):
-        """Test if an appointment request's service name is correct."""
-        self.assertEqual(self.ar.get_service_name(), "Test Service")
-
-    def test_service_price_retrieval(self):
-        self.assertEqual(self.ar.get_service_price(), 100)
-
-    def test_invalid_start_time(self):
-        """Start time must be before end time"""
-        self.ar.start_time = time(11, 0)
-        self.ar.end_time = time(9, 0)
-        with self.assertRaises(ValidationError):
-            self.ar.full_clean()
-
-    def test_invalid_payment_type(self):
-        """Payment type must be either 'full' or 'down'"""
-        self.ar.payment_type = "invalid"
-        with self.assertRaises(ValidationError):
-            self.ar.full_clean()
-
-    def test_get_date(self):
-        """Test if an appointment request's date is correct."""
-        self.assertEqual(self.ar.date, date.today())
-
-    def test_get_start_time(self):
-        """Test if an appointment request's start time is correct."""
-        self.assertEqual(self.ar.start_time, time(9, 0))
-
-    def test_get_end_time(self):
-        """Test if an appointment request's end time is correct."""
-        self.assertEqual(self.ar.end_time, time(10, 0))
-
-    def test_get_service_down_payment(self):
-        """Test if an appointment request's service down payment is correct."""
-        self.assertEqual(self.ar.get_service_down_payment(), 0)
-
-    def test_get_service_image(self):
-        """ test_get_service_image not implemented yet."""
-        # self.assertIsNone(self.ar.get_service_image())
-        pass
-
-    def test_get_service_image_url(self):
-        """test_get_service_image_url's implementation not finished yet."""
-        pass
-
-    def test_get_service_description(self):
-        """Test if an appointment request's service description is correct."""
-        self.assertIsNone(self.ar.get_service_description())
-
-    def test_get_id_request(self):
-        """Test if an appointment request's ID request is correct."""
         self.assertIsNotNone(self.ar.get_id_request())
-        self.assertIsInstance(self.ar.get_id_request(), str)
+        self.assertEqual(self.ar.date, timezone.now().date())
+        self.assertTrue(isinstance(self.ar.get_id_request(), str))
+        self.assertIsNotNone(self.ar.created_at)
+        self.assertIsNotNone(self.ar.updated_at)
 
-    def test_is_a_paid_service(self):
-        """Test if an appointment request's service is a paid service."""
+    def test_appointment_request_initial_state(self):
+        """Check the initial state of "reschedule attempts" and string representation."""
+        self.assertEqual(self.ar.reschedule_attempts, 0)
+        expected_representation = f"{self.ar.date} - {self.ar.start_time} to {self.ar.end_time} - {self.ar.service.name}"
+        self.assertEqual(str(self.ar), expected_representation)
+
+
+class AppointmentRequestServiceAttributesTests(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        return super().setUpTestData()
+
+    @classmethod
+    def tearDownClass(cls):
+        return super().tearDownClass()
+
+    def setUp(self) -> None:
+        self.ar = self.create_appt_request_for_sm1()
+        return super().setUp()
+
+    def tearDown(self):
+        self.ar.delete()
+        super().tearDown()
+
+    def test_service_related_attributes_are_correct(self):
+        """Validate attributes related to the service within an appointment request."""
+        self.assertEqual(self.ar.get_service_name(), self.service1.name)
+        self.assertEqual(self.ar.get_service_price(), self.service1.get_price())
+        self.assertEqual(self.ar.get_service_down_payment(), self.service1.get_down_payment())
+        self.assertEqual(self.ar.get_service_image(), self.service1.image)
+        self.assertEqual(self.ar.get_service_image_url(), self.service1.get_image_url())
+        self.assertEqual(self.ar.get_service_description(), self.service1.description)
         self.assertTrue(self.ar.is_a_paid_service())
-
-    def test_accepts_down_payment_false(self):
-        """Test if an appointment request's service accepts down payment."""
-        self.assertFalse(self.ar.accepts_down_payment())
-
-    def test_get_payment_type(self):
-        """Test if an appointment request's payment type is correct."""
         self.assertEqual(self.ar.payment_type, 'full')
+        self.assertFalse(self.ar.accepts_down_payment())
 
-    def test_created_at(self):
-        """Test if an appointment request's created at date is correctly set upon creation."""
-        self.assertIsNotNone(self.ar.created_at)
 
-    def test_updated_at(self):
-        """Test if an appointment request's updated at date is correctly set upon creation."""
-        self.assertIsNotNone(self.ar.updated_at)
+class AppointmentRequestAttributeValidation(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        return super().setUpTestData()
+
+    @classmethod
+    def tearDownClass(cls):
+        return super().tearDownClass()
+
+    def setUp(self) -> None:
+        self.ar = self.create_appt_request_for_sm1()
+        return super().setUp()
+
+    def tearDown(self):
+        self.ar.delete()
+        super().tearDown()
+
+    def test_appointment_request_time_validations(self):
+        """Ensure start and end times are validated correctly."""
+        ar = deepcopy(self.ar)
+
+        # End time before start time
+        ar.start_time = time(11, 0)
+        ar.end_time = time(9, 0)
+        with self.assertRaises(ValidationError):
+            ar.full_clean()
 
-    def test_appointment_with_same_start_and_end_time(self):
-        """
-        Test the situation where an appointment's start time is equal to the end time.
-        The model will prevent this.
-        """
+        # End time equal to start time
+        ar.end_time = time(11, 0)
         with self.assertRaises(ValidationError):
-            self.create_appointment_request_(self.service1, self.staff_member1, start_time=time(9, 0),
-                                             end_time=time(9, 0))
+            ar.full_clean()
 
-    def test_appointment_in_past(self):
-        """Test that an appointment cannot be created in the past."""
-        past_date = date.today() - timedelta(days=1)
+        with self.assertRaises(ValidationError, msg="Start time and end time cannot be the same"):
+            self.create_appointment_request_(
+                self.service1, self.staff_member1, date_=date.today(), start_time=time(10, 0), end_time=time(10, 0)
+            )
+
+    def test_appointment_request_date_validations(self):
+        """Validate that appointment requests cannot be in the past or have invalid durations."""
+        ar = deepcopy(self.ar)
+
+        past_date = date.today() - timedelta(days=30)
+        ar.date = past_date
         with self.assertRaises(ValidationError):
+            ar.full_clean()
+
+        with self.assertRaises(ValidationError, msg="Date cannot be in the past"):
             self.create_appointment_request_(self.service1, self.staff_member1, date_=past_date)
 
+        with self.assertRaises(ValidationError, msg="The date is not valid"):
+            date_ = datetime.strptime("31-03-2021", "%d-%m-%Y").date()
+            self.create_appointment_request_(
+                self.service1, self.staff_member1, date_=date_)
+
     def test_appointment_duration_exceeds_service_time(self):
         """Test that an appointment cannot be created with a duration greater than the service duration."""
         long_duration = timedelta(hours=3)
-        self.service1.duration = long_duration
-        self.service1.save()
+        service = self.create_service_(name="Asgard Technology Retrofit", duration=long_duration)
+        service.duration = long_duration
+        service.save()
 
-        # Assuming the appointment request uses the service duration
+        # Create an appointment request with a 4-hour duration and the 3-hour service (should not work)
         with self.assertRaises(ValidationError):
-            self.create_appointment_request_(self.service1, self.staff_member1, start_time=time(9, 0),
+            self.create_appointment_request_(service, self.staff_member1, start_time=time(9, 0),
                                              end_time=time(13, 0))
 
-    def test_reschedule_attempts_limit(self):
-        """Test appointment request's ability to be rescheduled based on service's limit."""
-        self.service1.reschedule_limit = 2
-        self.service1.save()
-
-        # Simulate rescheduling attempts
-        self.ar.increment_reschedule_attempts()
-        self.assertTrue(self.ar.can_be_rescheduled())
-
-        self.ar.increment_reschedule_attempts()
-        self.assertFalse(self.ar.can_be_rescheduled(),
-                         "Should not be reschedulable after reaching the limit")
-
-    def test_appointment_request_with_invalid_date(self):
-        """Appointment date should be valid and not in the past."""
-        invalid_date = self.today - timedelta(days=1)
-        with self.assertRaises(ValidationError, msg="Date cannot be in the past"):
-            self.create_appointment_request_(
-                self.service1, self.staff_member1, date_=invalid_date, start_time=time(10, 0), end_time=time(11, 0)
-            )
-        with self.assertRaises(ValidationError, msg="The date is not valid"):
-            date_ = datetime.datetime.strptime("31-03-2021", "%d-%m-%Y").date()
-            self.create_appointment_request_(
-                self.service1, self.staff_member1, date_=date_,
-                start_time=time(10, 0), end_time=time(11, 0)
-            )
+    def test_invalid_payment_type_raises_error(self):
+        """Payment type must be either 'full' or 'down'"""
+        ar = deepcopy(self.ar)
+        ar.payment_type = "Naquadah Instead of Credits"
+        with self.assertRaises(ValidationError):
+            ar.full_clean()
 
-    def test_start_time_after_end_time(self):
-        """Start time should not be after end time."""
-        with self.assertRaises(ValueError, msg="Start time must be before end time"):
-            self.create_appointment_request_(
-                self.service1, self.staff_member1, date_=self.today, start_time=time(11, 0), end_time=time(10, 0)
-            )
 
-    def test_start_time_equals_end_time(self):
-        """Start time and end time should not be the same."""
-        with self.assertRaises(ValidationError, msg="Start time and end time cannot be the same"):
-            self.create_appointment_request_(
-                self.service1, self.staff_member1, date_=self.today, start_time=time(10, 0), end_time=time(10, 0)
-            )
-
-    def test_appointment_duration_not_exceed_service(self):
-        """Appointment duration should not exceed the service's duration."""
-        extended_end_time = time(11, 30)  # 2.5 hours, exceeding the 1-hour service duration
-        with self.assertRaises(ValidationError, msg="Duration cannot exceed the service duration"):
-            self.create_appointment_request_(
-                self.service1, self.staff_member1, date_=self.today, start_time=time(9, 0), end_time=extended_end_time
-            )
+class AppointmentRequestRescheduleHistory(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        return super().setUpTestData()
+
+    @classmethod
+    def tearDownClass(cls):
+        return super().tearDownClass()
+
+    def setUp(self) -> None:
+        service = deepcopy(self.service1)
+        service.reschedule_limit = 2
+        service.allow_rescheduling = True
+        service.save()
+        self.ar_ = self.create_appt_request_for_sm1(service=service)
+        return super().setUp()
+
+    def test_ar_can_be_reschedule(self):
+        self.assertTrue(self.ar_.can_be_rescheduled())
+
+    def test_reschedule_attempts_increment(self):
+        self.assertTrue(self.ar_.can_be_rescheduled())
+        self.ar_.increment_reschedule_attempts()
+        self.assertEqual(self.ar_.reschedule_attempts, 1)
+        self.assertTrue(self.ar_.can_be_rescheduled())
+        self.ar_.increment_reschedule_attempts()
+        self.assertEqual(self.ar_.reschedule_attempts, 2)
+        self.assertFalse(self.ar_.can_be_rescheduled())
+
+    def test_no_reschedule_history(self):
+        service = deepcopy(self.service1)
+        ar = self.create_appointment_request_(service, self.staff_member1)
+        self.assertFalse(ar.get_reschedule_history().exists())
```

### Comparing `django-appointment-3.4.1/appointment/tests/models/test_model_day_off.py` & `django_appointment-3.5.0/appointment/tests/models/test_day_off.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,69 @@
+from copy import deepcopy
 from datetime import date, timedelta
 
 from django.core.exceptions import ValidationError
 from django.db import IntegrityError
 
 from appointment.models import DayOff
 from appointment.tests.base.base_test import BaseTest
 
 
-class DayOffModelTestCase(BaseTest):
+class DayOffCreationTestCase(BaseTest):
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+
     def setUp(self):
-        super().setUp()
         self.day_off = DayOff.objects.create(
             staff_member=self.staff_member1,
             start_date=date.today(),
-            end_date=date.today() + timedelta(days=1)
+            end_date=date.today() + timedelta(days=2)
         )
+        super().setUp()
+
+    def tearDown(self):
+        super().tearDown()
+        DayOff.objects.all().delete()
 
-    def test_day_off_creation(self):
+    def test_default_attributes_on_creation(self):
         """Test basic creation of DayOff."""
         self.assertIsNotNone(self.day_off)
         self.assertEqual(self.day_off.staff_member, self.staff_member1)
+        self.assertTrue(self.day_off.is_owner(self.users['staff1'].id))
+        self.assertFalse(self.day_off.is_owner(9999))  # Assuming 9999 is not a valid user ID
+
+    def test_day_off_str_method(self):
+        """Test that the string representation of a day off is correct."""
+        self.assertEqual(str(self.day_off), f"{date.today()} to {date.today() + timedelta(days=2)} - Day off")
+        day_off = deepcopy(self.day_off)
+        # Testing with a description
+        day_off.description = "Vacation"
+        day_off.save()
+        self.assertEqual(str(day_off), f"{date.today()} to {date.today() + timedelta(days=2)} - Vacation")
+
+
+class DayOffModelTestCase(BaseTest):
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
     def test_day_off_start_date_before_end_date(self):
         """Test that start date must be before end date upon day off creation."""
         with self.assertRaises(ValidationError):
             DayOff.objects.create(
                 staff_member=self.staff_member1,
                 start_date=date.today() + timedelta(days=1),
                 end_date=date.today()
             ).clean()
 
-    def test_day_off_is_owner(self):
-        """Test that is_owner method in day off model works as expected."""
-        self.assertTrue(self.day_off.is_owner(self.user1.id))
-        self.assertFalse(self.day_off.is_owner(9999))  # Assuming 9999 is not a valid user ID in your tests
-
     def test_day_off_without_staff_member(self):
         """Test that a day off cannot be created without a staff member."""
         with self.assertRaises(IntegrityError):
             DayOff.objects.create(
                 start_date=date.today(),
                 end_date=date.today() + timedelta(days=1)
             )
-
-    def test_day_off_str_method(self):
-        """Test that the string representation of a day off is correct."""
-        self.assertEqual(str(self.day_off), f"{date.today()} to {date.today() + timedelta(days=1)} - Day off")
-
-        # Testing with a description
-        self.day_off.description = "Vacation"
-        self.day_off.save()
-        self.assertEqual(str(self.day_off), f"{date.today()} to {date.today() + timedelta(days=1)} - Vacation")
```

### Comparing `django-appointment-3.4.1/appointment/tests/models/test_model_email_verification.py` & `django_appointment-3.5.0/appointment/tests/models/test_email_verification.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,49 +2,39 @@
 
 from django.test import TestCase
 
 from appointment.models import EmailVerificationCode
 from appointment.tests.mixins.base_mixin import UserMixin
 
 
-class EmailVerificationCodeModelTestCase(TestCase, UserMixin):
+class EmailVerificationCodeBasicTestCase(TestCase, UserMixin):
     def setUp(self):
         self.user = self.create_user_()
         self.code = EmailVerificationCode.generate_code(self.user)
 
-    def test_code_creation(self):
+    def tearDown(self):
+        super().tearDown()
+        EmailVerificationCode.objects.all().delete()
+        self.user.delete()
+
+    def test_default_attributes_on_creation(self):
         """Test if a verification code can be generated."""
         verification_code = EmailVerificationCode.objects.get(user=self.user)
         self.assertIsNotNone(verification_code)
         self.assertEqual(verification_code.code, self.code)
-
-    def test_code_length(self):
-        """Test that the code is six characters long."""
+        self.assertEqual(str(verification_code), self.code)
+        self.assertIsNotNone(verification_code.created_at)
+        self.assertIsNotNone(verification_code.updated_at)
         self.assertEqual(len(self.code), 6)
 
     def test_code_content(self):
         """Test that the code only contains uppercase letters and digits."""
         valid_characters = set(string.ascii_uppercase + string.digits)
         self.assertTrue(all(char in valid_characters for char in self.code))
 
-    def test_code_str_representation(self):
-        """Test that the string representation of a verification code is correct."""
-        verification_code = EmailVerificationCode.objects.get(user=self.user)
-        self.assertEqual(str(verification_code), self.code)
-
-    def test_created_at(self):
-        """Test if the created_at field is set when a code is generated."""
-        verification_code = EmailVerificationCode.objects.get(user=self.user)
-        self.assertIsNotNone(verification_code.created_at)
-
-    def test_updated_at(self):
-        """Test if the updated_at field is set when a code is generated."""
-        verification_code = EmailVerificationCode.objects.get(user=self.user)
-        self.assertIsNotNone(verification_code.updated_at)
-
     def test_multiple_codes_for_user(self):
         """
         Test if multiple verification codes can be generated for a user.
         This should ideally create a new code, but the old one will still exist.
         """
         new_code = EmailVerificationCode.generate_code(self.user)
         self.assertNotEqual(self.code, new_code)
```

### Comparing `django-appointment-3.4.1/appointment/tests/models/test_model_password_reset_token.py` & `django_appointment-3.5.0/appointment/tests/models/test_password_reset_token.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,52 @@
 
 from django.utils import timezone
 
 from appointment.models import PasswordResetToken
 from appointment.tests.base.base_test import BaseTest
 
 
-class PasswordResetTokenTests(BaseTest):
+class PasswordResetTokenCreationTests(BaseTest):
+
     def setUp(self):
         super().setUp()
-        self.user = self.create_user_(username='test_user', email='test@example.com', password='test_pass123')
+        self.user = self.create_user_(username='janet.fraiser', email='janet.fraiser@django-appointment.com',
+                                      password='LovedCassandra', first_name='Janet')
         self.expired_time = timezone.now() - datetime.timedelta(minutes=5)
+        self.token = PasswordResetToken.create_token(user=self.user)
 
-    def test_create_token(self):
-        """Test token creation for a user."""
-        token = PasswordResetToken.create_token(user=self.user)
-        self.assertIsNotNone(token)
-        self.assertFalse(token.is_expired)
-        self.assertFalse(token.is_verified)
+    def tearDown(self):
+        super().tearDown()
+        self.user.delete()
+        self.token.delete()
+
+    def test_default_attributes_on_creation(self):
+        self.assertIsNotNone(self.token)
+        self.assertFalse(self.token.is_expired)
+        self.assertFalse(self.token.is_verified)
 
     def test_str_representation(self):
         """Test the string representation of the token."""
-        token = PasswordResetToken.create_token(self.user)
         expected_str = (f"Password reset token for {self.user} "
-                        f"[{token.token} status: {token.status} expires at {token.expires_at}]")
-        self.assertEqual(str(token), expected_str)
+                        f"[{self.token.token} status: {self.token.status} expires at {self.token.expires_at}]")
+        self.assertEqual(str(self.token), expected_str)
+
+
+class PasswordResetTokenPropertiesTest(BaseTest):
+    def setUp(self):
+        super().setUp()
+        self.user = self.create_user_(username='janet.fraiser', email='janet.fraiser@django-appointment.com',
+                                      password='LovedCassandra', first_name='Janet')
+        self.expired_time = timezone.now() - datetime.timedelta(minutes=5)
+        self.token = PasswordResetToken.create_token(user=self.user)
+
+    def tearDown(self):
+        super().tearDown()
+        self.user.delete()
+        self.token.delete()
 
     def test_is_verified_property(self):
         """Test the is_verified property to check if the token status is correctly identified as verified."""
         token = PasswordResetToken.create_token(self.user)
         self.assertFalse(token.is_verified, "Newly created token should not be verified.")
         token.mark_as_verified()
         self.assertTrue(token.is_verified, "Token should be marked as verified after calling mark_as_verified.")
@@ -58,25 +77,34 @@
         self.assertTrue(token.is_invalidated, "Token should be marked as invalidated after status change.")
 
     def test_token_expiration(self):
         """Test that a token is considered expired after the expiration time."""
         token = PasswordResetToken.create_token(user=self.user, expiration_minutes=-1)  # Token already expired
         self.assertTrue(token.is_expired)
 
+
+class PasswordResetTokenVerificationTests(BaseTest):
+    def setUp(self):
+        super().setUp()
+        self.user = self.create_user_(username='janet.fraiser', email='janet.fraiser@django-appointment.com',
+                                      password='LovedCassandra', first_name='Janet')
+        self.expired_time = timezone.now() - datetime.timedelta(minutes=5)
+
     def test_verify_token_success(self):
         """Test successful token verification."""
         token = PasswordResetToken.create_token(user=self.user)
         verified_token = PasswordResetToken.verify_token(user=self.user, token=token.token)
         self.assertIsNotNone(verified_token)
 
     def test_verify_token_failure_expired(self):
         """Test token verification fails if the token has expired."""
         token = PasswordResetToken.create_token(user=self.user, expiration_minutes=-1)  # Token already expired
         verified_token = PasswordResetToken.verify_token(user=self.user, token=token.token)
-        self.assertIsNone(verified_token)
+
+        self.assertIsNone(verified_token, "Expired token should not verify")
 
     def test_verify_token_failure_wrong_user(self):
         """Test token verification fails if the token does not belong to the given user."""
         another_user = self.create_user_(username='another_user', email='another@example.com',
                                          password='test_pass456')
         token = PasswordResetToken.create_token(user=self.user)
         verified_token = PasswordResetToken.verify_token(user=another_user, token=token.token)
@@ -85,22 +113,14 @@
     def test_verify_token_failure_already_verified(self):
         """Test token verification fails if the token has already been verified."""
         token = PasswordResetToken.create_token(user=self.user)
         token.mark_as_verified()
         verified_token = PasswordResetToken.verify_token(user=self.user, token=token.token)
         self.assertIsNone(verified_token)
 
-    def test_mark_as_verified(self):
-        """Test marking a token as verified."""
-        token = PasswordResetToken.create_token(user=self.user)
-        self.assertFalse(token.is_verified)
-        token.mark_as_verified()
-        token.refresh_from_db()  # Refresh the token object from the database
-        self.assertTrue(token.is_verified)
-
     def test_verify_token_invalid_token(self):
         """Test token verification fails if the token does not exist."""
         PasswordResetToken.create_token(user=self.user)
         invalid_token_uuid = "12345678-1234-1234-1234-123456789012"  # An invalid token UUID
         verified_token = PasswordResetToken.verify_token(user=self.user, token=invalid_token_uuid)
         self.assertIsNone(verified_token)
 
@@ -119,46 +139,14 @@
 
         old_verified = PasswordResetToken.verify_token(user=self.user, token=old_token.token)
         new_verified = PasswordResetToken.verify_token(user=self.user, token=new_token.token)
 
         self.assertIsNone(old_verified, "Old token should not be valid after creating a new one")
         self.assertIsNotNone(new_verified, "New token should be valid")
 
-    def test_expired_token_does_not_verify(self):
-        """Test that an expired token does not verify even if correct."""
-        token = PasswordResetToken.create_token(user=self.user, expiration_minutes=-5)  # Already expired
-        # Fast-forward time to after expiration
-        token.expires_at = timezone.now() - datetime.timedelta(minutes=5)
-        token.save()
-
-        verified_token = PasswordResetToken.verify_token(user=self.user, token=token.token)
-        self.assertIsNone(verified_token, "Expired token should not verify")
-
-    def test_mark_as_verified_is_idempotent(self):
-        """Test that marking a token as verified multiple times has no adverse effect."""
-        token = PasswordResetToken.create_token(user=self.user)
-        token.mark_as_verified()
-        first_verification_time = token.updated_at
-
-        time.sleep(1)  # Ensure time has passed
-        token.mark_as_verified()
-        token.refresh_from_db()
-
-        self.assertTrue(token.is_verified)
-        self.assertEqual(first_verification_time, token.updated_at,
-                         "Token verification time should not update on subsequent calls")
-
-    def test_deleting_user_cascades_to_tokens(self):
-        """Test that deleting a user deletes associated password reset tokens."""
-        token = PasswordResetToken.create_token(user=self.user)
-        self.user.delete()
-
-        with self.assertRaises(PasswordResetToken.DoesNotExist):
-            PasswordResetToken.objects.get(pk=token.pk)
-
     def test_token_verification_resets_after_expiration(self):
         """Test that an expired token cannot be verified after its expiration, even if marked as verified."""
         token = PasswordResetToken.create_token(user=self.user, expiration_minutes=-1)  # Already expired
         token.mark_as_verified()
 
         verified_token = PasswordResetToken.verify_token(user=self.user, token=token.token)
         self.assertIsNone(verified_token, "Expired token should not verify, even if marked as verified")
@@ -181,7 +169,53 @@
 
     def test_token_verification_after_user_deletion(self):
         """Test that a token cannot be verified after the associated user is deleted."""
         token = PasswordResetToken.create_token(self.user)
         self.user.delete()
         verified_token = PasswordResetToken.verify_token(None, token.token)
         self.assertIsNone(verified_token, "Token should not verify after user deletion")
+
+
+class PasswordResetTokenTests(BaseTest):
+    def setUp(self):
+        super().setUp()
+        self.user = self.create_user_(username='janet.fraiser', email='janet.fraiser@django-appointment.com',
+                                      password='LovedCassandra', first_name='Janet')
+        self.expired_time = timezone.now() - datetime.timedelta(minutes=5)
+
+    def tearDown(self):
+        super().tearDown()
+        PasswordResetToken.objects.all().delete()
+        self.user.delete()
+
+    def test_mark_as_verified(self):
+        """Test marking a token as verified."""
+        token = PasswordResetToken.create_token(user=self.user)
+        self.assertFalse(token.is_verified)
+        token.mark_as_verified()
+        token.refresh_from_db()  # Refresh the token object from the database
+        self.assertTrue(token.is_verified)
+
+    def test_mark_as_verified_is_idempotent(self):
+        """Test that marking a token as verified multiple times has no adverse effect."""
+        token = PasswordResetToken.create_token(user=self.user)
+        token.mark_as_verified()
+        first_verification_time = token.updated_at
+
+        time.sleep(1)  # Ensure time has passed
+        token.mark_as_verified()
+        token.refresh_from_db()
+
+        self.assertTrue(token.is_verified)
+        self.assertEqual(first_verification_time, token.updated_at,
+                         "Token verification time should not update on subsequent calls")
+
+    def test_deleting_user_cascades_to_tokens(self):
+        """Test that deleting a user deletes associated password reset tokens."""
+
+        apophis = self.create_user_(username='apophis.false_god', email='apophis.false_god@django-appointment.com',
+                                    password='LovedSayingSholva', first_name='Apophis')
+        token = PasswordResetToken.create_token(user=apophis)
+        apophis.delete()
+
+        with self.assertRaises(PasswordResetToken.DoesNotExist):
+            PasswordResetToken.objects.get(pk=token.pk)
```

### Comparing `django-appointment-3.4.1/appointment/tests/models/test_model_service.py` & `django_appointment-3.5.0/appointment/tests/models/test_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,254 +1,266 @@
+from copy import deepcopy
 from datetime import timedelta
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.core.files.uploadedfile import SimpleUploadedFile
-from django.test import TestCase
 
 from appointment.models import Service
+from appointment.tests.base.base_test import BaseTest
 
 
-class ServiceModelTestCase(TestCase):
-    def setUp(self):
-        self.service = Service.objects.create(name="Test Service", duration=timedelta(hours=1, minutes=30), price=100)
+class ServiceCreationAndBasicAttributesTests(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.service = cls.service1
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
     def test_service_creation(self):
-        """Test if a service can be created."""
         self.assertIsNotNone(self.service)
-        self.assertEqual(self.service.duration, timedelta(hours=1, minutes=30))
-        self.assertEqual(self.service.price, 100)
 
-    def test_is_a_paid_service(self):
-        """Test if a service is a paid service."""
-        self.assertTrue(self.service.is_a_paid_service())
-
-    def test_service_name(self):
-        """Test if a service can be created with a name."""
-        self.assertEqual(self.service.name, "Test Service")
-
-    def test_get_service_description(self):
-        """Test if a service can be created with a description."""
-        self.assertEqual(self.service.description, None)
-        self.service.description = "Test Service - 1 hour - 100.0"
-        self.assertEqual(self.service.description, "Test Service - 1 hour - 100.0")
-
-    def test_get_service_duration_day(self):
-        """Test that the get_duration method returns the correct string for a service with a duration of 1 day."""
-        self.service.duration = timedelta(days=1)
-        self.assertEqual(self.service.get_duration(), '1 day')
-
-    def test_get_service_duration_hour(self):
-        """Test that the get_duration method returns the correct string for a service with a duration of 1 hour."""
-        self.service.duration = timedelta(hours=1)
-        self.assertEqual(self.service.get_duration(), '1 hour')
-
-    def test_get_service_duration_minute(self):
-        """Test that the get_duration method returns the correct string for a service with a duration of 30 minutes."""
-        self.service.duration = timedelta(minutes=30)
-        self.assertEqual(self.service.get_duration(), '30 minutes')
-
-    def test_get_service_duration_second(self):
-        """Test that the get_duration method returns the correct string for a service with a duration of 30 seconds."""
-        self.service.duration = timedelta(seconds=30)
-        self.assertEqual(self.service.get_duration(), '30 seconds')
-
-    def test_get_service_duration_hour_minute(self):
-        """Test that the get_duration method returns the correct string for a service with
-           a duration of 1 hour 30 minutes."""
-        self.service.duration = timedelta(hours=2, minutes=20)
-        self.assertEqual(self.service.get_duration(), '2 hours 20 minutes')
-
-    def test_get_service_price(self):
-        """Test that the get_price method returns the correct price for a service."""
-        self.assertEqual(self.service.get_price(), 100)
-
-    def test_get_service_price_display(self):
-        """Test that the get_price_text method returns the correct string price including the currency symbol."""
-        self.assertEqual(self.service.get_price_text(), "100$")
-
-    def test_get_service_price_display_cent(self):
-        """Test that the method returns the correct string price including the currency symbol for a service with a
-           price of 100.50."""
-        self.service.price = 100.50
-        self.assertEqual(self.service.get_price_text(), "100.5$")
-
-    def test_get_service_price_display_free(self):
-        """Test that if the price is 0, the method returns the string 'Free'."""
-        self.service.price = 0
-        self.assertEqual(self.service.get_price_text(), "Free")
-
-    def test_get_service_down_payment_none(self):
-        """Test that the get_down_payment method returns 0 if the service has no down payment."""
-        self.assertEqual(self.service.get_down_payment(), 0)
-
-    def test_get_service_down_payment(self):
-        """Test that the get_down_payment method returns the correct down payment for a service."""
-        self.service.down_payment = 50
-        self.assertEqual(self.service.get_down_payment(), 50)
-
-    def test_service_currency(self):
-        """Test if a service can be created with a currency."""
-        self.assertEqual(self.service.currency, "USD")
+    def test_basic_attributes_verification(self):
+        self.assertEqual(self.service.name, "Stargate Activation")
+        self.assertEqual(self.service.description, "Activate the Stargate")
+        self.assertEqual(self.service.duration, timedelta(hours=1))
 
-    def test_service_created_at(self):
-        """Test if a service can be created with a created at date."""
+    def test_timestamps_on_creation(self):
+        """Newly created services should have created_at and updated_at values."""
         self.assertIsNotNone(self.service.created_at)
-
-    def test_get_service_updated_at(self):
-        """Test if a service can be created with an updated at date."""
         self.assertIsNotNone(self.service.updated_at)
 
-    def test_accepts_down_payment_false(self):
-        """Test that the accepts_down_payment method returns False if the service has no down payment."""
-        self.assertFalse(self.service.accepts_down_payment())
 
-    def test_accepts_down_payment_true(self):
-        """Test that the accepts_down_payment method returns True if the service has a down payment."""
-        self.service.down_payment = 50
-        self.assertTrue(self.service.accepts_down_payment())
+class ServicePriceTests(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.service = cls.service1
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def test_service_price_verification(self):
+        self.assertEqual(self.service.price, 100000)
+        self.assertEqual(self.service.get_price(), 100000)
 
-    # Negative test cases
-    def test_invalid_service_name(self):
-        """Test that the max_length of the name field is 100 characters."""
-        self.service.name = "A" * 101  # Exceeding the max_length
-        with self.assertRaises(ValidationError):
-            self.service.full_clean()
+    def test_paid_service_verification(self):
+        self.assertTrue(self.service.is_a_paid_service())
 
-    def test_invalid_service_price_negative(self):
-        """A service cannot be created with a negative price."""
-        self.service.price = -100
-        with self.assertRaises(ValidationError):
-            self.service.full_clean()
+    def check_price(self, price, expected_string):
+        service = deepcopy(self.service)
+        service.price = price
+        self.assertEqual(service.get_price_text(), expected_string)
+
+    def test_dynamic_price_representation(self):
+        """Test that the get_price method returns the correct string for a service with a price of 100, 1000, etc."""
+        test_cases = [
+            (100, '100$'),
+            (100.50, '100.5$'),
+            (49.99, '49.99$'),
+            (0, 'Free')
+        ]
+        for price, expected in test_cases:
+            self.check_price(price, expected)
+
+
+class ServiceDurationTests(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.service = cls.service1
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def test_service_duration_verification(self):
+        """Test the duration of the service."""
+        self.assertEqual(self.service.duration, self.service1.duration)
+
+    def check_duration(self, duration, expected_string):
+        service = deepcopy(self.service)
+        service.duration = duration
+        self.assertEqual(service.get_duration(), expected_string)
+
+    def test_dynamic_duration_representation(self):
+        """Test that the get_duration method returns the correct string for a service with a duration of 30 seconds,
+        30 minutes, etc."""
+        test_cases = [
+            (timedelta(seconds=30), '30 seconds'),
+            (timedelta(minutes=30), '30 minutes'),
+            (timedelta(hours=1), '1 hour'),
+            (timedelta(hours=2, minutes=30), '2 hours 30 minutes'),
+            (timedelta(days=1), '1 day'),
+        ]
+        for duration, expected in test_cases:
+            self.check_duration(duration, expected)
+
+
+class ServiceDownPaymentTests(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.service = cls.service1
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def test_down_payment_value(self):
+        """By default, down payment value is 0"""
+        self.assertEqual(self.service.down_payment, 0)
+        self.assertEqual(self.service.get_down_payment(), 0)
 
-    def test_invalid_service_down_payment_negative(self):
-        """A service cannot be created with a negative down payment."""
-        self.service.down_payment = -50
-        with self.assertRaises(ValidationError):
-            self.service.full_clean()
+        self.assertEqual(self.service.get_down_payment_text(), "Free")
 
-    def test_invalid_service_currency_length(self):
-        """A service cannot be created with a currency of less or more than three characters."""
-        self.service.currency = "US"  # Less than 3 characters
-        with self.assertRaises(ValidationError):
-            self.service.full_clean()
-        self.service.currency = "USDD"  # More than 3 characters
-        with self.assertRaises(ValidationError):
-            self.service.full_clean()
+        # Change the down payment value to 69.99
+        s = deepcopy(self.service)
+        s.down_payment = 69.99
+        self.assertEqual(s.get_down_payment(), 69.99)
 
-    def test_service_duration_zero(self):
-        """A service cannot be created with a duration of zero."""
-        service = Service(name="Test Service", duration=timedelta(0), price=100)
-        self.assertRaises(ValidationError, service.full_clean)
+        self.assertEqual(s.get_down_payment_text(), "69.99$")
 
-    def test_price_and_down_payment_same(self):
-        """A service can be created with a price and down payment of the same value."""
-        service = Service.objects.create(name="Service Name", duration=timedelta(hours=1), price=100, down_payment=100)
+    def test_accepts_down_payment(self):
+        """By default, down payment is not accepted."""
+        self.assertFalse(self.service.accepts_down_payment())
+
+        # Change the accepts_down_payment value to True
+        s = deepcopy(self.service)
+        s.down_payment = 69.99
+        self.assertTrue(s.accepts_down_payment())
+
+    def test_equal_price_and_down_payment_scenario(self):
+        """A service can be created with a price and down payment of the same value.
+        This is useful when the service requires full payment upfront.
+        """
+        service = Service.objects.create(
+            name="Naquadah Generator Maintenance", duration=timedelta(hours=1), price=100, down_payment=100)
         self.assertEqual(service.price, service.down_payment)
 
-    def test_service_with_no_name(self):
-        """A service cannot be created with no name."""
-        with self.assertRaises(ValidationError):
-            Service.objects.create(name="", duration=timedelta(hours=1), price=100).full_clean()
 
-    def test_service_with_invalid_duration(self):
-        """Service should not be created with a negative or zero duration."""
-        service = Service(name="Invalid Duration Service", duration=timedelta(seconds=-1), price=50)
-        self.assertRaises(ValidationError, service.full_clean)
-        service = Service(name="Zero Duration Service", duration=timedelta(seconds=0), price=50)
-        self.assertRaises(ValidationError, service.full_clean)
+class ServiceRepresentationAndMiscTests(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.service = cls.service1
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
-    def test_service_with_empty_name(self):
-        """Service should not be created with an empty name."""
-        service = Service.objects.create(name="", duration=timedelta(hours=1), price=50)
-        self.assertRaises(ValidationError, service.full_clean)
+    def test_string_representation_of_service(self):
+        """Test the string representation of the Service model."""
+        service_name = "Test Service"
+        service = Service.objects.create(name=service_name, duration=timedelta(hours=1), price=100)
+        self.assertEqual(str(service), service_name)
 
-    def test_service_with_negative_price(self):
-        """Service should not be created with a negative price."""
-        service = Service(name="Negative Price Service", duration=timedelta(hours=1), price=-1)
-        self.assertRaises(ValidationError, service.full_clean)
+    def test_image_url_with_attached_image(self):
+        """Service should return the correct URL for the image if provided."""
+        # Create an image and attach it to the service
+        image_path = settings.BASE_DIR / 'appointment/static/img/texture.webp'  # Adjust the path as necessary
+        image = SimpleUploadedFile(name='test_image.png', content=open(image_path, 'rb').read(),
+                                   content_type='image/png')
+        service = Service.objects.create(name="Service with Image", duration=timedelta(hours=1), price=50, image=image)
 
-    def test_service_with_negative_down_payment(self):
-        """Service should not have a negative down payment."""
-        with self.assertRaises(ValidationError):
-            service = Service(name="Service with Negative Down Payment", duration=timedelta(hours=1), price=50,
-                                   down_payment=-1)
-            service.full_clean()
+        # Assuming you have MEDIA_URL set in your settings for development like '/media/'
+        expected_url = f"{settings.MEDIA_URL}{service.image}"
+        self.assertTrue(service.get_image_url().endswith(expected_url))
+
+    def test_image_url_without_attached_image(self):
+        """Service should handle cases where no image is provided gracefully."""
+        service = Service.objects.create(name="Gate Travel Coordination", duration=timedelta(hours=1), price=50)
+        self.assertEqual(service.get_image_url(), "")
 
-    def test_service_auto_generate_background_color(self):
+    def test_auto_generation_of_background_color(self):
         """Service should auto-generate a background color if none is provided."""
-        service = Service.objects.create(name="Service with Auto Background", duration=timedelta(hours=1), price=50)
+        service = Service.objects.create(name="Wormhole Stability Analysis", duration=timedelta(hours=1), price=50)
         self.assertIsNotNone(service.background_color)
         self.assertNotEqual(service.background_color, "")
 
-    def test_reschedule_limit_and_allowance(self):
-        """Service should correctly handle reschedule limits and rescheduling allowance."""
-        service = Service.objects.create(name="Reschedulable Service", duration=timedelta(hours=1), price=50,
-                                         reschedule_limit=3, allow_rescheduling=True)
-        self.assertEqual(service.reschedule_limit, 3)
-        self.assertTrue(service.allow_rescheduling)
-
-    def test_get_service_image_url_no_image(self):
-        """Service should handle cases where no image is provided gracefully."""
-        service = Service.objects.create(name="Service without Image", duration=timedelta(hours=1), price=50)
-        self.assertEqual(service.get_image_url(), "")
-
-    def test_to_dict_method(self):
+    def test_service_to_dict_representation(self):
         """Test the to_dict method returns the correct dictionary representation of the Service instance."""
-        service = Service.objects.create(name="Test Service", duration=timedelta(hours=1), price=150,
-                                         description="A test service")
+        service = Service.objects.create(name="Off-world Tactical Training", duration=timedelta(hours=1), price=150,
+                                         description="Train for off-world missions")
         expected_dict = {
             "id": service.id,
-            "name": "Test Service",
-            "description": "A test service",
+            "name": "Off-world Tactical Training",
+            "description": "Train for off-world missions",
             "price": "150"
         }
         self.assertEqual(service.to_dict(), expected_dict)
 
-    def test_get_down_payment_as_integer(self):
-        """Test the get_down_payment method returns an integer if the down payment has no decimal part."""
-        service = Service.objects.create(name="Test Service", duration=timedelta(hours=1), price=100, down_payment=50)
-        self.assertEqual(service.get_down_payment(), 50)
-
-    def test_get_down_payment_as_decimal(self):
-        """Test the get_down_payment method returns the original decimal value if it has a decimal part."""
-        service = Service.objects.create(name="Test Service", duration=timedelta(hours=1), price=100,
-                                         down_payment=50.50)
-        self.assertEqual(service.get_down_payment(), 50.50)
-
-    def test_get_down_payment_text_free(self):
-        """Test the get_down_payment_text method returns 'Free' if the down payment is 0."""
-        service = Service.objects.create(name="Free Service", duration=timedelta(hours=1), price=100, down_payment=0)
-        self.assertEqual(service.get_down_payment_text(), "Free")
-
-    def test_get_down_payment_text_with_value(self):
-        """Test the get_down_payment_text method returns the down payment amount followed by the currency icon."""
-        service = Service.objects.create(name="Paid Service", duration=timedelta(hours=1), price=100, down_payment=25)
-        # Assuming get_currency_icon method returns "$" for USD
-        expected_text = "25$"
-        self.assertEqual(service.get_down_payment_text(), expected_text)
-
-    def test_get_down_payment_text_with_decimal(self):
-        """Test the get_down_payment_text method for a service with a decimal down payment."""
-        service = Service.objects.create(name="Service with Decimal Down Payment", duration=timedelta(hours=1),
-                                         price=100, down_payment=25.75)
-        # Assuming get_currency_icon method returns "$" for USD
-        expected_text = "25.75$"
-        self.assertEqual(service.get_down_payment_text(), expected_text)
+    def test_reschedule_features(self):
+        """Service should correctly handle reschedule limits and rescheduling allowance."""
+        service = Service.objects.create(name="Goa'uld Artifact Decryption", duration=timedelta(hours=1), price=50,
+                                         reschedule_limit=3, allow_rescheduling=True)
+        self.assertEqual(service.reschedule_limit, 3)
+        self.assertTrue(service.allow_rescheduling)
 
-    def test_str_method(self):
-        """Test the string representation of the Service model."""
-        service_name = "Test Service"
-        service = Service.objects.create(name=service_name, duration=timedelta(hours=1), price=100)
-        self.assertEqual(str(service), service_name)
+    def test_default_currency_setting(self):
+        """The Default currency is USD."""
+        self.assertEqual(self.service.currency, 'USD')
+
+        # Change the currency to EUR
+        s = deepcopy(self.service)
+        s.currency = 'EUR'
+        self.assertEqual(s.currency, 'EUR')
+
+
+class ServiceModelNegativeTestCase(BaseTest):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+        cls.service = cls.service1
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
-    def test_get_service_image_url_with_image(self):
-        """Service should return the correct URL for the image if provided."""
-        # Create an image and attach it to the service
-        image_path = settings.BASE_DIR / 'appointment/static/img/texture.webp'  # Adjust the path as necessary
-        image = SimpleUploadedFile(name='test_image.png', content=open(image_path, 'rb').read(),
-                                   content_type='image/png')
-        service = Service.objects.create(name="Service with Image", duration=timedelta(hours=1), price=50, image=image)
+    def test_exceeding_service_name_length(self):
+        """Test that the max_length of the name field is 100 characters."""
+        s = deepcopy(self.service)
+        s.name = ("Gate Diagnostics and Calibration for Intergalactic Travel through the Quantum Bridge Device "
+                  "Portal - Series SG-1")  # Exceeding the max_length (112 characters)
+        with self.assertRaises(ValidationError):
+            s.full_clean()
 
-        # Assuming you have MEDIA_URL set in your settings for development like '/media/'
-        expected_url = f"{settings.MEDIA_URL}{service.image}"
-        self.assertTrue(service.get_image_url().endswith(expected_url))
+    def test_negative_price_and_down_payment_values(self):
+        """Test that the price and down_payment fields cannot be negative."""
+        s = deepcopy(self.service)
+        s.price = -100
+        with self.assertRaises(ValidationError):
+            s.full_clean()
+
+        s = deepcopy(self.service)
+        s.down_payment = -100
+        with self.assertRaises(ValidationError):
+            s.full_clean()
+
+    def test_invalid_currency_code_length(self):
+        """A service cannot be created with a currency of less or more than three characters."""
+        s = deepcopy(self.service)
+        s.currency = "US"
+
+        with self.assertRaises(ValidationError):
+            s.full_clean()
+
+        s.currency = "DOLLAR"
+        with self.assertRaises(ValidationError):
+            s.full_clean()
+
+    def test_zero_or_negative_duration_handling(self):
+        """A service cannot be created with a duration being zero or negative."""
+        service = Service(name="Zat'nik'tel Tune-Up", duration=timedelta(0), price=100, description="Tune-up the Zat")
+        self.assertRaises(ValidationError, service.full_clean)
+        service = Service(name="Ancient's Archive Retrieval ", duration=timedelta(seconds=-1), price=50,
+                          description="Retrieve the Ancient's Archive")
+        self.assertRaises(ValidationError, service.full_clean)
+
+    def test_creation_without_service_name(self):
+        """A service cannot be created with no name."""
+        with self.assertRaises(ValidationError):
+            Service.objects.create(name="", duration=timedelta(hours=1), price=100).full_clean()
```

### Comparing `django-appointment-3.4.1/appointment/tests/models/test_model_working_hours.py` & `django_appointment-3.5.0/appointment/tests/models/test_working_hours.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 from datetime import time
 
 from django.core.exceptions import ValidationError
 from django.db import IntegrityError
 from django.test import TestCase
+from django.utils.translation import gettext as _
 
 from appointment.models import WorkingHours
 from appointment.tests.mixins.base_mixin import ServiceMixin, StaffMemberMixin, UserMixin
 
 
 class WorkingHoursModelTestCase(TestCase, UserMixin, ServiceMixin, StaffMemberMixin):
     def setUp(self):
         self.user = self.create_user_()
         self.service = self.create_service_()
         self.staff_member = self.create_staff_member_(self.user, self.service)
         self.working_hours = WorkingHours.objects.create(
-            staff_member=self.staff_member,
-            day_of_week=1,
-            start_time=time(9, 0),
-            end_time=time(17, 0)
+                staff_member=self.staff_member,
+                day_of_week=1,
+                start_time=time(9, 0),
+                end_time=time(17, 0)
         )
 
-    def test_working_hours_creation(self):
+    def test_default_attributes_on_creation(self):
         """Test if a WorkingHours instance can be created."""
         self.assertIsNotNone(self.working_hours)
         self.assertEqual(self.working_hours.staff_member, self.staff_member)
+        self.assertEqual(self.working_hours.get_start_time(), time(9, 0))
+        self.assertEqual(self.working_hours.get_end_time(), time(17, 0))
+
+    def test_working_hours_str_method(self):
+        """Test that the string representation of a WorkingHours instance is correct."""
+        self.assertEqual(str(self.working_hours), "Monday - 09:00:00 to 17:00:00")
+
+    def test_get_day_of_week_str(self):
+        """Test that the get_day_of_week_str method in WorkingHours model works as expected."""
+        self.assertEqual(self.working_hours.get_day_of_week_str(), _("Monday"))
+
+
+class WorkingHoursValidationTestCase(TestCase, UserMixin, ServiceMixin, StaffMemberMixin):
+    def setUp(self):
+        self.user = self.create_user_()
+        self.service = self.create_service_()
+        self.staff_member = self.create_staff_member_(self.user, self.service)
+        self.working_hours = WorkingHours.objects.create(
+                staff_member=self.staff_member,
+                day_of_week=1,
+                start_time=time(9, 0),
+                end_time=time(17, 0)
+        )
 
     def test_working_hours_start_time_before_end_time(self):
         """A WorkingHours instance cannot be created if start_time is after end_time."""
         with self.assertRaises(ValidationError):
             WorkingHours.objects.create(
                 staff_member=self.staff_member,
                 day_of_week=2,
                 start_time=time(17, 0),
                 end_time=time(9, 0)
             ).clean()
 
-    def test_working_hours_is_owner(self):
-        """Test that is_owner method in WorkingHours model works as expected."""
-        self.assertTrue(self.working_hours.is_owner(self.user.id))
-        self.assertFalse(self.working_hours.is_owner(9999))  # Assuming 9999 is not a valid user ID in your tests
-
     def test_working_hours_without_staff_member(self):
         """A WorkingHours instance cannot be created without a staff member."""
         with self.assertRaises(IntegrityError):
             WorkingHours.objects.create(
                 day_of_week=3,
                 start_time=time(9, 0),
                 end_time=time(17, 0)
             )
 
-    def test_working_hours_duplicate_day(self):
-        """A WorkingHours instance cannot be created if the staff member already has a working hours on that day."""
-        with self.assertRaises(IntegrityError):
-            WorkingHours.objects.create(
-                staff_member=self.staff_member,
-                day_of_week=1,  # Same day as the working_hours created in setUp
-                start_time=time(9, 0),
-                end_time=time(17, 0)
-            )
-
-    def test_working_hours_str_method(self):
-        """Test that the string representation of a WorkingHours instance is correct."""
-        self.assertEqual(str(self.working_hours), "Monday - 09:00:00 to 17:00:00")
-
-    def test_get_day_of_week_str(self):
-        """Test that the get_day_of_week_str method in WorkingHours model works as expected."""
-        self.assertEqual(self.working_hours.get_day_of_week_str(), "Monday")
+    def test_working_hours_is_owner(self):
+        """Test that is_owner method in WorkingHours model works as expected."""
+        self.assertTrue(self.working_hours.is_owner(self.user.id))
+        self.assertFalse(self.working_hours.is_owner(9999))  # Assuming 9999 is not a valid user ID in your tests
 
     def test_staff_member_weekend_status_update(self):
         """Test that the staff member's weekend status is updated when a WorkingHours instance is created."""
         WorkingHours.objects.create(
             staff_member=self.staff_member,
             day_of_week=6,  # Saturday
             start_time=time(9, 0),
@@ -83,11 +89,16 @@
             day_of_week=0,  # Sunday
             start_time=time(9, 0),
             end_time=time(12, 0)
         )
         self.staff_member.refresh_from_db()
         self.assertTrue(self.staff_member.work_on_sunday)
 
-    def test_get_start_time_and_get_end_time(self):
-        """Test that the get_start_time and get_end_time methods in WorkingHours model work as expected."""
-        self.assertEqual(self.working_hours.get_start_time(), time(9, 0))
-        self.assertEqual(self.working_hours.get_end_time(), time(17, 0))
+    def test_working_hours_duplicate_day(self):
+        """A WorkingHours instance cannot be created if the staff member already has a working hours on that day."""
+        with self.assertRaises(IntegrityError):
+            WorkingHours.objects.create(
+                staff_member=self.staff_member,
+                day_of_week=1,  # Same day as the working_hours created in setUp
+                start_time=time(9, 0),
+                end_time=time(17, 0)
+            )
```

### Comparing `django-appointment-3.4.1/appointment/tests/test_services.py` & `django_appointment-3.5.0/appointment/tests/test_services.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,188 +1,279 @@
 # test_services.py
 # Path: appointment/tests/test_services.py
 
 import datetime
 import json
 from _decimal import Decimal
+from datetime import date, time, timedelta
 from unittest.mock import patch
 
 from django.core.cache import cache
-from django.test import Client
+from django.test import Client, override_settings
 from django.test.client import RequestFactory
-from django.utils.translation import gettext as _
+from django.utils import timezone
+from django.utils.translation import gettext as _, gettext_lazy as _
 
 from appointment.forms import StaffDaysOffForm
-from appointment.services import create_staff_member_service, email_change_verification_service, \
-    fetch_user_appointments, get_available_slots_for_staff, handle_day_off_form, handle_entity_management_request, \
-    handle_service_management_request, handle_working_hours_form, prepare_appointment_display_data, \
+from appointment.services import (
+    create_staff_member_service, email_change_verification_service, fetch_user_appointments, get_available_slots,
+    get_available_slots_for_staff, get_finish_button_text, handle_day_off_form, handle_entity_management_request,
+    handle_service_management_request, handle_working_hours_form, prepare_appointment_display_data,
     prepare_user_profile_data, save_appointment, save_appt_date_time, update_personal_info_service
+)
 from appointment.tests.base.base_test import BaseTest
+from appointment.tests.mixins.base_mixin import (
+    ConfigMixin)
 from appointment.utils.date_time import convert_str_to_time, get_ar_end_time
 from appointment.utils.db_helpers import Config, DayOff, EmailVerificationCode, StaffMember, WorkingHours
+from appointment.views import get_appointments_and_slots
+
+
+class GetAvailableSlotsTests(BaseTest):
+    """Test cases for get_available_slots"""
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        self.tomorrow = timezone.now().date() + datetime.timedelta(days=1)
+        ar = self.create_appt_request_for_sm1(date_=self.tomorrow, start_time=time(11, 0), end_time=time(12, 0))
+        self.appointment = self.create_appt_for_sm1(appointment_request=ar)
+
+    @override_settings(DEBUG=True)
+    def tearDown(self):
+        Config.objects.all().delete()
+        super().tearDown()
+        cache.clear()
+
+    def test_get_available_slots(self):
+        slots = get_available_slots(self.tomorrow, [self.appointment])
+        self.assertIsInstance(slots, list)
+        self.assertNotIn('11:00 AM', slots)
+
+    def test_get_available_slots_with_config(self):
+        Config.objects.create(
+                lead_time=datetime.time(11, 0),
+                finish_time=datetime.time(15, 0),
+                slot_duration=30,
+                appointment_buffer_time=2.0
+        )
+        slots = get_available_slots(self.tomorrow, [self.appointment])
+        self.assertIsInstance(slots, list)
+        self.assertNotIn('11:00 AM', slots)
 
 
 class FetchUserAppointmentsTests(BaseTest):
     """Test suite for the `fetch_user_appointments` service function."""
 
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
-
         # Create some appointments for testing purposes
-        self.appointment_for_user1 = self.create_appointment_for_user1()
-        self.appointment_for_user2 = self.create_appointment_for_user2()
-        self.staff_user = self.create_user_(username='staff_user', password='test')
-        self.staff_user.is_staff = True
-        self.staff_user.save()
+        self.appointment_for_user1 = self.create_appt_for_sm1()
+        self.appointment_for_user2 = self.create_appt_for_sm2()
 
     def test_fetch_appointments_for_superuser(self):
         """Test that a superuser can fetch all appointments."""
         # Make user1 a superuser
-        self.user1.is_superuser = True
-        self.user1.save()
+        jack = self.users['superuser']
+        jack.is_superuser = True
+        jack.save()
 
         # Fetch appointments for superuser
-        appointments = fetch_user_appointments(self.user1)
+        appointments = fetch_user_appointments(jack)
 
         # Assert that the superuser sees all appointments
         self.assertIn(self.appointment_for_user1, appointments,
                       "Superuser should be able to see all appointments, including those created for user1.")
         self.assertIn(self.appointment_for_user2, appointments,
                       "Superuser should be able to see all appointments, including those created for user2.")
 
     def test_fetch_appointments_for_staff_member(self):
         """Test that a staff member can only fetch their own appointments."""
         # Fetch appointments for staff member (user1 in this case)
-        appointments = fetch_user_appointments(self.user1)
+        daniel = self.users['staff1']
+        daniel.is_staff = True
+        daniel.save()
+
+        appointments = fetch_user_appointments(daniel)
 
         # Assert that the staff member sees only their own appointments
         self.assertIn(self.appointment_for_user1, appointments,
                       "Staff members should only see appointments linked to them. User1's appointment is missing.")
         self.assertNotIn(self.appointment_for_user2, appointments,
                          "Staff members should not see appointments not linked to them. User2's appointment was found.")
 
     def test_fetch_appointments_for_regular_user(self):
         """Test that a regular user (not a user with staff member instance or staff) cannot fetch appointments."""
         # Fetching appointments for a regular user (client1 in this case) should raise ValueError
+        georges = self.users['client1']
         with self.assertRaises(ValueError,
                                msg="Regular users without staff or superuser status should raise a ValueError."):
-            fetch_user_appointments(self.client1)
+            fetch_user_appointments(georges)
 
     def test_fetch_appointments_for_staff_user_without_staff_member_instance(self):
         """Test that a staff user without a staff member instance gets an empty list of appointments."""
-        appointments = fetch_user_appointments(self.staff_user)
+        janet = self.create_user_()
+        janet.is_staff = True
+        janet.save()
+
+        appointments = fetch_user_appointments(janet)
         # Check that the returned value is an empty list
         self.assertEqual(appointments, [], "Expected an empty list for a staff user without a staff member instance.")
 
 
 class PrepareAppointmentDisplayDataTests(BaseTest):
     """Test suite for the `prepare_appointment_display_data` service function."""
 
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
 
         # Create an appointment for testing purposes
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
+        self.daniel = self.users['staff1']
+        self.samantha = self.users['staff2']
+        self.georges = self.users['client1']
 
     def test_non_existent_appointment(self):
         """Test that the function handles a non-existent appointment correctly."""
         # Fetch data for a non-existent appointment
-        x, y, error_message, status_code = prepare_appointment_display_data(self.user2, 9999)
+        x, y, error_message, status_code = prepare_appointment_display_data(self.samantha, 9999)
 
         self.assertEqual(status_code, 404, "Expected status code to be 404 for a non-existent appointment.")
         self.assertEqual(error_message, _("Appointment does not exist."))
 
     def test_unauthorized_user(self):
         """A user who doesn't own the appointment cannot view it."""
         # Fetch data for an appointment that user2 doesn't own
-        x, y, error_message, status_code = prepare_appointment_display_data(self.client1, self.appointment.id)
+        x, y, error_message, status_code = prepare_appointment_display_data(self.georges, self.appointment.id)
 
         self.assertEqual(status_code, 403, "Expected status code to be 403 for an unauthorized user.")
         self.assertEqual(error_message, _("You are not authorized to view this appointment."))
 
     def test_authorized_user(self):
         """An authorized user can view the appointment."""
         # Fetch data for the appointment owned by user1
-        appointment, page_title, error_message, status_code = prepare_appointment_display_data(self.user1,
+        appointment, page_title, error_message, status_code = prepare_appointment_display_data(self.daniel,
                                                                                                self.appointment.id)
 
         self.assertEqual(status_code, 200, "Expected status code to be 200 for an authorized user.")
         self.assertIsNone(error_message)
         self.assertEqual(appointment, self.appointment)
-        self.assertTrue(self.client1.first_name in page_title)
+        self.assertTrue(self.georges.first_name in page_title)
 
     def test_superuser(self):
         """A superuser can view any appointment and sees the staff member name in the title."""
-        self.user1.is_superuser = True
-        self.user1.save()
+
+        jack = self.users['superuser']
+        jack.is_superuser = True
+        jack.save()
 
         # Fetch data for the appointment as a superuser
-        appointment, page_title, error_message, status_code = prepare_appointment_display_data(self.user1,
+        appointment, page_title, error_message, status_code = prepare_appointment_display_data(jack,
                                                                                                self.appointment.id)
 
         self.assertEqual(status_code, 200, "Expected status code to be 200 for a superuser.")
         self.assertIsNone(error_message)
         self.assertEqual(appointment, self.appointment)
-        self.assertTrue(self.client1.first_name in page_title)
-        self.assertTrue(self.user1.first_name in page_title)
+        self.assertTrue(self.georges.first_name in page_title)
+        self.assertTrue(self.daniel.first_name in page_title)
 
 
 class PrepareUserProfileDataTests(BaseTest):
 
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
+        self.jack = self.users['superuser']
+        self.jack.is_superuser = True
+        self.jack.save()
 
     def test_superuser_without_staff_user_id(self):
         """A superuser without a staff_user_id should see the staff list page."""
-        self.user1.is_superuser = True
-        self.user1.save()
-        data = prepare_user_profile_data(self.user1, None)
+        data = prepare_user_profile_data(self.jack, None)
         self.assertFalse(data['error'])
         self.assertEqual(data['template'], 'administration/staff_list.html')
         self.assertIn('btn_staff_me', data['extra_context'])
 
     def test_regular_user_with_mismatched_staff_user_id(self):
         """A regular user cannot view another user's profile."""
-        data = prepare_user_profile_data(self.user1, self.user2.pk)
+        data = prepare_user_profile_data(self.jack, self.users['client2'].pk)
         self.assertTrue(data['error'])
         self.assertEqual(data['status_code'], 403)
 
     def test_superuser_with_non_existent_staff_user_id(self):
         """A superuser with a non-existent staff_user_id cannot view the staff's profile."""
-        self.user1.is_superuser = True
-        self.user1.save()
-        data = prepare_user_profile_data(self.user1, 9999)
+        data = prepare_user_profile_data(self.jack, 9999)
         self.assertTrue(data['error'])
         self.assertEqual(data['status_code'], 403)
 
     def test_regular_user_with_matching_staff_user_id(self):
         """A regular user can view their own profile."""
-        data = prepare_user_profile_data(self.user1, self.user1.pk)
+        data = prepare_user_profile_data(self.users['staff1'], self.staff_member1.pk)
         self.assertFalse(data['error'])
         self.assertEqual(data['template'], 'administration/user_profile.html')
         self.assertIn('user', data['extra_context'])
-        self.assertEqual(data['extra_context']['user'], self.user1)
+        self.assertEqual(data['extra_context']['user'], self.users['staff1'])
 
     def test_regular_user_with_non_existent_staff_user_id(self):
         """A regular user with a non-existent staff_user_id cannot view their profile."""
-        data = prepare_user_profile_data(self.user1, 9999)
+        data = prepare_user_profile_data(self.jack, 9999)
         self.assertTrue(data['error'])
         self.assertEqual(data['status_code'], 403)
 
 
 class HandleEntityManagementRequestTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
     def setUp(self):
         super().setUp()
         self.client = Client()
         self.factory = RequestFactory()
 
         # Setup request object
         self.request = self.factory.post('/')
-        self.request.user = self.user1
+        self.request.user = self.staff_member1.user
+
+    def tearDown(self):
+        WorkingHours.objects.all().delete()
+        super().tearDown()
 
     def test_staff_member_none(self):
         """A day off cannot be created for a staff member that doesn't exist."""
         response = handle_entity_management_request(self.request, None, 'day_off')
         self.assertEqual(response.status_code, 403)
 
     def test_day_off_get(self):
@@ -240,38 +331,50 @@
                                                     staff_user_id=self.staff_member1.user.id,
                                                     instance=working_hours_instance)
         content = json.loads(response.content)
         self.assertTrue(content['success'])
 
 
 class HandleWorkingHoursFormTest(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
     def setUp(self):
         super().setUp()
 
+    def tearDown(self):
+        WorkingHours.objects.all().delete()
+        super().tearDown()
+
     def test_add_working_hours(self):
         """Test if working hours can be added."""
         response = handle_working_hours_form(self.staff_member1, 1, '09:00 AM', '05:00 PM', True)
         self.assertEqual(response.status_code, 200)
 
     def test_update_working_hours(self):
         """Test if working hours can be updated."""
         wh = WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=2, start_time='09:00',
                                          end_time='17:00')
         response = handle_working_hours_form(self.staff_member1, 3, '10:00 AM', '06:00 PM', False, wh_id=wh.id)
         self.assertEqual(response.status_code, 200)
 
     def test_invalid_data(self):
-        """If the form is invalid, the function should return a JsonResponse with appropriate error message."""
+        """If the form is invalid, the function should return a JsonResponse with the appropriate error message."""
         response = handle_working_hours_form(None, 1, '09:00 AM', '05:00 PM', True)  # Missing staff_member
         self.assertEqual(response.status_code, 400)
         self.assertFalse(json.loads(response.getvalue())['success'])
 
     def test_invalid_time(self):
-        """If the start time is after the end time, the function should return a JsonResponse with appropriate error"""
+        """If the start time is after the end time, the function should return a JsonResponse with the
+        appropriate error"""
         response = handle_working_hours_form(self.staff_member1, 1, '05:00 PM', '09:00 AM', True)
         self.assertEqual(response.status_code, 400)
         content = json.loads(response.getvalue())
         self.assertEqual(content['errorCode'], 5)
         self.assertFalse(content['success'])
 
     def test_working_hours_conflict(self):
@@ -281,23 +384,24 @@
         response = handle_working_hours_form(self.staff_member1, 4, '10:00 AM', '06:00 PM', True)
         self.assertEqual(response.status_code, 400)
         content = json.loads(response.getvalue())
         self.assertEqual(content['errorCode'], 11)
         self.assertFalse(content['success'])
 
     def test_invalid_working_hours_id(self):
-        """If the working hours ID is invalid, the function should return a JsonResponse with appropriate error"""
+        """If the working hours ID is invalid, the function should return a JsonResponse with the appropriate error"""
         response = handle_working_hours_form(self.staff_member1, 1, '10:00 AM', '06:00 PM', False, wh_id=9999)
         self.assertEqual(response.status_code, 400)
         content = json.loads(response.getvalue())
         self.assertEqual(content['success'], False)
         self.assertEqual(content['errorCode'], 10)
 
     def test_no_working_hours_id(self):
-        """If the working hours ID is not provided, the function should return a JsonResponse with appropriate error"""
+        """If the working hours ID is not provided, the function should return a JsonResponse with the
+        appropriate error"""
         response = handle_working_hours_form(self.staff_member1, 1, '10:00 AM', '06:00 PM', False)
         self.assertEqual(response.status_code, 400)
         content = json.loads(response.getvalue())
         self.assertEqual(content['success'], False)
         self.assertEqual(content['errorCode'], 5)
 
 
@@ -329,29 +433,37 @@
         self.assertEqual(response.status_code, 400)
         content = json.loads(response.content)
         self.assertFalse(content['success'])
 
 
 class SaveAppointmentTests(BaseTest):
 
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
 
         # Assuming self.create_default_appointment creates an appointment with default values
-        self.appt = self.create_appointment_for_user1()
+        self.appt = self.create_appt_for_sm1()
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
 
     def test_save_appointment(self):
         """Test if an appointment can be saved with valid data."""
-        client_name = "New Client Name"
-        client_email = "newclient@example.com"
+        client_name = "Teal'c of Chulak"
+        client_email = "tealc@chulak.com"
         start_time_str = "10:00 AM"
         phone_number = "+1234567890"
-        client_address = "123 New St, TestCity"
+        client_address = "123 Stargate Command, Cheyenne Mountain"
         service_id = self.service2.id
         staff_member_id = self.staff_member2.id
 
         # Call the function
         updated_appt = save_appointment(self.appt, client_name, client_email, start_time_str, phone_number,
                                         client_address, service_id, self.request, staff_member_id)
 
@@ -371,16 +483,16 @@
 
 
 class SaveApptDateTimeTests(BaseTest):
 
     def setUp(self):
         super().setUp()
 
-        # Assuming create_appointment_for_user1 creates an appointment for user1 with default values
-        self.appt = self.create_appointment_for_user1()
+        # Assuming create_appt_for_sm1 creates an appointment for user1 with default values
+        self.appt = self.create_appt_for_sm1()
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
 
     def test_save_appt_date_time(self):
         """Test if an appointment's date and time can be updated."""
         # Given new appointment date and time details
         appt_start_time_str = "10:00:00.000000Z"
@@ -409,23 +521,30 @@
     """
     Get the date of the next weekday from the given date.
     This function uses python's weekday format, where Monday is 0, and Sunday is 6.
     Remember that in my implementation for work days, I had to use a custom one where Monday is 1, and Sunday is 0.
     So in the setup, I will use my format to create day-offs, working hours, etc. But when calling this function, I will
     use the python format.
     """
-    days_of_week = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]
     days_ahead = weekday - d.weekday()
     if days_ahead <= 0:  # Target day already happened this week
         days_ahead += 7
     next_day = d + datetime.timedelta(days_ahead)
     return next_day
 
 
-class GetAvailableSlotsTests(BaseTest):
+class GetAvailableSlotsForStaffTests(BaseTest):
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
     def setUp(self):
         super().setUp()
         cache.clear()
         self.today = datetime.date.today()
         # Staff member1 works only on Mondays and Wednesday (day_of_week: 1, 3)
         self.wh1 = WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=1,
@@ -440,14 +559,22 @@
         self.next_friday = get_next_weekday(self.today, 4)
         self.next_saturday = get_next_weekday(self.today, 5)
         self.next_sunday = get_next_weekday(self.today, 6)
         DayOff.objects.create(staff_member=self.staff_member1, start_date=self.next_monday, end_date=self.next_monday)
         Config.objects.create(slot_duration=60, lead_time=datetime.time(9, 0), finish_time=datetime.time(17, 0),
                               appointment_buffer_time=0)
 
+    @override_settings(DEBUG=True)
+    def tearDown(self):
+        WorkingHours.objects.all().delete()
+        DayOff.objects.all().delete()
+        Config.objects.all().delete()
+        cache.clear()
+        super().tearDown()
+
     def test_day_off(self):
         """Test if a day off is handled correctly when getting available slots."""
         # Ask for slots for it, and it should return an empty list since next Monday is a day off
         slots = get_available_slots_for_staff(self.next_monday, self.staff_member1)
         self.assertEqual(slots, [])
 
     def test_staff_does_not_work(self):
@@ -483,176 +610,197 @@
         end_time = datetime.time(11, 0)
 
         # Create an appointment request for that time
         appt_request = self.create_appointment_request_(service=self.service1, staff_member=self.staff_member1,
                                                         date_=self.next_wednesday, start_time=start_time,
                                                         end_time=end_time)
         # Create an appointment using that request
-        self.create_appointment_(user=self.client1, appointment_request=appt_request)
+        self.create_appointment_(user=self.users['client1'], appointment_request=appt_request)
 
         # Now, the staff member should not have that slot available
         slots = get_available_slots_for_staff(self.next_wednesday, self.staff_member1)
         expected_slots = [
             datetime.datetime(self.next_wednesday.year, self.next_wednesday.month, self.next_wednesday.day, hour, 0) for
             hour in range(9, 17) if hour != 10]
         self.assertEqual(slots, expected_slots)
 
+    @override_settings(DEBUG=True)
     def test_no_working_hours(self):
         """If a staff member doesn't have working hours on a given day, no slots should be available."""
         # Let's ask for slots on a Thursday, which the staff member doesn't work
         # Let's remove the config object also since it may contain default working days
         Config.objects.all().delete()
         # Now no slots should be available
         slots = get_available_slots_for_staff(self.next_thursday, self.staff_member1)
         self.assertEqual(slots, [])
 
 
 class UpdatePersonalInfoServiceTest(BaseTest):
 
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
+        self.daniel = self.users['staff1']
         self.post_data_valid = {
             'first_name': 'UpdatedName',
             'last_name': 'UpdatedLastName',
-            'email': self.user1.email
+            'email': self.daniel.email
         }
 
     def test_update_name(self):
         """Test if the user's name can be updated."""
         user, is_valid, error_message = update_personal_info_service(self.staff_member1.user.id, self.post_data_valid,
-                                                                     self.user1)
+                                                                     self.daniel)
         self.assertTrue(is_valid)
         self.assertIsNone(error_message)
         self.assertEqual(user.first_name, 'UpdatedName')
         self.assertEqual(user.last_name, 'UpdatedLastName')
 
     def test_update_invalid_user_id(self):
         """Updating a user that doesn't exist should return an error message."""
         user, is_valid, error_message = update_personal_info_service(9999, self.post_data_valid,
-                                                                     self.user1)  # Assuming 9999 is an invalid user ID
+                                                                     self.daniel)  # Assuming 9999 is an invalid user ID
 
         self.assertFalse(is_valid)
         self.assertEqual(error_message, _("User not found."))
         self.assertIsNone(user)
 
     def test_invalid_form(self):
         """Updating a user with invalid form data should return an error message."""
-        user, is_valid, error_message = update_personal_info_service(self.staff_member1.user.id, {}, self.user1)
+        user, is_valid, error_message = update_personal_info_service(self.staff_member1.user.id, {}, self.daniel)
         self.assertFalse(is_valid)
         self.assertEqual(error_message, _("Empty fields are not allowed."))
 
     def test_invalid_form_(self):
         """Updating a user with invalid form data should return an error message."""
         # remove email in post_data
         del self.post_data_valid['email']
         user, is_valid, error_message = update_personal_info_service(self.staff_member1.user.id, self.post_data_valid,
-                                                                     self.user1)
+                                                                     self.daniel)
         self.assertFalse(is_valid)
         self.assertEqual(error_message, "email: This field is required.")
 
 
 class EmailChangeVerificationServiceTest(BaseTest):
 
     def setUp(self):
         super().setUp()
-        self.valid_code = EmailVerificationCode.generate_code(self.client1)
+        self.georges = self.users['client1']
+        self.valid_code = EmailVerificationCode.generate_code(self.georges)
         self.invalid_code = "INVALID_CODE456"
 
-        self.old_email = self.client1.email
-        self.new_email = "newemail@gmail.com"
+        self.old_email = self.georges.email
+        self.new_email = "georges.hammond@django-appointment.com"
 
     def test_valid_code_and_email(self):
         """Test if a valid code and email can be verified."""
         is_verified = email_change_verification_service(self.valid_code, self.new_email, self.old_email)
 
         self.assertTrue(is_verified)
-        self.client1.refresh_from_db()  # Refresh the user object to get the updated email
-        self.assertEqual(self.client1.email, self.new_email)
+        self.georges.refresh_from_db()  # Refresh the user object to get the updated email
+        self.assertEqual(self.georges.email, self.new_email)
 
     def test_invalid_code(self):
         """If the code is invalid, the email should not be updated."""
         is_verified = email_change_verification_service(self.invalid_code, self.new_email, self.old_email)
 
         self.assertFalse(is_verified)
-        self.client1.refresh_from_db()
-        self.assertEqual(self.client1.email, self.old_email)  # Email should not change
+        self.georges.refresh_from_db()
+        self.assertEqual(self.georges.email, self.old_email)  # Email should not change
 
     def test_valid_code_no_user(self):
         """If the code is valid but the user doesn't exist, the email should not be updated."""
         is_verified = email_change_verification_service(self.valid_code, self.new_email, "nonexistent@gmail.com")
 
         self.assertFalse(is_verified)
 
     def test_code_doesnt_match_users_code(self):
         """If the code is valid but doesn't match the user's code, the email should not be updated."""
         # Using valid code but for another user
-        is_verified = email_change_verification_service(self.valid_code, self.new_email, "anotheremail@gmail.com")
+        is_verified = email_change_verification_service(self.valid_code, self.new_email,
+                                                        "g.hammond@django-appointment.com")
 
         self.assertFalse(is_verified)
 
 
 class CreateStaffMemberServiceTest(BaseTest):
 
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.factory = RequestFactory()
 
         # Setup request object
         self.request = self.factory.post('/')
 
     def test_valid_data(self):
         """Test if a staff member can be created with valid data."""
         post_data = {
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'email': 'john.doe@gmail.com'
+            'first_name': 'Catherine',
+            'last_name': 'Langford',
+            'email': 'catherine.langford@django-appointment.com'
         }
+
         user, success, error_message = create_staff_member_service(post_data, self.request)
 
         self.assertTrue(success)
         self.assertIsNotNone(user)
-        self.assertEqual(user.first_name, 'John')
-        self.assertEqual(user.last_name, 'Doe')
-        self.assertEqual(user.email, 'john.doe@gmail.com')
+        self.assertEqual(user.first_name, 'Catherine')
+        self.assertEqual(user.last_name, 'Langford')
+        self.assertEqual(user.email, 'catherine.langford@django-appointment.com')
         self.assertTrue(StaffMember.objects.filter(user=user).exists())
 
     def test_invalid_data(self):
         """Empty fields should not be allowed when creating a staff member."""
         post_data = {
             'first_name': '',  # Missing first name
-            'last_name': 'Doe',
-            'email': 'john.doe@gmail.com'
+            'last_name': 'Langford',
+            'email': 'catherine.langford@django-appointment.com'
         }
         user, success, error_message = create_staff_member_service(post_data, self.request)
 
         self.assertFalse(success)
         self.assertIsNone(user)
         self.assertIsNotNone(error_message)
 
     def test_email_already_exists(self):
         """If the email already exists, the staff member should not be created."""
-        self.create_user_(email="existing@gmail.com")
+        self.create_user_()
         post_data = {
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'email': 'existing@gmail.com'  # Using an email that already exists
+            'first_name': 'Janet',
+            'last_name': 'Fraiser',
+            'email': 'janet.fraiser@django-appointment.com'  # Using an email that already exists
         }
         user, success, error_message = create_staff_member_service(post_data, self.request)
 
         self.assertFalse(success)
         self.assertIsNone(user)
         self.assertEqual(error_message, "email: This email is already taken.")
 
     @patch('appointment.services.send_reset_link_to_staff_member')
     def test_send_reset_link_to_new_staff_member(self, mock_send_reset_link):
         """Test if a reset password link is sent to a new staff member."""
         post_data = {
-            'first_name': 'Jane',
-            'last_name': 'Smith',
-            'email': 'jane.smith@gmail.com'
+            'first_name': 'Janet',
+            'last_name': 'Fraiser',
+            'email': 'janet.fraiser@django-appointment.com'
         }
         user, success, _ = create_staff_member_service(post_data, self.request)
         self.assertTrue(success)
         self.assertIsNotNone(user)
 
         # Check that the mock_send_reset_link function was called once
         mock_send_reset_link.assert_called_once_with(user, self.request, user.email)
@@ -662,46 +810,46 @@
 
     def setUp(self):
         super().setUp()
 
     def test_create_new_service(self):
         """Test if a new service can be created with valid data."""
         post_data = {
-            'name': 'Test Service',
+            'name': "Goa'uld extraction",
             'duration': '1:00:00',
-            'price': '100',
+            'price': '10000',
             'currency': 'USD',
-            'down_payment': '50',
+            'down_payment': '5000',
         }
         service, success, message = handle_service_management_request(post_data)
         self.assertTrue(success)
         self.assertIsNotNone(service)
-        self.assertEqual(service.name, 'Test Service')
+        self.assertEqual(service.name, "Goa'uld extraction")
         self.assertEqual(service.duration, datetime.timedelta(hours=1))
-        self.assertEqual(service.price, Decimal('100'))
-        self.assertEqual(service.down_payment, Decimal('50'))
+        self.assertEqual(service.price, Decimal('10000'))
+        self.assertEqual(service.down_payment, Decimal('5000'))
         self.assertEqual(service.currency, 'USD')
 
     def test_update_existing_service(self):
         """Test if an existing service can be updated with valid data."""
         existing_service = self.create_service_()
         post_data = {
-            'name': 'Updated Service Name',
+            'name': 'Quantum Mirror Repair',
             'duration': '2:00:00',
-            'price': '150',
-            'down_payment': '75',
+            'price': '15000',
+            'down_payment': '7500',
             'currency': 'EUR'
         }
         service, success, message = handle_service_management_request(post_data, service_id=existing_service.id)
 
         self.assertTrue(success)
         self.assertIsNotNone(service)
-        self.assertEqual(service.name, 'Updated Service Name')
+        self.assertEqual(service.name, 'Quantum Mirror Repair')
         self.assertEqual(service.duration, datetime.timedelta(hours=2))
-        self.assertEqual(service.price, Decimal('150'))
+        self.assertEqual(service.price, Decimal('15000'))
         self.assertEqual(service.currency, 'EUR')
 
     def test_invalid_data(self):
         """Empty fields should not be allowed when creating a service."""
         post_data = {
             'name': '',  # Missing name
             'duration': '1:00:00',
@@ -714,17 +862,87 @@
         self.assertFalse(success)
         self.assertIsNone(service)
         self.assertEqual(message, "name: This field is required.")
 
     def test_service_not_found(self):
         """If the service ID is invalid, the service should not be updated."""
         post_data = {
-            'name': 'Another Test Service',
+            'name': 'DHD maintenance',
             'duration': '1:00:00',
-            'price': '100',
+            'price': '10000',
             'currency': 'USD'
         }
         service, success, message = handle_service_management_request(post_data, service_id=9999)  # Invalid service_id
 
         self.assertFalse(success)
         self.assertIsNone(service)
-        self.assertIn(_("Service matching query does not exist"), message)
+        self.assertIn(str(_("Service matching query does not exist")), str(message))
+
+
+class GetFinishButtonTextTests(BaseTest):
+    """Test cases for get_finish_button_text"""
+
+    def test_get_finish_button_text_free_service(self):
+        button_text = get_finish_button_text(self.service1)
+        self.assertEqual(button_text, _("Finish"))
+
+    def test_get_finish_button_text_paid_service(self):
+        with patch('appointment.services.APPOINTMENT_PAYMENT_URL', 'https://payment.com'):
+            button_text = get_finish_button_text(self.service1)
+            self.assertEqual(button_text, _("Pay Now"))
+
+
+class SlotAvailabilityTest(BaseTest, ConfigMixin):
+
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        self.service = self.create_service_(duration=timedelta(hours=2))
+        self.config = self.create_config_(lead_time=time(11, 0), finish_time=time(15, 0), slot_duration=120)
+        self.test_date = date.today() + timedelta(days=1)  # Use tomorrow's date for the tests
+
+    @override_settings(DEBUG=True)
+    def tearDown(self):
+        self.service.delete()
+        cache.clear()
+
+    def test_slot_availability_without_appointments(self):
+        """Test if the available slots are correct when there are no appointments."""
+        _, available_slots = get_appointments_and_slots(self.test_date, self.service)
+        expected_slots = ['11:00 AM', '01:00 PM']
+        self.assertEqual(available_slots, expected_slots)
+
+    def test_slot_availability_with_first_slot_booked(self):
+        """Available slots (total 2) should be one when the first slot is booked."""
+        self.ar = self.create_appt_request_for_sm1(service=self.service, date_=self.test_date, start_time=time(11, 0),
+                                                   end_time=time(13, 0))
+        self.create_appt_for_sm1(appointment_request=self.ar)
+        _, available_slots = get_appointments_and_slots(self.test_date, self.service)
+        expected_slots = ['01:00 PM']
+        self.assertEqual(available_slots, expected_slots)
+
+    def test_slot_availability_with_second_slot_booked(self):
+        """Available slots (total 2) should be one when the second slot is booked."""
+        self.ar = self.create_appt_request_for_sm1(service=self.service, date_=self.test_date, start_time=time(13, 0),
+                                                   end_time=time(15, 0))
+        self.create_appt_for_sm1(appointment_request=self.ar)
+        _, available_slots = get_appointments_and_slots(self.test_date, self.service)
+        expected_slots = ['11:00 AM']
+        self.assertEqual(available_slots, expected_slots)
+
+    def test_slot_availability_with_both_slots_booked(self):
+        """Available slots (total 2) should be zero when both slots are booked."""
+        self.ar1 = self.create_appt_request_for_sm1(service=self.service, date_=self.test_date, start_time=time(11, 0),
+                                                    end_time=time(13, 0))
+        self.ar2 = self.create_appt_request_for_sm1(service=self.service, date_=self.test_date, start_time=time(13, 0),
+                                                    end_time=time(15, 0))
+        self.create_appt_for_sm1(appointment_request=self.ar1)
+        self.create_appt_for_sm1(appointment_request=self.ar2)
+        _, available_slots = get_appointments_and_slots(self.test_date, self.service)
+        expected_slots = []
+        self.assertEqual(available_slots, expected_slots)
```

### Comparing `django-appointment-3.4.1/appointment/tests/test_settings.py` & `django_appointment-3.5.0/appointment/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/tests/test_views.py` & `django_appointment-3.5.0/appointment/tests/test_views.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,193 +16,175 @@
 from django.test.client import RequestFactory
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.encoding import force_bytes
 from django.utils.http import urlsafe_base64_encode
 from django.utils.translation import gettext as _
 
+from appointment.forms import StaffMemberForm
 from appointment.messages_ import passwd_error
 from appointment.models import (
     Appointment, AppointmentRequest, AppointmentRescheduleHistory, Config, DayOff, EmailVerificationCode,
     PasswordResetToken, StaffMember
 )
 from appointment.tests.base.base_test import BaseTest
 from appointment.utils.db_helpers import Service, WorkingHours, create_user_with_username
 from appointment.utils.error_codes import ErrorCode
 from appointment.views import (
-    create_appointment, get_appointment_data_from_post_request, get_client_data_from_post,
-    redirect_to_payment_or_thank_you_page, verify_user_and_login
+    create_appointment, redirect_to_payment_or_thank_you_page, verify_user_and_login
 )
 
 
-class ViewsTestCase(BaseTest):
+class SlotTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.client = Client()
-        self.factory = RequestFactory()
-        self.staff_member = self.staff_member1
-        WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=0,
-                                    start_time=datetime.time(8, 0), end_time=datetime.time(12, 0))
-        WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=2,
-                                    start_time=datetime.time(8, 0), end_time=datetime.time(12, 0))
-        self.ar = self.create_appt_request_for_sm1()
-        self.request = self.factory.get('/')
-        self.user1.is_staff = True
-        self.request.user = self.user1
-        middleware = SessionMiddleware(lambda req: None)
-        middleware.process_request(self.request)
-        self.request.session.save()
-
-        middleware = MessageMiddleware(lambda req: None)
-        middleware.process_request(self.request)
-        self.request.session.save()
-        self.appointment = self.create_appointment_for_user1()
-        self.tomorrow = date.today() + timedelta(days=1)
-        self.appt = self.create_appointment_for_user1()
-        self.data = {
-            'isCreating': False, 'service_id': '1', 'appointment_id': self.appt.id, 'client_name': 'Bryan Zap',
-            'client_email': 'bz@gmail.com', 'client_phone': '+33769992738', 'client_address': 'Naples, Florida',
-            'want_reminder': 'false', 'additional_info': '', 'start_time': '15:00:26', 'staff_id': self.staff_member.id,
-            'date': self.tomorrow.strftime('%Y-%m-%d')
-        }
-        self.url_display_appt = reverse('appointment:display_appointment', args=[self.appointment.id])
-        self.url_add_day_off = reverse('appointment:add_day_off', args=[self.staff_member.user_id])
-        self.other_staff_member = self.staff_member2
-        self.day_off = DayOff.objects.create(staff_member=self.staff_member,
-                                             start_date=date.today() + timedelta(days=1),
-                                             end_date=date.today() + timedelta(days=2), description="Day off")
-        self.random_user = self.create_user_()
-
-    def need_normal_login(self):
-        self.client.force_login(self.random_user)
-
-    def need_staff_login(self, user=None):
-        if user is not None:
-            user.is_staff = True
-            user.save()
-            self.client.force_login(user)
-        self.user1.is_staff = True
-        self.user1.save()
-        self.client.force_login(self.user1)
-
-    def need_superuser_login(self):
-        self.user1.is_superuser = True
-        self.user1.save()
-        self.client.force_login(self.user1)
-
-    def clean_staff_member_objects(self):
-        """Delete all AppointmentRequests and Appointments linked to the StaffMember instance of self.user1."""
-        AppointmentRequest.objects.filter(staff_member__user=self.user1).delete()
-        Appointment.objects.filter(appointment_request__staff_member__user=self.user1).delete()
-
-    def remove_staff_member(self):
-        """Remove the StaffMember instance of self.user1."""
-        self.clean_staff_member_objects()
-        StaffMember.objects.filter(user=self.user1).delete()
+        self.url = reverse('appointment:available_slots_ajax')
 
     def test_get_available_slots_ajax(self):
         """get_available_slots_ajax view should return a JSON response with available slots for the selected date."""
-        url = reverse('appointment:available_slots_ajax')
-        response = self.client.get(url, {'selected_date': date.today().isoformat()},
+        response = self.client.get(self.url, {'selected_date': date.today().isoformat(), 'staff_member': '1'},
                                    HTTP_X_REQUESTED_WITH='XMLHttpRequest')
-        self.assertEqual(response.status_code, 403)
+        print(f"response: {response.content}")
+        self.assertEqual(response.status_code, 200)
         response_data = response.json()
         self.assertIn('date_chosen', response_data)
         self.assertIn('available_slots', response_data)
         self.assertFalse(response_data.get('error'))
 
     def test_get_available_slots_ajax_past_date(self):
         """get_available_slots_ajax view should return an error if the selected date is in the past."""
-        url = reverse('appointment:available_slots_ajax')
         past_date = (date.today() - timedelta(days=1)).isoformat()
-        response = self.client.get(url, {'selected_date': past_date}, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+        response = self.client.get(self.url, {'selected_date': past_date}, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.json()['error'], True)
         self.assertEqual(response.json()['message'], 'Date is in the past')
 
-    def test_get_next_available_date_ajax(self):
-        """get_next_available_date_ajax view should return a JSON response with the next available date."""
-        data = {'staff_id': self.staff_member.id}
-        url = reverse('appointment:request_next_available_slot', args=[self.service1.id])
-        response = self.client.get(url, data=data, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
-        self.assertEqual(response.status_code, 200)
-        response_data = json.loads(response.content)
-        self.assertIsNotNone(response_data)
-        self.assertIsNotNone(response_data['next_available_date'])
+
+class AppointmentRequestTestCase(BaseTest):
+    def setUp(self):
+        super().setUp()
+        self.url = reverse('appointment:appointment_request_submit')
 
     def test_appointment_request(self):
         """Test if the appointment request form can be rendered."""
         url = reverse('appointment:appointment_request', args=[self.service1.id])
         response = self.client.get(url)
         self.assertEqual(response.status_code, 200)
         self.assertIn(self.service1.name, str(response.content))
         self.assertIn('all_staff_members', response.context)
         self.assertIn('service', response.context)
 
     def test_appointment_request_submit_valid(self):
         """Test if a valid appointment request can be submitted."""
-        url = reverse('appointment:appointment_request_submit')
         post_data = {
             'date': date.today().isoformat(),
             'start_time': time(9, 0),
             'end_time': time(10, 0),
             'service': self.service1.id,
-            'staff_member': self.staff_member.id,
+            'staff_member': self.staff_member1.id,
         }
-        response = self.client.post(url, post_data)
+        response = self.client.post(self.url, post_data)
         self.assertEqual(response.status_code, 302)  # Redirect status
         # Check if an AppointmentRequest object was created
         self.assertTrue(AppointmentRequest.objects.filter(service=self.service1).exists())
 
     def test_appointment_request_submit_invalid(self):
         """Test if an invalid appointment request can be submitted."""
-        url = reverse('appointment:appointment_request_submit')
         post_data = {}  # Missing required data
-        response = self.client.post(url, post_data)
+        response = self.client.post(self.url, post_data)
         self.assertEqual(response.status_code, 200)  # Rendering the form with errors
         self.assertIn('form', response.context)
         self.assertTrue(response.context['form'].errors)  # Ensure there are form errors
 
+
+class VerificationCodeTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        super().setUp()
+        self.daniel = self.users['staff1']
+        self.factory = RequestFactory()
+        self.request = self.factory.get('/')
+
+        # Simulate session middleware
+        middleware = SessionMiddleware(lambda req: None)
+        middleware.process_request(self.request)
+        self.request.session.save()
+
+        # Attach message storage
+        middleware = MessageMiddleware(lambda req: None)
+        middleware.process_request(self.request)
+        self.request.session.save()
+
+        self.ar = self.create_appt_request_for_sm1()
+        self.url = reverse('appointment:enter_verification_code', args=[self.ar.id, self.ar.id_request])
+
     def test_verify_user_and_login_valid(self):
         """Test if a user can be verified and logged in."""
-        code = EmailVerificationCode.generate_code(user=self.user1)
-        result = verify_user_and_login(self.request, self.user1, code)
+        code = EmailVerificationCode.generate_code(user=self.daniel)
+        result = verify_user_and_login(self.request, self.daniel, code)
         self.assertTrue(result)
 
     def test_verify_user_and_login_invalid(self):
         """Test if a user cannot be verified and logged in with an invalid code."""
         invalid_code = '000000'  # An invalid code
-        result = verify_user_and_login(self.request, self.user1, invalid_code)
+        result = verify_user_and_login(self.request, self.daniel, invalid_code)
         self.assertFalse(result)
 
     def test_enter_verification_code_valid(self):
         """Test if a valid verification code can be entered."""
-        code = EmailVerificationCode.generate_code(user=self.user1)
-        url = reverse('appointment:enter_verification_code', args=[self.ar.id, self.ar.id_request])
+        code = EmailVerificationCode.generate_code(user=self.daniel)
         post_data = {'code': code}  # Assuming a valid code for the test setup
-        response = self.client.post(url, post_data)
+        response = self.client.post(self.url, post_data)
         self.assertEqual(response.status_code, 200)
 
     def test_enter_verification_code_invalid(self):
         """Test if an invalid verification code can be entered."""
-        url = reverse('appointment:enter_verification_code', args=[self.ar.id, self.ar.id_request])
         post_data = {'code': '000000'}  # Invalid code
-        response = self.client.post(url, post_data)
+        response = self.client.post(self.url, post_data)
         self.assertEqual(response.status_code, 200)  # Stay on the same page
         # Check for an error message
         messages_list = list(messages.get_messages(response.wsgi_request))
         self.assertIn(_("Invalid verification code."), [str(msg) for msg in messages_list])
 
-    def test_default_thank_you(self):
-        """Test if the default thank you page can be rendered."""
-        appointment = Appointment.objects.create(client=self.user1, appointment_request=self.ar)
-        url = reverse('appointment:default_thank_you', args=[appointment.id])
-        response = self.client.get(url)
-        self.assertEqual(response.status_code, 200)
-        self.assertIn(appointment.get_service_name(), str(response.content))
+
+class StaffMemberTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        super().setUp()
+        self.user1 = self.users['staff1']
+        self.staff_member = self.staff_member1
+        self.appointment = self.create_appt_for_sm1()
+
+    def remove_staff_member(self):
+        """Remove the StaffMember instance of self.user1."""
+        self.clean_staff_member_objects()
+        StaffMember.objects.filter(user=self.user1).delete()
 
     def test_staff_user_without_staff_member_instance(self):
         """Test that a staff user without a staff member instance receives an appropriate error message."""
         self.clean_staff_member_objects()
 
         # Now safely delete the StaffMember instance
         StaffMember.objects.filter(user=self.user1).delete()
@@ -211,17 +193,125 @@
         self.need_staff_login()
 
         url = reverse('appointment:get_user_appointments')
         response = self.client.get(url)
 
         message_list = list(get_messages(response.wsgi_request))
         self.assertTrue(any(
-            message.message == "User doesn't have a staff member instance. Please contact the administrator." for
-            message in message_list),
-            "Expected error message not found in messages.")
+                message.message == "User doesn't have a staff member instance. Please contact the administrator." for
+                message in message_list),
+                "Expected error message not found in messages.")
+
+    def test_remove_staff_member(self):
+        self.need_superuser_login()
+        self.clean_staff_member_objects()
+
+        url = reverse('appointment:remove_staff_member', args=[self.staff_member.user_id])
+        response = self.client.get(url)
+
+        self.assertEqual(response.status_code, 302)  # Redirect status code
+        self.assertRedirects(response, reverse('appointment:user_profile'))
+
+        # Check for success messages
+        messages_list = list(get_messages(response.wsgi_request))
+        self.assertTrue(any(_("Staff member deleted successfully!") in str(message) for message in messages_list))
+
+        # Check if staff member is deleted
+        staff_member_exists = StaffMember.objects.filter(pk=self.staff_member.id).exists()
+        self.assertFalse(staff_member_exists, "Appointment should be deleted but still exists.")
+
+    def test_remove_staff_member_with_superuser(self):
+        self.need_superuser_login()
+        self.clean_staff_member_objects()
+        # Test removal of staff member by a superuser
+        self.jack = self.users['superuser']
+
+        self.client.get(reverse('appointment:make_superuser_staff_member'))
+        response = self.client.get(reverse('appointment:remove_superuser_staff_member'))
+
+        # Check if the StaffMember instance was deleted
+        self.assertFalse(StaffMember.objects.filter(user=self.jack).exists())
+
+        # Check if it redirects to the user profile
+        self.assertRedirects(response, reverse('appointment:user_profile'))
+
+    def test_remove_staff_member_without_superuser(self):
+        # Log out superuser and log in as a regular user
+        self.need_staff_login()
+        response = self.client.get(reverse('appointment:remove_superuser_staff_member'))
+
+        # Check for a forbidden status code, as only superusers should be able to remove staff members
+        self.assertEqual(response.status_code, 403)
+
+    def test_make_staff_member_with_superuser(self):
+        self.need_superuser_login()
+        self.remove_staff_member()
+        self.jack = self.users['superuser']
+        # Test creating a staff member by a superuser
+        response = self.client.get(reverse('appointment:make_superuser_staff_member'))
+
+        # Check if the StaffMember instance was created
+        self.assertTrue(StaffMember.objects.filter(user=self.jack).exists())
+
+        # Check if it redirects to the user profile
+        self.assertRedirects(response, reverse('appointment:user_profile'))
+
+    def test_make_staff_member_without_superuser(self):
+        self.need_staff_login()
+        response = self.client.get(reverse('appointment:make_superuser_staff_member'))
+
+        # Check for a forbidden status code, as only superusers should be able to create staff members
+        self.assertEqual(response.status_code, 403)
+
+    def test_is_user_staff_admin_with_staff_member(self):
+        """Test that a user with a StaffMember instance is identified as a staff member."""
+        self.need_staff_login()
+
+        # Ensure the user has a StaffMember instance
+        if not StaffMember.objects.filter(user=self.user1).exists():
+            StaffMember.objects.create(user=self.user1)
+
+        url = reverse('appointment:is_user_staff_admin')
+        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+
+        # Check the response status code and content
+        self.assertEqual(response.status_code, 200)
+        response_data = response.json()
+        self.assertIn('message', response_data)
+        self.assertEqual(response_data['message'], _("User is a staff member."))
+
+    def test_is_user_staff_admin_without_staff_member(self):
+        """Test that a user without a StaffMember instance is not identified as a staff member."""
+        self.need_staff_login()
+
+        # Ensure the user does not have a StaffMember instance
+        StaffMember.objects.filter(user=self.user1).delete()
+
+        url = reverse('appointment:is_user_staff_admin')
+        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+
+        # Check the response status code and content
+        self.assertEqual(response.status_code, 200)
+        response_data = response.json()
+        self.assertIn('message', response_data)
+        self.assertEqual(response_data['message'], _("User is not a staff member."))
+
+
+class AppointmentTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        super().setUp()
+        self.appointment = self.create_appt_for_sm1()
 
     def test_delete_appointment(self):
         self.need_staff_login()
 
         url = reverse('appointment:delete_appointment', args=[self.appointment.id])
         response = self.client.get(url)
 
@@ -253,15 +343,15 @@
         self.assertFalse(appointment_exists, "Appointment should be deleted but still exists.")
 
     def test_delete_appointment_without_permission(self):
         """Test that deleting an appointment without permission fails."""
         self.need_staff_login()  # Login as a regular staff user
 
         # Try to delete an appointment belonging to a different staff member
-        different_appointment = self.create_appointment_for_user2()
+        different_appointment = self.create_appt_for_sm2()
         url = reverse('appointment:delete_appointment', args=[different_appointment.id])
 
         response = self.client.post(url)
 
         # Check that the user is redirected due to lack of permissions
         self.assertEqual(response.status_code, 403)
 
@@ -269,110 +359,51 @@
         self.assertTrue(Appointment.objects.filter(id=different_appointment.id).exists())
 
     def test_delete_appointment_ajax_without_permission(self):
         """Test that deleting an appointment via AJAX without permission fails."""
         self.need_staff_login()  # Login as a regular staff user
 
         # Try to delete an appointment belonging to a different staff member
-        different_appointment = self.create_appointment_for_user2()
+        different_appointment = self.create_appt_for_sm2()
         url = reverse('appointment:delete_appointment_ajax')
 
         response = self.client.post(url, {'appointment_id': different_appointment.id}, content_type='application/json')
 
         # Check that the response indicates failure due to lack of permissions
         self.assertEqual(response.status_code, 403)
         response_data = response.json()
         self.assertEqual(response_data['message'], _("You can only delete your own appointments."))
         self.assertFalse(response_data['success'])
 
         # Verify that the appointment still exists in the database
         self.assertTrue(Appointment.objects.filter(id=different_appointment.id).exists())
 
-    def test_remove_staff_member(self):
-        self.need_superuser_login()
-        self.clean_staff_member_objects()
 
-        url = reverse('appointment:remove_staff_member', args=[self.staff_member.user_id])
-        response = self.client.get(url)
-
-        self.assertEqual(response.status_code, 302)  # Redirect status code
-        self.assertRedirects(response, reverse('appointment:user_profile'))
+class UpdateAppointmentTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
-        # Check for success messages
-        messages_list = list(get_messages(response.wsgi_request))
-        self.assertTrue(any(_("Staff member deleted successfully!") in str(message) for message in messages_list))
-
-        # Check if staff member is deleted
-        staff_member_exists = StaffMember.objects.filter(pk=self.staff_member.id).exists()
-        self.assertFalse(staff_member_exists, "Appointment should be deleted but still exists.")
-
-    def test_fetch_service_list_for_staff(self):
-        self.need_staff_login()
-
-        # Assuming self.service1 and self.service2 are services linked to self.staff_member1
-        self.staff_member1.services_offered.add(self.service1, self.service2)
-        staff_member_services = [self.service1, self.service2]
-
-        # Simulate a request without appointmentId
-        url = reverse('appointment:fetch_service_list_for_staff')
-        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
-        self.assertEqual(response.status_code, 200)
-        response_data = response.json()
-        self.assertEqual(response_data["message"], "Successfully fetched services.")
-        self.assertCountEqual(
-            response_data["services_offered"],
-            [{"id": service.id, "name": service.name} for service in staff_member_services]
-        )
-
-        # Create a test appointment and link it to self.staff_member1
-        test_appointment = self.create_appointment_for_user1()
-
-        # Simulate a request with appointmentId
-        url_with_appointment = f"{url}?appointmentId={test_appointment.id}"
-        response_with_appointment = self.client.get(url_with_appointment, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
-        self.assertEqual(response_with_appointment.status_code, 200)
-        response_data_with_appointment = response_with_appointment.json()
-        self.assertEqual(response_data_with_appointment["message"], "Successfully fetched services.")
-        # Assuming the staff member linked to the appointment offers the same services
-        self.assertCountEqual(
-            response_data_with_appointment["services_offered"],
-            [{"id": service.id, "name": service.name} for service in staff_member_services]
-        )
-
-    def test_fetch_service_list_for_staff_no_staff_member_instance(self):
-        """Test that a superuser without a StaffMember instance receives no inappropriate error message."""
-        self.need_superuser_login()
-
-        # Ensure the superuser does not have a StaffMember instance
-        StaffMember.objects.filter(user=self.user1).delete()
-
-        url = reverse('appointment:fetch_service_list_for_staff')
-        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
-
-        # Check the response status code and content
-        self.assertEqual(response.status_code, 200)
-        response_data = response.json()
-        self.assertIn('message', response_data)
-
-    def test_fetch_service_list_for_staff_no_services_offered(self):
-        """Test fetching services for a staff member who offers no services."""
-        self.need_staff_login()
-
-        # Assuming self.staff_member1 offers no services
-        self.staff_member1.services_offered.clear()
-
-        url = reverse('appointment:fetch_service_list_for_staff')
-        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
-
-        # Check response status code and content
-        self.assertEqual(response.status_code, 404)
-        response_data = response.json()
-        self.assertIn('message', response_data)
-        self.assertEqual(response_data['message'], _("No services offered by this staff member."))
-        self.assertFalse(response_data['success'])
+    def setUp(self):
+        super().setUp()
+        self.appointment = self.create_appt_for_sm1()
+        self.tomorrow = date.today() + timedelta(days=1)
+        self.data = {
+            'isCreating': False, 'service_id': self.service1.pk, 'appointment_id': self.appointment.id,
+            'client_name': 'Vala Mal Doran',
+            'client_email': 'vala.mal-doran@django-appointment.com', 'client_phone': '+12392350345',
+            'client_address': '456 Outer Rim, Free Jaffa Nation',
+            'want_reminder': 'false', 'additional_info': '', 'start_time': '15:00:26',
+            'staff_id': self.staff_member1.id,
+            'date': self.tomorrow.strftime('%Y-%m-%d')
+        }
 
     def test_update_appt_min_info_create(self):
         self.need_staff_login()
 
         # Preparing data
         self.data.update({'isCreating': True, 'appointment_id': None})
         url = reverse('appointment:update_appt_min_info')
@@ -395,14 +426,15 @@
         self.assertTrue(Appointment.objects.filter(id=appointment_id).exists())
 
     def test_update_appt_min_info_update(self):
         self.need_superuser_login()
 
         # Create an appointment to update
         url = reverse('appointment:update_appt_min_info')
+        self.staff_member1.services_offered.add(self.service1)
 
         # Making the request
         response = self.client.post(url, data=json.dumps(self.data), content_type='application/json',
                                     **{'HTTP_X_REQUESTED_WITH': 'XMLHttpRequest'})
         print(f"response: {response.content}")
 
         # Check response status
@@ -411,15 +443,15 @@
         # Check response content
         response_data = response.json()
         self.assertIn('message', response_data)
         self.assertEqual(response_data['message'], 'Appointment updated successfully.')
         self.assertIn('appt', response_data)
 
         # Verify appointment updated in the database
-        updated_appt = Appointment.objects.get(id=self.appt.id)
+        updated_appt = Appointment.objects.get(id=self.appointment.id)
         self.assertEqual(updated_appt.client.email, self.data['client_email'])
 
     def test_update_nonexistent_appointment(self):
         self.need_superuser_login()
 
         # Preparing data with a non-existent appointment ID
         self.data['appointment_id'] = 999
@@ -453,27 +485,106 @@
         self.assertEqual(response_data['message'], "Service does not exist.")
 
     def test_update_with_invalid_data_causing_exception(self):
         self.need_superuser_login()
 
         # Preparing invalid data to trigger an exception, for example here, no email address
         data = {
-            'isCreating': False, 'service_id': '1', 'appointment_id': self.appt.id,
+            'isCreating': False, 'service_id': '1', 'appointment_id': self.appointment.id,
         }
         url = reverse('appointment:update_appt_min_info')
 
         # Making the request
         response = self.client.post(url, data=json.dumps(data), content_type='application/json',
                                     **{'HTTP_X_REQUESTED_WITH': 'XMLHttpRequest'})
 
         # Check response status and content
         self.assertEqual(response.status_code, 400)
         response_data = response.json()
         self.assertIn('message', response_data)
 
+
+class ServiceViewTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        super().setUp()
+
+    def test_fetch_service_list_for_staff(self):
+        self.need_staff_login()
+
+        # Assuming self.service1 and self.service2 are services linked to self.staff_member1
+        self.staff_member1.services_offered.add(self.service1, self.service2)
+        staff_member_services = [self.service1, self.service2]
+
+        # Simulate a request without appointmentId
+        url = reverse('appointment:fetch_service_list_for_staff')
+        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+        self.assertEqual(response.status_code, 200)
+        response_data = response.json()
+        self.assertEqual(response_data["message"], "Successfully fetched services.")
+        self.assertCountEqual(
+                response_data["services_offered"],
+                [{"id": service.id, "name": service.name} for service in staff_member_services]
+        )
+
+        # Create a test appointment and link it to self.staff_member1
+        test_appointment = self.create_appt_for_sm1()
+
+        # Simulate a request with appointmentId
+        url_with_appointment = f"{url}?appointmentId={test_appointment.id}"
+        response_with_appointment = self.client.get(url_with_appointment, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+        self.assertEqual(response_with_appointment.status_code, 200)
+        response_data_with_appointment = response_with_appointment.json()
+        self.assertEqual(response_data_with_appointment["message"], "Successfully fetched services.")
+        # Assuming the staff member linked to the appointment offers the same services
+        self.assertCountEqual(
+                response_data_with_appointment["services_offered"],
+                [{"id": service.id, "name": service.name} for service in staff_member_services]
+        )
+
+    def test_fetch_service_list_for_staff_no_staff_member_instance(self):
+        """Test that a superuser without a StaffMember instance receives no inappropriate error message."""
+        self.need_superuser_login()
+        jack = self.users['superuser']
+
+        # Ensure the superuser does not have a StaffMember instance
+        StaffMember.objects.filter(user=jack).delete()
+
+        url = reverse('appointment:fetch_service_list_for_staff')
+        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+
+        # Check the response status code and content
+        self.assertEqual(response.status_code, 200)
+        response_data = response.json()
+        self.assertIn('message', response_data)
+
+    def test_fetch_service_list_for_staff_no_services_offered(self):
+        """Test fetching services for a staff member who offers no services."""
+        self.need_staff_login()
+
+        # Assuming self.staff_member1 offers no services
+        self.staff_member1.services_offered.clear()
+
+        url = reverse('appointment:fetch_service_list_for_staff')
+        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+
+        # Check response status code and content
+        self.assertEqual(response.status_code, 404)
+        response_data = response.json()
+        self.assertIn('message', response_data)
+        self.assertEqual(response_data['message'], _("No services offered by this staff member."))
+        self.assertFalse(response_data['success'])
+
     def test_delete_service_with_superuser(self):
         self.need_superuser_login()
         # Test deletion with a superuser
         response = self.client.get(reverse('appointment:delete_service', args=[self.service1.id]))
 
         # Check if the service was deleted
         self.assertFalse(Service.objects.filter(id=self.service1.id).exists())
@@ -498,85 +609,28 @@
         self.need_superuser_login()
         # Try to delete a service that does not exist
         response = self.client.get(reverse('appointment:delete_service', args=[99999]))
 
         # Check for a 404-status code
         self.assertEqual(response.status_code, 404)
 
-    def test_remove_staff_member_with_superuser(self):
-        self.need_superuser_login()
-        self.clean_staff_member_objects()
-        # Test removal of staff member by a superuser
-        response = self.client.get(reverse('appointment:remove_superuser_staff_member'))
-
-        # Check if the StaffMember instance was deleted
-        self.assertFalse(StaffMember.objects.filter(user=self.user1).exists())
-
-        # Check if it redirects to the user profile
-        self.assertRedirects(response, reverse('appointment:user_profile'))
-
-    def test_remove_staff_member_without_superuser(self):
-        # Log out superuser and log in as a regular user
-        self.need_staff_login()
-        response = self.client.get(reverse('appointment:remove_superuser_staff_member'))
-
-        # Check for a forbidden status code, as only superusers should be able to remove staff members
-        self.assertEqual(response.status_code, 403)
-
-    def test_make_staff_member_with_superuser(self):
-        self.need_superuser_login()
-        self.remove_staff_member()
-        # Test creating a staff member by a superuser
-        response = self.client.get(reverse('appointment:make_superuser_staff_member'))
-
-        # Check if the StaffMember instance was created
-        self.assertTrue(StaffMember.objects.filter(user=self.user1).exists())
-
-        # Check if it redirects to the user profile
-        self.assertRedirects(response, reverse('appointment:user_profile'))
-
-    def test_make_staff_member_without_superuser(self):
-        self.need_staff_login()
-        response = self.client.get(reverse('appointment:make_superuser_staff_member'))
-
-        # Check for a forbidden status code, as only superusers should be able to create staff members
-        self.assertEqual(response.status_code, 403)
-
-    def test_is_user_staff_admin_with_staff_member(self):
-        """Test that a user with a StaffMember instance is identified as a staff admin."""
-        self.need_staff_login()
-
-        # Ensure the user has a StaffMember instance
-        if not StaffMember.objects.filter(user=self.user1).exists():
-            StaffMember.objects.create(user=self.user1)
-
-        url = reverse('appointment:is_user_staff_admin')
-        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
-
-        # Check the response status code and content
-        self.assertEqual(response.status_code, 200)
-        response_data = response.json()
-        self.assertIn('message', response_data)
-        self.assertEqual(response_data['message'], _("User is a staff member."))
-
-    def test_is_user_staff_admin_without_staff_member(self):
-        """Test that a user without a StaffMember instance is not identified as a staff admin."""
-        self.need_staff_login()
-
-        # Ensure the user does not have a StaffMember instance
-        StaffMember.objects.filter(user=self.user1).delete()
 
-        url = reverse('appointment:is_user_staff_admin')
-        response = self.client.get(url, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+class AppointmentDisplayViewTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
-        # Check the response status code and content
-        self.assertEqual(response.status_code, 200)
-        response_data = response.json()
-        self.assertIn('message', response_data)
-        self.assertEqual(response_data['message'], _("User is not a staff member."))
+    def setUp(self):
+        super().setUp()
+        self.appointment = self.create_appt_for_sm1()
+        self.url_display_appt = reverse('appointment:display_appointment', args=[self.appointment.id])
 
     def test_display_appointment_authenticated_staff_user(self):
         # Log in as staff user
         self.need_staff_login()
         response = self.client.get(self.url_display_appt)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, 'administration/display_appointment.html')
@@ -602,14 +656,24 @@
     def test_display_appointment_non_existent(self):
         # Log in as staff user
         self.need_superuser_login()
         non_existent_url = reverse('appointment:display_appointment', args=[99999])  # Non-existent appointment ID
         response = self.client.get(non_existent_url)
         self.assertEqual(response.status_code, 404)  # Expect 404 error
 
+
+class DayOffViewsTestCase(BaseTest):
+    def setUp(self):
+        super().setUp()
+        self.url_add_day_off = reverse('appointment:add_day_off', args=[self.staff_member1.user_id])
+        self.other_staff_member = self.staff_member2
+        self.day_off = DayOff.objects.create(staff_member=self.staff_member1,
+                                             start_date=date.today() + timedelta(days=1),
+                                             end_date=date.today() + timedelta(days=2), description="Day off")
+
     def test_add_day_off_authenticated_staff_user(self):
         # Log in as staff user
         self.need_staff_login()
         response = self.client.post(self.url_add_day_off, data={'start_date': '2050-01-01', 'end_date': '2050-01-01',
                                                                 'description': 'Test reason'})
         self.assertEqual(response.status_code, 200)  # Assuming success redirects or shows a success message
 
@@ -679,21 +743,132 @@
         self.need_staff_login()
         non_existent_day_off_id = 99999
         url = reverse('appointment:delete_day_off', args=[non_existent_day_off_id])
         response = self.client.get(url)
         self.assertEqual(response.status_code, 404)
 
 
+class ViewsTestCase(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        super().setUp()
+        self.client = Client()
+        self.factory = RequestFactory()
+        self.request = self.factory.get('/')
+        self.staff_member = self.staff_member1
+        WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=0,
+                                    start_time=datetime.time(8, 0), end_time=datetime.time(12, 0))
+        WorkingHours.objects.create(staff_member=self.staff_member1, day_of_week=2,
+                                    start_time=datetime.time(8, 0), end_time=datetime.time(12, 0))
+        self.ar = self.create_appt_request_for_sm1()
+        self.user1 = self.users['staff1']
+        self.user1.is_staff = True
+        self.request.user = self.user1
+
+    def test_get_next_available_date_ajax(self):
+        """get_next_available_date_ajax view should return a JSON response with the next available date."""
+        data = {'staff_id': self.staff_member.id}
+        url = reverse('appointment:request_next_available_slot', args=[self.service1.id])
+        response = self.client.get(url, data=data, HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+        self.assertEqual(response.status_code, 200)
+        response_data = json.loads(response.content)
+        self.assertIsNotNone(response_data)
+        self.assertIsNotNone(response_data['next_available_date'])
+
+    def test_default_thank_you(self):
+        """Test if the default thank you page can be rendered."""
+        appointment = Appointment.objects.create(client=self.user1, appointment_request=self.ar)
+        url = reverse('appointment:default_thank_you', args=[appointment.id])
+        response = self.client.get(url)
+        self.assertEqual(response.status_code, 200)
+        self.assertIn(appointment.get_service_name(), str(response.content))
+
+
+class AddStaffMemberInfoTestCase(ViewsTestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        super().setUp()
+        self.staff_member = self.staff_member1
+        self.url = reverse('appointment:add_staff_member_info')
+        self.user_test = self.create_user_(
+                first_name="Great Tester", email="great.tester@django-appointment.com", username="great_tester"
+        )
+        self.data = {
+            "user": self.user_test.id,
+            "services_offered": [self.service1.id, self.service2.id],
+            "working_hours": [
+                {"day_of_week": 0, "start_time": "08:00", "end_time": "12:00"},
+                {"day_of_week": 2, "start_time": "08:00", "end_time": "12:00"}
+            ]
+        }
+
+    def test_add_staff_member_info_access_by_superuser(self):
+        """Test that the add staff member page is accessible by a superuser."""
+        self.need_superuser_login()
+        response = self.client.get(self.url)
+        self.assertEqual(response.status_code, 200)
+        self.assertIsInstance(response.context['form'], StaffMemberForm)
+
+    def test_add_staff_member_info_access_by_non_superuser(self):
+        """Test that non-superusers cannot access the add staff member page."""
+        self.need_staff_login()
+        response = self.client.get(self.url)
+        self.assertEqual(response.status_code, 403)
+
+    def test_add_staff_member_info_successful_submission(self):
+        """Test successful submission of the "add staff member" form."""
+        self.need_superuser_login()
+        response = self.client.post(self.url, data=self.data)
+        self.assertEqual(response.status_code, 302)  # Expect a redirect
+        self.assertTrue(StaffMember.objects.filter(user=self.user_test).exists())
+
+    def test_add_staff_member_info_invalid_form_submission(self):
+        """Test submission of an invalid form."""
+        self.need_superuser_login()
+        data = self.data.copy()
+        data.pop('user')
+        response = self.client.post(self.url, data=data)
+        self.assertEqual(response.status_code, 200)
+        self.assertIsInstance(response.context['form'], StaffMemberForm)
+        self.assertTrue(response.context['form'].errors)
+
+
 class SetPasswordViewTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         user_data = {
-            'username': 'test_user', 'email': 'test@example.com', 'password': 'oldpassword', 'first_name': 'John',
-            'last_name': 'Doe'
+            'username': 'bratac.of-chulak',
+            'email': 'bratac.of-chulak@django-',
+            'password': 'oldpassword',
+            'first_name': "Bra'tac",
+            'last_name': 'of Chulak'
         }
+
         self.user = create_user_with_username(user_data)
         self.token = PasswordResetToken.create_token(user=self.user, expiration_minutes=2880)  # 2 days expiration
         self.ui_db64 = urlsafe_base64_encode(force_bytes(self.user.pk))
         self.relative_set_passwd_link = reverse('appointment:set_passwd', args=[self.ui_db64, self.token.token])
         self.valid_link = reverse('appointment:set_passwd', args=[self.ui_db64, str(self.token.token)])
 
     def test_get_request_with_valid_token(self):
@@ -723,15 +898,15 @@
     def test_get_request_with_invalid_token(self):
         invalid_token = str(uuid.uuid4())
         invalid_token_link = reverse('appointment:set_passwd', args=[self.ui_db64, invalid_token])
         response = self.client.get(invalid_token_link, follow=True)
         self.assertEqual(response.status_code, 200)
         messages_ = list(get_messages(response.wsgi_request))
         self.assertTrue(
-            any(msg.message == _("The password reset link is invalid or has expired.") for msg in messages_))
+                any(msg.message == _("The password reset link is invalid or has expired.") for msg in messages_))
 
     def test_post_request_with_invalid_token(self):
         invalid_token = str(uuid.uuid4())
         invalid_token_link = reverse('appointment:set_passwd', args=[self.ui_db64, invalid_token])
         new_password = 'newpassword123'
         post_data = {'new_password1': new_password, 'new_password2': new_password}
         response = self.client.post(invalid_token_link, post_data)
@@ -744,18 +919,26 @@
         expired_token = PasswordResetToken.create_token(user=self.user, expiration_minutes=-60)
         expired_token_link = reverse('appointment:set_passwd', args=[self.ui_db64, str(expired_token.token)])
         new_password_data = {'new_password1': 'newpassword', 'new_password2': 'newpassword'}
         response = self.client.post(expired_token_link, new_password_data)
         self.assertEqual(response.status_code, 200)
         messages_ = list(get_messages(response.wsgi_request))
         self.assertTrue(
-            any(msg.message == _("The password reset link is invalid or has expired.") for msg in messages_))
+                any(msg.message == _("The password reset link is invalid or has expired.") for msg in messages_))
 
 
 class GetNonWorkingDaysAjaxTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.client = Client()
         self.url = reverse('appointment:get_non_working_days_ajax')
 
     def test_no_staff_member_selected(self):
         """Test the response when no staff member is selected."""
@@ -781,28 +964,36 @@
     def test_ajax_required(self):
         """Ensure the view only responds to AJAX requests."""
         non_ajax_response = self.client.get(self.url, {'staff_id': self.staff_member1.id})
         self.assertEqual(non_ajax_response.status_code, 200)
 
 
 class AppointmentClientInformationTest(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.client = Client()
         self.ar = self.create_appt_request_for_sm1()
         self.url = reverse('appointment:appointment_client_information', args=[self.ar.pk, self.ar.id_request])
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
         self.valid_form_data = {
-            'name': 'Test Client',
+            'name': 'Adria Origin',
             'service_id': '1',
             'payment_type': 'full',
-            'email': 'testuser@example.com',
+            'email': 'adria@django-appointment.com',
             'phone': '+1234567890',
-            'address': '123 Test St.',
+            'address': '123 Ori Temple, Celestis',
         }
 
     def test_get_request(self):
         """Test the view with a GET request."""
         response = self.client.get(self.url)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, 'appointment/appointment_client_information.html')
@@ -821,14 +1012,22 @@
 
         response = self.client.get(self.url)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, 'error_pages/304_already_submitted.html')
 
 
 class PrepareRescheduleAppointmentViewTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.client = Client()
         self.ar = self.create_appt_request_for_sm1()
         self.url = reverse('appointment:prepare_reschedule_appointment', args=[self.ar.id_request])
 
     @patch('appointment.utils.db_helpers.can_appointment_be_rescheduled', return_value=True)
@@ -856,19 +1055,27 @@
         self.assertEqual(response.context['page_title'], f"Rescheduling appointment for {self.service1.name}")
         self.assertTrue('date_chosen' in response.context)
         self.assertTrue('page_description' in response.context)
         self.assertTrue('timezoneTxt' in response.context)
 
 
 class RescheduleAppointmentSubmitViewTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.client = Client()
         self.ar = self.create_appt_request_for_sm1(date_=timezone.now().date() + datetime.timedelta(days=1))
-        self.appointment = self.create_appointment_for_user1(appointment_request=self.ar)
+        self.appointment = self.create_appt_for_sm1(appointment_request=self.ar)
         self.url = reverse('appointment:reschedule_appointment_submit')
         self.post_data = {
             'appointment_request_id': self.ar.id_request,
             'date': (timezone.now().date() + datetime.timedelta(days=2)).isoformat(),
             'start_time': '10:00',
             'end_time': '11:00',
             'staff_member': self.staff_member1.id,
@@ -901,32 +1108,41 @@
         self.service1.save()
 
         response = self.client.post(self.url, self.post_data)
         self.assertEqual(response.status_code, 200)
         self.assertTemplateUsed(response, 'appointment/appointments.html')
         messages_list = list(get_messages(response.wsgi_request))
         self.assertTrue(any(
-            _("There was an error in your submission. Please check the form and try again.") in str(message) for message
-            in messages_list))
+                _("There was an error in your submission. Please check the form and try again.") in str(message) for
+                message
+                in messages_list))
 
 
 class ConfirmRescheduleViewTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.client = Client()
         self.ar = self.create_appt_request_for_sm1()
-        self.create_appointment_for_user1(appointment_request=self.ar)
+        self.create_appt_for_sm1(appointment_request=self.ar)
         self.reschedule_history = AppointmentRescheduleHistory.objects.create(
-            appointment_request=self.ar,
-            date=timezone.now().date() + timezone.timedelta(days=2),
-            start_time='10:00',
-            end_time='11:00',
-            staff_member=self.staff_member1,
-            id_request='unique_id_request',
-            reschedule_status='pending'
+                appointment_request=self.ar,
+                date=timezone.now().date() + timezone.timedelta(days=2),
+                start_time='10:00',
+                end_time='11:00',
+                staff_member=self.staff_member1,
+                id_request='unique_id_request',
+                reschedule_status='pending'
         )
         self.url = reverse('appointment:confirm_reschedule', args=[self.reschedule_history.id_request])
 
     def test_confirm_reschedule_valid(self):
         response = self.client.get(self.url)
         self.reschedule_history.refresh_from_db()
         self.ar.refresh_from_db()
@@ -956,126 +1172,26 @@
     @patch('appointment.views.notify_admin_about_reschedule')
     def test_notify_admin_about_reschedule_called(self, mock_notify_admin):
         self.client.get(self.url)
         mock_notify_admin.assert_called_once()
         self.assertTrue(mock_notify_admin.called)
 
 
-class GetAppointmentDataFromPostRequestTests(BaseTest):
-    def setUp(self):
-        self.factory = RequestFactory()
-        self.post_data = {
-            'phone': '1234567890',
-            'want_reminder': 'on',
-            'address': '123 Test St, Test City',
-            'additional_info': 'Please ring the bell.'
-        }
-
-    def test_get_appointment_data_from_post_request_with_data(self):
-        """Test retrieving appointment data from a POST request with all data provided."""
-        request = self.factory.post('/fake-url/', self.post_data)
-
-        appointment_data = get_appointment_data_from_post_request(request)
-
-        self.assertEqual(appointment_data['phone'], self.post_data['phone'])
-        self.assertTrue(appointment_data['want_reminder'])
-        self.assertEqual(appointment_data['address'], self.post_data['address'])
-        self.assertEqual(appointment_data['additional_info'], self.post_data['additional_info'])
-
-    def test_get_appointment_data_from_post_request_partial_data(self):
-        """Test retrieving appointment data from a POST request with partial data provided."""
-        partial_post_data = {
-            'phone': '1234567890',
-            # 'want_reminder' omitted to simulate unchecked checkbox
-            'address': '123 Test St, Test City',
-            # 'additional_info' omitted to simulate empty field
-        }
-        request = self.factory.post('/fake-url/', partial_post_data)
-
-        appointment_data = get_appointment_data_from_post_request(request)
-
-        self.assertEqual(appointment_data['phone'], partial_post_data['phone'])
-        self.assertFalse(appointment_data['want_reminder'], "want_reminder should be False if not 'on'")
-        self.assertEqual(appointment_data['address'], partial_post_data['address'])
-        self.assertEqual(appointment_data['additional_info'], None, "additional_info should be None if not provided")
-
-    def test_get_appointment_data_from_post_request_missing_data(self):
-        """Test retrieving appointment data from a POST request with missing data."""
-        missing_data_post = {}
-        request = self.factory.post('/fake-url/', missing_data_post)
-
-        appointment_data = get_appointment_data_from_post_request(request)
-
-        self.assertEqual(appointment_data['phone'], None, "phone should be None if not provided")
-        self.assertFalse(appointment_data['want_reminder'], "want_reminder should be False if not provided")
-        self.assertEqual(appointment_data['address'], None, "address should be None if not provided")
-        self.assertEqual(appointment_data['additional_info'], None, "additional_info should be None if not provided")
-
-
-class GetClientDataFromPostTests(BaseTest):
-    def setUp(self):
-        self.factory = RequestFactory()
-
-    def test_get_client_data_with_full_data(self):
-        """Test retrieving client data from a POST request with all fields provided."""
-        post_data = {
-            'name': 'John Doe',
-            'email': 'john.doe@example.com',
-        }
-        request = self.factory.post('/fake-url/', post_data)
-
-        client_data = get_client_data_from_post(request)
-
-        self.assertEqual(client_data['name'], post_data['name'])
-        self.assertEqual(client_data['email'], post_data['email'])
-
-    def test_get_client_data_with_missing_name(self):
-        """Test retrieving client data from a POST request with the name missing."""
-        post_data = {
-            # 'name' is missing
-            'email': 'john.doe@example.com',
-        }
-        request = self.factory.post('/fake-url/', post_data)
-
-        client_data = get_client_data_from_post(request)
-
-        self.assertIsNone(client_data['name'], "name should be None if not provided")
-        self.assertEqual(client_data['email'], post_data['email'])
-
-    def test_get_client_data_with_missing_email(self):
-        """Test retrieving client data from a POST request with the email missing."""
-        post_data = {
-            'name': 'John Doe',
-            # 'email' is missing
-        }
-        request = self.factory.post('/fake-url/', post_data)
-
-        client_data = get_client_data_from_post(request)
-
-        self.assertEqual(client_data['name'], post_data['name'])
-        self.assertIsNone(client_data['email'], "email should be None if not provided")
-
-    def test_get_client_data_with_empty_fields(self):
-        """Test retrieving client data from a POST request with empty fields."""
-        post_data = {
-            'name': '',
-            'email': '',
-        }
-        request = self.factory.post('/fake-url/', post_data)
-
-        client_data = get_client_data_from_post(request)
-
-        self.assertEqual(client_data['name'], '', "name should be empty string if provided as such")
-        self.assertEqual(client_data['email'], '', "email should be empty string if provided as such")
-
-
 class RedirectToPaymentOrThankYouPageTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
 
     @patch('appointment.views.APPOINTMENT_PAYMENT_URL', 'http://example.com/payment/')
     @patch('appointment.views.create_payment_info_and_get_url')
     def test_redirect_to_payment_page(self, mock_create_payment_info_and_get_url):
         """Test redirection to the payment page when APPOINTMENT_PAYMENT_URL is set."""
         mock_create_payment_info_and_get_url.return_value = 'http://example.com/payment/12345'
         response = redirect_to_payment_or_thank_you_page(self.appointment)
@@ -1087,33 +1203,41 @@
     @patch('appointment.views.APPOINTMENT_THANK_YOU_URL', 'appointment:default_thank_you')
     def test_redirect_to_custom_thank_you_page(self):
         """Test redirection to a custom thank-you page when APPOINTMENT_THANK_YOU_URL is set."""
         response = redirect_to_payment_or_thank_you_page(self.appointment)
 
         self.assertIsInstance(response, HttpResponseRedirect)
         self.assertTrue(response.url.startswith(
-            reverse('appointment:default_thank_you', kwargs={'appointment_id': self.appointment.id})))
+                reverse('appointment:default_thank_you', kwargs={'appointment_id': self.appointment.id})))
 
     @patch('appointment.views.APPOINTMENT_PAYMENT_URL', '')
     @patch('appointment.views.APPOINTMENT_THANK_YOU_URL', '')
     def test_redirect_to_default_thank_you_page(self):
         """Test redirection to the default thank-you page when no specific URL is set."""
         response = redirect_to_payment_or_thank_you_page(self.appointment)
 
         self.assertIsInstance(response, HttpResponseRedirect)
         self.assertTrue(response.url.startswith(
-            reverse('appointment:default_thank_you', kwargs={'appointment_id': self.appointment.id})))
+                reverse('appointment:default_thank_you', kwargs={'appointment_id': self.appointment.id})))
 
 
 class CreateAppointmentTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.appointment_request = self.create_appt_request_for_sm1()
-        self.client_data = {'name': 'John Doe', 'email': 'john@example.com'}
-        self.appointment_data = {'phone': '1234567890', 'want_reminder': True, 'address': '123 Test St.',
+        self.client_data = {'name': 'Orlin Ascended', 'email': 'orlin.ascended@django-appointment.com'}
+        self.appointment_data = {'phone': '1234567890', 'want_reminder': True, 'address': '123 Ancient St, Velona',
                                  'additional_info': 'Test info'}
         self.request = RequestFactory().get('/')
 
     @patch('appointment.views.create_and_save_appointment')
     @patch('appointment.views.redirect_to_payment_or_thank_you_page')
     def test_create_appointment_success(self, mock_redirect, mock_create_and_save):
         """Test successful creation of an appointment and redirection."""
```

### Comparing `django-appointment-3.4.1/appointment/tests/utils/test_date_time.py` & `django_appointment-3.5.0/appointment/tests/utils/test_date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,20 +11,20 @@
     convert_minutes_in_human_readable_format, convert_str_to_date,
     convert_str_to_time, get_ar_end_time, get_current_year, get_timestamp, get_weekday_num,
     time_difference
 )
 
 
 class Convert12HourTo24HourTimeTests(TestCase):
-    def test_valid_basic_conversion(self):
+    def test_basic_conversion(self):
         """Test basic 12-hour to 24-hour conversions."""
         self.assertEqual(convert_12_hour_time_to_24_hour_time("01:10 AM"), "01:10:00")
         self.assertEqual(convert_12_hour_time_to_24_hour_time("01:20 PM"), "13:20:00")
 
-    def test_convert_midnight_and_noon(self):
+    def test_midnight_and_noon(self):
         """Test conversion of midnight and noon times."""
         self.assertEqual(convert_12_hour_time_to_24_hour_time("12:00 AM"), "00:00:00")
         self.assertEqual(convert_12_hour_time_to_24_hour_time("12:00 PM"), "12:00:00")
 
     def test_boundary_times(self):
         """Test conversion of boundary times."""
         self.assertEqual(convert_12_hour_time_to_24_hour_time("12:00 AM"), "00:00:00")
@@ -38,70 +38,62 @@
         self.assertEqual(convert_12_hour_time_to_24_hour_time(time_obj), "14:30:00")
 
     def test_case_insensitivity_and_whitespace(self):
         """Test conversion handling of different case formats and white-space."""
         self.assertEqual(convert_12_hour_time_to_24_hour_time(" 12:00 am "), "00:00:00")
         self.assertEqual(convert_12_hour_time_to_24_hour_time("01:00 pM "), "13:00:00")
 
-    def test_out_of_bounds_values(self):
-        """Test conversion with out-of-bounds values."""
+    def test_invalid_values(self):
+        """Test invalid values."""
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time("13:00 PM")
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time("12:60 AM")
-
-    def test_invalid_datatypes(self):
-        """Test conversion with invalid data types."""
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time(["12:00 AM"])
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time({"time": "12:00 AM"})
-
-    def test_invalid_inputs(self):
-        """Test conversion with various invalid inputs."""
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time("25:00 AM")
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time("01:00")
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time("Random String")
         with self.assertRaises(ValueError):
             convert_12_hour_time_to_24_hour_time("01:60 AM")
 
 
 class Convert24HourTimeTo12HourTimeTests(TestCase):
 
-    def test_valid_24_hour_time_strings(self):
+    def test_valid_24_hour_strings(self):
         self.assertEqual(convert_24_hour_time_to_12_hour_time("13:00"), "01:00 PM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("00:00"), "12:00 AM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("23:59"), "11:59 PM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("12:00"), "12:00 PM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("01:00"), "01:00 AM")
 
-    def test_valid_24_hour_time_with_seconds(self):
+    def test_valid_24_hour_with_seconds(self):
         self.assertEqual(convert_24_hour_time_to_12_hour_time("13:00:01"), "01:00:01 PM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("00:00:59"), "12:00:59 AM")
 
-    def test_datetime_time_object_input(self):
+    def test_time_object_input(self):
         time_input = datetime.time(13, 15)
         self.assertEqual(convert_24_hour_time_to_12_hour_time(time_input), "01:15 PM")
         time_input = datetime.time(0, 0)
         self.assertEqual(convert_24_hour_time_to_12_hour_time(time_input), "12:00 AM")
 
     def test_invalid_time_strings(self):
         with self.assertRaises(ValueError):
             convert_24_hour_time_to_12_hour_time("25:00")
         with self.assertRaises(ValueError):
             convert_24_hour_time_to_12_hour_time("-01:00")
         with self.assertRaises(ValueError):
             convert_24_hour_time_to_12_hour_time("13:60")
         with self.assertRaises(ValueError):
             convert_24_hour_time_to_12_hour_time("invalid")
-
-    def test_incorrect_format(self):
         with self.assertRaises(ValueError):
             convert_24_hour_time_to_12_hour_time("1 PM")
         with self.assertRaises(ValueError):
             convert_24_hour_time_to_12_hour_time("13 PM")
         with self.assertRaises(ValueError):
             convert_24_hour_time_to_12_hour_time("24:00")
 
@@ -109,15 +101,15 @@
         self.assertEqual(convert_24_hour_time_to_12_hour_time("12:00"), "12:00 PM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("00:00"), "12:00 AM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("11:59"), "11:59 AM")
         self.assertEqual(convert_24_hour_time_to_12_hour_time("23:59"), "11:59 PM")
 
 
 class ConvertMinutesInHumanReadableFormatTests(TestCase):
-    def test_valid_basic_conversions(self):
+    def test_basic_conversions(self):
         """Test basic conversions"""
         self.assertEqual(convert_minutes_in_human_readable_format(30), "30 minutes")
         self.assertEqual(convert_minutes_in_human_readable_format(90), "1 hour and 30 minutes")
 
     def test_edge_cases(self):
         """Test edgy cases"""
         self.assertEqual(convert_minutes_in_human_readable_format(59), "59 minutes")
@@ -157,21 +149,21 @@
             convert_minutes_in_human_readable_format({"minutes": 30})
         with self.assertRaises(TypeError):
             convert_minutes_in_human_readable_format(None)
 
 
 class ConvertStrToDateTests(TestCase):
 
-    def test_valid_date_strings_with_hyphen_separator(self):
+    def test_valid_date_with_hyphen_separator(self):
         """Test valid date with hyphen separator works correctly"""
         self.assertEqual(convert_str_to_date("2023-12-31"), datetime.date(2023, 12, 31))
         self.assertEqual(convert_str_to_date("2020-02-29"), datetime.date(2020, 2, 29))  # Leap year
         self.assertEqual(convert_str_to_date("2021-02-28"), datetime.date(2021, 2, 28))
 
-    def test_valid_date_strings_with_slash_separator(self):
+    def test_valid_date_with_slash_separator(self):
         """Test valid date with slash separator works correctly"""
         self.assertEqual(convert_str_to_date("2021/01/01"), datetime.date(2021, 1, 1))
         self.assertEqual(convert_str_to_date("2023/12/31"), datetime.date(2023, 12, 31))
         self.assertEqual(convert_str_to_date("2023.12.31"), datetime.date(2023, 12, 31))
 
     def test_invalid_date_formats(self):
         """The date format "MM-DD-YYY" & "DD/MM/YYYY" are not supported, hence it should raise an error."""
@@ -194,35 +186,35 @@
         with self.assertRaises(ValueError):
             convert_str_to_date("RandomString")
         with self.assertRaises(ValueError):
             convert_str_to_date("0000-00-00")
 
 
 class ConvertStrToTimeTests(TestCase):
-    def test_convert_12h_format_str_to_time(self):
+    def test_12h_format_str_to_time(self):
         """Test valid time strings"""
         # These tests check if a 12-hour time format string converts correctly.
         self.assertEqual(convert_str_to_time("10:00 AM"), datetime.time(10, 0))
         self.assertEqual(convert_str_to_time("12:00 PM"), datetime.time(12, 0))
         self.assertEqual(convert_str_to_time("01:30 PM"), datetime.time(13, 30))
 
-    def test_convert_24h_format_str_to_time(self):
+    def test_24h_format_str_to_time(self):
         """Test if a 24-hour time format string converts correctly."""
         # These tests check if a 24-hour time format string converts correctly.
         self.assertEqual(convert_str_to_time("10:00:00"), datetime.time(10, 0))
         self.assertEqual(convert_str_to_time("12:00:00"), datetime.time(12, 0))
         self.assertEqual(convert_str_to_time("13:30:00"), datetime.time(13, 30))
 
     def test_case_insensitivity_and_whitespace(self):
         """Test conversion handling of different case formats and white-space."""
         self.assertEqual(convert_str_to_time(" 12:00 am "), datetime.time(0, 0))
         self.assertEqual(convert_str_to_time("01:00 pM "), datetime.time(13, 0))
         self.assertEqual(convert_str_to_time(" 13:00:00 "), datetime.time(13, 0))
 
-    def test_convert_str_to_time_invalid(self):
+    def test_invalid_time_strings(self):
         """Test invalid time strings"""
         with self.assertRaises(ValueError):
             convert_str_to_time("")
         with self.assertRaises(ValueError):
             convert_str_to_time("13:00 PM")
         with self.assertRaises(ValueError):
             convert_str_to_time("25:00 AM")
@@ -272,22 +264,22 @@
             get_ar_end_time(12345, 30)  # Passing an integer
         with self.assertRaises(TypeError):
             get_ar_end_time(None, 30)  # Passing None
 
 
 class TimeDifferenceTests(TestCase):
 
-    def test_valid_difference_with_time_objects(self):
+    def test_difference_with_time_objects(self):
         """Test difference between two time objects"""
         time1 = datetime.time(10, 0)
         time2 = datetime.time(11, 0)
         difference = time_difference(time1, time2)
         self.assertEqual(difference, datetime.timedelta(hours=1))
 
-    def test_valid_difference_with_datetime_objects(self):
+    def test_difference_with_datetime_objects(self):
         """Test difference between two datetime objects"""
         datetime1 = datetime.datetime(2023, 1, 1, 10, 0)
         datetime2 = datetime.datetime(2023, 1, 1, 11, 0)
         difference = time_difference(datetime1, datetime2)
         self.assertEqual(difference, datetime.timedelta(hours=1))
 
     def test_negative_difference_with_time_objects(self):
@@ -320,15 +312,15 @@
             time_difference(datetime_obj, time_obj)
 
         self.assertEqual(str(context.exception),
                          "Both inputs should be of the same type, either datetime.time or datetime.datetime")
 
 
 class CombineDateAndTimeTests(TestCase):
-    def test_combine_valid_date_and_time(self):
+    def test_valid_date_and_time(self):
         """Test combining a valid date and time."""
         date = datetime.date(2023, 1, 1)
         time = datetime.time(12, 30)
         expected_datetime = datetime.datetime(2023, 1, 1, 12, 30)
         result = combine_date_and_time(date, time)
         self.assertEqual(result, expected_datetime)
```

### Comparing `django-appointment-3.4.1/appointment/tests/utils/test_db_helpers.py` & `django_appointment-3.5.0/appointment/tests/utils/test_db_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,38 +4,34 @@
 import datetime
 from unittest.mock import MagicMock, PropertyMock, patch
 
 from django.apps import apps
 from django.conf import settings
 from django.core.cache import cache
 from django.core.exceptions import FieldDoesNotExist
-from django.test import TestCase
+from django.test import TestCase, override_settings
 from django.test.client import RequestFactory
 from django.urls import reverse
 from django.utils import timezone
 from django_q.models import Schedule
 
-from appointment.models import DayOff, PaymentInfo
+from appointment.models import Config, DayOff, PaymentInfo
 from appointment.tests.base.base_test import BaseTest
 from appointment.tests.mixins.base_mixin import ConfigMixin
 from appointment.utils.db_helpers import (
-    Config, WorkingHours, calculate_slots, calculate_staff_slots, can_appointment_be_rescheduled,
-    cancel_existing_reminder, check_day_off_for_staff,
-    create_and_save_appointment, create_new_user, create_payment_info_and_get_url, create_user_with_email,
-    day_off_exists_for_date_range,
+    Appointment, AppointmentRequest, AppointmentRescheduleHistory, Config, WorkingHours, calculate_slots,
+    calculate_staff_slots, can_appointment_be_rescheduled, cancel_existing_reminder, check_day_off_for_staff,
+    create_and_save_appointment, create_new_user, create_payment_info_and_get_url, day_off_exists_for_date_range,
     exclude_booked_slots, exclude_pending_reschedules, generate_unique_username_from_email, get_absolute_url_,
-    get_all_appointments,
-    get_all_staff_members,
-    get_appointment_buffer_time, get_appointment_by_id, get_appointment_finish_time, get_appointment_lead_time,
-    get_appointment_slot_duration, get_appointments_for_date_and_time, get_config, get_day_off_by_id,
-    get_non_working_days_for_staff, get_staff_member_appointment_list, get_staff_member_buffer_time,
-    get_staff_member_by_user_id, get_staff_member_end_time, get_staff_member_from_user_id_or_logged_in,
-    get_staff_member_slot_duration, get_staff_member_start_time, get_times_from_config, get_user_by_email,
-    get_user_model, get_website_name, get_weekday_num_from_date, get_working_hours_by_id,
-    get_working_hours_for_staff_and_day, is_working_day, parse_name, schedule_email_reminder,
+    get_all_appointments, get_all_staff_members, get_appointment_buffer_time, get_appointment_by_id,
+    get_appointment_finish_time, get_appointment_lead_time, get_appointment_slot_duration,
+    get_appointments_for_date_and_time, get_config, get_day_off_by_id, get_non_working_days_for_staff,
+    get_staff_member_appointment_list, get_staff_member_by_user_id, get_staff_member_from_user_id_or_logged_in,
+    get_times_from_config, get_user_by_email, get_user_model, get_website_name, get_weekday_num_from_date,
+    get_working_hours_by_id, get_working_hours_for_staff_and_day, is_working_day, parse_name, schedule_email_reminder,
     staff_change_allowed_on_reschedule, update_appointment_reminder, username_in_user_model, working_hours_exist
 )
 
 
 class TestCalculateSlots(TestCase):
     def setUp(self):
         self.start_time = datetime.datetime(2023, 10, 8, 8, 0)  # 8:00 AM
@@ -85,29 +81,44 @@
 
         expected = [datetime.datetime(2023, 10, 8, 8, 0), datetime.datetime(2023, 10, 8, 8, 30)]
         result = calculate_slots(self.start_time, end_time, buffer_time, slot_duration)
         self.assertEqual(result, expected)
 
 
 class TestCalculateStaffSlots(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
         self.slot_duration = datetime.timedelta(minutes=30)
         # Not working today but tomorrow
         self.date_not_working = datetime.date.today()
-        self.working_date = datetime.date.today() + datetime.timedelta(days=1)
+        self.working_date = datetime.date.today() + datetime.timedelta(days=3)
         weekday_num = get_weekday_num_from_date(self.working_date)
-        WorkingHours.objects.create(
-            staff_member=self.staff_member1,
-            day_of_week=weekday_num,
-            start_time=datetime.time(9, 0),
-            end_time=datetime.time(17, 0)
+        self.wh = WorkingHours.objects.create(
+                staff_member=self.staff_member1,
+                day_of_week=weekday_num,
+                start_time=datetime.time(9, 0),
+                end_time=datetime.time(17, 0)
         )
         self.staff_member1.appointment_buffer_time = 25.0
-        self.buffer_time = datetime.timedelta(minutes=25)
+
+    @override_settings(DEBUG=True)
+    def tearDown(self):
+        self.wh.delete()
+        if Config.objects.exists():
+            Config.objects.all().delete()
+        cache.clear()
+        super().tearDown()
 
     def test_calculate_slots_on_working_day_without_appointments(self):
         slots = calculate_staff_slots(self.working_date, self.staff_member1)
         # Slot duration is 30 minutes, so 8 working hours minus 25-minute buffer, divided by slot duration
         expected_number_of_slots = int((8 * 60 - 25) / 30)
         # 15 slots should be available instead of 16 because of the 25-minute buffer
         self.assertEqual(len(slots), expected_number_of_slots)
@@ -130,14 +141,17 @@
         super().setUp()  # Call the parent class setup
         # Specific setups for this test class
         self.day_off1 = DayOff.objects.create(staff_member=self.staff_member1, start_date="2023-10-08",
                                               end_date="2023-10-10")
         self.day_off2 = DayOff.objects.create(staff_member=self.staff_member2, start_date="2023-10-05",
                                               end_date="2023-10-05")
 
+    def tearDown(self):
+        DayOff.objects.all().delete()
+
     def test_staff_member_has_day_off(self):
         # Test for a date within the range of days off for staff_member1
         self.assertTrue(check_day_off_for_staff(self.staff_member1, "2023-10-09"))
 
     def test_staff_member_does_not_have_day_off(self):
         # Test for a date outside the range of days off for staff_member1
         self.assertFalse(check_day_off_for_staff(self.staff_member1, "2023-10-11"))
@@ -156,24 +170,28 @@
     def setUp(self):
         super().setUp()  # Call the parent class setup
         # Specific setups for this test class
         self.ar = self.create_appt_request_for_sm1()
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
 
+    def tearDown(self):
+        Appointment.objects.all().delete()
+        AppointmentRequest.objects.all().delete()
+
     def test_create_and_save_appointment(self):
         client_data = {
-            'email': 'tester2@gmail.com',
-            'name': 'Tester2',
+            'email': 'georges.s.hammond@django-appointment.com',
+            'name': 'georges.hammond',
         }
         appointment_data = {
             'phone': '123456789',
             'want_reminder': True,
-            'address': '123 Main St',
-            'additional_info': 'Additional Test Info'
+            'address': '123, Stargate Command, Cheyenne Mountain, Colorado, USA',
+            'additional_info': 'Please bring a Zat gun.'
         }
 
         appointment = create_and_save_appointment(self.ar, client_data, appointment_data, self.request)
 
         self.assertIsNotNone(appointment)
         self.assertEqual(appointment.client.email, client_data['email'])
         self.assertEqual(appointment.phone, appointment_data['phone'])
@@ -190,52 +208,59 @@
 
 
 class ScheduleEmailReminderTest(BaseTest):
     def setUp(self):
         super().setUp()
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
+        self.appointment = self.create_appt_for_sm1()
+
+    def tearDown(self):
+        Appointment.objects.all().delete()
+        AppointmentRequest.objects.all().delete()
 
     def test_schedule_email_reminder_cluster_running(self):
-        appointment = self.create_appointment_for_user1()
         with patch('appointment.settings.check_q_cluster', return_value=True), \
                 patch('appointment.utils.db_helpers.schedule') as mock_schedule:
-            schedule_email_reminder(appointment, self.request)
+            schedule_email_reminder(self.appointment, self.request)
             mock_schedule.assert_called_once()
             # Further assertions can be made here based on the arguments passed to schedule
 
     def test_schedule_email_reminder_cluster_not_running(self):
-        appointment = self.create_appointment_for_user2()
         with patch('appointment.settings.check_q_cluster', return_value=False), \
                 patch('appointment.utils.db_helpers.logger') as mock_logger:
-            schedule_email_reminder(appointment, self.request)
+            schedule_email_reminder(self.appointment, self.request)
             mock_logger.warning.assert_called_with(
-                "Django-Q cluster is not running. Email reminder will not be scheduled.")
+                    "Django-Q cluster is not running. Email reminder will not be scheduled.")
 
 
 class UpdateAppointmentReminderTest(BaseTest):
     def setUp(self):
         super().setUp()
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
+
+    def tearDown(self):
+        Appointment.objects.all().delete()
+        AppointmentRequest.objects.all().delete()
 
     def test_update_appointment_reminder_date_time_changed(self):
-        appointment = self.create_appointment_for_user1()
+        appointment = self.create_appt_for_sm1()
         new_date = timezone.now().date() + timezone.timedelta(days=10)
         new_start_time = timezone.now().time()
 
         with patch('appointment.utils.db_helpers.schedule_email_reminder') as mock_schedule_email_reminder, \
                 patch('appointment.utils.db_helpers.cancel_existing_reminder') as mock_cancel_existing_reminder:
             update_appointment_reminder(appointment, new_date, new_start_time, self.request, True)
             mock_cancel_existing_reminder.assert_called_once_with(appointment.id_request)
             mock_schedule_email_reminder.assert_called_once()
 
     def test_update_appointment_reminder_no_change(self):
-        appointment = self.create_appointment_for_user2()
+        appointment = self.create_appt_for_sm2()
         # Use existing date and time
         new_date = appointment.appointment_request.date
         new_start_time = appointment.appointment_request.start_time
 
         with patch('appointment.utils.db_helpers.schedule_email_reminder') as mock_schedule_email_reminder, \
                 patch('appointment.utils.db_helpers.cancel_existing_reminder') as mock_cancel_existing_reminder:
             update_appointment_reminder(appointment, new_date, new_start_time, self.request, appointment.want_reminder)
@@ -249,43 +274,48 @@
         new_date = timezone.now().date() + datetime.timedelta(days=1)
         new_start_time = timezone.now().time()
 
         update_appointment_reminder(self.appointment, new_date, new_start_time, self.request, want_reminder)
 
         # Check that the logger.info was called with the expected message
         mock_logger.info.assert_called_once_with(
-            f"Reminder for appointment {self.appointment.id} is not scheduled per user's preference or past datetime."
+                f"Reminder for appointment {self.appointment.id} is not scheduled per user's preference or past datetime."
         )
 
     @patch('appointment.utils.db_helpers.logger')  # Adjust the import path as necessary
     def test_reminder_not_scheduled_due_to_past_datetime(self, mock_logger):
         # Scenario where the new datetime is in the past
         want_reminder = True
         new_date = timezone.now().date() - datetime.timedelta(days=1)  # Date in the past
         new_start_time = timezone.now().time()
 
         update_appointment_reminder(self.appointment, new_date, new_start_time, self.request, want_reminder)
 
         # Check that the logger.info was called with the expected message
         mock_logger.info.assert_called_once_with(
-            f"Reminder for appointment {self.appointment.id} is not scheduled per user's preference or past datetime."
+                f"Reminder for appointment {self.appointment.id} is not scheduled per user's preference or past datetime."
         )
 
 
 # Helper method for modifying service rescheduling settings
 def modify_service_rescheduling(service, **kwargs):
     for key, value in kwargs.items():
         setattr(service, key, value)
     service.save()
 
 
 class CanAppointmentBeRescheduledTests(BaseTest, ConfigMixin):
     def setUp(self):
         super().setUp()
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
+
+    def tearDown(self):
+        Appointment.objects.all().delete()
+        AppointmentRescheduleHistory.objects.all().delete()
+        AppointmentRequest.objects.all().delete()
 
     @patch('appointment.models.Service.reschedule_limit', new_callable=PropertyMock)
     @patch('appointment.models.Config.default_reschedule_limit', new=3)
     def test_can_appointment_be_rescheduled(self, mock_reschedule_limit):
         mock_reschedule_limit.return_value = 3
         self.assertTrue(can_appointment_be_rescheduled(self.appointment.appointment_request))
 
@@ -297,26 +327,31 @@
         modify_service_rescheduling(self.service1, allow_rescheduling=True, reschedule_limit=3)
         ar = self.create_appointment_request_with_histories(service=self.service1, count=4)
         self.assertFalse(can_appointment_be_rescheduled(ar))
 
     def test_rescheduling_with_default_limit(self):
         ar = self.create_appointment_request_with_histories(service=self.service1, count=2, use_default_limit=True)
         self.assertTrue(can_appointment_be_rescheduled(ar))
-        self.create_appointment_reschedule_for_user1(appointment_request=ar)
+        self.create_appt_reschedule_for_sm1(appointment_request=ar)
         self.assertFalse(can_appointment_be_rescheduled(ar))
 
     # Helper method to create appointment request with rescheduled histories
     def create_appointment_request_with_histories(self, service, count, use_default_limit=False):
         ar = self.create_appointment_request_(service=service, staff_member=self.staff_member1)
         for _ in range(count):
-            self.create_appointment_reschedule_for_user1(appointment_request=ar)
+            self.create_appt_reschedule_for_sm1(appointment_request=ar)
         return ar
 
 
 class StaffChangeAllowedOnRescheduleTests(TestCase):
+    def tearDown(self):
+        super().tearDown()
+        # Reset or delete the Config instance to ensure test isolation
+        Config.objects.all().delete()
+
     @patch('appointment.models.Config.objects.first')
     def test_staff_change_allowed(self, mock_config_first):
         # Mock the Config object to return True for allow_staff_change_on_reschedule
         mock_config = MagicMock()
         mock_config.allow_staff_change_on_reschedule = True
         mock_config_first.return_value = mock_config
 
@@ -330,88 +365,31 @@
         mock_config.allow_staff_change_on_reschedule = False
         mock_config_first.return_value = mock_config
 
         # Call the function and assert that staff change is not allowed
         self.assertFalse(staff_change_allowed_on_reschedule())
 
 
-class CreateUserWithEmailTests(TestCase):
-    def setUp(self):
-        self.User = get_user_model()
-        self.User.USERNAME_FIELD = 'email'
-
-    # def test_create_user_with_full_data(self):
-    #     """Test creating a user with complete client data."""
-    #     client_data = {
-    #         'email': 'test@example.com',
-    #         'first_name': 'Test',
-    #         'last_name': 'User',
-    #         'username': 'test_user',
-    #     }
-    #     user = create_user_with_email(client_data)
-    #
-    #     # Verify that the user was created with the correct attributes
-    #     self.assertEqual(user.email, 'test@example.com')
-    #     self.assertEqual(user.first_name, 'Test')
-    #     self.assertEqual(user.last_name, 'User')
-    #     self.assertTrue(user.is_active)
-    #     self.assertFalse(user.is_staff)
-    #     self.assertFalse(user.is_superuser)
-
-    # def test_create_user_with_partial_data(self):
-    #     """Test creating a user with only an email provided."""
-    #     client_data = {
-    #         'email': 'partial@example.com',
-    #         'username': 'partial_user',
-    #         # First name and last name are omitted
-    #     }
-    #     user = create_user_with_email(client_data)
-    #
-    #     # Verify that the user was created with default values for missing attributes
-    #     self.assertEqual(user.email, 'partial@example.com')
-    #     self.assertEqual(user.first_name, '')
-    #     self.assertEqual(user.last_name, '')
-
-    # def test_create_user_with_duplicate_email(self):
-    #     """Test attempting to create a user with a duplicate email."""
-    #     client_data = {
-    #         'email': 'duplicate@example.com',
-    #         'first_name': 'Original',
-    #         'last_name': 'User',
-    #         'username': 'original_user',
-    #     }
-    #     # Create the first user
-    #     create_user_with_email(client_data)
-    #
-    #     # Attempt to create another user with the same email
-    #     with self.assertRaises(Exception) as context:
-    #         create_user_with_email(client_data)
-    #
-    #     # Verify that the expected exception is raised (e.g., IntegrityError for duplicate key)
-    #     self.assertTrue('duplicate key value violates unique constraint' in str(context.exception) or
-    #                     'UNIQUE constraint failed' in str(context.exception))
-
-
 class CancelExistingReminderTest(BaseTest):
     def test_cancel_existing_reminder(self):
-        appointment = self.create_appointment_for_user1()
+        appointment = self.create_appt_for_sm1()
         Schedule.objects.create(func='appointment.tasks.send_email_reminder', name=f"reminder_{appointment.id_request}")
 
         self.assertEqual(Schedule.objects.count(), 1)
         cancel_existing_reminder(appointment.id_request)
         self.assertEqual(Schedule.objects.filter(name=f"reminder_{appointment.id_request}").count(), 0)
 
 
 class TestCreatePaymentInfoAndGetUrl(BaseTest):
 
     def setUp(self):
         super().setUp()  # Call the parent class setup
         # Specific setups for this test class
         self.ar = self.create_appt_request_for_sm1()
-        self.appointment = self.create_appointment_for_user2(appointment_request=self.ar)
+        self.appointment = self.create_appt_for_sm2(appointment_request=self.ar)
 
     def test_create_payment_info_and_get_url_string(self):
         expected_url = "https://payment.com/1/1234567890"
         with patch('appointment.utils.db_helpers.APPOINTMENT_PAYMENT_URL', expected_url):
             payment_url = create_payment_info_and_get_url(self.appointment)
             self.assertEqual(payment_url, expected_url)
 
@@ -439,15 +417,15 @@
                 self.assertEqual(payment_url, expected_mocked_url)
 
 
 class TestExcludeBookedSlots(BaseTest):
 
     def setUp(self):
         super().setUp()
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
 
         # Sample slots for testing
         self.today = datetime.date.today()
 
         self.slots = [
             datetime.datetime.combine(self.today, datetime.time(8, 0)),
             datetime.datetime.combine(self.today, datetime.time(9, 0)),
@@ -482,29 +460,29 @@
             datetime.datetime.combine(self.today, datetime.time(12, 0))
         ]
         self.assertEqual(result, expected)
 
     def test_multiple_overlapping_appointments(self):
         ar2 = self.create_appt_request_for_sm2(start_time=datetime.time(10, 30),
                                                end_time=datetime.time(11, 30))
-        appointment2 = self.create_appointment_for_user2(appointment_request=ar2)
+        appointment2 = self.create_appt_for_sm2(appointment_request=ar2)
         appointment2.save()
         result = exclude_booked_slots([self.appointment, appointment2], self.slots, self.slot_duration)
         expected = [
             datetime.datetime.combine(self.today, datetime.time(8, 0)),
             datetime.datetime.combine(self.today, datetime.time(12, 0))
         ]
         self.assertEqual(result, expected)
 
 
 class TestDayOffExistsForDateRange(BaseTest):
 
     def setUp(self):
         super().setUp()
-        self.user = self.create_user_(email="tester@gmail.com")
+        self.user = self.create_user_()
         self.service = self.create_service_()
         self.staff_member = self.create_staff_member_(user=self.user, service=self.service)
         self.day_off1 = DayOff.objects.create(staff_member=self.staff_member, start_date="2023-10-08",
                                               end_date="2023-10-10")
         self.day_off2 = DayOff.objects.create(staff_member=self.staff_member, start_date="2023-10-15",
                                               end_date="2023-10-17")
 
@@ -515,27 +493,28 @@
     def test_day_off_does_not_exist(self):
         # Check for a date range that doesn't intersect with any day off
         self.assertFalse(day_off_exists_for_date_range(self.staff_member, "2023-10-11", "2023-10-14"))
 
     def test_day_off_exists_but_excluded(self):
         # Check for a date range that intersects with day_off1 but exclude day_off1 from the check using its ID
         self.assertFalse(
-            day_off_exists_for_date_range(self.staff_member, "2023-10-09", "2023-10-11", days_off_id=self.day_off1.id))
+                day_off_exists_for_date_range(self.staff_member, "2023-10-09", "2023-10-11",
+                                              days_off_id=self.day_off1.id))
 
     def test_day_off_exists_for_other_range(self):
         # Check for a date range that intersects with day_off2
         self.assertTrue(day_off_exists_for_date_range(self.staff_member, "2023-10-16", "2023-10-18"))
 
 
 class TestGetAllAppointments(BaseTest):
 
     def setUp(self):
         super().setUp()
-        self.appointment1 = self.create_appointment_for_user1()
-        self.appointment2 = self.create_appointment_for_user2()
+        self.appointment1 = self.create_appt_for_sm1()
+        self.appointment2 = self.create_appt_for_sm2()
 
     def test_get_all_appointments(self):
         appointments = get_all_appointments()
         self.assertEqual(len(appointments), 2)
         self.assertIn(self.appointment1, appointments)
         self.assertIn(self.appointment2, appointments)
 
@@ -552,15 +531,15 @@
         self.assertIn(self.staff_member2, staff_members)
 
 
 class TestGetAppointmentByID(BaseTest):
 
     def setUp(self):
         super().setUp()
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
 
     def test_existing_appointment(self):
         """Test fetching an existing appointment."""
         fetched_appointment = get_appointment_by_id(self.appointment.id)
         self.assertEqual(fetched_appointment, self.appointment)
 
     def test_non_existing_appointment(self):
@@ -572,14 +551,19 @@
 
 @patch('appointment.utils.db_helpers.APPOINTMENT_BUFFER_TIME', 60)
 @patch('appointment.utils.db_helpers.APPOINTMENT_LEAD_TIME', '07:00:00')
 @patch('appointment.utils.db_helpers.APPOINTMENT_FINISH_TIME', '15:00:00')
 @patch('appointment.utils.db_helpers.APPOINTMENT_SLOT_DURATION', 30)
 @patch('appointment.utils.db_helpers.APPOINTMENT_WEBSITE_NAME', "django-appointment-website")
 class TestGetAppointmentConfigTimes(TestCase):
+    def tearDown(self):
+        super().tearDown()
+        # Reset or delete the Config instance to ensure test isolation
+        Config.objects.all().delete()
+
     def test_no_config_object(self):
         """Test when there's no Config object in the database."""
         self.assertIsNone(Config.objects.first())  # Ensure no Config object exists
         self.assertEqual(get_appointment_buffer_time(), 60)
         self.assertEqual(get_appointment_lead_time(), '07:00:00')
         self.assertEqual(get_appointment_finish_time(), '15:00:00')
         self.assertEqual(get_appointment_slot_duration(), 30)
@@ -610,22 +594,31 @@
         self.assertEqual(get_appointment_lead_time(), '07:00:00')
         self.assertEqual(get_appointment_finish_time(), '15:00:00')
         self.assertEqual(get_appointment_slot_duration(), 30)
         self.assertEqual(get_website_name(), "django-appointment-website")
 
 
 class TestGetAppointmentsForDateAndTime(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
     def setUp(self):
         super().setUp()
 
         # Setting up some appointment requests and appointments for testing
         self.date_sample = datetime.datetime.today()
 
         # Creating overlapping appointments for staff_member1
+        self.client1 = self.users['client1']
+        self.client2 = self.users['client2']
         ar1 = self.create_appt_request_for_sm1(start_time=datetime.time(9, 0), end_time=datetime.time(10, 0))
         self.appointment1 = self.create_appointment_(user=self.client1, appointment_request=ar1)
 
         ar2 = self.create_appt_request_for_sm1(start_time=datetime.time(10, 30), end_time=datetime.time(11, 30))
         self.appointment2 = self.create_appointment_(user=self.client2, appointment_request=ar2)
 
         # Creating a non-overlapping appointment for staff_member1
@@ -661,14 +654,20 @@
 
 class TestGetConfig(TestCase):
 
     def setUp(self):
         # Clear the cache at the start of each test to ensure a clean state
         cache.clear()
 
+    def tearDown(self):
+        super().tearDown()
+        # Reset or delete the Config instance to ensure test isolation
+        Config.objects.all().delete()
+        cache.clear()
+
     def test_no_config_in_cache_or_db(self):
         """Test when there's no Config in cache or the database."""
         config = get_config()
         self.assertIsNone(config)
 
     def test_config_in_db_not_in_cache(self):
         """Test when there's a Config object in the database but not in the cache."""
@@ -676,19 +675,20 @@
         config = get_config()
         self.assertEqual(config, db_config)
 
     def test_config_in_cache(self):
         """Test when there's a Config object in the cache."""
         db_config = Config.objects.create(finish_time='17:00:00')
         cache.set('config', db_config)
-        # Use 'patch' to ensure the Config model isn't hit during the test
-        with patch('appointment.models.Config.objects.first') as mock_first:
-            config = get_config()
-            self.assertEqual(config, db_config)
-            mock_first.assert_not_called()  # Ensure the database wasn't hit
+
+        # Clear the database to ensure it won't be accessed
+        Config.objects.all().delete()
+
+        config = get_config()
+        self.assertEqual(config, db_config)
 
 
 class TestGetDayOffById(BaseTest):  # Assuming you have a BaseTest class with some initial setups
     def setUp(self):
         super().setUp()  # Call the parent class setup
 
         # Assuming you have already set up some StaffMember objects in the BaseTest
@@ -735,20 +735,29 @@
         """Test trying to retrieve non-working days using a non-existent StaffMember ID."""
         nonexistent_id = self.staff_member_with_working_days.id + 100  # Just to ensure a non-existent ID
         non_working_days = get_non_working_days_for_staff(nonexistent_id)
         self.assertListEqual(non_working_days, [])
 
 
 class TestGetStaffMemberAppointmentList(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
+        self.client1 = self.users['client1']
 
         # Creating appointments for each staff member.
-        self.appointment1_for_user1 = self.create_appointment_for_user1()
-        self.appointment2_for_user2 = self.create_appointment_for_user2()
+        self.appointment1_for_user1 = self.create_appt_for_sm1()
+        self.appointment2_for_user2 = self.create_appt_for_sm2()
 
     def test_retrieve_appointments_for_specific_staff_member(self):
         """Test retrieving appointments for a specific StaffMember."""
         # Testing for staff_member1
         appointments_for_staff_member1 = get_staff_member_appointment_list(self.staff_member1)
         self.assertIn(self.appointment1_for_user1, appointments_for_staff_member1)
         self.assertNotIn(self.appointment2_for_user2, appointments_for_staff_member1)
@@ -779,105 +788,40 @@
             datetime.date(2023, 10, 15): 0,  # Sunday
         }
 
         for date, expected_weekday_num in sample_dates.items():
             self.assertEqual(get_weekday_num_from_date(date), expected_weekday_num)
 
 
-@patch('appointment.utils.db_helpers.APPOINTMENT_BUFFER_TIME', 60)
-@patch('appointment.utils.db_helpers.APPOINTMENT_SLOT_DURATION', 30)
-class TestStaffMemberTimeFunctions(BaseTest):
-    """Test suite for staff member time functions."""
-
-    def setUp(self):
-        super().setUp()
-
-        # Set staff member-specific settings
-        self.staff_member1.slot_duration = 15
-        self.staff_member1.lead_time = datetime.time(8, 30)
-        self.staff_member1.finish_time = datetime.time(18, 0)
-        self.staff_member1.appointment_buffer_time = 45
-        self.staff_member1.save()
-
-        # Setting WorkingHours for staff_member1 for Monday
-        self.wh = WorkingHours.objects.create(
-            staff_member=self.staff_member1,
-            day_of_week=1,
-            start_time=datetime.time(9, 0),
-            end_time=datetime.time(17, 0)
-        )
-
-    def test_staff_member_buffer_time_with_global_setting(self):
-        """Test buffer time when staff member-specific setting is None."""
-        self.staff_member1.appointment_buffer_time = None
-        self.staff_member1.save()
-        buffer_time = get_staff_member_buffer_time(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(buffer_time, 60)  # Global setting
-
-    def test_staff_member_buffer_time_with_staff_member_setting(self):
-        """Test buffer time using staff member-specific setting."""
-        buffer_time = get_staff_member_buffer_time(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(buffer_time, 45)  # Staff member specific setting
-
-    def test_staff_member_slot_duration_with_global_setting(self):
-        """Test slot duration when staff member-specific setting is None."""
-        self.staff_member1.slot_duration = None
-        self.staff_member1.save()
-        slot_duration = get_staff_member_slot_duration(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(slot_duration, 30)  # Global setting
-
-    def test_staff_member_slot_duration_with_staff_member_setting(self):
-        """Test slot duration using staff member-specific setting."""
-        slot_duration = get_staff_member_slot_duration(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(slot_duration, 15)  # Staff member specific setting
-
-    def test_staff_member_start_time(self):
-        """Test start time based on WorkingHours."""
-        start_time = get_staff_member_start_time(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(start_time, datetime.time(9, 0))
-
-    def test_staff_member_end_time(self):
-        """Test end time based on WorkingHours."""
-        end_time = get_staff_member_end_time(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(end_time, datetime.time(17, 0))
-
-    def test_staff_member_start_time_with_lead_time(self):
-        """Test start time when both lead_time and WorkingHours are available."""
-        start_time = get_staff_member_start_time(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(start_time, self.wh.start_time)  # lead_time should prevail
-
-    def test_staff_member_end_time_with_finish_time(self):
-        """Test end time when both finish_time and WorkingHours are available."""
-        end_time = get_staff_member_end_time(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(end_time, self.wh.end_time)  # finish_time should prevail
-
-    def test_staff_member_buffer_time_with_working_hours_conflict(self):
-        """Test buffer time when it conflicts with WorkingHours."""
-        self.staff_member1.appointment_buffer_time = 120  # Set a buffer time greater than WorkingHours start time
-        self.staff_member1.save()
-        buffer_time = get_staff_member_buffer_time(self.staff_member1, datetime.date(2023, 10, 9))
-        self.assertEqual(buffer_time, 120)  # Should still use staff member-specific setting even if it causes conflict
-
-
 class TestDBHelpers(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
     def setUp(self):
         super().setUp()
+        self.user1 = self.users['staff1']
+        self.user2 = self.users['staff2']
 
     def test_get_staff_member_by_user_id(self):
         """Test retrieving a StaffMember object using a user id works as expected."""
         staff = get_staff_member_by_user_id(self.user1.id)
         self.assertIsNotNone(staff)
         self.assertEqual(staff, self.staff_member1)
 
         # Test for a non-existent user id
         staff = get_staff_member_by_user_id(99999)
         self.assertIsNone(staff)
 
     def test_get_staff_member_from_user_id_or_logged_in(self):
-        """Test retrieving a StaffMember object using a user id or the logged in user works as expected."""
+        """Test retrieving a StaffMember object using a user id or the logged-in user works as expected."""
         staff = get_staff_member_from_user_id_or_logged_in(self.user1)
         self.assertIsNotNone(staff)
         self.assertEqual(staff, self.staff_member1)
 
         staff = get_staff_member_from_user_id_or_logged_in(self.user1, self.user2.id)
         self.assertIsNotNone(staff)
         self.assertEqual(staff, self.staff_member2)
@@ -890,31 +834,31 @@
         """Test retrieving the user model works as expected."""
         user_model = get_user_model()
         user_model_in_settings = apps.get_model(settings.AUTH_USER_MODEL)
         self.assertEqual(user_model, user_model_in_settings)
 
     def test_get_user_by_email(self):
         """Retrieve a user by email."""
-        user = get_user_by_email("tester1@gmail.com")
+        user = get_user_by_email("daniel.jackson@django-appointment.com")
         self.assertIsNotNone(user)
         self.assertEqual(user, self.user1)
 
         # Test for a non-existent email
-        user = get_user_by_email("nonexistent@gmail.com")
+        user = get_user_by_email("nonexistent@django-appointment.com")
         self.assertIsNone(user)
 
 
 class TestWorkingHoursFunctions(BaseTest):
     def setUp(self):
         super().setUp()
         self.working_hours = WorkingHours.objects.create(
-            staff_member=self.staff_member1,
-            day_of_week=1,  # Monday
-            start_time=datetime.time(9, 0),
-            end_time=datetime.time(17, 0)
+                staff_member=self.staff_member1,
+                day_of_week=1,  # Monday
+                start_time=datetime.time(9, 0),
+                end_time=datetime.time(17, 0)
         )
 
     def test_get_working_hours_by_id(self):
         """Test retrieving a WorkingHours object by ID."""
         working_hours = get_working_hours_by_id(self.working_hours.id)
         self.assertEqual(working_hours, self.working_hours)
 
@@ -940,36 +884,42 @@
     def test_is_working_day(self):
         """is_working_day() should return True if there are WorkingHours for the staff member and day,
            False otherwise."""
         self.assertTrue(is_working_day(self.staff_member1, 1))  # Monday
         self.assertFalse(is_working_day(self.staff_member1, 2))  # Tuesday
 
     def test_working_hours_exist(self):
-        """working_hours_exist() should return True if there are WorkingHours for the staff member and day,"""
+        """working_hours_exist() should return True if there are WorkingHours for the staff member and day,
+           False otherwise."""
         self.assertTrue(working_hours_exist(1, self.staff_member1))  # Monday
         self.assertFalse(working_hours_exist(2, self.staff_member1))  # Tuesday
 
 
 @patch('appointment.utils.db_helpers.APPOINTMENT_LEAD_TIME', (7, 0))
 @patch('appointment.utils.db_helpers.APPOINTMENT_FINISH_TIME', (15, 0))
 @patch('appointment.utils.db_helpers.APPOINTMENT_SLOT_DURATION', 30)
 @patch('appointment.utils.db_helpers.APPOINTMENT_BUFFER_TIME', 60)
 class TestGetTimesFromConfig(TestCase):
     def setUp(self):
         self.sample_date = datetime.date(2023, 10, 9)
         cache.clear()
 
+    def tearDown(self):
+        super().tearDown()
+        # Reset or delete the Config instance to ensure test isolation
+        Config.objects.all().delete()
+
     def test_times_from_config_object(self):
         """Test retrieving times from a Config object."""
         # Create a Config object with custom values
         Config.objects.create(
-            lead_time=datetime.time(9, 0),
-            finish_time=datetime.time(17, 0),
-            slot_duration=45,
-            appointment_buffer_time=90
+                lead_time=datetime.time(9, 0),
+                finish_time=datetime.time(17, 0),
+                slot_duration=45,
+                appointment_buffer_time=90
         )
 
         start_time, end_time, slot_duration, buff_time = get_times_from_config(self.sample_date)
 
         # Assert times from 'Config' object
         self.assertEqual(start_time, datetime.datetime(2023, 10, 9, 9, 0))
         self.assertEqual(end_time, datetime.datetime(2023, 10, 9, 17, 0))
@@ -989,56 +939,61 @@
         self.assertEqual(slot_duration, datetime.timedelta(minutes=30))
         self.assertEqual(buff_time, datetime.timedelta(minutes=60))
 
 
 class CreateNewUserTest(TestCase):
     def test_create_new_user_unique_username(self):
         """Test creating a new user with a unique username."""
-        client_data = {'name': 'John Doe', 'email': 'john.doe@example.com'}
+        client_data = {'name': 'Cameron Mitchell', 'email': 'cameron.mitchell@django-appointment.com'}
         user = create_new_user(client_data)
-        self.assertEqual(user.username, 'john.doe')
-        self.assertEqual(user.first_name, 'John')
-        self.assertEqual(user.email, 'john.doe@example.com')
+        self.assertEqual(user.username, 'cameron.mitchell')
+        self.assertEqual(user.first_name, 'Cameron')
+        self.assertEqual(user.email, 'cameron.mitchell@django-appointment.com')
 
     def test_create_new_user_duplicate_username(self):
         """Test creating a new user with a duplicate username."""
-        client_data1 = {'name': 'John Doe', 'email': 'john.doe@example.com'}
+        client_data1 = {'name': 'Martouf of Malkshur', 'email': 'the.malkshur@django-appointment.com'}
         user1 = create_new_user(client_data1)
-        self.assertEqual(user1.username, 'john.doe')
+        self.assertEqual(user1.username, 'the.malkshur')
 
-        client_data2 = {'name': 'Jane Doe', 'email': 'john.doe@example.com'}
+        client_data2 = {'name': 'Jolinar of Malkshur', 'email': 'the.malkshur@django-appointment.com'}
         user2 = create_new_user(client_data2)
-        self.assertEqual(user2.username, 'john.doe01')  # Suffix added
+        self.assertEqual(user2.username, 'the.malkshur01')  # Suffix added
 
-        client_data3 = {'name': 'James Doe', 'email': 'john.doe@example.com'}
+        client_data3 = {'name': 'Lantash of Malkshur', 'email': 'the.malkshur@django-appointment.com'}
         user3 = create_new_user(client_data3)
-        self.assertEqual(user3.username, 'john.doe02')  # Next suffix
+        self.assertEqual(user3.username, 'the.malkshur02')  # Next suffix
 
     def test_generate_unique_username(self):
         """Test if generate_unique_username_from_email function generates unique usernames."""
-        email = 'john.doe@example.com'
+        email = 'jacob.carter@django-appointment.com'
         username = generate_unique_username_from_email(email)
-        self.assertEqual(username, 'john.doe')
+        self.assertEqual(username, 'jacob.carter')
 
         # Assuming we have a user with the same username
         CLIENT_MODEL = get_user_model()
-        CLIENT_MODEL.objects.create_user(username='john.doe', email=email)
+        CLIENT_MODEL.objects.create_user(username='jacob.carter', email=email)
         new_username = generate_unique_username_from_email(email)
-        self.assertEqual(new_username, 'john.doe01')
+        self.assertEqual(new_username, 'jacob.carter01')
 
     def test_parse_name(self):
         """Test if parse_name function splits names correctly."""
-        name = "John Doe"
+        name = "Garshaw of Belote"
+        first_name, last_name = parse_name(name)
+        self.assertEqual(first_name, 'Garshaw')
+        self.assertEqual(last_name, 'of Belote')
+
+        name = "Teal'c"
         first_name, last_name = parse_name(name)
-        self.assertEqual(first_name, 'John')
-        self.assertEqual(last_name, 'Doe')
+        self.assertEqual(first_name, "Teal'c")
+        self.assertEqual(last_name, '')
 
     def test_create_new_user_check_password(self):
         """Test creating a new user with a password."""
-        client_data = {'name': 'John Doe', 'email': 'john.doe@example.com'}
+        client_data = {'name': 'Harry Maybourne', 'email': 'harry.maybourne@django-appointment.com'}
         user = create_new_user(client_data)
         # Check that no password has been set
         self.assertFalse(user.has_usable_password())
 
 
 class UsernameInUserModelTests(TestCase):
 
@@ -1077,52 +1032,52 @@
         filtered_slots = exclude_pending_reschedules(self.slots, self.staff_member1, self.date)
         self.assertEqual(len(filtered_slots), len(self.slots))
 
     def test_exclude_with_pending_reschedules_outside_last_5_minutes(self):
         """Slots should remain unchanged if pending reschedules are outside the last 5 minutes."""
         appointment_request = self.create_appointment_request_(self.service1, self.staff_member1)
         self.create_reschedule_history_(
-            appointment_request,
-            date_=self.date,
-            start_time=(timezone.now() - datetime.timedelta(minutes=10)).time(),
-            end_time=(timezone.now() - datetime.timedelta(minutes=5)).time(),
-            staff_member=self.staff_member1,
-            reason_for_rescheduling="Scheduling conflict"
+                appointment_request,
+                date_=self.date,
+                start_time=(timezone.now() - datetime.timedelta(minutes=10)).time(),
+                end_time=(timezone.now() - datetime.timedelta(minutes=5)).time(),
+                staff_member=self.staff_member1,
+                reason_for_rescheduling="Scheduling conflict"
         )
         filtered_slots = exclude_pending_reschedules(self.slots, self.staff_member1, self.date)
         self.assertEqual(len(filtered_slots), len(self.slots))
 
     def test_exclude_with_pending_reschedules_within_last_5_minutes(self):
         """Slots overlapping with pending rescheduling within the last 5 minutes should be excluded."""
         appointment_request = self.create_appointment_request_(self.service1, self.staff_member1)
         reschedule_start_time = (timezone.now() - datetime.timedelta(minutes=4)).time()
         reschedule_end_time = (timezone.now() + datetime.timedelta(minutes=1)).time()
         self.create_reschedule_history_(
-            appointment_request,
-            date_=self.date,
-            start_time=reschedule_start_time,
-            end_time=reschedule_end_time,
-            staff_member=self.staff_member1,
-            reason_for_rescheduling="Client request"
+                appointment_request,
+                date_=self.date,
+                start_time=reschedule_start_time,
+                end_time=reschedule_end_time,
+                staff_member=self.staff_member1,
+                reason_for_rescheduling="Client request"
         )
         filtered_slots = exclude_pending_reschedules(self.slots, self.staff_member1, self.date)
         self.assertEqual(len(filtered_slots), len(self.slots) - 1)  # Assuming only one slot overlaps
 
     def test_exclude_with_non_pending_reschedules_within_last_5_minutes(self):
         """Slots should remain unchanged if reschedules within the last 5 minutes are not pending."""
         appointment_request = self.create_appointment_request_(self.service1, self.staff_member1)
         reschedule_start_time = (timezone.now() - datetime.timedelta(minutes=4)).time()
         reschedule_end_time = (timezone.now() + datetime.timedelta(minutes=1)).time()
         reschedule = self.create_reschedule_history_(
-            appointment_request,
-            date_=self.date,
-            start_time=reschedule_start_time,
-            end_time=reschedule_end_time,
-            staff_member=self.staff_member1,
-            reason_for_rescheduling="Urgent issue"
+                appointment_request,
+                date_=self.date,
+                start_time=reschedule_start_time,
+                end_time=reschedule_end_time,
+                staff_member=self.staff_member1,
+                reason_for_rescheduling="Urgent issue"
         )
         reschedule.reschedule_status = 'confirmed'
         reschedule.save()
         filtered_slots = exclude_pending_reschedules(self.slots, self.staff_member1, self.date)
         self.assertEqual(len(filtered_slots), len(self.slots))
```

### Comparing `django-appointment-3.4.1/appointment/tests/utils/test_email_ops.py` & `django_appointment-3.5.0/appointment/tests/utils/test_email_ops.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,170 +1,231 @@
+from copy import deepcopy
+from datetime import datetime
 from unittest import mock
 from unittest.mock import MagicMock, patch
 
 from django.test.client import RequestFactory
 from django.utils import timezone
 from django.utils.translation import gettext as _
 
 from appointment.messages_ import thank_you_no_payment, thank_you_payment, thank_you_payment_plus_down
 from appointment.models import AppointmentRescheduleHistory
 from appointment.tests.base.base_test import BaseTest
 from appointment.utils.email_ops import (
-    get_thank_you_message, notify_admin_about_appointment, send_reschedule_confirmation_email,
+    get_thank_you_message, notify_admin_about_appointment, notify_admin_about_reschedule,
+    send_reschedule_confirmation_email,
     send_reset_link_to_staff_member, send_thank_you_email,
     send_verification_email
 )
 
 
 class SendResetLinkToStaffMemberTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
 
     def setUp(self):
         super().setUp()
-        self.user = self.user1
+        self.user = deepcopy(self.users['staff1'])
         self.user.is_staff = True
         self.user.save()
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
-        self.email = 'staff@example.com'
+        self.email = 'daniel.jackson@django-appointment.com'
 
     @mock.patch('appointment.utils.email_ops.send_email')
     @mock.patch('appointment.models.PasswordResetToken.create_token')
-    def test_send_reset_link(self, mock_create_token, mock_send_email):
-        # Setup the token
+    @mock.patch('appointment.utils.email_ops.get_absolute_url_')
+    @mock.patch('appointment.utils.email_ops.get_website_name')
+    def test_send_reset_link(self, mock_get_website_name, mock_get_absolute_url, mock_create_token, mock_send_email):
+        # Set up the token
         mock_token = mock.Mock()
-        mock_token.token = 'token123'
+        mock_token.token = "Colonel_Samantha_Carter_a_Tau_ri_Scientist"
         mock_create_token.return_value = mock_token
 
-        # Assume get_absolute_url_ and get_website_name are utility functions you've defined somewhere
-        with mock.patch('appointment.utils.email_ops.get_absolute_url_') as mock_get_absolute_url:
-            with mock.patch('appointment.utils.email_ops.get_website_name') as mock_get_website_name:
-                mock_get_absolute_url.return_value = 'http://testserver/reset_password'
-                mock_get_website_name.return_value = 'TestCompany'
-
-                send_reset_link_to_staff_member(self.user, self.request, self.email)
-
-                # Check send_email was called with correct parameters
-                mock_send_email.assert_called_once()
-                args, kwargs = mock_send_email.call_args
-                self.assertEqual(kwargs['recipient_list'], [self.email])
-                self.assertIn('TestCompany', kwargs['message'])
-                self.assertIn('http://testserver/reset_password', kwargs['message'])
+        mock_get_absolute_url.return_value = f"http://gateroomserver/reset_password/{mock_token.token}"
+        mock_get_website_name.return_value = 'Gate Room Server'
+
+        send_reset_link_to_staff_member(self.user, self.request, self.email)
+
+        # Check send_email was called with correct parameters
+        mock_send_email.assert_called_once()
+        args, kwargs = mock_send_email.call_args
+        self.assertEqual(kwargs['recipient_list'], [self.email])
+        self.assertIn('Gate Room Server', kwargs['message'])
+        self.assertIn('http://gateroomserver/reset_password', kwargs['message'])
+        self.assertIn('Colonel_Samantha_Carter_a_Tau_ri_Scientist', kwargs['message'])
+
+        # Additional assertions to verify more parts of the message content
+        self.assertIn('Hello', kwargs['message'])
+        self.assertIn(self.user.first_name, kwargs['message'])
+        self.assertIn(str(datetime.now().year), kwargs['message'])
+        self.assertIn('No additional details provided.', kwargs['message'])
+        self.assertIn(self.user.username, kwargs['message'])
 
 
 class GetThankYouMessageTests(BaseTest):
+
+    def setUp(self):
+        super().setUp()
+        self.ar = MagicMock()
+
     def test_thank_you_no_payment(self):
         with patch('appointment.utils.email_ops.APPOINTMENT_PAYMENT_URL', None):
-            ar = MagicMock()
-            message = get_thank_you_message(ar)
+            message = get_thank_you_message(self.ar)
             self.assertIn(thank_you_no_payment, message)
 
     def test_thank_you_payment_plus_down(self):
         with patch('appointment.utils.email_ops.APPOINTMENT_PAYMENT_URL', "http://payment.url"):
-            ar = MagicMock()
-            ar.accepts_down_payment.return_value = True
-            message = get_thank_you_message(ar)
+            self.ar.accepts_down_payment.return_value = True
+            message = get_thank_you_message(self.ar)
             self.assertIn(thank_you_payment_plus_down, message)
 
     def test_thank_you_payment(self):
         with patch('appointment.utils.email_ops.APPOINTMENT_PAYMENT_URL', "http://payment.url"):
-            ar = MagicMock()
-            ar.accepts_down_payment.return_value = False
-            message = get_thank_you_message(ar)
+            self.ar.accepts_down_payment.return_value = False
+            message = get_thank_you_message(self.ar)
             self.assertIn(thank_you_payment, message)
 
 
 class SendThankYouEmailTests(BaseTest):
     def setUp(self):
         super().setUp()
         self.factory = RequestFactory()
         self.request = self.factory.get('/')
+        self.ar = self.create_appt_request_for_sm1()
+        self.email = "georges.s.hammond@django-appointment.com"
+        self.appointment_details = "Details about the appointment"
+        self.account_details = "Details about the account"
 
     @patch('appointment.utils.email_ops.send_email')
     @patch('appointment.utils.email_ops.get_thank_you_message')
     def test_send_thank_you_email(self, mock_get_thank_you_message, mock_send_email):
-        ar = self.create_appt_request_for_sm1()
-        email = "test@example.com"
-        appointment_details = "Details about the appointment"
-        account_details = "Details about the account"
-
         mock_get_thank_you_message.return_value = "Thank you message"
 
-        send_thank_you_email(ar, self.user1, self.request, email, appointment_details, account_details)
+        send_thank_you_email(self.ar, self.users['client1'], self.request, self.email, self.appointment_details,
+                             self.account_details)
 
         mock_send_email.assert_called_once()
         args, kwargs = mock_send_email.call_args
-        self.assertIn(email, kwargs['recipient_list'])
+        self.assertIn(self.email, kwargs['recipient_list'])
         self.assertIn("Thank you message", kwargs['context']['message_1'])
 
 
 class NotifyAdminAboutAppointmentTests(BaseTest):
     def setUp(self):
         super().setUp()
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
+        self.client_name = "Oma Desala"
 
     @patch('appointment.utils.email_ops.notify_admin')
     @patch('appointment.utils.email_ops.send_email')
     def test_notify_admin_about_appointment(self, mock_send_email, mock_notify_admin):
-        client_name = "John Doe"
-
-        notify_admin_about_appointment(self.appointment, client_name)
-
+        notify_admin_about_appointment(self.appointment, self.client_name)
         mock_notify_admin.assert_called_once()
         mock_send_email.assert_called_once()
 
 
 class SendVerificationEmailTests(BaseTest):
     def setUp(self):
         super().setUp()
-        self.appointment = self.create_appointment_for_user1()
+        self.appointment = self.create_appt_for_sm1()
+        self.email = "richard.woolsey@django-appointment.com"
 
     @patch('appointment.utils.email_ops.send_email')
     @patch('appointment.models.EmailVerificationCode.generate_code', return_value="123456")
     def test_send_verification_email(self, mock_generate_code, mock_send_email):
         user = MagicMock()
-        email = "test@example.com"
 
-        send_verification_email(user, email)
+        send_verification_email(user, self.email)
 
         mock_send_email.assert_called_once_with(
-            recipient_list=[email],
-            subject=_("Email Verification"),
-            message=mock.ANY
+                recipient_list=[self.email],
+                subject=_("Email Verification"),
+                message=mock.ANY
         )
         self.assertIn("123456", mock_send_email.call_args[1]['message'])
 
 
 class SendRescheduleConfirmationEmailTests(BaseTest):
     def setUp(self):
-        # Setup test data
         super().setUp()
-        self.user = self.user1
         self.appointment_request = self.create_appt_request_for_sm1()
         self.reschedule_history = AppointmentRescheduleHistory.objects.create(
-            appointment_request=self.appointment_request,
-            date=self.appointment_request.date + timezone.timedelta(days=1),
-            start_time=self.appointment_request.start_time,
-            end_time=self.appointment_request.end_time,
-            staff_member=self.staff_member1,
-            reason_for_rescheduling="Test reason"
+                appointment_request=self.appointment_request,
+                date=self.appointment_request.date + timezone.timedelta(days=1),
+                start_time=self.appointment_request.start_time,
+                end_time=self.appointment_request.end_time,
+                staff_member=self.staff_member1,
+                reason_for_rescheduling="Had to reschedule because I got stuck in a time loop. Again"
         )
-        self.first_name = "Test"
-        self.email = "test@example.com"
+        self.first_name = "Jack"
+        self.email = "jack.oneill@django-appointment.com"
 
     @mock.patch('appointment.utils.email_ops.get_absolute_url_')
     @mock.patch('appointment.utils.email_ops.send_email')
     def test_send_reschedule_confirmation_email(self, mock_send_email, mock_get_absolute_url):
         request = mock.MagicMock()
-        mock_get_absolute_url.return_value = "http://testserver/confirmation_link"
+        mock_get_absolute_url.return_value = "http://gateroomserver/confirmation_link"
 
         send_reschedule_confirmation_email(request, self.reschedule_history, self.appointment_request, self.first_name,
                                            self.email)
 
         # Check if `send_email` was called correctly
         mock_send_email.assert_called_once()
         call_args, call_kwargs = mock_send_email.call_args
 
         self.assertEqual(call_kwargs['recipient_list'], [self.email])
         self.assertEqual(call_kwargs['subject'], _("Confirm Your Appointment Rescheduling"))
         self.assertIn('reschedule_date', call_kwargs['context'])
         self.assertIn('confirmation_link', call_kwargs['context'])
-        self.assertEqual(call_kwargs['context']['confirmation_link'], "http://testserver/confirmation_link")
+        self.assertEqual(call_kwargs['context']['confirmation_link'], "http://gateroomserver/confirmation_link")
+
+
+class NotifyAdminAboutRescheduleTests(BaseTest):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+    @classmethod
+    def tearDownClass(cls):
+        super().tearDownClass()
+
+    def setUp(self):
+        super().setUp()
+        self.appointment_request = self.create_appt_request_for_sm1()
+        self.reschedule_history = AppointmentRescheduleHistory.objects.create(
+                appointment_request=self.appointment_request,
+                date=self.appointment_request.date + timezone.timedelta(days=1),
+                start_time=self.appointment_request.start_time,
+                end_time=self.appointment_request.end_time,
+                staff_member=self.staff_member1,
+                reason_for_rescheduling="Captured by Anubis"
+        )
+        self.client_name = "Jonas Quinn"
+
+    @patch('appointment.utils.email_ops.notify_admin')
+    @patch('appointment.utils.email_ops.send_email')
+    @patch('appointment.utils.email_ops.get_website_name', return_value="Stargate Command")
+    @patch('appointment.utils.email_ops.convert_24_hour_time_to_12_hour_time',
+           side_effect=lambda x: x.strftime("%I:%M %p"))
+    def test_notify_admin_about_reschedule(self, mock_convert_time, mock_get_website_name, mock_send_email,
+                                           mock_notify_admin):
+        notify_admin_about_reschedule(self.reschedule_history, self.appointment_request, self.client_name)
+
+        # Check if notify_admin was called correctly
+        mock_notify_admin.assert_called_once()
+        notify_admin_args, notify_admin_kwargs = mock_notify_admin.call_args
+        self.assertIn(self.client_name, notify_admin_kwargs['subject'])
+        self.assertEqual(notify_admin_kwargs['context']['client_name'], self.client_name)
+        self.assertEqual(notify_admin_kwargs['context']['service_name'], self.appointment_request.service.name)
+        self.assertEqual(notify_admin_kwargs['context']['reason_for_rescheduling'],
+                         self.reschedule_history.reason_for_rescheduling)
+        self.assertEqual(notify_admin_kwargs['context']['old_date'],
+                         self.appointment_request.date.strftime("%A, %d %B %Y"))
+        self.assertEqual(notify_admin_kwargs['context']['reschedule_date'],
+                         self.reschedule_history.date.strftime("%A, %d %B %Y"))
+        self.assertEqual(notify_admin_kwargs['context']['company'], "Stargate Command")
```

### Comparing `django-appointment-3.4.1/appointment/urls.py` & `django_appointment-3.5.0/appointment/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 
 from appointment.views import (
     appointment_client_information, appointment_request, appointment_request_submit, confirm_reschedule,
     default_thank_you, enter_verification_code, get_available_slots_ajax, get_next_available_date_ajax,
     get_non_working_days_ajax, prepare_reschedule_appointment, reschedule_appointment_submit, set_passwd
 )
 from appointment.views_admin import (
-    add_day_off, add_or_update_service, add_or_update_staff_info, add_working_hours, create_new_staff_member,
-    delete_appointment, delete_appointment_ajax, delete_day_off, delete_service, delete_working_hours,
-    display_appointment, email_change_verification_code, fetch_service_list_for_staff, fetch_staff_list,
-    get_service_list, get_user_appointments, is_user_staff_admin, make_superuser_staff_member, remove_staff_member,
-    remove_superuser_staff_member, update_appt_date_time, update_appt_min_info, update_day_off, update_personal_info,
-    update_working_hours, user_profile, validate_appointment_date
+    add_day_off, add_or_update_service, add_or_update_staff_info, add_staff_member_info, add_working_hours,
+    create_new_staff_member, delete_appointment, delete_appointment_ajax, delete_day_off, delete_service,
+    delete_working_hours, display_appointment, email_change_verification_code, fetch_service_list_for_staff,
+    fetch_staff_list, get_service_list, get_user_appointments, is_user_staff_admin, make_superuser_staff_member,
+    remove_staff_member, remove_superuser_staff_member, update_appt_date_time, update_appt_min_info, update_day_off,
+    update_personal_info, update_working_hours, user_profile, validate_appointment_date
 )
 
 app_name = 'appointment'
 
 admin_urlpatterns = [
     # display the calendar with the events
     path('appointments/<str:response_type>/', get_user_appointments, name='get_user_event_type'),
     path('appointments/', get_user_appointments, name='get_user_appointments'),
 
     # create a new staff member and make/remove superuser staff member
-    path('staff-member-personal-info/', create_new_staff_member, name='add_staff_member_personal_info'),
+    path('add-staff-member-info/', add_staff_member_info, name='add_staff_member_info'),
+    path('create-new-staff-member/', create_new_staff_member, name='add_staff_member_personal_info'),
     path('update-staff-member/<int:user_id>/', add_or_update_staff_info, name='update_staff_other_info'),
     path('add-staff-member/', add_or_update_staff_info, name='add_staff_other_info'),
     path('make-superuser-staff-member/', make_superuser_staff_member, name='make_superuser_staff_member'),
     path('remove-superuser-staff-member/', remove_superuser_staff_member, name='remove_superuser_staff_member'),
 
     # remove staff member
     path('remove-staff-member/<int:staff_user_id>/', remove_staff_member, name='remove_staff_member'),
```

### Comparing `django-appointment-3.4.1/appointment/utils/date_time.py` & `django_appointment-3.5.0/appointment/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/utils/db_helpers.py` & `django_appointment-3.5.0/appointment/utils/db_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import datetime
 from typing import Optional
 from urllib.parse import urlparse
 
 from django.apps import apps
-from django.conf import settings
+from django.contrib.auth import get_user_model
 from django.core.cache import cache
 from django.core.exceptions import FieldDoesNotExist
 from django.urls import reverse
 from django.utils import timezone
 from django_q.models import Schedule
 from django_q.tasks import schedule
 
@@ -99,16 +99,16 @@
     :param client_data: The data of the client making the appointment.
     :param appointment_data: Additional data for the appointment, including phone number, address, etc.
     :param request: The request object.
     :return: The newly created appointment.
     """
     user = get_user_by_email(client_data['email'])
     appointment = Appointment.objects.create(
-        client=user, appointment_request=ar,
-        **appointment_data
+            client=user, appointment_request=ar,
+            **appointment_data
     )
     appointment.save()
     logger.info(f"New appointment created: {appointment.to_dict()}")
     schedule_email_reminder(appointment, request)
     return appointment
 
 
@@ -175,15 +175,15 @@
         cancel_existing_reminder(appointment.id_request)
 
         # If a reminder is still desired and the appointment is in the future, schedule a new one
         if want_reminder and new_datetime > timezone.now():
             schedule_email_reminder(appointment, request, new_datetime)
         else:
             logger.info(
-                f"Reminder for appointment {appointment.id} is not scheduled per user's preference or past datetime.")
+                    f"Reminder for appointment {appointment.id} is not scheduled per user's preference or past datetime.")
 
     # Update the appointment's reminder preference
     appointment.want_reminder = want_reminder
     appointment.save()
 
 
 def cancel_existing_reminder(appointment_id_request):
@@ -230,15 +230,18 @@
         suffix_str = f"{suffix:02}"
         username = f"{username_base}{suffix_str}"
         suffix += 1
     return username
 
 
 def parse_name(name: str):
-    return name.split(' ', 1)
+    parts = name.split(' ', 1)
+    if len(parts) == 1:
+        parts.append('')  # Add an empty string for the last name if not provided
+    return parts[0], parts[1]
 
 
 def create_user_with_email(client_data: dict):
     CLIENT_MODEL = get_user_model()
     # Valid fields
     valid_fields = ['email', 'first_name', 'last_name']
 
@@ -305,16 +308,16 @@
     payment_info.save()
 
     # Check if APPOINTMENT_PAYMENT_URL is a Django reverse URL (e.g. "app:view_name") or an external link
     if (":" in APPOINTMENT_PAYMENT_URL and "/" not in APPOINTMENT_PAYMENT_URL) and not bool(
             urlparse(APPOINTMENT_PAYMENT_URL).netloc):
         # It's a Django reverse URL; generate the URL
         payment_url = reverse(
-            APPOINTMENT_PAYMENT_URL,
-            kwargs={'object_id': payment_info.id, 'id_request': payment_info.get_id_request()}
+                APPOINTMENT_PAYMENT_URL,
+                kwargs={'object_id': payment_info.id, 'id_request': payment_info.get_id_request()}
         )
     else:
         # It's an external link; return as is or append necessary data
         payment_url = APPOINTMENT_PAYMENT_URL
 
     return payment_url
 
@@ -346,18 +349,18 @@
     """
     Exclude the slots that are pending reschedule for the given staff member and date.
     """
 
     # Calculate the time window for "last 5 minutes"
     ten_minutes_ago = timezone.now() - datetime.timedelta(minutes=5)
     pending_reschedules = AppointmentRescheduleHistory.objects.filter(
-        appointment_request__staff_member=staff_member,
-        date=date,
-        reschedule_status='pending',
-        created_at__gte=ten_minutes_ago
+            appointment_request__staff_member=staff_member,
+            date=date,
+            reschedule_status='pending',
+            created_at__gte=ten_minutes_ago
     )
 
     # Filter out slots that overlap with any pending rescheduling
     filtered_slots = slots[:]
     for reschedule in pending_reschedules:
         reschedule_start_time = datetime.datetime.combine(date, reschedule.start_time)
         reschedule_end_time = datetime.datetime.combine(date, reschedule.end_time)
@@ -474,18 +477,18 @@
     :param start_time: The starting time to filter appointments on.
     :param end_time: The ending time to filter appointments on.
     :param staff_member: The staff member to filter appointments on.
 
     :return: QuerySet, all appointments that overlap with the specified date and time range
     """
     return Appointment.objects.filter(
-        appointment_request__date=date,
-        appointment_request__start_time__lte=end_time,
-        appointment_request__end_time__gte=start_time,
-        appointment_request__staff_member=staff_member
+            appointment_request__date=date,
+            appointment_request__start_time__lte=end_time,
+            appointment_request__end_time__gte=start_time,
+            appointment_request__staff_member=staff_member
     )
 
 
 def get_config():
     """Returns the configuration object from the database or the cache."""
     config = cache.get('config')
     if not config:
@@ -602,22 +605,14 @@
         finish_hour, finish_minute = APPOINTMENT_FINISH_TIME
         end_time = datetime.datetime.combine(date, datetime.time(hour=finish_hour, minute=finish_minute))
         slot_duration = datetime.timedelta(minutes=APPOINTMENT_SLOT_DURATION)
         buff_time = datetime.timedelta(minutes=APPOINTMENT_BUFFER_TIME)
     return start_time, end_time, slot_duration, buff_time
 
 
-def get_user_model():
-    """Get the client models from the settings file.
-
-    :return: The user model
-    """
-    return apps.get_model(settings.AUTH_USER_MODEL)
-
-
 def get_user_by_email(email: str):
     """Get a user by their email address.
 
     :param email: The email address of the user.
     :return: The user with the specified email address, if found; otherwise, None.
     """
     CLIENT_MODEL = get_user_model()
```

### Comparing `django-appointment-3.4.1/appointment/utils/email_ops.py` & `django_appointment-3.5.0/appointment/utils/email_ops.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/utils/error_codes.py` & `django_appointment-3.5.0/appointment/utils/error_codes.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/utils/json_context.py` & `django_appointment-3.5.0/appointment/utils/json_context.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/utils/permissions.py` & `django_appointment-3.5.0/appointment/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/utils/session.py` & `django_appointment-3.5.0/appointment/utils/session.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/utils/view_helpers.py` & `django_appointment-3.5.0/appointment/utils/view_helpers.py`

 * *Files identical despite different names*

### Comparing `django-appointment-3.4.1/appointment/views.py` & `django_appointment-3.5.0/appointment/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.encoding import force_str
 from django.utils.http import urlsafe_base64_decode
 from django.utils.timezone import get_current_timezone_name
 from django.utils.translation import gettext as _
 
-from appointment.forms import AppointmentForm, AppointmentRequestForm
+from appointment.forms import AppointmentForm, AppointmentRequestForm, SlotForm, ClientDataForm
 from appointment.logger_config import logger
 from appointment.models import (
     Appointment, AppointmentRequest, AppointmentRescheduleHistory, Config, DayOff, EmailVerificationCode,
     PasswordResetToken, Service,
     StaffMember
 )
 from appointment.utils.db_helpers import (
@@ -53,44 +53,41 @@
 @require_ajax
 def get_available_slots_ajax(request):
     """This view function handles AJAX requests to get available slots for a selected date.
 
     :param request: The request instance.
     :return: A JSON response containing available slots, selected date, an error flag, and an optional error message.
     """
-    selected_date = convert_str_to_date(request.GET.get('selected_date'))
-    staff_id = request.GET.get('staff_id')
 
-    if selected_date < date.today():
+    slot_form = SlotForm(request.GET)
+    if not slot_form.is_valid():
         custom_data = {'error': True, 'available_slots': [], 'date_chosen': ''}
-        message = _('Date is in the past')
+        if 'selected_date' in slot_form.errors:
+            error_code = ErrorCode.PAST_DATE
+        elif 'staff_member' in slot_form.errors:
+            error_code = ErrorCode.STAFF_ID_REQUIRED
+        message = list(slot_form.errors.as_data().items())[0][1][0].messages[0]  # dirty way to keep existing behavior
         return json_response(message=message, custom_data=custom_data, success=False,
-                             error_code=ErrorCode.PAST_DATE)
+                             error_code=error_code)
 
+    selected_date = slot_form.cleaned_data['selected_date']
+    sm = slot_form.cleaned_data['staff_member']
     date_chosen = selected_date.strftime("%a, %B %d, %Y")
     custom_data = {'date_chosen': date_chosen}
 
-    # If no staff_id provided, return an empty list of slots
-    if not staff_id or staff_id == 'none':
-        custom_data['available_slots'] = []
-        custom_data['error'] = False
-        message = _('No staff member selected')
-        return json_response(message=message, custom_data=custom_data, success=False,
-                             error_code=ErrorCode.STAFF_ID_REQUIRED, status=403)
-
-    sm = get_object_or_404(StaffMember, pk=staff_id)
-    custom_data['staff_member'] = sm.get_staff_member_name()
     days_off_exist = check_day_off_for_staff(staff_member=sm, date=selected_date)
     if days_off_exist:
         message = _("Day off. Please select another date!")
         custom_data['available_slots'] = []
         return json_response(message=message, custom_data=custom_data, success=False, error_code=ErrorCode.INVALID_DATE)
     # if selected_date is not a working day for the staff, return an empty list of slots and 'message' is Day Off
     weekday_num = get_weekday_num_from_date(selected_date)
     is_working_day_ = is_working_day(staff_member=sm, day=weekday_num)
+
+    custom_data['staff_member'] = sm.get_staff_member_name()
     if not is_working_day_:
         message = _("Not a working day for {staff_member}. Please select another date!").format(
             staff_member=sm.get_staff_member_first_name())
         custom_data['available_slots'] = []
         return json_response(message=message, custom_data=custom_data, success=False, error_code=ErrorCode.INVALID_DATE)
     available_slots = get_available_slots_for_staff(selected_date, sm)
 
@@ -104,14 +101,15 @@
         custom_data['error'] = True
         message = _('No availability')
         return json_response(message=message, custom_data=custom_data, success=False, error_code=ErrorCode.INVALID_DATE)
     custom_data['error'] = False
     return json_response(message='Successfully retrieved available slots', custom_data=custom_data, success=True)
 
 
+# TODO: service id and staff id are not checked
 @require_ajax
 def get_next_available_date_ajax(request, service_id):
     """This view function handles AJAX requests to get the next available date for a service.
 
     :param request: The request instance.
     :param service_id: The ID of the service.
     :return: A JSON response containing the next available date.
@@ -155,14 +153,15 @@
         data = {'error': True}
         message = _('No staff member selected')
         return json_response(message=message, custom_data=data, success=False, error_code=ErrorCode.STAFF_ID_REQUIRED)
 
 
 def get_non_working_days_ajax(request):
     staff_id = request.GET.get('staff_id')
+    print(f"staff_id: {staff_id}")
     error = False
     message = _('Successfully retrieved non-working days')
 
     if not staff_id or staff_id == 'none':
         message = _('No staff member selected')
         error_code = ErrorCode.STAFF_ID_REQUIRED
         error = True
@@ -288,40 +287,14 @@
     :return: The redirect response.
     """
     appointment = create_and_save_appointment(appointment_request_obj, client_data, appointment_data, request)
     notify_admin_about_appointment(appointment, appointment.client.first_name)
     return redirect_to_payment_or_thank_you_page(appointment)
 
 
-def get_client_data_from_post(request):
-    """This function retrieves client data from the POST request.
-
-    :param request: The request instance.
-    :return: The client data.
-    """
-    return {
-        'name': request.POST.get('name'),
-        'email': request.POST.get('email'),
-    }
-
-
-def get_appointment_data_from_post_request(request):
-    """This function retrieves appointment data from the POST request.
-
-    :param request: The request instance.
-    :return: The appointment data.
-    """
-    return {
-        'phone': request.POST.get('phone'),
-        'want_reminder': request.POST.get('want_reminder') == 'on',
-        'address': request.POST.get('address'),
-        'additional_info': request.POST.get('additional_info'),
-    }
-
-
 def appointment_client_information(request, appointment_request_id, id_request):
     """This view function handles client information submission for an appointment.
 
     :param request: The request instance.
     :param appointment_request_id: The ID of the appointment request.
     :param id_request: The unique ID of the appointment request.
     :return: The rendered HTML page.
@@ -329,18 +302,19 @@
     ar = get_object_or_404(AppointmentRequest, pk=appointment_request_id)
     if request.session.get(f'appointment_submitted_{id_request}', False):
         context = get_generic_context_with_extra(request, {'service_id': ar.service_id}, admin=False)
         return render(request, 'error_pages/304_already_submitted.html', context=context)
 
     if request.method == 'POST':
         appointment_form = AppointmentForm(request.POST)
+        client_data_form = ClientDataForm(request.POST)
 
-        if appointment_form.is_valid():
+        if appointment_form.is_valid() and client_data_form.is_valid():
             appointment_data = appointment_form.cleaned_data
-            client_data = get_client_data_from_post(request)
+            client_data = client_data_form.cleaned_data
             payment_type = request.POST.get('payment_type')
             ar.payment_type = payment_type
             ar.save()
 
             # Check if email is already in the database
             is_email_in_db = CLIENT_MODEL.objects.filter(email__exact=client_data['email']).exists()
             if is_email_in_db:
@@ -352,19 +326,21 @@
 
             # Create a new appointment
             response = create_appointment(request, ar, client_data, appointment_data)
             request.session.setdefault(f'appointment_submitted_{id_request}', True)
             return response
     else:
         appointment_form = AppointmentForm()
+        client_data_form = ClientDataForm()
 
     extra_context = {
         'ar': ar,
         'APPOINTMENT_PAYMENT_URL': APPOINTMENT_PAYMENT_URL,
         'form': appointment_form,
+        'client_data_form': client_data_form,
         'service_name': ar.service.name,
     }
     context = get_generic_context_with_extra(request, extra_context, admin=False)
     return render(request, 'appointment/appointment_client_information.html', context=context)
 
 
 def verify_user_and_login(request, user, code):
```

### Comparing `django-appointment-3.4.1/appointment/views_admin.py` & `django_appointment-3.5.0/appointment/views_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from django.core.exceptions import ValidationError
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_POST
 
 from appointment.decorators import (
     require_ajax, require_staff_or_superuser, require_superuser, require_user_authenticated)
-from appointment.forms import PersonalInformationForm, ServiceForm, StaffAppointmentInformationForm
+from appointment.forms import PersonalInformationForm, ServiceForm, StaffAppointmentInformationForm, StaffMemberForm
 from appointment.messages_ import appt_updated_successfully
 from appointment.models import Appointment, DayOff, StaffMember, WorkingHours
 from appointment.services import (
     create_new_appointment, create_staff_member_service, email_change_verification_service,
     fetch_user_appointments, handle_entity_management_request, handle_service_management_request,
     prepare_appointment_display_data, prepare_user_profile_data, save_appt_date_time, update_existing_appointment,
     update_personal_info_service)
@@ -61,16 +61,14 @@
             user=request.user).exists() and not request.user.is_superuser:
         messages.error(request, _("User doesn't have a staff member instance. Please contact the administrator."))
     return render(request, 'administration/staff_index.html', context)
 
 
 @require_user_authenticated
 @require_staff_or_superuser
-@require_user_authenticated
-@require_staff_or_superuser
 def display_appointment(request, appointment_id):
     appointment, page_title, error_message, status_code = prepare_appointment_display_data(request.user, appointment_id)
 
     if error_message:
         context = get_generic_context(request=request)
         return render(request, 'error_pages/404_not_found.html', context=context, status=status_code)
     # If everything is okay, render the HTML template.
@@ -272,15 +270,15 @@
 @require_superuser
 def fetch_staff_list(request):
     staff_members = StaffMember.objects.all()
     staff_data = []
     for staff in staff_members:
         staff_data.append({
             'id': staff.id,
-            'name': staff.user.get_full_name(),
+            'name': staff.get_staff_member_name(),
         })
     return json_response("Successfully fetched staff members.", custom_data={'staff_members': staff_data}, safe=False)
 
 
 @require_user_authenticated
 @require_staff_or_superuser
 @require_ajax
@@ -399,14 +397,29 @@
 
 
 ###############################################################
 
 
 @require_user_authenticated
 @require_superuser
+def add_staff_member_info(request):
+    if request.method == 'POST':
+        form = StaffMemberForm(request.POST)
+        if form.is_valid():
+            form.save()
+            return redirect('appointment:user_profile')
+    else:
+        form = StaffMemberForm()
+
+    context = get_generic_context_with_extra(request=request, extra={'form': form})
+    return render(request, 'administration/manage_staff_member.html', context)
+
+
+@require_user_authenticated
+@require_superuser
 def create_new_staff_member(request):
     if request.method == 'POST':
         user, is_valid, error_message = create_staff_member_service(request.POST, request)
         if is_valid:
             return redirect('appointment:user_profile', staff_user_id=user.pk)
         else:
             messages.error(request, error_message)
```

### Comparing `django-appointment-3.4.1/django_appointment.egg-info/PKG-INFO` & `django_appointment-3.5.0/django_appointment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 3.4.1
+Version: 3.5.0
 Summary: Managing appointment scheduling with customizable slots, staff features, and conflict handling.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
-Author-email: adamspd.developer@gmail.com
+Author-email: django-appt@adamspierredavid.com
 License: Apache License 2.0
 Project-URL: Author's Website, https://adamspierredavid.com/
-Project-URL: Package's Website, https://django-appt.adamspierredavid.com/
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Package's demo Website, https://django-appt.adamspierredavid.com/
+Project-URL: Documentation, https://django-appt-doc.adamspierredavid.com/overview.html
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -37,15 +38,14 @@
 
 ![Tests](https://github.com/adamspd/django-appointment/actions/workflows/tests.yml/badge.svg)
 ![Published on PyPi](https://github.com/adamspd/django-appointment/actions/workflows/publish.yml/badge.svg)
 [![Doc](https://github.com/adamspd/django-appointment-doc/actions/workflows/build-docs.yml/badge.svg)](https://django-appt-doc.adamspierredavid.com/overview.html)
 [![Current Release Version](https://img.shields.io/github/release/adamspd/django-appointment.svg?style=flat-square&logo=github)](https://github.com/adamspd/django-appointment/releases)
 [![pypi Version](https://img.shields.io/pypi/v/django-appointment.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/django-appointment/)
 [![PyPi downloads](https://static.pepy.tech/personalized-badge/django-appointment?period=total&units=international_system&left_color=grey&right_color=orange&left_text=pip%20downloads)](https://pypi.org/project/django-appointment/)
-[![codecov](https://codecov.io/gh/adamspd/django-appointment/branch/main/graph/badge.svg?token=ZQZQZQZQZQ)](https://codecov.io/gh/adamspd/django-appointment)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/commits/main)
 [![GitHub last commit](https://img.shields.io/github/last-commit/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/commit/main)
 [![GitHub issues](https://img.shields.io/github/issues/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/pulls)
 [![GitHub contributors](https://img.shields.io/github/contributors/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/graphs/contributors)
 [![GitHub stars](https://img.shields.io/github/stars/adamspd/django-appointment)](https://github.com/adamspd/django-appointment/stargazers)
@@ -331,15 +331,14 @@
 ## Security policy 🔒
 
 Please refer to the [security policy](https://github.com/adamspd/django-appointment/tree/main/SECURITY.md) for more
 information.
 
 ## Notes 📝⚠️
 
-I'm working on a testing website for the application
-that is not fully functional yet, no hard feelings. But you can check it out
-at [https://django-appt.adamspierredavid.com/](https://django-appt.adamspierredavid.com/). Ideas are welcome here since
-I'm blocked on a few points.
+I'm working on a testing website for the application that is not fully functional yet, no hard feelings. Before using it, 
+it's important to me that you read the terms of use, only then you can use it if you agree to them. The demo website is located
+at [https://django-appt.adamspierredavid.com/](https://django-appt.adamspierredavid.com/terms-and-conditions/). Ideas are welcome.
 
 ## About the Author
 
 Adams Pierre David - [Website](https://adamspierredavid.com/)
```

### Comparing `django-appointment-3.4.1/django_appointment.egg-info/SOURCES.txt` & `django_appointment-3.5.0/django_appointment.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -67,49 +67,51 @@
 appointment/templates/error_pages/403_forbidden.html
 appointment/templates/error_pages/403_forbidden_rescheduling.html
 appointment/templates/error_pages/404_not_found.html
 appointment/templates/modal/confirm_modal.html
 appointment/templates/modal/error_modal.html
 appointment/templates/modal/event_details_modal.html
 appointment/tests/__init__.py
-appointment/tests/test_availability_slot.py
 appointment/tests/test_services.py
 appointment/tests/test_settings.py
 appointment/tests/test_tasks.py
-appointment/tests/test_utils.py
 appointment/tests/test_views.py
 appointment/tests/base/__init__.py
 appointment/tests/base/base_test.py
 appointment/tests/mixins/base_mixin.py
 appointment/tests/models/__init__.py
+appointment/tests/models/test_appointment.py
+appointment/tests/models/test_appointment_request.py
 appointment/tests/models/test_appointment_reschedule_history.py
-appointment/tests/models/test_model_appointment.py
-appointment/tests/models/test_model_appointment_request.py
-appointment/tests/models/test_model_config.py
-appointment/tests/models/test_model_day_off.py
-appointment/tests/models/test_model_email_verification.py
-appointment/tests/models/test_model_password_reset_token.py
-appointment/tests/models/test_model_payment_info.py
-appointment/tests/models/test_model_service.py
-appointment/tests/models/test_model_staff_member.py
-appointment/tests/models/test_model_working_hours.py
+appointment/tests/models/test_config.py
+appointment/tests/models/test_day_off.py
+appointment/tests/models/test_email_verification.py
+appointment/tests/models/test_password_reset_token.py
+appointment/tests/models/test_payment_info.py
+appointment/tests/models/test_service.py
+appointment/tests/models/test_staff_member.py
+appointment/tests/models/test_working_hours.py
 appointment/tests/utils/__init__.py
 appointment/tests/utils/test_date_time.py
 appointment/tests/utils/test_db_helpers.py
 appointment/tests/utils/test_email_ops.py
 appointment/tests/utils/test_json_context.py
 appointment/tests/utils/test_permissions.py
 appointment/tests/utils/test_session.py
+appointment/tests/utils/test_staff_member_time.py
+appointment/tests/utils/test_validators.py
+appointment/tests/utils/test_view_helpers.py
 appointment/utils/__init__.py
 appointment/utils/date_time.py
 appointment/utils/db_helpers.py
 appointment/utils/email_ops.py
 appointment/utils/error_codes.py
 appointment/utils/json_context.py
 appointment/utils/permissions.py
 appointment/utils/session.py
+appointment/utils/validators.py
 appointment/utils/view_helpers.py
 django_appointment.egg-info/PKG-INFO
 django_appointment.egg-info/SOURCES.txt
 django_appointment.egg-info/dependency_links.txt
 django_appointment.egg-info/requires.txt
 django_appointment.egg-info/top_level.txt
```

### Comparing `django-appointment-3.4.1/setup.cfg` & `django_appointment-3.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license = Apache License 2.0
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Framework :: Django
 	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `django-appointment-3.4.1/setup.py` & `django_appointment-3.5.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 from appointment import (__author__, __author_email__, __author_website__, __description__, __package_name__, __url__,
-                         __version__, __package_website__)
+                         __version__, __package_website__, __package_doc_url__)
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=__package_name__,
     version=__version__,
@@ -13,10 +13,11 @@
     author_email=__author_email__,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=__url__,
     description=__description__,
     project_urls={
         "Author's Website": __author_website__,
-        "Package's Website": __package_website__,
+        "Package's demo Website": __package_website__,
+        "Documentation": __package_doc_url__,
     },
 )
```

