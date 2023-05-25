# Comparing `tmp/cofactr-5.8.0.tar.gz` & `tmp/cofactr-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofactr-5.8.0.tar", max compression
+gzip compressed data, was "cofactr-5.9.0.tar", max compression
```

## Comparing `cofactr-5.8.0.tar` & `cofactr-5.9.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1063 2022-04-25 20:30:48.813559 cofactr-5.8.0/LICENSE.txt
--rw-r--r--   0        0        0      407 2022-05-19 21:43:48.329452 cofactr-5.8.0/README.md
--rw-r--r--   0        0        0        0 2022-05-13 00:05:54.890551 cofactr-5.8.0/cofactr/__init__.py
--rw-r--r--   0        0        0    17821 2022-07-27 14:16:45.629660 cofactr-5.8.0/cofactr/graph.py
--rw-r--r--   0        0        0      747 2022-05-11 17:24:24.039422 cofactr-5.8.0/cofactr/helpers.py
--rw-r--r--   0        0        0        0 2022-05-13 00:06:22.350816 cofactr-5.8.0/cofactr/kb/__init__.py
--rw-r--r--   0        0        0       46 2022-05-11 17:24:24.039422 cofactr-5.8.0/cofactr/kb/entity/__init__.py
--rw-r--r--   0        0        0      608 2022-06-12 02:22:50.223769 cofactr-5.8.0/cofactr/kb/entity/aliases.py
--rw-r--r--   0        0        0      388 2022-06-12 02:22:50.223769 cofactr-5.8.0/cofactr/kb/entity/labels.py
--rw-r--r--   0        0        0      331 2022-06-12 02:22:50.223769 cofactr-5.8.0/cofactr/kb/entity/qualifier.py
--rw-r--r--   0        0        0      857 2022-06-12 02:22:50.223769 cofactr-5.8.0/cofactr/kb/entity/statement_object.py
--rw-r--r--   0        0        0     3979 2022-05-11 17:24:24.043422 cofactr-5.8.0/cofactr/kb/entity/types.py
--rw-r--r--   0        0        0      801 2022-05-11 17:24:24.043422 cofactr-5.8.0/cofactr/render.py
--rw-r--r--   0        0        0     2791 2022-07-19 18:59:07.650212 cofactr-5.8.0/cofactr/schema/__init__.py
--rw-r--r--   0        0        0        0 2022-05-13 00:06:10.262699 cofactr-5.8.0/cofactr/schema/flagship/__init__.py
--rw-r--r--   0        0        0     1777 2022-07-19 19:16:35.914080 cofactr-5.8.0/cofactr/schema/flagship/offer.py
--rw-r--r--   0        0        0      787 2022-06-09 18:15:57.431785 cofactr-5.8.0/cofactr/schema/flagship/part.py
--rw-r--r--   0        0        0      706 2022-06-09 18:15:57.431785 cofactr-5.8.0/cofactr/schema/flagship/seller.py
--rw-r--r--   0        0        0        0 2022-06-23 16:03:16.440503 cofactr-5.8.0/cofactr/schema/flagship_v2/__init__.py
--rw-r--r--   0        0        0      450 2022-06-23 16:03:16.440503 cofactr-5.8.0/cofactr/schema/flagship_v2/part.py
--rw-r--r--   0        0        0        0 2022-07-08 20:30:16.641306 cofactr-5.8.0/cofactr/schema/flagship_v3/__init__.py
--rw-r--r--   0        0        0      305 2022-07-08 20:30:16.641306 cofactr-5.8.0/cofactr/schema/flagship_v3/part.py
--rw-r--r--   0        0        0        0 2022-05-13 00:06:03.206631 cofactr-5.8.0/cofactr/schema/logistics/__init__.py
--rw-r--r--   0        0        0      468 2022-05-11 17:24:24.043422 cofactr-5.8.0/cofactr/schema/logistics/offer.py
--rw-r--r--   0        0        0     1100 2022-06-23 16:03:16.440503 cofactr-5.8.0/cofactr/schema/logistics/part.py
--rw-r--r--   0        0        0        0 2022-06-23 16:03:16.440503 cofactr-5.8.0/cofactr/schema/logistics_v2/__init__.py
--rw-r--r--   0        0        0      296 2022-07-15 16:29:55.199387 cofactr-5.8.0/cofactr/schema/logistics_v2/part.py
--rw-r--r--   0        0        0        0 2022-07-08 20:30:16.645305 cofactr-5.8.0/cofactr/schema/logistics_v3/__init__.py
--rw-r--r--   0        0        0      270 2022-07-08 20:30:16.645305 cofactr-5.8.0/cofactr/schema/logistics_v3/part.py
--rw-r--r--   0        0        0        0 2022-07-15 16:18:14.441798 cofactr-5.8.0/cofactr/schema/logistics_v4/__init__.py
--rw-r--r--   0        0        0      711 2022-07-19 18:54:24.735374 cofactr-5.8.0/cofactr/schema/logistics_v4/part.py
--rw-r--r--   0        0        0        0 2022-07-19 18:53:55.875103 cofactr-5.8.0/cofactr/schema/price_solver_v0/__init__.py
--rw-r--r--   0        0        0      514 2022-07-19 19:16:17.217860 cofactr-5.8.0/cofactr/schema/price_solver_v0/part.py
--rw-r--r--   0        0        0      478 2022-06-23 16:03:16.440503 cofactr-5.8.0/cofactr/schema/types.py
--rw-r--r--   0        0        0      854 2022-07-27 14:16:45.630174 cofactr-5.8.0/pyproject.toml
--rw-r--r--   0        0        0     1397 2022-07-27 14:16:50.585906 cofactr-5.8.0/setup.py
--rw-r--r--   0        0        0     1026 2022-07-27 14:16:50.586056 cofactr-5.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2022-04-25 20:30:48.813559 cofactr-5.9.0/LICENSE.txt
+-rw-r--r--   0        0        0      407 2022-05-19 21:43:48.329452 cofactr-5.9.0/README.md
+-rw-r--r--   0        0        0        0 2022-05-13 00:05:54.890551 cofactr-5.9.0/cofactr/__init__.py
+-rw-r--r--   0        0        0    19203 2022-07-27 16:30:00.844711 cofactr-5.9.0/cofactr/graph.py
+-rw-r--r--   0        0        0      747 2022-05-11 17:24:24.039422 cofactr-5.9.0/cofactr/helpers.py
+-rw-r--r--   0        0        0        0 2022-05-13 00:06:22.350816 cofactr-5.9.0/cofactr/kb/__init__.py
+-rw-r--r--   0        0        0       46 2022-05-11 17:24:24.039422 cofactr-5.9.0/cofactr/kb/entity/__init__.py
+-rw-r--r--   0        0        0      608 2022-06-12 02:22:50.223769 cofactr-5.9.0/cofactr/kb/entity/aliases.py
+-rw-r--r--   0        0        0      388 2022-06-12 02:22:50.223769 cofactr-5.9.0/cofactr/kb/entity/labels.py
+-rw-r--r--   0        0        0      331 2022-06-12 02:22:50.223769 cofactr-5.9.0/cofactr/kb/entity/qualifier.py
+-rw-r--r--   0        0        0      857 2022-06-12 02:22:50.223769 cofactr-5.9.0/cofactr/kb/entity/statement_object.py
+-rw-r--r--   0        0        0     3979 2022-05-11 17:24:24.043422 cofactr-5.9.0/cofactr/kb/entity/types.py
+-rw-r--r--   0        0        0      801 2022-05-11 17:24:24.043422 cofactr-5.9.0/cofactr/render.py
+-rw-r--r--   0        0        0     2791 2022-07-19 18:59:07.650212 cofactr-5.9.0/cofactr/schema/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-13 00:06:10.262699 cofactr-5.9.0/cofactr/schema/flagship/__init__.py
+-rw-r--r--   0        0        0     1777 2022-07-19 19:16:35.914080 cofactr-5.9.0/cofactr/schema/flagship/offer.py
+-rw-r--r--   0        0        0      787 2022-06-09 18:15:57.431785 cofactr-5.9.0/cofactr/schema/flagship/part.py
+-rw-r--r--   0        0        0      706 2022-06-09 18:15:57.431785 cofactr-5.9.0/cofactr/schema/flagship/seller.py
+-rw-r--r--   0        0        0        0 2022-06-23 16:03:16.440503 cofactr-5.9.0/cofactr/schema/flagship_v2/__init__.py
+-rw-r--r--   0        0        0      450 2022-06-23 16:03:16.440503 cofactr-5.9.0/cofactr/schema/flagship_v2/part.py
+-rw-r--r--   0        0        0        0 2022-07-08 20:30:16.641306 cofactr-5.9.0/cofactr/schema/flagship_v3/__init__.py
+-rw-r--r--   0        0        0      305 2022-07-08 20:30:16.641306 cofactr-5.9.0/cofactr/schema/flagship_v3/part.py
+-rw-r--r--   0        0        0        0 2022-05-13 00:06:03.206631 cofactr-5.9.0/cofactr/schema/logistics/__init__.py
+-rw-r--r--   0        0        0      468 2022-05-11 17:24:24.043422 cofactr-5.9.0/cofactr/schema/logistics/offer.py
+-rw-r--r--   0        0        0     1100 2022-06-23 16:03:16.440503 cofactr-5.9.0/cofactr/schema/logistics/part.py
+-rw-r--r--   0        0        0        0 2022-06-23 16:03:16.440503 cofactr-5.9.0/cofactr/schema/logistics_v2/__init__.py
+-rw-r--r--   0        0        0      296 2022-07-15 16:29:55.199387 cofactr-5.9.0/cofactr/schema/logistics_v2/part.py
+-rw-r--r--   0        0        0        0 2022-07-08 20:30:16.645305 cofactr-5.9.0/cofactr/schema/logistics_v3/__init__.py
+-rw-r--r--   0        0        0      270 2022-07-08 20:30:16.645305 cofactr-5.9.0/cofactr/schema/logistics_v3/part.py
+-rw-r--r--   0        0        0        0 2022-07-15 16:18:14.441798 cofactr-5.9.0/cofactr/schema/logistics_v4/__init__.py
+-rw-r--r--   0        0        0      711 2022-07-19 18:54:24.735374 cofactr-5.9.0/cofactr/schema/logistics_v4/part.py
+-rw-r--r--   0        0        0        0 2022-07-19 18:53:55.875103 cofactr-5.9.0/cofactr/schema/price_solver_v0/__init__.py
+-rw-r--r--   0        0        0      514 2022-07-19 19:16:17.217860 cofactr-5.9.0/cofactr/schema/price_solver_v0/part.py
+-rw-r--r--   0        0        0      478 2022-06-23 16:03:16.440503 cofactr-5.9.0/cofactr/schema/types.py
+-rw-r--r--   0        0        0      854 2022-07-27 16:30:00.844711 cofactr-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1397 2022-07-27 16:30:07.698503 cofactr-5.9.0/setup.py
+-rw-r--r--   0        0        0     1026 2022-07-27 16:30:07.698647 cofactr-5.9.0/PKG-INFO
```

### Comparing `cofactr-5.8.0/LICENSE.txt` & `cofactr-5.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/graph.py` & `cofactr-5.9.0/cofactr/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     client_id,
     api_key,
     query,
     before,
     after,
     limit,
     schema,
+    timeout,
 ) -> Response:
     """Get orgs."""
 
     res = httpx.get(
         f"{url}/orgs",
         headers=drop_none_values(
             {
@@ -101,14 +102,15 @@
                 "q": query,
                 "before": before,
                 "after": after,
                 "limit": limit,
                 "schema": schema,
             }
         ),
+        timeout=timeout,
     )
 
     res.raise_for_status()
 
     return res
 
 
@@ -154,14 +156,15 @@
         before: Optional[str] = None,
         after: Optional[str] = None,
         limit: Optional[int] = None,
         external: Optional[bool] = True,
         force_refresh: bool = False,
         schema: Optional[ProductSchemaName] = None,
         filtering: Optional[List[Dict]] = None,
+        timeout: Optional[int] = None,
     ):
         """Get products.
 
         Args:
             query: Search query.
             fields: Used to filter properties that the response should contain. A field can be a
                 concrete property like "mpn" or an abstract group of properties like "assembly".
@@ -171,14 +174,15 @@
             limit: Restrict the results of the query to a particular number of documents.
             external: Whether to query external sources.
             force_refresh: Whether to force re-ingestion from external sources. Overrides
                 `external`.
             schema: Response schema.
             filtering: Filter products.
                 Example: `[{"field":"id","operator":"IN","value":["CCCQSA3G9SMR","CCV1F7A8UIYH"]}]`.
+            timeout: Time to wait (in seconds) for the server to issue a response.
         """
         if not schema:
             schema = self.default_product_schema
 
         res = get_products(
             url=self.url,
             client_id=self.client_id,
@@ -188,14 +192,15 @@
             external=external,
             force_refresh=force_refresh,
             before=before,
             after=after,
             limit=limit,
             schema=schema.value,
             filtering=filtering,
+            timeout=timeout,
         )
 
         extracted_producs = res.json()
 
         Product = schema_to_product[schema]  # pylint: disable=invalid-name
 
         extracted_producs["data"] = [
@@ -206,23 +211,25 @@
 
     def get_products_by_searches(
         self,
         queries: List[str],
         external: bool = True,
         force_refresh: bool = False,
         schema: Optional[ProductSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Search for products associated with each query.
 
         Args:
             queries: Queries to find products for.
             external: Whether to query external sources in order to refresh data if applicable.
             force_refresh: Whether to force re-ingestion from external sources. Overrides
                 `external`.
             schema: Response schema.
+            timeout: Time to wait (in seconds) for the server to issue a response.
 
         Returns:
             A dictionary mapping each MPN to a list of matching products.
         """
 
         if not queries:
             return {}
@@ -244,14 +251,15 @@
                     "relative_url": (
                         f"?q={query}&schema={schema.value}&external={bool(external)}"
                         f"&force_refresh={force_refresh}"
                     ),
                 }
                 for query in queries
             ],
+            timeout=timeout,
         )
 
         res.raise_for_status()
 
         responses = res.json()
 
         Product = schema_to_product[schema]  # pylint: disable=invalid-name
@@ -272,27 +280,29 @@
 
     def get_products_by_ids(
         self,
         ids: List[str],
         external: Optional[bool] = True,
         force_refresh: bool = False,
         schema: Optional[ProductSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Get a batch of products.
 
         Note:
             A maximum of 500 IDs can be provided. Any more than that, and the server will return
             a 422 error. Consider breaking the request into batches.
 
         Args:
             ids: Cofactr product IDs to match on.
             external: Whether to query external sources in order to refresh data if applicable.
             force_refresh: Whether to force re-ingestion from external sources. Overrides
                 `external`.
             schema: Response schema.
+            timeout: Time to wait (in seconds) for the server to issue a response.
         """
         num_requested = len(ids)
 
         if num_requested > BATCH_LIMIT:
             raise ValueError(
                 "Too many products requested in one call: Requested"
                 f" {num_requested}, but the limit is {BATCH_LIMIT}."
@@ -303,14 +313,15 @@
 
         extracted_products = self.get_products(
             external=external,
             force_refresh=force_refresh,
             schema=schema,
             filtering=[{"field": "id", "operator": "IN", "value": ids}],
             limit=BATCH_LIMIT,
+            timeout=timeout,
         )
 
         id_to_product = {p.id: p for p in extracted_products["data"]}
 
         product_dataclass = schema_to_product[schema]
 
         if "deprecated_ids" in {
@@ -329,36 +340,39 @@
     def get_orgs(
         self,
         query: Optional[str] = None,
         before: Optional[str] = None,
         after: Optional[str] = None,
         limit: Optional[int] = None,
         schema: Optional[OrgSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Get organizations.
 
         Args:
             query: Search query.
             before: Upper page boundry, expressed as a product ID.
             after: Lower page boundry, expressed as a product ID.
             limit: Restrict the results of the query to a particular number of documents.
             schema: Response schema.
+            timeout: Time to wait (in seconds) for the server to issue a response.
         """
         if not schema:
             schema = self.default_org_schema
 
         res = get_orgs(
             url=self.url,
             client_id=self.client_id,
             api_key=self.api_key,
             query=query,
             before=before,
             after=after,
             limit=limit,
             schema=schema.value,
+            timeout=timeout,
         )
 
         res_json = res.json()
 
         Org = schema_to_org[schema]  # pylint: disable=invalid-name
 
         res_json["data"] = [Org(**data) for data in res_json["data"]]
@@ -368,36 +382,39 @@
     def get_suppliers(
         self,
         query: Optional[str] = None,
         before: Optional[str] = None,
         after: Optional[str] = None,
         limit: Optional[int] = None,
         schema: Optional[OrgSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Get suppliers.
 
         Args:
             query: Search query.
             before: Upper page boundry, expressed as a product ID.
             after: Lower page boundry, expressed as a product ID.
             limit: Restrict the results of the query to a particular number of documents.
             schema: Response schema.
+            timeout: Time to wait (in seconds) for the server to issue a response.
         """
         if not schema:
             schema = self.default_org_schema
 
         res = get_orgs(
             url=self.url,
             client_id=self.client_id,
             api_key=self.api_key,
             query=query,
             before=before,
             after=after,
             limit=limit,
             schema=schema.value,
+            timeout=timeout,
         )
 
         res_json = res.json()
 
         Org = schema_to_org[schema]  # pylint: disable=invalid-name
 
         res_json["data"] = [Org(**data) for data in res_json["data"]]
@@ -405,27 +422,29 @@
         return res_json
 
     def autocomplete_orgs(
         self,
         query: Optional[str] = None,
         limit: Optional[int] = None,
         types: Optional[str] = None,
+        timeout: Optional[int] = None,
     ) -> Dict[Literal["data"], Completion]:
         """Autocomplete organizations.
 
         Args:
             query: Search query.
             before: Upper page boundry, expressed as a product ID.
             after: Lower page boundry, expressed as a product ID.
             limit: Restrict the results of the query to a particular number of
                 documents.
             types: Filter for types of organizations.
                 Example: "supplier" filters to suppliers.
                 Example: "supplier|manufacturer" filters to orgs that are a
                     supplier or a manufacturer.
+            timeout: Time to wait (in seconds) for the server to issue a response.
         """
 
         res = httpx.get(
             f"{self.url}/orgs/autocomplete",
             headers=drop_none_values(
                 {
                     "X-CLIENT-ID": self.client_id,
@@ -435,39 +454,42 @@
             params=drop_none_values(
                 {
                     "q": query,
                     "limit": limit,
                     "types": types,
                 }
             ),
+            timeout=timeout,
         )
 
         res.raise_for_status()
 
         return res.json()
 
     def get_product(
         self,
         id: str,
         fields: Optional[str] = None,
         external: Optional[bool] = True,
         force_refresh: bool = False,
         schema: Optional[ProductSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Get product.
 
         Args:
             fields: Used to filter properties that the response should contain. A field can be a
                 concrete property like "mpn" or an abstract group of properties like "assembly".
                 Example: "id,aliases,labels,statements{spec,assembly},offers"
             external: Whether to query external sources in order to update information for the
                 given product.
             force_refresh: Whether to force re-ingestion from external sources. Overrides
                 `external`.
             schema: Response schema.
+            timeout: Time to wait (in seconds) for the server to issue a response.
         """
         if not schema:
             schema = self.default_product_schema
 
         res = httpx.get(
             f"{self.url}/products/{id}",
             headers=drop_none_values(
@@ -480,14 +502,15 @@
                 {
                     "fields": fields,
                     "external": external,
                     "force_refresh": force_refresh,
                     "schema": schema.value,
                 }
             ),
+            timeout=timeout,
         )
 
         res.raise_for_status()
 
         res_json = res.json()
 
         Product = schema_to_product[schema]  # pylint: disable=invalid-name
@@ -501,24 +524,26 @@
     def get_offers(
         self,
         product_id: str,
         fields: Optional[str] = None,
         external: Optional[bool] = True,
         force_refresh: bool = False,
         schema: Optional[OfferSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Get product.
 
         Args:
             product_id: ID of the product to get offers for.
             fields: Used to filter properties that the response should contain.
             external: Whether to query external sources in order to update information.
             force_refresh: Whether to force re-ingestion from external sources. Overrides
                 `external`.
             schema: Response schema.
+            timeout: Time to wait (in seconds) for the server to issue a response.
         """
         if not schema:
             schema = self.default_offer_schema
 
         res = httpx.get(
             f"{self.url}/products/{product_id}/offers",
             headers=drop_none_values(
@@ -531,14 +556,15 @@
                 {
                     "fields": fields,
                     "external": external,
                     "force_refresh": force_refresh,
                     "schema": schema.value,
                 }
             ),
+            timeout=timeout,
         )
 
         res.raise_for_status()
 
         res_json = res.json()
 
         Offer = schema_to_offer[schema]  # pylint: disable=invalid-name
@@ -547,28 +573,30 @@
 
         return res_json
 
     def get_org(
         self,
         id: str,
         schema: Optional[OrgSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Get organization."""
         if not schema:
             schema = self.default_org_schema
 
         res = httpx.get(
             f"{self.url}/orgs/{id}",
             headers=drop_none_values(
                 {
                     "X-CLIENT-ID": self.client_id,
                     "X-API-KEY": self.api_key,
                 }
             ),
             params=drop_none_values({"schema": schema.value}),
+            timeout=timeout,
         )
 
         res.raise_for_status()
 
         res_json = res.json()
 
         Org = schema_to_org[schema]  # pylint: disable=invalid-name
@@ -579,28 +607,30 @@
 
         return res_json
 
     def get_supplier(
         self,
         id: str,
         schema: Optional[SupplierSchemaName] = None,
+        timeout: Optional[int] = None,
     ):
         """Get supplier."""
         if not schema:
             schema = self.default_supplier_schema
 
         res = httpx.get(
             f"{self.url}/orgs/{id}",
             headers=drop_none_values(
                 {
                     "X-CLIENT-ID": self.client_id,
                     "X-API-KEY": self.api_key,
                 }
             ),
             params=drop_none_values({"schema": schema.value}),
+            timeout=timeout,
         )
 
         res.raise_for_status()
 
         res_json = res.json()
 
         Supplier = schema_to_supplier[schema]  # pylint: disable=invalid-name
```

### Comparing `cofactr-5.8.0/cofactr/helpers.py` & `cofactr-5.9.0/cofactr/helpers.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/kb/entity/aliases.py` & `cofactr-5.9.0/cofactr/kb/entity/aliases.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/kb/entity/statement_object.py` & `cofactr-5.9.0/cofactr/kb/entity/statement_object.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/kb/entity/types.py` & `cofactr-5.9.0/cofactr/kb/entity/types.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/render.py` & `cofactr-5.9.0/cofactr/render.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/schema/__init__.py` & `cofactr-5.9.0/cofactr/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/schema/flagship/offer.py` & `cofactr-5.9.0/cofactr/schema/flagship/offer.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/schema/flagship/part.py` & `cofactr-5.9.0/cofactr/schema/flagship/part.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/schema/flagship/seller.py` & `cofactr-5.9.0/cofactr/schema/flagship/seller.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/schema/logistics/part.py` & `cofactr-5.9.0/cofactr/schema/logistics/part.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/schema/logistics_v4/part.py` & `cofactr-5.9.0/cofactr/schema/logistics_v4/part.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/cofactr/schema/price_solver_v0/part.py` & `cofactr-5.9.0/cofactr/schema/price_solver_v0/part.py`

 * *Files identical despite different names*

### Comparing `cofactr-5.8.0/pyproject.toml` & `cofactr-5.9.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cofactr"
-version = "5.8.0"
+version = "5.9.0"
 description = "Client library for accessing Cofactr data."
 authors = ["Noah Trueblood <noah@cofactr.com>", "Riley Harrington <riley@cofactr.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Cofactr/cofactr-client"
 repository = "https://github.com/Cofactr/cofactr-client"
 keywords = ["cofactr"]
```

### Comparing `cofactr-5.8.0/setup.py` & `cofactr-5.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.0,<0.24.0']
 
 setup_kwargs = {
     'name': 'cofactr',
-    'version': '5.8.0',
+    'version': '5.9.0',
     'description': 'Client library for accessing Cofactr data.',
     'long_description': '# Cofactr\n\nPython client library for accessing Cofactr.\n\n## Example\n\n```python\nfrom typing import List\nfrom cofactr.graph import GraphAPI\n\n# Flagship is the default schema.\nfrom cofactr.schema.flagship.part import Part\n\ngraph = GraphAPI()\n\npart_res = graph.get_product(id="IM60640MOX6H")\npart: Part = part_res["data"]\n\nparts_res = graph.get_products(query="esp32")\nparts: List[Part] = parts_res["data"]\n```\n',
     'author': 'Noah Trueblood',
     'author_email': 'noah@cofactr.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Cofactr/cofactr-client',
```

### Comparing `cofactr-5.8.0/PKG-INFO` & `cofactr-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofactr
-Version: 5.8.0
+Version: 5.9.0
 Summary: Client library for accessing Cofactr data.
 Home-page: https://github.com/Cofactr/cofactr-client
 License: MIT
 Keywords: cofactr
 Author: Noah Trueblood
 Author-email: noah@cofactr.com
 Requires-Python: >=3.10,<4.0
```

