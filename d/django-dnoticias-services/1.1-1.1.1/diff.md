# Comparing `tmp/django_dnoticias_services-1.1.tar.gz` & `tmp/django_dnoticias_services-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_dnoticias_services-1.1.tar", max compression
+gzip compressed data, was "django_dnoticias_services-1.1.1.tar", max compression
```

## Comparing `django_dnoticias_services-1.1.tar` & `django_dnoticias_services-1.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     8504 2022-05-23 10:44:57.902943 django_dnoticias_services-1.1/README.md
--rw-r--r--   0        0        0        0 2022-05-25 13:23:14.922229 django_dnoticias_services-1.1/dnoticias_services/__init__.py
--rw-r--r--   0        0        0      110 2023-03-14 11:53:02.164481 django_dnoticias_services-1.1/dnoticias_services/apps.py
--rw-r--r--   0        0        0        0 2022-05-25 13:23:14.922229 django_dnoticias_services-1.1/dnoticias_services/authentication/__init__.py
--rw-r--r--   0        0        0    16268 2022-09-14 09:17:36.996105 django_dnoticias_services-1.1/dnoticias_services/authentication/__pycache__/keycloak.cpython-39.pyc
--rw-r--r--   0        0        0    21793 2023-05-03 09:52:34.714117 django_dnoticias_services-1.1/dnoticias_services/authentication/keycloak.py
--rw-r--r--   0        0        0     1780 2022-12-12 11:52:10.567533 django_dnoticias_services-1.1/dnoticias_services/authentication/utils.py
--rw-r--r--   0        0        0     1458 2023-03-14 11:53:06.048556 django_dnoticias_services-1.1/dnoticias_services/base_service.py
--rw-r--r--   0        0        0     9977 2022-05-31 09:52:15.081929 django_dnoticias_services-1.1/dnoticias_services/communications/README.md
--rw-r--r--   0        0        0      546 2022-05-25 14:40:55.088980 django_dnoticias_services-1.1/dnoticias_services/communications/__init__.py
--rw-r--r--   0        0        0      312 2022-05-31 13:36:07.428819 django_dnoticias_services-1.1/dnoticias_services/communications/base.py
--rw-r--r--   0        0        0     1932 2022-06-15 09:52:04.884099 django_dnoticias_services-1.1/dnoticias_services/communications/campaign.py
--rw-r--r--   0        0        0      830 2022-05-27 11:36:17.379337 django_dnoticias_services-1.1/dnoticias_services/communications/context_processors.py
--rw-r--r--   0        0        0     9992 2023-03-15 11:08:34.805569 django_dnoticias_services-1.1/dnoticias_services/communications/forms.py
--rw-r--r--   0        0        0     7986 2022-08-08 13:32:02.586796 django_dnoticias_services-1.1/dnoticias_services/communications/mail.py
--rw-r--r--   0        0        0    16467 2023-03-29 11:01:55.674248 django_dnoticias_services-1.1/dnoticias_services/communications/notification.py
--rw-r--r--   0        0        0     1258 2022-05-25 16:30:00.343321 django_dnoticias_services-1.1/dnoticias_services/communications/urls.py
--rw-r--r--   0        0        0     9535 2023-02-28 13:20:39.922125 django_dnoticias_services-1.1/dnoticias_services/communications/views.py
--rw-r--r--   0        0        0       69 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/editions/__init__.py
--rw-r--r--   0        0        0      318 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/editions/base.py
--rw-r--r--   0        0        0      463 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/editions/editions.py
--rw-r--r--   0        0        0      559 2023-03-14 11:53:08.144596 django_dnoticias_services-1.1/dnoticias_services/mail.py
--rw-r--r--   0        0        0      911 2022-05-25 16:05:47.245917 django_dnoticias_services-1.1/dnoticias_services/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-05-25 16:04:02.278616 django_dnoticias_services-1.1/dnoticias_services/migrations/__init__.py
--rw-r--r--   0        0        0      600 2022-05-25 16:05:05.166185 django_dnoticias_services-1.1/dnoticias_services/models.py
--rw-r--r--   0        0        0      429 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/__init__.py
--rw-r--r--   0        0        0      315 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/base.py
--rw-r--r--   0        0        0      118 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/choices.py
--rw-r--r--   0        0        0      956 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/coupons.py
--rw-r--r--   0        0        0     3989 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1/dnoticias_services/payments/items.py
--rw-r--r--   0        0        0     3003 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/orders.py
--rw-r--r--   0        0        0     2909 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/payments.py
--rw-r--r--   0        0        0      641 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/providers.py
--rw-r--r--   0        0        0      790 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/payments/subscriptions.py
--rw-r--r--   0        0        0      380 2022-09-09 15:13:31.674218 django_dnoticias_services-1.1/dnoticias_services/subscriptions/__init__.py
--rw-r--r--   0        0        0     2301 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/address.py
--rw-r--r--   0        0        0      288 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/base.py
--rw-r--r--   0        0        0     1825 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/billing.py
--rw-r--r--   0        0        0      680 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/coupons.py
--rw-r--r--   0        0        0     1120 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/digital.py
--rw-r--r--   0        0        0     7402 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/product.py
--rw-r--r--   0        0        0      728 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1/dnoticias_services/subscriptions/subscription.py
--rw-r--r--   0        0        0     2667 2022-09-09 15:19:18.788266 django_dnoticias_services-1.1/dnoticias_services/subscriptions/user.py
--rw-r--r--   0        0        0    31442 2022-05-26 11:25:32.824297 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/form.html
--rw-r--r--   0        0        0    13998 2023-03-14 12:08:55.758648 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/list.html
--rw-r--r--   0        0        0    12182 2022-05-25 15:36:10.049172 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/form.html
--rw-r--r--   0        0        0    11431 2022-05-26 14:30:21.971269 django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/list.html
--rw-r--r--   0        0        0     8239 2022-05-27 11:34:25.955533 django_dnoticias_services-1.1/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js
--rw-r--r--   0        0        0      129 2022-05-25 13:23:14.934229 django_dnoticias_services-1.1/dnoticias_services/utils/__init__.py
--rw-r--r--   0        0        0     1060 2022-10-12 11:04:19.148455 django_dnoticias_services-1.1/dnoticias_services/utils/request.py
--rw-r--r--   0        0        0      227 2023-02-10 15:49:58.731527 django_dnoticias_services-1.1/dnoticias_services/utils/urls.py
--rw-r--r--   0        0        0     4608 2023-02-14 11:01:33.706003 django_dnoticias_services-1.1/dnoticias_services/utils/views.py
--rw-r--r--   0        0        0      699 2023-05-03 11:29:20.696188 django_dnoticias_services-1.1/pyproject.toml
--rw-r--r--   0        0        0     9351 1970-01-01 00:00:00.000000 django_dnoticias_services-1.1/PKG-INFO
+-rw-r--r--   0        0        0     8504 2022-05-23 10:44:57.902943 django_dnoticias_services-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2022-05-25 13:23:14.922229 django_dnoticias_services-1.1.1/dnoticias_services/__init__.py
+-rw-r--r--   0        0        0      110 2023-03-14 11:53:02.164481 django_dnoticias_services-1.1.1/dnoticias_services/apps.py
+-rw-r--r--   0        0        0        0 2022-05-25 13:23:14.922229 django_dnoticias_services-1.1.1/dnoticias_services/authentication/__init__.py
+-rw-r--r--   0        0        0    16268 2022-09-14 09:17:36.996105 django_dnoticias_services-1.1.1/dnoticias_services/authentication/__pycache__/keycloak.cpython-39.pyc
+-rw-r--r--   0        0        0    21793 2023-05-03 09:52:34.714117 django_dnoticias_services-1.1.1/dnoticias_services/authentication/keycloak.py
+-rw-r--r--   0        0        0     1780 2022-12-12 11:52:10.567533 django_dnoticias_services-1.1.1/dnoticias_services/authentication/utils.py
+-rw-r--r--   0        0        0     1458 2023-03-14 11:53:06.048556 django_dnoticias_services-1.1.1/dnoticias_services/base_service.py
+-rw-r--r--   0        0        0     9977 2022-05-31 09:52:15.081929 django_dnoticias_services-1.1.1/dnoticias_services/communications/README.md
+-rw-r--r--   0        0        0      546 2022-05-25 14:40:55.088980 django_dnoticias_services-1.1.1/dnoticias_services/communications/__init__.py
+-rw-r--r--   0        0        0      312 2022-05-31 13:36:07.428819 django_dnoticias_services-1.1.1/dnoticias_services/communications/base.py
+-rw-r--r--   0        0        0     1932 2022-06-15 09:52:04.884099 django_dnoticias_services-1.1.1/dnoticias_services/communications/campaign.py
+-rw-r--r--   0        0        0      830 2022-05-27 11:36:17.379337 django_dnoticias_services-1.1.1/dnoticias_services/communications/context_processors.py
+-rw-r--r--   0        0        0     9992 2023-03-15 11:08:34.805569 django_dnoticias_services-1.1.1/dnoticias_services/communications/forms.py
+-rw-r--r--   0        0        0     7986 2022-08-08 13:32:02.586796 django_dnoticias_services-1.1.1/dnoticias_services/communications/mail.py
+-rw-r--r--   0        0        0    16467 2023-03-29 11:01:55.674248 django_dnoticias_services-1.1.1/dnoticias_services/communications/notification.py
+-rw-r--r--   0        0        0     1258 2022-05-25 16:30:00.343321 django_dnoticias_services-1.1.1/dnoticias_services/communications/urls.py
+-rw-r--r--   0        0        0     9535 2023-02-28 13:20:39.922125 django_dnoticias_services-1.1.1/dnoticias_services/communications/views.py
+-rw-r--r--   0        0        0       69 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/editions/__init__.py
+-rw-r--r--   0        0        0      318 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/editions/base.py
+-rw-r--r--   0        0        0      463 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/editions/editions.py
+-rw-r--r--   0        0        0      559 2023-03-14 11:53:08.144596 django_dnoticias_services-1.1.1/dnoticias_services/mail.py
+-rw-r--r--   0        0        0      911 2022-05-25 16:05:47.245917 django_dnoticias_services-1.1.1/dnoticias_services/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-05-25 16:04:02.278616 django_dnoticias_services-1.1.1/dnoticias_services/migrations/__init__.py
+-rw-r--r--   0        0        0      600 2022-05-25 16:05:05.166185 django_dnoticias_services-1.1.1/dnoticias_services/models.py
+-rw-r--r--   0        0        0      429 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/payments/__init__.py
+-rw-r--r--   0        0        0      315 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/payments/base.py
+-rw-r--r--   0        0        0      118 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/payments/choices.py
+-rw-r--r--   0        0        0      956 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/payments/coupons.py
+-rw-r--r--   0        0        0     3989 2022-05-25 13:23:14.926229 django_dnoticias_services-1.1.1/dnoticias_services/payments/items.py
+-rw-r--r--   0        0        0     3003 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/payments/orders.py
+-rw-r--r--   0        0        0     2909 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/payments/payments.py
+-rw-r--r--   0        0        0      641 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/payments/providers.py
+-rw-r--r--   0        0        0      790 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/payments/subscriptions.py
+-rw-r--r--   0        0        0      380 2022-09-09 15:13:31.674218 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/__init__.py
+-rw-r--r--   0        0        0     2301 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/address.py
+-rw-r--r--   0        0        0      288 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/base.py
+-rw-r--r--   0        0        0     1825 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/billing.py
+-rw-r--r--   0        0        0      680 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/coupons.py
+-rw-r--r--   0        0        0     1120 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/digital.py
+-rw-r--r--   0        0        0     7402 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/product.py
+-rw-r--r--   0        0        0      728 2022-05-25 13:23:14.930230 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/subscription.py
+-rw-r--r--   0        0        0     2667 2022-09-09 15:19:18.788266 django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/user.py
+-rw-r--r--   0        0        0    31442 2022-05-26 11:25:32.824297 django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-notifications/form.html
+-rw-r--r--   0        0        0    13998 2023-03-14 12:08:55.758648 django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-notifications/list.html
+-rw-r--r--   0        0        0    12182 2022-05-25 15:36:10.049172 django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-topics/form.html
+-rw-r--r--   0        0        0    11431 2022-05-26 14:30:21.971269 django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-topics/list.html
+-rw-r--r--   0        0        0     8239 2022-05-27 11:34:25.955533 django_dnoticias_services-1.1.1/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js
+-rw-r--r--   0        0        0      129 2022-05-25 13:23:14.934229 django_dnoticias_services-1.1.1/dnoticias_services/utils/__init__.py
+-rw-r--r--   0        0        0     1177 2023-05-25 15:26:52.235666 django_dnoticias_services-1.1.1/dnoticias_services/utils/request.py
+-rw-r--r--   0        0        0      227 2023-02-10 15:49:58.731527 django_dnoticias_services-1.1.1/dnoticias_services/utils/urls.py
+-rw-r--r--   0        0        0     4608 2023-02-14 11:01:33.706003 django_dnoticias_services-1.1.1/dnoticias_services/utils/views.py
+-rw-r--r--   0        0        0      701 2023-05-25 15:28:03.267528 django_dnoticias_services-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9353 1970-01-01 00:00:00.000000 django_dnoticias_services-1.1.1/PKG-INFO
```

### Comparing `django_dnoticias_services-1.1/README.md` & `django_dnoticias_services-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/authentication/__pycache__/keycloak.cpython-39.pyc` & `django_dnoticias_services-1.1.1/dnoticias_services/authentication/__pycache__/keycloak.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/authentication/keycloak.py` & `django_dnoticias_services-1.1.1/dnoticias_services/authentication/keycloak.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/authentication/utils.py` & `django_dnoticias_services-1.1.1/dnoticias_services/authentication/utils.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/base_service.py` & `django_dnoticias_services-1.1.1/dnoticias_services/base_service.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/README.md` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/README.md`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/__init__.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/__init__.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/campaign.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/campaign.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/context_processors.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/forms.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/forms.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/mail.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/mail.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/notification.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/notification.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/urls.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/urls.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/communications/views.py` & `django_dnoticias_services-1.1.1/dnoticias_services/communications/views.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/mail.py` & `django_dnoticias_services-1.1.1/dnoticias_services/mail.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/migrations/0001_initial.py` & `django_dnoticias_services-1.1.1/dnoticias_services/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/models.py` & `django_dnoticias_services-1.1.1/dnoticias_services/models.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/payments/coupons.py` & `django_dnoticias_services-1.1.1/dnoticias_services/payments/coupons.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/payments/items.py` & `django_dnoticias_services-1.1.1/dnoticias_services/payments/items.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/payments/orders.py` & `django_dnoticias_services-1.1.1/dnoticias_services/payments/orders.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/payments/payments.py` & `django_dnoticias_services-1.1.1/dnoticias_services/payments/payments.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/payments/providers.py` & `django_dnoticias_services-1.1.1/dnoticias_services/payments/providers.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/payments/subscriptions.py` & `django_dnoticias_services-1.1.1/dnoticias_services/payments/subscriptions.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/subscriptions/address.py` & `django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/address.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/subscriptions/billing.py` & `django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/billing.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/subscriptions/coupons.py` & `django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/coupons.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/subscriptions/digital.py` & `django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/digital.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/subscriptions/product.py` & `django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/product.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/subscriptions/subscription.py` & `django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/subscriptions/user.py` & `django_dnoticias_services-1.1.1/dnoticias_services/subscriptions/user.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/form.html` & `django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-notifications/form.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-notifications/list.html` & `django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-notifications/list.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/form.html` & `django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-topics/form.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/templates/backoffice/fcm-topics/list.html` & `django_dnoticias_services-1.1.1/dnoticias_services/templates/backoffice/fcm-topics/list.html`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js` & `django_dnoticias_services-1.1.1/dnoticias_services/templates/frontoffice/includes/firebase-notifications.js`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/dnoticias_services/utils/request.py` & `django_dnoticias_services-1.1.1/dnoticias_services/utils/request.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,19 @@
     Used in get user email list datatable because the MetronicProcess class
     uses the request methods.
     """
     def __call__(self, GET={}, POST={}, user_id=None, ajax=False):
         self.GET = GET
         self.POST = POST
         self.ajax = ajax
+        self.headers = {}
+
+        if ajax:
+            self.headers.update({"X-Requested-With": "XMLHttpRequest"})
+
         self.user = self.set_user(user_id) if user_id else None
 
     def is_ajax(self):
         return self.ajax
 
     def set_ajax(self, value):
         self.ajax = bool(value)
```

### Comparing `django_dnoticias_services-1.1/dnoticias_services/utils/views.py` & `django_dnoticias_services-1.1.1/dnoticias_services/utils/views.py`

 * *Files identical despite different names*

### Comparing `django_dnoticias_services-1.1/pyproject.toml` & `django_dnoticias_services-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "django_dnoticias_services"
-version = "1.1"
+version = "1.1.1"
 authors = [
     "Pedro Mendes <pedro.trabalho.uma@gmail.com>",
     "Nélson Gomes <ngoncalves@dnoticias.pt>",
 ]
 description = "Dnoticias Services"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `django_dnoticias_services-1.1/PKG-INFO` & `django_dnoticias_services-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dnoticias-services
-Version: 1.1
+Version: 1.1.1
 Summary: Dnoticias Services
 License: MIT
 Author: Pedro Mendes
 Author-email: pedro.trabalho.uma@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

