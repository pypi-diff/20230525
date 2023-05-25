# Comparing `tmp/ptal_api-0.11.6.tar.gz` & `tmp/ptal_api-0.11.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptal_api-0.11.6.tar", max compression
+gzip compressed data, was "ptal_api-0.11.6.1.tar", max compression
```

## Comparing `ptal_api-0.11.6.tar` & `ptal_api-0.11.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      627 2023-05-10 15:03:49.316666 ptal_api-0.11.6/README.md
--rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/__init__.py
--rw-r--r--   0        0        0    99304 2023-05-18 08:13:25.673710 ptal_api-0.11.6/ptal_api/adapter.py
--rw-r--r--   0        0        0      184 2023-05-15 08:57:46.905949 ptal_api-0.11.6/ptal_api/core/kb_sync/kb_iterator_config.py
--rw-r--r--   0        0        0      160 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/kb_sync/object_time_interval.py
--rw-r--r--   0        0        0      435 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/app_settings/logging.conf
--rw-r--r--   0        0        0      737 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/common/common.py
--rw-r--r--   0        0        0    12302 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/base_data_model.py
--rw-r--r--   0        0        0      904 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/config_data_model.py
--rw-r--r--   0        0        0     3255 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/custom_data_model.py
--rw-r--r--   0        0        0     3501 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
--rw-r--r--   0        0        0     2194 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/custom_data_handler.py
--rw-r--r--   0        0        0     1464 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/file_generator.py
--rw-r--r--   0        0        0     4556 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/object_name_transformer.py
--rw-r--r--   0        0        0    23314 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_generator.py
--rw-r--r--   0        0        0     1800 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
--rw-r--r--   0        0        0      418 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
--rw-r--r--   0        0        0      192 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/core/values/date_dataclass.py
--rw-r--r--   0        0        0     3279 2023-05-18 08:13:25.673710 ptal_api-0.11.6/ptal_api/core/values/value_mapping.py
--rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/providers/__init__.py
--rw-r--r--   0        0        0     4668 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/providers/gql_providers.py
--rw-r--r--   0        0        0     1186 2023-05-10 15:03:49.316666 ptal_api-0.11.6/ptal_api/schema/README.md
--rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/schema/__init__.py
--rw-r--r--   0        0        0   289804 2023-05-18 08:28:23.351074 ptal_api-0.11.6/ptal_api/schema/api_schema.py
--rw-r--r--   0        0        0    93413 2023-05-18 08:28:23.351074 ptal_api-0.11.6/ptal_api/schema/crawlers_api_schema.py
--rw-r--r--   0        0        0    74033 2023-05-10 15:03:49.320666 ptal_api-0.11.6/ptal_api/schema/tcontroller_api_schema.py
--rw-r--r--   0        0        0   136845 2023-05-18 08:28:23.351074 ptal_api-0.11.6/ptal_api/schema/utils_api_schema.py
--rw-r--r--   0        0        0     3662 2023-05-10 15:03:49.320666 ptal_api-0.11.6/ptal_api/scripts/type_mapper.py
--rw-r--r--   0        0        0        0 2023-05-18 08:44:15.320708 ptal_api-0.11.6/ptal_api/tdm_builder/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-10 15:03:49.320666 ptal_api-0.11.6/ptal_api/tdm_builder/tdm_builder.py
--rw-r--r--   0        0        0     1871 2023-05-18 08:28:23.351074 ptal_api-0.11.6/pyproject.toml
--rw-r--r--   0        0        0     1688 1970-01-01 00:00:00.000000 ptal_api-0.11.6/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-04-24 11:23:04.939750 ptal_api-0.11.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/__init__.py
+-rw-r--r--   0        0        0   100253 2023-05-25 16:45:27.776257 ptal_api-0.11.6.1/ptal_api/adapter.py
+-rw-r--r--   0        0        0      184 2023-05-16 13:32:51.877997 ptal_api-0.11.6.1/ptal_api/core/kb_sync/kb_iterator_config.py
+-rw-r--r--   0        0        0      160 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/kb_sync/object_time_interval.py
+-rw-r--r--   0        0        0      435 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/type_mapper/app_settings/logging.conf
+-rw-r--r--   0        0        0      737 2023-05-02 10:24:35.487480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/common/common.py
+-rw-r--r--   0        0        0    14955 2023-05-25 14:41:26.834648 ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/base_data_model.py
+-rw-r--r--   0        0        0      904 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/config_data_model.py
+-rw-r--r--   0        0        0     3255 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/custom_data_model.py
+-rw-r--r--   0        0        0     3501 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml
+-rw-r--r--   0        0        0     2194 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/custom_data_handler.py
+-rw-r--r--   0        0        0     1464 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/file_generator.py
+-rw-r--r--   0        0        0     4556 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/object_name_transformer.py
+-rw-r--r--   0        0        0    23314 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py
+-rw-r--r--   0        0        0     1800 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py
+-rw-r--r--   0        0        0      418 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader_interface.py
+-rw-r--r--   0        0        0      192 2023-04-24 11:23:04.943750 ptal_api-0.11.6.1/ptal_api/core/values/date_dataclass.py
+-rw-r--r--   0        0        0     3279 2023-05-25 16:31:12.226717 ptal_api-0.11.6.1/ptal_api/core/values/value_mapping.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/providers/__init__.py
+-rw-r--r--   0        0        0     4668 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/providers/gql_providers.py
+-rw-r--r--   0        0        0     1186 2023-05-02 11:37:55.718860 ptal_api-0.11.6.1/ptal_api/schema/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/schema/__init__.py
+-rw-r--r--   0        0        0   289804 2023-05-25 16:31:12.230717 ptal_api-0.11.6.1/ptal_api/schema/api_schema.py
+-rw-r--r--   0        0        0    93413 2023-05-25 16:31:12.230717 ptal_api-0.11.6.1/ptal_api/schema/crawlers_api_schema.py
+-rw-r--r--   0        0        0    74033 2023-05-02 11:37:55.722860 ptal_api-0.11.6.1/ptal_api/schema/tcontroller_api_schema.py
+-rw-r--r--   0        0        0   136845 2023-05-25 16:31:12.234717 ptal_api-0.11.6.1/ptal_api/schema/utils_api_schema.py
+-rw-r--r--   0        0        0     3662 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/scripts/type_mapper.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:49:19.030532 ptal_api-0.11.6.1/ptal_api/tdm_builder/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-02 10:24:35.491480 ptal_api-0.11.6.1/ptal_api/tdm_builder/tdm_builder.py
+-rw-r--r--   0        0        0     1873 2023-05-25 16:45:27.776257 ptal_api-0.11.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 ptal_api-0.11.6.1/PKG-INFO
```

### Comparing `ptal_api-0.11.6/README.md` & `ptal_api-0.11.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/adapter.py` & `ptal_api-0.11.6.1/ptal_api/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,31 +112,35 @@
 
     return wrapper
 
 
 class TalismanAPIAdapter:
     def __init__(
         self,
-        gql_client: Optional[AbstractGQLClient],
+        gql_client: AbstractGQLClient,
         type_mapping: Optional[Union[str, dict, TypeMapping]] = None,
         type_mapping_loader: Optional[TypeMappingLoaderInterface] = None,
-        tdm_builder: AbstractTdmBuilder = None,
+        tdm_builder: Optional[AbstractTdmBuilder] = None,
         utils_gql_client: Optional[AbstractGQLClient] = None,
-        kb_iterator_config: KBIteratorConfig = None,
+        kb_iterator_config: Optional[KBIteratorConfig] = None,
         limit: int = 100,
         perform_synchronously: bool = True,
     ) -> None:
         self._gql_client = gql_client
         self._utils_gql_client = utils_gql_client
         self._type_mapping_loader = type_mapping_loader if type_mapping_loader else TypeMappingLoader(logger)
         self._type_mapping = self._type_mapping_loader.load_type_mapping(type_mapping)
         self._limit = limit
         self._perform_synchronously = perform_synchronously
 
-        self.document_fields_truncated = ("id", "external_url", "uuid",)
+        self.document_fields_truncated = (
+            "id",
+            "external_url",
+            "uuid",
+        )
         self.document_fields = (
             "id",
             "title",
             "external_url",
             "publication_author",
             "publication_date",
             "internal_url",
@@ -146,19 +150,28 @@
             "notes",
             "access_level",
             "trust_level",
             "uuid",
         )
 
         self.document_text_fields_truncated = ("text",)
-        self.document_text_fields = ("node_id", "text")
+        self.document_text_fields = (
+            "node_id",
+            "text",
+        )
         self.document_text_metadata_fields = ("paragraph_type",)
 
-        self.document_platform_fields = ("id", "name")
-        self.document_account_fields = ("id", "name")
+        self.document_platform_fields = (
+            "id",
+            "name",
+        )
+        self.document_account_fields = (
+            "id",
+            "name",
+        )
 
         self.user_fields = ("id",)
 
         self.concept_fields = (
             "id",
             "name",
             "notes",
@@ -197,15 +210,15 @@
         self.tdm_builder = tdm_builder
 
         if kb_iterator_config:
             self.kb_iterator_config = kb_iterator_config
         else:
             self.kb_iterator_config = KBIteratorConfig(1000, 1609448400)  # Fri Jan 01 2021 00:00:00 GMT+0300
 
-    def get_tdm_builder(self) -> AbstractTdmBuilder:
+    def get_tdm_builder(self) -> Optional[AbstractTdmBuilder]:
         return self.tdm_builder
 
     @property
     def type_mapping(self):
         return self._type_mapping
 
     @type_mapping.setter
@@ -405,18 +418,18 @@
         kafka_topic.__fields__(*self.pipeline_topic_fields)
         kafka_topic.metrics().__fields__(*self.pipeline_metrics_fields)
         kafka_topic.pipeline().pipeline_config().__fields__(*self.pipeline_config_fields)
 
     def get_all_documents(
         self,
         grouping: DocumentGrouping = "none",
-        filter_settings: DocumentFilterSettings = None,
+        filter_settings: Optional[DocumentFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: DocumentSorting = "score",
-        extra_settings: ExtraSettings = None,
+        extra_settings: Optional[ExtraSettings] = None,
         with_extended_information: bool = False,
     ) -> Iterable[Story]:
         if filter_settings is None:
             filter_settings = DocumentFilterSettings()
         if extra_settings is None:
             extra_settings = ExtraSettings()
 
@@ -473,18 +486,18 @@
             i += 1
 
     def get_documents(
         self,
         skip: int = 0,
         take: Optional[int] = None,
         grouping: DocumentGrouping = "none",
-        filter_settings: DocumentFilterSettings = None,
+        filter_settings: Optional[DocumentFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: DocumentSorting = "score",
-        extra_settings: ExtraSettings = None,
+        extra_settings: Optional[ExtraSettings] = None,
         with_extended_information: bool = False,
     ) -> Sequence[Story]:
         take = self.get_take_value(take)
         pagination_story_kwargs = {}
         if filter_settings is None:
             filter_settings = DocumentFilterSettings()
         if extra_settings is None:
@@ -512,15 +525,15 @@
             m.__fields__(*self.document_fields_truncated)
         m.text().__fields__(*self.document_text_fields_truncated)
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_story.list_story
 
-    def get_documents_count(self, filter_settings: DocumentFilterSettings = None) -> int:
+    def get_documents_count(self, filter_settings: Optional[DocumentFilterSettings] = None) -> int:
         if filter_settings is None:
             filter_settings = DocumentFilterSettings()
 
         op = Operation(Query)
         ps: StoryPagination = op.pagination_story(
             limit=1, filter_settings=filter_settings, extra_settings=ExtraSettings()
         )
@@ -571,30 +584,32 @@
         cd.last_updater().__fields__(*self.user_fields)
         cd.metadata().platform().__fields__(*self.document_platform_fields)
         cd.metadata().account().__fields__(*self.document_account_fields)
         cd.creator().__fields__(*self.user_fields)
         cdt = cd.text(show_hidden=True)
         cdt.__fields__(*self.document_text_fields)
         cdt.metadata().__fields__(*self.document_text_metadata_fields)
+        fc = d.list_concept_fact()
+        fc.__fields__(*self.concept_fact_fields)
 
         res = self._gql_client.execute(op)
         res = op + res
         return res.document
 
-    def get_concept_count(self, filter_settings: ConceptFilterSettings = None) -> int:
+    def get_concept_count(self, filter_settings: Optional[ConceptFilterSettings] = None) -> int:
         op = Operation(Query)
         pc: ConceptPagination = op.pagination_concept(
             filter_settings=filter_settings if filter_settings else ConceptFilterSettings()
         )
         pc.show_total()
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.show_total
 
-    def get_concept_link_count(self, filter_settings: ConceptLinkFilterSettings = None) -> int:
+    def get_concept_link_count(self, filter_settings: Optional[ConceptLinkFilterSettings] = None) -> int:
         op = Operation(Query)
         pcl: ConceptLinkPagination = op.pagination_concept_link(
             filter_settings=filter_settings if filter_settings else ConceptLinkFilterSettings()
         )
         pcl.total()
         res = self._gql_client.execute(op)
         res = op + res
@@ -625,16 +640,28 @@
         res = op + res
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.concept)
 
         return res.concept
 
+    def get_concept_property(self, concept_property_id: str) -> Concept:
+        op = Operation(Query)
+        cp: ConceptProperty = op.concept_property(id=concept_property_id)
+
+        cp.__fields__(*self.concept_property_fields)
+        cp.property_type().__fields__(*self.concept_property_type_fields)
+        self._configure_output_value_fields(cp.value)
+        res = self._gql_client.execute(op)
+        res = op + res
+
+        return res.concept_property
+
     def get_concept_facts(
-        self, concept_id: str, filter_settings: DocumentLinkFilterSetting = None
+        self, concept_id: str, filter_settings: Optional[DocumentLinkFilterSetting] = None
     ) -> Sequence[ConceptFact]:
         op = Operation(Query)
         c: Concept = op.concept(id=concept_id)
         pcf: ConceptFactPagination = c.pagination_concept_fact(
             filter_settings=filter_settings if filter_settings else DocumentLinkFilterSetting()
         )
         lcf = pcf.list_concept_fact()
@@ -665,15 +692,15 @@
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_fact(res.concept_link)
 
         return res.concept_link
 
     def get_all_concepts(
         self,
-        filter_settings: ConceptFilterSettings = None,
+        filter_settings: Optional[ConceptFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: ConceptSorting = "score",
         with_aliases: bool = False,
         with_properties: bool = False,
         with_links: bool = False,
         with_link_properties: bool = False,
         with_facts: bool = False,
@@ -739,15 +766,15 @@
             yield from concepts
             i += 1
 
     def get_concepts(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: ConceptFilterSettings = None,
+        filter_settings: Optional[ConceptFilterSettings] = None,
         direction: SortDirection = "descending",
         sort_field: ConceptSorting = "score",
         with_aliases: bool = False,
         with_properties: bool = False,
         with_links: bool = False,
         with_link_properties: bool = False,
         with_facts: bool = False,
@@ -801,15 +828,15 @@
             with_potential_facts=with_potential_facts,
         )
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept.list_concept
 
     def get_all_concept_links(
-        self, filter_settings: ConceptLinkFilterSettings = None, with_link_properties: bool = False
+        self, filter_settings: Optional[ConceptLinkFilterSettings] = None, with_link_properties: bool = False
     ) -> Iterable[ConceptLink]:
         if not filter_settings:
             filter_settings = ConceptLinkFilterSettings()
 
         total = self.get_concept_link_count(filter_settings=filter_settings)
 
         if total > self.kb_iterator_config.max_total_count:
@@ -854,15 +881,15 @@
             yield from links
             i += 1
 
     def get_concept_links_by_limit_offset_filter_settings(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: ConceptLinkFilterSettings = None,
+        filter_settings: Optional[ConceptLinkFilterSettings] = None,
         with_link_properties: bool = False,
     ) -> Sequence[ConceptLink]:
         take = self.get_take_value(take)
         op = Operation(Query)
         pcl: ConceptLinkPagination = op.pagination_concept_link(
             filter_settings=filter_settings if filter_settings else ConceptLinkFilterSettings(), offset=skip, limit=take
         )
@@ -1083,29 +1110,29 @@
             lcp.__fields__("list_concept_property_fact")
 
         res = self._gql_client.execute(op)
         res = op + res  # type: Query
         return res.concept_link.pagination_concept_link_property.list_concept_property
 
     def get_concept_time_intervals(
-        self, filter_settings: ConceptFilterSettings = None, max_interval_size: Optional[int] = None
+        self, filter_settings: Optional[ConceptFilterSettings] = None, max_interval_size: Optional[int] = None
     ) -> Iterable[ObjectTimeInterval]:
         if not filter_settings:
             filter_settings = ConceptFilterSettings()
         yield from self._get_object_time_intervals(filter_settings, max_interval_size)
 
     def get_concept_link_time_intervals(
-        self, filter_settings: ConceptLinkFilterSettings = None, max_interval_size: Optional[int] = None
+        self, filter_settings: Optional[ConceptLinkFilterSettings] = None, max_interval_size: Optional[int] = None
     ) -> Iterable[ObjectTimeInterval]:
         if not filter_settings:
             filter_settings = ConceptLinkFilterSettings()
         yield from self._get_object_time_intervals(filter_settings, max_interval_size)
 
     def get_document_time_intervals(
-        self, filter_settings: DocumentFilterSettings = None, max_interval_size: Optional[int] = None
+        self, filter_settings: Optional[DocumentFilterSettings] = None, max_interval_size: Optional[int] = None
     ) -> Iterable[ObjectTimeInterval]:
         if not filter_settings:
             filter_settings = DocumentFilterSettings()
         yield from self._get_object_time_intervals(filter_settings, max_interval_size)
 
     def _get_object_time_intervals(
         self,
@@ -1140,18 +1167,18 @@
                 start_time=start, end_time=end, object_count=object_count, max_interval_size=max_interval_size
             )
 
     def create_concept(
         self,
         name: str,
         type_id: str,
-        notes: str = None,
-        with_properties=False,
-        with_links=False,
-        with_link_properties=False,
+        notes: Optional[str] = None,
+        with_properties: bool = False,
+        with_links: bool = False,
+        with_link_properties: bool = False,
         perform_synchronously: Optional[bool] = None,
     ) -> Concept:
         cmi: ConceptMutationInput = ConceptMutationInput(name=name, concept_type_id=type_id, notes=notes)
         return self._create_concept_with_input(
             cmi,
             with_properties=with_properties,
             with_links=with_links,
@@ -1230,53 +1257,53 @@
         res = op + res
 
         return res.update_concept_property
 
     def update_concept_composite_property(self, cp: ConceptProperty) -> ConceptProperty:
         value_input = []
         for value in cp.value.list_value:
-            if type(value.value) is StringValue:
+            if type(value.value) is StringValue or type(value.value) is uas.StringValue:
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(string_value_input=StringValueInput(value=value.value.value))
                     )
                 )
-            elif type(value.value) is IntValue:
+            elif type(value.value) is IntValue or type(value.value) is uas.IntValue:
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(int_value_input=IntValueInput(value=value.value.number))
                     )
                 )
-            elif type(value.value) is DateTimeValue:
+            elif type(value.value) is DateTimeValue or type(value.value) is uas.DateTimeValue:
                 value_input.append(
                     ComponentValueInput(
                         id=value.id,
                         value=ValueInput(
                             date_time_value_input=DateTimeValueInput(date=value.value.date, time=value.value.time)
                         ),
                     )
                 )
-            elif type(value.value) is StringLocaleValue:
+            elif type(value.value) is StringLocaleValue or type(value.value) is uas.StringLocaleValue:
                 value_input.append(
                     ComponentValueInput(
                         id=value.id,
                         value=ValueInput(
                             string_locale_value_input=StringLocaleValueInput(
                                 value=value.value.value, locale=value.value.locale
                             )
                         ),
                     )
                 )
-            elif type(value.value) is LinkValue:
+            elif type(value.value) is LinkValue or type(value.value) is uas.LinkValue:
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(link_value_input=LinkValueInput(link=value.value.link))
                     )
                 )
-            elif type(value.value) is DoubleValue:
+            elif type(value.value) is DoubleValue or type(value.value) is uas.DoubleValue:
                 value_input.append(
                     ComponentValueInput(
                         id=value.id, value=ValueInput(double_value_input=DoubleValueInput(double=value.value.double))
                     )
                 )
         op = Operation(Mutation)
         ucp: ConceptProperty = op.update_concept_property(
@@ -1295,15 +1322,15 @@
         res = self._gql_client.execute(op)
         res = op + res
 
         return res.delete_concept_property.is_success
 
     def get_all_concept_types(
         self,
-        filter_settings: ConceptTypeFilterSettings = None,
+        filter_settings: Optional[ConceptTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptTypeSorting = "id",
     ) -> Iterable[ConceptType]:
         current_step = 0
         while True:
             concept_types = self.get_concept_types(
                 skip=current_step,
@@ -1317,15 +1344,15 @@
             current_step += self.limit
             yield from concept_types
 
     def get_concept_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: ConceptTypeFilterSettings = None,
+        filter_settings: Optional[ConceptTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptTypeSorting = "id",
     ) -> Sequence[ConceptType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptTypeFilterSettings()
 
@@ -1371,15 +1398,15 @@
             if concept_type.name == concept_type_name:
                 self._type_mapping.add_concept_type(concept_type_code, concept_type)
                 return concept_type
         return None
 
     def get_all_concept_property_types(
         self,
-        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_property_types = self.get_concept_property_types(
                 skip=current_step,
@@ -1393,15 +1420,15 @@
             current_step += self.limit
             yield from concept_property_types
 
     def get_concept_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyTypeFilterSettings()
 
@@ -1428,15 +1455,15 @@
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_property_type.list_concept_property_type
 
     def get_all_concept_composite_property_types(
         self,
-        filter_settings: CompositePropertyTypeFilterSettings = None,
+        filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_composite_property_types = self.get_concept_composite_property_types(
                 skip=current_step,
@@ -1450,15 +1477,15 @@
             current_step += self.limit
             yield from concept_composite_property_types
 
     def get_concept_composite_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: CompositePropertyTypeFilterSettings = None,
+        filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = CompositePropertyTypeFilterSettings()
 
@@ -1490,15 +1517,15 @@
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_property_type(concept_type_code, property_type_code, property_type)
                 return property_type
         return None
 
     def get_all_concept_property_value_types(
         self,
-        filter_settings: ConceptPropertyValueTypeFilterSettings = None,
+        filter_settings: Optional[ConceptPropertyValueTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyValueTypeSorting = "id",
     ) -> Iterable[ConceptPropertyValueType]:
         current_step = 0
         while True:
             concept_property_value_types = self.get_concept_property_value_types(
                 skip=current_step,
@@ -1512,15 +1539,15 @@
             current_step += self.limit
             yield from concept_property_value_types
 
     def get_concept_property_value_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: ConceptPropertyValueTypeFilterSettings = None,
+        filter_settings: Optional[ConceptPropertyValueTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyValueTypeSorting = "id",
     ) -> Sequence[ConceptPropertyValueType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyValueTypeFilterSettings()
 
@@ -1560,15 +1587,15 @@
             if value_type.name == value_type_name:
                 self._type_mapping.add_concept_property_value_type(concept_property_value_type_code, value_type)
                 return value_type
         return None
 
     def get_all_concept_link_property_types(
         self,
-        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_link_property_types = self.get_link_property_types(
                 skip=current_step,
@@ -1582,15 +1609,15 @@
             current_step += self.limit
             yield from concept_link_property_types
 
     def get_link_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: ConceptPropertyTypeFilterSettings = None,
+        filter_settings: Optional[ConceptPropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptPropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptPropertyTypeFilterSettings()
 
@@ -1615,15 +1642,15 @@
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_property_type.list_concept_property_type
 
     def get_all_concept_link_composite_property_types(
         self,
-        filter_settings: CompositePropertyTypeFilterSettings = None,
+        filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
     ) -> Iterable[ConceptPropertyType]:
         current_step = 0
         while True:
             concept_link_composite_property_types = self.get_link_composite_property_types(
                 skip=current_step,
@@ -1637,15 +1664,15 @@
             current_step += self.limit
             yield from concept_link_composite_property_types
 
     def get_link_composite_property_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: CompositePropertyTypeFilterSettings = None,
+        filter_settings: Optional[CompositePropertyTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: CompositePropertyTypeSorting = "name",
     ) -> Sequence[ConceptPropertyType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = CompositePropertyTypeFilterSettings()
 
@@ -1670,35 +1697,35 @@
         lcpt = cptp.list_concept_property_type()
         lcpt.__fields__(*self.concept_property_type_fields)
         self._configure_property_value_type_fields(lcpt.value_type, True)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_composite_link_property_type.list_concept_property_type
 
-    def get_link_property_type(
-        self, link_type_code: str, link_type: ConceptLinkType, property_type_code: str
-    ) -> Optional[ConceptPropertyType]:
+    def get_link_property_type(self, link_type_code: str, property_type_code: str) -> Optional[ConceptPropertyType]:
         property_type = self._type_mapping.get_concept_link_property_type(link_type_code, property_type_code)
         if property_type:
             return property_type
+        link_type = self.get_link_type(link_type_code)
 
         property_type_name = self._type_mapping.get_concept_link_property_type_name(link_type_code, property_type_code)
         property_types = self.get_link_properties_types_by_name(link_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
                 self._type_mapping.add_concept_link_property_type(link_type_code, property_type_code, property_type)
                 return property_type
         return None
 
     def get_link_composite_property_type(
-        self, link_type_code: str, link_type: ConceptLinkType, property_type_code: str
+        self, link_type_code: str, property_type_code: str
     ) -> Optional[ConceptPropertyType]:
         property_type = self._type_mapping.get_concept_link_composite_property_type(link_type_code, property_type_code)
         if property_type:
             return property_type
+        link_type = self.get_link_type(link_type_code)
 
         property_type_name = self._type_mapping.get_concept_link_composite_property_type_name(
             link_type_code, property_type_code
         )
         property_types = self.get_composite_link_properties_types_by_name(link_type.id, property_type_name)
         for property_type in property_types:
             if property_type.name == property_type_name:
@@ -1744,23 +1771,22 @@
         is_main: bool = False,
         perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
         property_type: ConceptPropertyType = self.get_concept_property_type(concept_type_code, property_type_code)
         if not property_type:
             raise Exception("Cannot add property: no property type id")
         if type(property_type.value_type) is CompositePropertyValueTemplate:
+            component_values = self._type_mapping.get_concept_composite_property_component_values(
+                concept_type_code, property_type_code
+            )
+            components_type_mapping: Dict[str, CompositePropertyValueType] = self._get_components_mapping(
+                component_values, property_type.value_type.component_value_types
+            )
             prop = self.add_composite_property_by_id(
-                concept_id,
-                property_type.id,
-                value,
-                is_main,
-                property_type.value_type.component_value_types,
-                concept_type_code,
-                property_type_code,
-                perform_synchronously,
+                concept_id, property_type.id, value, is_main, components_type_mapping, perform_synchronously
             )
         else:
             prop = self.add_property_by_id(
                 concept_id, property_type.id, value, is_main, property_type.value_type.value_type, perform_synchronously
             )
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_property_fact(prop, self.get_concept(concept_id), value, property_type)
@@ -1864,25 +1890,18 @@
         return res.delete_concept_property_type
 
     def add_link_composite_property_by_id(
         self,
         link_id: str,
         property_type_id: str,
         values: dict,
-        component_value_types: List[CompositePropertyValueType],
-        link_composite_property_code: str,
-        link_code: str,
+        components_type_mapping: Dict[str, CompositePropertyValueType],
         is_main: bool,
         perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
-        components_type_mapping: Dict[str, CompositePropertyValueType] = {}
-        for relation in self._type_mapping.relations_types_mapping:
-            if relation.old_relation_type == link_code:
-                component_values = relation.composite_properties[link_composite_property_code].component_values
-                components_type_mapping = self._get_components_mapping(component_values, component_value_types)
         value_input = self._get_value_input(values, components_type_mapping)
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
 
         op = Operation(Mutation)
         aclp = op.add_concept_link_property(
             performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptLinkPropertyInput(
@@ -1898,22 +1917,17 @@
 
     def add_composite_property_by_id(
         self,
         id: str,
         type_id: str,
         values: dict,
         is_main: bool,
-        component_value_types: List[CompositePropertyValueType],
-        concept_type_code: str,
-        property_type_code: str,
+        components_type_mapping: Dict[str, CompositePropertyValueType],
         perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
-        concept_composite_properties = self._type_mapping.concepts_types_mapping[concept_type_code].composite_properties
-        concept_component_values = concept_composite_properties[property_type_code].component_values
-        components_type_mapping = self._get_components_mapping(concept_component_values, component_value_types)
         value_input = self._get_value_input(values, components_type_mapping)
         perform_synchronously = self.get_perform_synchronously_value(perform_synchronously)
 
         op = Operation(Mutation)
         acp = op.add_concept_property(
             performance_control=PerformSynchronously(perform_synchronously=perform_synchronously),
             form=ConceptPropertyCreateInput(
@@ -1927,58 +1941,62 @@
 
         return res.add_concept_property
 
     def add_link_property(
         self,
         link_id: str,
         link_type_code: str,
-        link_type: ConceptLinkType,
         property_type_code: str,
         value: Any,
         is_composite: Optional[bool] = False,
         is_main: bool = False,
         perform_synchronously: Optional[bool] = None,
     ) -> ConceptProperty:
         property_type = (
-            self.get_link_composite_property_type(link_type_code, link_type, property_type_code)
+            self.get_link_composite_property_type(link_type_code, property_type_code)
             if is_composite
-            else self.get_link_property_type(link_type_code, link_type, property_type_code)
+            else self.get_link_property_type(link_type_code, property_type_code)
         )
         if not property_type:
             raise Exception("Cannot add property: no property type id")
 
         if is_composite:
+            component_values = self._type_mapping.get_concept_link_composite_property_component_values(
+                link_type_code, property_type_code
+            )
+            components_type_mapping: Dict[str, CompositePropertyValueType] = self._get_components_mapping(
+                component_values, property_type.value_type.component_value_types
+            )
+
             link_property = self.add_link_composite_property_by_id(
                 link_id,
                 property_type.id,
                 value,
-                property_type.value_type.component_value_types,
-                property_type_code,
-                link_type_code,
+                components_type_mapping,
                 is_main,
                 perform_synchronously,
             )
         else:
             link_property = self.add_link_property_by_id(
                 link_id,
                 property_type.id,
                 value,
                 is_main,
                 property_type.value_type.value_type,
-                perform_synchronously=perform_synchronously,
+                perform_synchronously,
             )
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_link_property_fact(link_property, self.get_concept_link(link_id), value, property_type)
 
         return link_property
 
     def get_all_concept_link_types(
         self,
-        filter_settings: ConceptLinkTypeFilterSettings = None,
+        filter_settings: Optional[ConceptLinkTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptLinkTypeSorting = "id",
     ) -> Iterable[ConceptLinkType]:
         current_step = 0
         while True:
             concept_link_types = self.get_concept_link_types(
                 skip=current_step,
@@ -1992,15 +2010,15 @@
             current_step += self.limit
             yield from concept_link_types
 
     def get_concept_link_types(
         self,
         skip: int = 0,
         take: Optional[int] = None,
-        filter_settings: ConceptLinkTypeFilterSettings = None,
+        filter_settings: Optional[ConceptLinkTypeFilterSettings] = None,
         direction: SortDirection = "ascending",
         sort_field: ConceptLinkTypeSorting = "id",
     ) -> Sequence[ConceptLinkType]:
         take = self.get_take_value(take)
         if not filter_settings:
             filter_settings = ConceptLinkTypeFilterSettings()
 
@@ -2030,21 +2048,21 @@
         lclt.__fields__(*self.concept_link_type_fields)
         lclt.concept_from_type().__fields__(*self.concept_type_fields)
         lclt.concept_to_type().__fields__(*self.concept_type_fields)
         res = self._gql_client.execute(op)
         res = op + res
         return res.pagination_concept_link_type.list_concept_link_type
 
-    def get_link_type(
-        self, concept_from_type_code: str, concept_to_type_code: str, link_type_code: str
-    ) -> Optional[ConceptLinkType]:
+    def get_link_type(self, link_type_code: str) -> Optional[ConceptLinkType]:
         link_type = self._type_mapping.get_concept_link_type(link_type_code)
         if link_type:
             return link_type
 
+        concept_from_type_code = self._type_mapping.get_source_concept_type_code(link_type_code)
+        concept_to_type_code = self._type_mapping.get_target_concept_type_code(link_type_code)
         concept_from_type = self.get_concept_type(concept_from_type_code)
         concept_to_type = self.get_concept_type(concept_to_type_code)
         link_type_name = self._type_mapping.get_concept_link_type_name(link_type_code)
         link_types = self.get_concept_link_type_by_name(link_type_name, concept_from_type.id, concept_to_type.id)
         for link_type in link_types:
             if link_type.name == link_type_name:
                 self._type_mapping.add_concept_link_type(link_type_code, link_type)
@@ -2073,20 +2091,18 @@
 
         return res.add_concept_link
 
     def add_relation(
         self,
         concept_from_id: str,
         concept_to_id: str,
-        concept_from_type_code: str,
-        concept_to_type_code: str,
         type_code: str,
         perform_synchronously: Optional[bool] = None,
     ) -> ConceptLink:
-        link_type = self.get_link_type(concept_from_type_code, concept_to_type_code, type_code)
+        link_type = self.get_link_type(type_code)
         if not link_type:
             raise Exception("Cannot add relation: no link type")
         relation = self.add_relation_by_id(
             concept_from_id, concept_to_id, link_type.id, perform_synchronously=perform_synchronously
         )
 
         if self.tdm_builder is not None:
@@ -2277,21 +2293,21 @@
     # region Utils methods
 
     @check_utils_gql_client
     def create_or_get_concept_by_name(
         self,
         name: str,
         type_id: str,
-        notes: str = None,
+        notes: Optional[str] = None,
         take_first_result: bool = False,
-        with_properties=False,
-        with_links=False,
-        with_link_properties=False,
-        with_facts=False,
-        with_potential_facts=False,
+        with_properties: bool = False,
+        with_links: bool = False,
+        with_link_properties: bool = False,
+        with_facts: bool = False,
+        with_potential_facts: bool = False,
     ) -> Concept:
         """Finds concept by near name"""
 
         if type_id:
             concept_filter_settings: ConceptFilterSettings = uas.ConceptFilterSettings(
                 exact_name=name, concept_type_ids=[type_id]
             )
@@ -2306,15 +2322,15 @@
         )
         self._configure_output_concept_fields(
             goac,
             with_properties=with_properties,
             with_links=with_links,
             with_link_properties=with_link_properties,
             with_facts=with_facts,
-            with_potential_facts=with_potential_facts
+            with_potential_facts=with_potential_facts,
         )
 
         res = self._utils_gql_client.execute(op)
         res = op + res  # type: uas.Mutation
 
         if self.tdm_builder is not None:
             self.tdm_builder.add_concept_fact(res.get_or_add_concept)
@@ -2332,15 +2348,15 @@
     # endregion
 
     # region tcontroller methods
 
     def get_pipeline_configs(
         self,
         with_transforms: bool = True,
-        filter_settings: tc.PipelineConfigFilter = None,
+        filter_settings: Optional[tc.PipelineConfigFilter] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         sort_by: tc.PipelineConfigSort = "id",
         sort_direction: tc.SortDirection = "ascending",
     ) -> tc.PipelineConfigList:
         op = Operation(tc.Query)
         pcl: tc.PipelineConfigList = op.pipeline_configs(
@@ -2353,15 +2369,15 @@
             pc.transforms().__fields__("params")
         res = self._gql_client.execute(op)
         res = op + res
         return res.pipeline_configs
 
     def get_pipeline_topics(
         self,
-        filter_settings: tc.KafkaTopicFilter = None,
+        filter_settings: Optional[tc.KafkaTopicFilter] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         sort_by: tc.KafkaTopicSort = "topic",
         sort_direction: tc.SortDirection = "ascending",
     ) -> tc.KafkaTopicList:
         op = Operation(tc.Query)
         ktl: tc.KafkaTopicList = op.kafka_topics(
@@ -2381,15 +2397,15 @@
         res = self._gql_client.execute(op)
         res = op + res
         return res.put_kafka_topic
 
     def get_failed_messages_from_topic(
         self,
         topic_id: str,
-        filter_settings: tc.MessageFilter = None,
+        filter_settings: Optional[tc.MessageFilter] = None,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         sort_by: tc.MessageSort = "timestamp",
         sort_direction: tc.SortDirection = "descending",
     ) -> tc.FailedMessageList:
         op = Operation(tc.Query)
         fm: tc.FailedMessageList = op.failed_messages(
@@ -2406,15 +2422,15 @@
         res = self._gql_client.execute(op)
         res = op + res
         return res.failed_messages
 
     def get_ok_messages_from_topic(
         self,
         topic_id: str,
-        filter_settings: tc.MessageFilter = None,
+        filter_settings: Optional[tc.MessageFilter] = None,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         sort_by: tc.MessageSort = "timestamp",
         sort_direction: tc.SortDirection = "descending",
     ) -> tc.CompletedOkMessageList:
         op = Operation(tc.Query)
         om: tc.CompletedOkMessageList = op.completed_ok_messages(
@@ -2430,15 +2446,15 @@
         res = self._gql_client.execute(op)
         res = op + res
         return res.completed_ok_messages
 
     def get_active_messages_from_topic(
         self,
         topic_id: str,
-        filter_settings: tc.MessageFilter = None,
+        filter_settings: Optional[tc.MessageFilter] = None,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         sort_by: tc.MessageSort = "timestamp",
         sort_direction: tc.SortDirection = "descending",
     ) -> tc.CompletedOkMessageList:
         op = Operation(tc.Query)
         am: tc.CompletedOkMessageList = op.active_messages(
```

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/common/common.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/common/common.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/base_data_model.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/base_data_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -168,66 +168,118 @@
 
     def get_concept_link_type_name(self, concept_link_type_code: str) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
                 return relation_type_mapping.new_relation_type
         return None
 
+    def get_source_concept_type_code(self, concept_link_type_code: str) -> typing.Optional[str]:
+        for relation_type_mapping in self.relations_types_mapping:
+            if relation_type_mapping.old_relation_type == concept_link_type_code:
+                return relation_type_mapping.source_type
+        return None
+
+    def get_target_concept_type_code(self, concept_link_type_code: str) -> typing.Optional[str]:
+        for relation_type_mapping in self.relations_types_mapping:
+            if relation_type_mapping.old_relation_type == concept_link_type_code:
+                return relation_type_mapping.target_type
+        return None
+
     def get_concept_link_property_type_name(
         self, concept_link_type_code: str, property_type_code: str
     ) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
-                return relation_type_mapping.properties.get(property_type_code, None)
+                return relation_type_mapping.properties.get(property_type_code)
         return None
 
     def get_concept_composite_property_type_name(
         self, concept_type_code: str, composite_property_type_code: str
     ) -> typing.Optional[str]:
         if concept_type_code in self.concepts_types_mapping:
             mapped_concept_type = self.concepts_types_mapping.get(concept_type_code)
+            if mapped_concept_type is None:
+                return None
             if composite_property_type_code in mapped_concept_type.composite_properties:
-                return mapped_concept_type.composite_properties.get(composite_property_type_code).name
+                mapped_composite_property_type = mapped_concept_type.composite_properties.get(
+                    composite_property_type_code
+                )
+                if mapped_composite_property_type:
+                    return mapped_composite_property_type.name
             return None
         return None
 
     def get_concept_composite_property_component_value_type_name(
         self, concept_type_code: str, composite_property_type_code: str, component_value_type_code: str
     ) -> typing.Optional[str]:
         if concept_type_code in self.concepts_types_mapping:
             mapped_concept_type = self.concepts_types_mapping.get(concept_type_code)
+            if mapped_concept_type is None:
+                return None
+            if composite_property_type_code in mapped_concept_type.composite_properties:
+                mapped_composite_property = mapped_concept_type.composite_properties.get(composite_property_type_code)
+                if mapped_composite_property:
+                    return mapped_composite_property.component_values.get(component_value_type_code)
+            return None
+        return None
+
+    def get_concept_composite_property_component_values(
+        self, concept_type_code: str, composite_property_type_code: str
+    ) -> typing.Optional[typing.Dict[str, str]]:
+        if concept_type_code in self.concepts_types_mapping:
+            mapped_concept_type = self.concepts_types_mapping.get(concept_type_code)
+            if mapped_concept_type is None:
+                return None
             if composite_property_type_code in mapped_concept_type.composite_properties:
                 mapped_composite_property = mapped_concept_type.composite_properties.get(composite_property_type_code)
-                return mapped_composite_property.component_values.get(component_value_type_code, None)
+                if mapped_composite_property:
+                    return mapped_composite_property.component_values
             return None
         return None
 
     def get_concept_link_composite_property_type_name(
         self, concept_link_type_code: str, composite_property_type_code: str
     ) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
                 if composite_property_type_code in relation_type_mapping.composite_properties:
-                    return relation_type_mapping.composite_properties.get(composite_property_type_code).name
+                    mapped_composite_property_type = relation_type_mapping.composite_properties.get(
+                        composite_property_type_code
+                    )
+                    if mapped_composite_property_type:
+                        return mapped_composite_property_type.name
                 return None
         return None
 
     def get_concept_link_composite_property_component_value_type_name(
         self, concept_link_type_code: str, composite_property_type_code: str, component_value_type_code: str
     ) -> typing.Optional[str]:
         for relation_type_mapping in self.relations_types_mapping:
             if relation_type_mapping.old_relation_type == concept_link_type_code:
                 if composite_property_type_code in relation_type_mapping.composite_properties:
                     mapped_composite_property = relation_type_mapping.composite_properties.get(
                         composite_property_type_code
                     )
-                    return mapped_composite_property.component_values.get(component_value_type_code, None)
+                    if mapped_composite_property:
+                        return mapped_composite_property.component_values.get(component_value_type_code)
                 return None
         return None
 
+    def get_concept_link_composite_property_component_values(
+        self, concept_link_type_code: str, composite_property_type_code: str
+    ) -> typing.Optional[typing.Dict[str, str]]:
+        for relation_type_mapping in self.relations_types_mapping:
+            if relation_type_mapping.old_relation_type == concept_link_type_code:
+                mapped_composite_property_type = relation_type_mapping.composite_properties.get(
+                    composite_property_type_code
+                )
+                if mapped_composite_property_type:
+                    return mapped_composite_property_type.component_values
+        return None
+
     def add_mapped_concept_type(self, concept_type_code: str, mapped_concept_type: MappedConceptType) -> None:
         self.concepts_types_mapping[concept_type_code] = mapped_concept_type
 
     def add_mapped_concept_link_type(self, mapped_concept_link_type: MappedConceptLinkType) -> None:
         self.relations_types_mapping.append(mapped_concept_link_type)
 
     def add_mapped_concept_property_value_type(
```

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/config_data_model.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/config_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/data_model/custom_data_model.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/data_model/custom_data_model.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/model_parameters/name_code_mapping.yml`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/custom_data_handler.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/custom_data_handler.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/file_generator.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/file_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/object_name_transformer.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/object_name_transformer.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_generator.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_generator.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py` & `ptal_api-0.11.6.1/ptal_api/core/type_mapper/modules/type_mapping_loader/type_mapping_loader.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/core/values/value_mapping.py` & `ptal_api-0.11.6.1/ptal_api/core/values/value_mapping.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/providers/gql_providers.py` & `ptal_api-0.11.6.1/ptal_api/providers/gql_providers.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/schema/README.md` & `ptal_api-0.11.6.1/ptal_api/schema/README.md`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/schema/api_schema.py` & `ptal_api-0.11.6.1/ptal_api/schema/api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/schema/crawlers_api_schema.py` & `ptal_api-0.11.6.1/ptal_api/schema/crawlers_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/schema/tcontroller_api_schema.py` & `ptal_api-0.11.6.1/ptal_api/schema/tcontroller_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/schema/utils_api_schema.py` & `ptal_api-0.11.6.1/ptal_api/schema/utils_api_schema.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/scripts/type_mapper.py` & `ptal_api-0.11.6.1/ptal_api/scripts/type_mapper.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/ptal_api/tdm_builder/tdm_builder.py` & `ptal_api-0.11.6.1/ptal_api/tdm_builder/tdm_builder.py`

 * *Files identical despite different names*

### Comparing `ptal_api-0.11.6/pyproject.toml` & `ptal_api-0.11.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ptal-api"
-version = "0.11.6"
+version = "0.11.6.1"
 description = "TALISMAN API adapter"
 authors = ["Evgeny Bechkalo <bechkalo@ispras.ru>", "Ivan Medvedev <medvedev.iv@ispras.ru>", "Alexey Isakov <isakov@ispras.ru>"]
 readme = "README.md"
 packages = [{include = "ptal_api"}]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Programming Language :: Python :: 3',
```

### Comparing `ptal_api-0.11.6/PKG-INFO` & `ptal_api-0.11.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 Metadata-Version: 2.1
 Name: ptal-api
-Version: 0.11.6
+Version: 0.11.6.1
 Summary: TALISMAN API adapter
 Author: Evgeny Bechkalo
 Author-email: bechkalo@ispras.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: graphql-core (>=3.2.3)
 Requires-Dist: marshmallow-dataclass (>=8.5.11)
 Requires-Dist: python-keycloak (>=2.6.0)
 Requires-Dist: ruamel.yaml (>=0.17.21)
 Requires-Dist: sgqlc (>=16.0)
 Requires-Dist: transliterate (>=1.10.2)
```

