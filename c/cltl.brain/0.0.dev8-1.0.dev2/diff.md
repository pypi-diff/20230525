# Comparing `tmp/cltl.brain-0.0.dev8.tar.gz` & `tmp/cltl.brain-1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/selbaez/Documents/PhD/leolani/cltl-knowledgerepresentation/dist/tmpdar6hw3j/cltl.brain-0.0.dev8.tar", last modified: Mon Mar 14 14:52:45 2022, max compression
+gzip compressed data, was "cltl.brain-1.0.dev2.tar", last modified: Thu May 25 12:38:47 2023, max compression
```

## Comparing `cltl.brain-0.0.dev8.tar` & `cltl.brain-1.0.dev2.tar`

### file list

```diff
@@ -1,125 +1,128 @@
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/
--rw-r--r--   0 selbaez    (501) staff       (20)     1069 2020-11-19 02:00:37.000000 cltl.brain-0.0.dev8/LICENSE
--rw-r--r--   0 selbaez    (501) staff       (20)       15 2021-10-14 10:52:21.000000 cltl.brain-0.0.dev8/MANIFEST.in
--rw-r--r--   0 selbaez    (501) staff       (20)     3753 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/PKG-INFO
--rw-r--r--   0 selbaez    (501) staff       (20)     3439 2022-01-18 13:19:11.000000 cltl.brain-0.0.dev8/README.md
--rw-r--r--   0 selbaez    (501) staff       (20)        9 2022-03-14 14:52:35.000000 cltl.brain-0.0.dev8/VERSION
--rw-r--r--   0 selbaez    (501) staff       (20)       70 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/setup.cfg
--rw-r--r--   0 selbaez    (501) staff       (20)     1327 2022-01-09 19:34:04.000000 cltl.brain-0.0.dev8/setup.py
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/
--rw-r--r--   0 selbaez    (501) staff       (20)     6356 2022-01-09 19:34:04.000000 cltl.brain-0.0.dev8/src/cltl/brain/LTM_question_processing.py
--rw-r--r--   0 selbaez    (501) staff       (20)    18754 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/LTM_statement_processing.py
--rw-r--r--   0 selbaez    (501) staff       (20)      517 2022-01-24 13:24:25.000000 cltl.brain-0.0.dev8/src/cltl/brain/__init__.py
--rw-r--r--   0 selbaez    (501) staff       (20)    12478 2022-03-03 13:22:11.000000 cltl.brain-0.0.dev8/src/cltl/brain/basic_brain.py
--rw-r--r--   0 selbaez    (501) staff       (20)     3727 2022-02-02 22:41:07.000000 cltl.brain-0.0.dev8/src/cltl/brain/fame_aware.py
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/
--rw-r--r--   0 selbaez    (501) staff       (20)      152 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/__init__.py
--rw-r--r--   0 selbaez    (501) staff       (20)    28715 2022-03-14 13:12:31.000000 cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/api.py
--rw-r--r--   0 selbaez    (501) staff       (20)    16423 2022-02-27 13:53:08.000000 cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/rdf_builder.py
--rw-r--r--   0 selbaez    (501) staff       (20)     1937 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/store_connector.py
--rw-r--r--   0 selbaez    (501) staff       (20)    10229 2022-02-27 16:48:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/long_term_memory.py
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/
--rw-r--r--   0 selbaez    (501) staff       (20)    93553 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/blackbox_dataset.csv
--rw-r--r--   0 selbaez    (501) staff       (20)     1166 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/catalog-v001.xml
--rw-r--r--   0 selbaez    (501) staff       (20)   961832 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/ceo_original.owl
--rw-r--r--   0 selbaez    (501) staff       (20)   643872 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/ceo_original.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)     1745 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/eps.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    41814 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/gaf_extended.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)     4577 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/gaf_original.rdf
--rw-r--r--   0 selbaez    (501) staff       (20)    13314 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/grasp_extended.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    10977 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/grasp_original.rdf
--rw-r--r--   0 selbaez    (501) staff       (20)  1156223 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/integration.jsonld
--rw-r--r--   0 selbaez    (501) staff       (20)    42749 2022-01-09 19:34:04.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/integration.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    22230 2021-08-23 17:39:40.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/integration_context.jsonld
--rw-r--r--   0 selbaez    (501) staff       (20)    31241 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/n2mu.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    18569 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-dc.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    17621 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-dictionary.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)     3732 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-links.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)   124985 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-o-inverses.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    79571 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-o.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    21896 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/sem_extended.ttl
--rw-r--r--   0 selbaez    (501) staff       (20)    22715 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/ontologies/sem_original.rdf
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/
--rw-r--r--   0 selbaez    (501) staff       (20)     1531 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/all_negation_conflicts.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      556 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/best_friends.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      260 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/count_friends.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      263 2022-03-03 11:46:32.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/count_instances.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      268 2022-02-24 22:10:12.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/count_perspectives.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      264 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/count_statements.rq
--rw-r--r--   0 selbaez    (501) staff       (20)       56 2022-03-03 11:44:58.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/count_triples.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      259 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/my_friends.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      159 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/triples_with_predicate.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/context/
--rw-r--r--   0 selbaez    (501) staff       (20)      556 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/context/detections_per_context.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      887 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/context/ranked_object_ids_per_type.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      777 2021-08-23 19:22:50.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/context/rename_location.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      233 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/count_of_type.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     2818 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/famous_person.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/id/
--rw-r--r--   0 selbaez    (501) staff       (20)      188 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/id/id_of_instance.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      911 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/one_to_one_conflicts.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1232 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/prefixes.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/structure exploration/
--rw-r--r--   0 selbaez    (501) staff       (20)      250 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/structure exploration/classes.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      167 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/structure exploration/labels_and_classes.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1347 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/structure exploration/ontology_elements.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      217 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/structure exploration/ontology_uploaded.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      259 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/structure exploration/predicates.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/
--rw-r--r--   0 selbaez    (501) staff       (20)      129 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/entity_novelty.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1245 2022-02-27 17:37:39.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/negation_conflicts.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1179 2022-03-14 13:47:40.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/object_cardinality_conflicts.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      396 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/object_gaps.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1251 2022-03-14 14:04:22.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/object_overlap.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      747 2022-03-14 13:12:31.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/statement_novelty.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      396 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/subject_gaps.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1251 2022-03-14 14:04:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/subject_overlap.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/
--rw-r--r--   0 selbaez    (501) staff       (20)      129 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/entity_novelty.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1141 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/negation_conflicts.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1058 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/object_cardinality_conflicts.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      396 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/object_gaps.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1152 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/object_overlap.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      732 2022-02-27 13:49:17.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/statement_novelty.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      396 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/subject_gaps.rq
--rw-r--r--   0 selbaez    (501) staff       (20)     1139 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/subject_overlap.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/
--rw-r--r--   0 selbaez    (501) staff       (20)     1588 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/conflicts_by.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      414 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/count_chat_with.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      405 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/count_statements_by.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      103 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/delete_trust.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      401 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/novel_statements_by.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      423 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/trust_by.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      697 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/when_last_chat_with.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/typing/
--rw-r--r--   0 selbaez    (501) staff       (20)      682 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/typing/dbpedia_type_and_description.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      157 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/typing/instance_of_type.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      277 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/typing/type_of_instance.rq
--rw-r--r--   0 selbaez    (501) staff       (20)      404 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/queries/typing/wikidata_type_and_description.rq
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/reasoners/
--rw-r--r--   0 selbaez    (501) staff       (20)      369 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/reasoners/__init__.py
--rw-r--r--   0 selbaez    (501) staff       (20)     6915 2022-02-02 22:41:07.000000 cltl.brain-0.0.dev8/src/cltl/brain/reasoners/location_reasoner.py
--rw-r--r--   0 selbaez    (501) staff       (20)    13955 2022-03-01 17:56:10.000000 cltl.brain-0.0.dev8/src/cltl/brain/reasoners/thought_generator.py
--rw-r--r--   0 selbaez    (501) staff       (20)     4288 2022-03-03 12:55:57.000000 cltl.brain-0.0.dev8/src/cltl/brain/reasoners/trust_calculator.py
--rw-r--r--   0 selbaez    (501) staff       (20)     6887 2022-02-02 22:41:07.000000 cltl.brain-0.0.dev8/src/cltl/brain/reasoners/type_reasoner.py
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/brain/utils/
--rw-r--r--   0 selbaez    (501) staff       (20)        0 2021-08-23 15:17:38.000000 cltl.brain-0.0.dev8/src/cltl/brain/utils/__init__.py
--rw-r--r--   0 selbaez    (501) staff       (20)    73857 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/utils/base_cases.py
--rw-r--r--   0 selbaez    (501) staff       (20)      795 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/brain/utils/constants.py
--rw-r--r--   0 selbaez    (501) staff       (20)     3817 2021-11-03 16:11:49.000000 cltl.brain-0.0.dev8/src/cltl/brain/utils/helper_functions.py
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/combot/
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/combot/backend/
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/combot/backend/api/
--rw-r--r--   0 selbaez    (501) staff       (20)      646 2022-02-08 16:14:04.000000 cltl.brain-0.0.dev8/src/cltl/combot/backend/api/discrete.py
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl/combot/backend/utils/
--rw-r--r--   0 selbaez    (501) staff       (20)     1004 2022-01-12 11:47:20.000000 cltl.brain-0.0.dev8/src/cltl/combot/backend/utils/casefolding.py
--rw-r--r--   0 selbaez    (501) staff       (20)     2452 2022-02-24 22:08:30.000000 cltl.brain-0.0.dev8/src/cltl/combot/backend/utils/triple_helpers.py
-drwxr-xr-x   0 selbaez    (501) staff       (20)        0 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl.brain.egg-info/
--rw-r--r--   0 selbaez    (501) staff       (20)     3753 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl.brain.egg-info/PKG-INFO
--rw-r--r--   0 selbaez    (501) staff       (20)     4729 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl.brain.egg-info/SOURCES.txt
--rw-r--r--   0 selbaez    (501) staff       (20)        1 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl.brain.egg-info/dependency_links.txt
--rw-r--r--   0 selbaez    (501) staff       (20)      162 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl.brain.egg-info/requires.txt
--rw-r--r--   0 selbaez    (501) staff       (20)        5 2022-03-14 14:52:45.000000 cltl.brain-0.0.dev8/src/cltl.brain.egg-info/top_level.txt
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.578605 cltl.brain-1.0.dev2/
+-rw-r--r--   0 sbaez      (501) staff       (20)     1069 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/LICENSE
+-rw-r--r--   0 sbaez      (501) staff       (20)       15 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/MANIFEST.in
+-rw-r--r--   0 sbaez      (501) staff       (20)     3924 2023-05-25 12:38:47.578672 cltl.brain-1.0.dev2/PKG-INFO
+-rw-r--r--   0 sbaez      (501) staff       (20)     3605 2023-05-25 09:10:36.000000 cltl.brain-1.0.dev2/README.md
+-rw-r--r--   0 sbaez      (501) staff       (20)        9 2023-05-25 12:37:48.000000 cltl.brain-1.0.dev2/VERSION
+-rw-r--r--   0 sbaez      (501) staff       (20)       70 2023-05-25 12:38:47.578876 cltl.brain-1.0.dev2/setup.cfg
+-rw-r--r--   0 sbaez      (501) staff       (20)     1341 2022-12-26 15:09:18.000000 cltl.brain-1.0.dev2/setup.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.549187 cltl.brain-1.0.dev2/src/
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.548276 cltl.brain-1.0.dev2/src/cltl/
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.552742 cltl.brain-1.0.dev2/src/cltl/brain/
+-rw-r--r--   0 sbaez      (501) staff       (20)     4374 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/LTM_context_processing.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2549 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/LTM_experience_processing.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     1347 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/LTM_mention_processing.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     6589 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/LTM_question_processing.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    10838 2022-11-15 18:45:45.000000 cltl.brain-1.0.dev2/src/cltl/brain/LTM_shared.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     1704 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/LTM_statement_processing.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      517 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    12521 2023-05-25 12:25:04.000000 cltl.brain-1.0.dev2/src/cltl/brain/basic_brain.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     3888 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/fame_aware.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.553892 cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/
+-rw-r--r--   0 sbaez      (501) staff       (20)      152 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    27397 2022-11-15 18:45:45.000000 cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/api.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    16521 2022-12-12 14:37:33.000000 cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/rdf_builder.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2343 2022-12-28 19:17:19.000000 cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/store_connector.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    13973 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/long_term_memory.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.568669 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/
+-rw-r--r--   0 sbaez      (501) staff       (20)     1473 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/BASIC-REPOSITORY-CONFIG-GRAPHDB.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    93553 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/blackbox_dataset.csv
+-rw-r--r--   0 sbaez      (501) staff       (20)     1166 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/catalog-v001.xml
+-rw-r--r--   0 sbaez      (501) staff       (20)   961832 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/ceo_original.owl
+-rw-r--r--   0 sbaez      (501) staff       (20)   643872 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/ceo_original.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)     1745 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/eps.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    41814 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/gaf_extended.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)     4577 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/gaf_original.rdf
+-rw-r--r--   0 sbaez      (501) staff       (20)    13314 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/grasp_extended.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    10977 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/grasp_original.rdf
+-rw-r--r--   0 sbaez      (501) staff       (20)  1156223 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/integration.jsonld
+-rw-r--r--   0 sbaez      (501) staff       (20)    75612 2022-11-15 18:45:40.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/integration.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    22230 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/integration_context.jsonld
+-rw-r--r--   0 sbaez      (501) staff       (20)    21819 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/n2mu.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    15935 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/n2mu_sensory.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    18569 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-dc.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    17621 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-dictionary.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)     3732 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-links.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)   124985 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-o-inverses.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    79571 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-o.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    21896 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/sem_extended.ttl
+-rw-r--r--   0 sbaez      (501) staff       (20)    22715 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/ontologies/sem_original.rdf
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.569464 cltl.brain-1.0.dev2/src/cltl/brain/queries/
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.570839 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/
+-rw-r--r--   0 sbaez      (501) staff       (20)     1562 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/all_negation_conflicts.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      556 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/best_friends.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      260 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/count_friends.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      263 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/count_instances.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      268 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/count_perspectives.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      264 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/count_statements.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)       56 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/count_triples.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      318 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/my_friends.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      159 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/triples_with_predicate.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.571331 cltl.brain-1.0.dev2/src/cltl/brain/queries/context/
+-rw-r--r--   0 sbaez      (501) staff       (20)      556 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/context/detections_per_context.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1096 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/context/ranked_object_ids_per_type.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      777 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/context/rename_location.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      233 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/count_of_type.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     2818 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/famous_person.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.571480 cltl.brain-1.0.dev2/src/cltl/brain/queries/id/
+-rw-r--r--   0 sbaez      (501) staff       (20)      188 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/id/id_of_instance.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      911 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/one_to_one_conflicts.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1232 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/prefixes.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.572202 cltl.brain-1.0.dev2/src/cltl/brain/queries/structure_exploration/
+-rw-r--r--   0 sbaez      (501) staff       (20)      250 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/structure_exploration/classes.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      167 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/structure_exploration/labels_and_classes.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1347 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/structure_exploration/ontology_elements.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      217 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/structure_exploration/ontology_uploaded.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      259 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/structure_exploration/predicates.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.573403 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/
+-rw-r--r--   0 sbaez      (501) staff       (20)      129 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/entity_novelty.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1245 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/negation_conflicts.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1179 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/object_cardinality_conflicts.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      396 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/object_gaps.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1251 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/object_overlap.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      750 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/statement_novelty.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      396 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/subject_gaps.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1251 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/subject_overlap.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.574520 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/
+-rw-r--r--   0 sbaez      (501) staff       (20)      129 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/entity_novelty.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1141 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/negation_conflicts.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1058 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/object_cardinality_conflicts.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      396 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/object_gaps.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1152 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/object_overlap.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      735 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/statement_novelty.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      396 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/subject_gaps.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)     1139 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/subject_overlap.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.575920 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/
+-rw-r--r--   0 sbaez      (501) staff       (20)     1619 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/conflicts_by.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      414 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/count_chat_with.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      405 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/count_statements_by.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      103 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/delete_trust.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      401 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/novel_statements_by.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      423 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/trust_by.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      697 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/when_last_chat_with.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.576527 cltl.brain-1.0.dev2/src/cltl/brain/queries/typing/
+-rw-r--r--   0 sbaez      (501) staff       (20)      682 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/typing/dbpedia_type_and_description.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      157 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/typing/instance_of_type.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      277 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/typing/type_of_instance.rq
+-rw-r--r--   0 sbaez      (501) staff       (20)      476 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/queries/typing/wikidata_type_and_description.rq
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.577287 cltl.brain-1.0.dev2/src/cltl/brain/reasoners/
+-rw-r--r--   0 sbaez      (501) staff       (20)      369 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/reasoners/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     6950 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/reasoners/location_reasoner.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    14076 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/reasoners/thought_generator.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     4288 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/reasoners/trust_calculator.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     6874 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/reasoners/type_reasoner.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.578203 cltl.brain-1.0.dev2/src/cltl/brain/utils/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/utils/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)    86652 2022-11-15 18:45:40.000000 cltl.brain-1.0.dev2/src/cltl/brain/utils/base_cases.py
+-rw-r--r--   0 sbaez      (501) staff       (20)      795 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl/brain/utils/constants.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     2941 2022-11-15 18:45:40.000000 cltl.brain-1.0.dev2/src/cltl/brain/utils/helper_functions.py
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.550790 cltl.brain-1.0.dev2/src/cltl.brain.egg-info/
+-rw-r--r--   0 sbaez      (501) staff       (20)     3924 2023-05-25 12:38:47.000000 cltl.brain-1.0.dev2/src/cltl.brain.egg-info/PKG-INFO
+-rw-r--r--   0 sbaez      (501) staff       (20)     4925 2023-05-25 12:38:47.000000 cltl.brain-1.0.dev2/src/cltl.brain.egg-info/SOURCES.txt
+-rw-r--r--   0 sbaez      (501) staff       (20)        1 2023-05-25 12:38:47.000000 cltl.brain-1.0.dev2/src/cltl.brain.egg-info/dependency_links.txt
+-rw-r--r--   0 sbaez      (501) staff       (20)      199 2023-05-25 12:38:47.000000 cltl.brain-1.0.dev2/src/cltl.brain.egg-info/requires.txt
+-rw-r--r--   0 sbaez      (501) staff       (20)       18 2023-05-25 12:38:47.000000 cltl.brain-1.0.dev2/src/cltl.brain.egg-info/top_level.txt
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.549234 cltl.brain-1.0.dev2/src/cltl_service/
+drwxr-xr-x   0 sbaez      (501) staff       (20)        0 2023-05-25 12:38:47.578426 cltl.brain-1.0.dev2/src/cltl_service/brain/
+-rw-r--r--   0 sbaez      (501) staff       (20)        0 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl_service/brain/__init__.py
+-rw-r--r--   0 sbaez      (501) staff       (20)     3962 2022-11-10 16:19:22.000000 cltl.brain-1.0.dev2/src/cltl_service/brain/service.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cltl.brain-0.0.dev8/LICENSE` & `cltl.brain-1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/PKG-INFO` & `cltl.brain-1.0.dev2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: cltl.brain
-Version: 0.0.dev8
-Summary: The Leolani Brain module for knowledge representation
-Home-page: https://github.com/leolani/cltl-knowledgerepresentation
-License: MIT License
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cltl-knowledgerepresentation
 
 A knowledge representation service (aka Leolani's Brain). This service expects structures data and outputs an RDF graph.
 
 ## Description
 
 This package contains the necessary functionality for creating an RDF episodic knowledge graph. It features:
@@ -49,15 +38,15 @@
     ```
 
 2. Additionally, you need to install [GraphDB Free](http://graphdb.ontotext.com/) with a repository named `sandbox`. You
    will need to launch this before running the package.
 
 ### Usage
 
-For using this repository as a package different project and on a different virtual environment, you may
+For using this repository as a package for different project and on a different virtual environment, you may
 
 - install a published version from PyPI:
 
     ```bash
     pip install cltl.brain
     ```
 
@@ -67,14 +56,24 @@
     pip install git+git://github.com/leolani/cltl-knowledgerepresentation.git@main
     ```
 
 Then you can import it in a python script as:
 
     import cltl.brain
 
+
+You can also modify the logger level as such:
+
+```python
+import logging
+
+from cltl.brain import logger as brain_logger
+
+brain_logger.setLevel(logging.ERROR)
+```
 ## Examples
 
 Please take a look at the example scripts provided to get an idea on how to run and use this package. Each example has a
 comment at the top of the script describing the behaviour of the script.
 
 For these example scripts, you need
 
@@ -102,9 +101,8 @@
 Distributed under the MIT License.
 See [`LICENSE`](https://github.com/leolani/cltl-knowledgerepresentation/blob/main/LICENCE) for more information.
 
 ## Authors
 
 * [Selene Báez Santamaría](https://selbaez.github.io/)
 * [Thomas Baier](https://www.linkedin.com/in/thomas-baier-05519030/)
-* [Piek Vossen](https://github.com/piekvossen)
-
+* [Piek Vossen](https://github.com/piekvossen)
```

### Comparing `cltl.brain-0.0.dev8/README.md` & `cltl.brain-1.0.dev2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: cltl.brain
+Version: 1.0.dev2
+Summary: The Leolani Brain module for knowledge representation
+Home-page: https://github.com/leolani/cltl-knowledgerepresentation
+License: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: service
+License-File: LICENSE
+
 # cltl-knowledgerepresentation
 
 A knowledge representation service (aka Leolani's Brain). This service expects structures data and outputs an RDF graph.
 
 ## Description
 
 This package contains the necessary functionality for creating an RDF episodic knowledge graph. It features:
@@ -38,15 +49,15 @@
     ```
 
 2. Additionally, you need to install [GraphDB Free](http://graphdb.ontotext.com/) with a repository named `sandbox`. You
    will need to launch this before running the package.
 
 ### Usage
 
-For using this repository as a package different project and on a different virtual environment, you may
+For using this repository as a package for different project and on a different virtual environment, you may
 
 - install a published version from PyPI:
 
     ```bash
     pip install cltl.brain
     ```
 
@@ -56,14 +67,24 @@
     pip install git+git://github.com/leolani/cltl-knowledgerepresentation.git@main
     ```
 
 Then you can import it in a python script as:
 
     import cltl.brain
 
+
+You can also modify the logger level as such:
+
+```python
+import logging
+
+from cltl.brain import logger as brain_logger
+
+brain_logger.setLevel(logging.ERROR)
+```
 ## Examples
 
 Please take a look at the example scripts provided to get an idea on how to run and use this package. Each example has a
 comment at the top of the script describing the behaviour of the script.
 
 For these example scripts, you need
 
@@ -91,8 +112,8 @@
 Distributed under the MIT License.
 See [`LICENSE`](https://github.com/leolani/cltl-knowledgerepresentation/blob/main/LICENCE) for more information.
 
 ## Authors
 
 * [Selene Báez Santamaría](https://selbaez.github.io/)
 * [Thomas Baier](https://www.linkedin.com/in/thomas-baier-05519030/)
-* [Piek Vossen](https://github.com/piekvossen)
+* [Piek Vossen](https://github.com/piekvossen)
```

### Comparing `cltl.brain-0.0.dev8/setup.py` & `cltl.brain-1.0.dev2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,25 +15,30 @@
     url="https://github.com/leolani/cltl-knowledgerepresentation",
     license='MIT License',
     authors={
         "Baez Santamaria": ("Selene Baez Santamaria", "s.baezsantamaria@vu.nl"),
         "Baier": ("Thomas Baier", "t.baier@vu.nl")
     },
     package_dir={'': 'src'},
-    packages=find_namespace_packages(include=['cltl.*'], where='src'),
+    packages=find_namespace_packages(include=['cltl.*', 'cltl_service.*'], where='src'),
     package_data={'cltl.brain': ['ontologies/*', 'ontologies/**/*', 'queries/*', 'queries/**/*']},
     python_requires='>=3.7',
     install_requires=[
-        # 'cltl.combot @ git+https://github.com/leolani/cltl-combot.git#e76f2baa4668d9546e93c7e5a5df102648d40c17',
-        'requests>=2.25',
-        'rdflib>=5.0',
-        'sparqlwrapper>=1.8',
-        'numpy>=1.20',
-        'fuzzywuzzy>=0.18',
-        'nltk>=3.4',
-        'iribaker>=0.2',
-        'python-Levenshtein>=0.12',
-        'importlib_resources>=5.2',
-        'tqdm==4.62.3'
+        'requests~=2.25',
+        'rdflib~=6.1.1',
+        'sparqlwrapper~=1.8',
+        'numpy~=1.20',
+        'fuzzywuzzy~=0.18',
+        'nltk~=3.4.4',
+        'iribaker~=0.2',
+        'python-Levenshtein~=0.12',
+        'importlib_resources~=5.2',
+        'tqdm~=4.62',
+        "cltl.combot"
     ],
+    extras_require={
+        "service": [
+            "cltl.combot",
+        ]
+    },
     setup_requires=['flake8']
 )
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/LTM_question_processing.py` & `cltl.brain-1.0.dev2/src/cltl/brain/LTM_question_processing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from rdflib import Literal
 
 
 ######################################### Helpers for question processing #########################################
 
-def create_query(self, utterance):
-    empty = ['', Literal(''), 'unknown', 'none']
 
+def _is_empty(entry):
+    return str(entry).lower() in ['', Literal(''), 'unknown', 'none']
+
+
+def create_query(self, utterance):
     # Query subject
-    if utterance['subject']['label'] is None or utterance['subject']['uri'].lower() in empty:
+    if _is_empty(utterance['subject']['label']) or _is_empty(utterance['subject']['uri']):
         query = """
         SELECT distinct ?p ?pOriginal ?s ?slabel ?o ?olabel 
                         ?authorlabel ?certaintyValue ?polarityValue ?sentimentValue ?emotionValue ?temporalValue
            WHERE { 
                BIND(<%s> AS ?p).
                BIND(<%s> AS ?o).
 
@@ -22,19 +25,21 @@
                 ?s rdfs:label ?slabel .
                 ?o rdfs:label ?olabel .
                }
 
                GRAPH ?g {
                    ?s ?pOriginal ?o . 
                } . 
+               
+               OPTIONAL {
                ?g gaf:denotedBy ?m . 
                ?m grasp:wasAttributedTo ?author . 
                ?author rdfs:label ?authorlabel .
-
                ?m grasp:hasAttribution ?att .
+               }
 
                OPTIONAL {
                ?att rdf:value ?certainty .
                ?certainty rdf:type graspf:CertaintyValue .
                ?certainty rdfs:label ?certaintyValue .
                }
 
@@ -62,15 +67,15 @@
                ?sentiment rdfs:label ?sentimentValue .
                }
            }
            """ % (utterance['predicate']['uri'],
                   utterance['object']['uri'])
 
     # Query complement
-    elif utterance['object']['label'] is None or utterance['object']['uri'].lower() in empty:
+    elif _is_empty(utterance['object']['label']) or _is_empty(utterance['object']['uri']):
         query = """
         SELECT distinct ?p ?pOriginal ?s ?slabel ?o ?olabel 
                         ?authorlabel ?certaintyValue ?polarityValue ?sentimentValue ?emotionValue ?temporalValue
            WHERE { 
                BIND(<%s> AS ?s).
                BIND(<%s> AS ?p).
             
@@ -81,19 +86,21 @@
                 ?s rdfs:label ?slabel .
                 ?o rdfs:label ?olabel .
                }
                
                GRAPH ?g {
                    ?s ?pOriginal ?o . 
                } . 
+               
+               OPTIONAL {
                ?g gaf:denotedBy ?m . 
                ?m grasp:wasAttributedTo ?author . 
                ?author rdfs:label ?authorlabel .
-
                ?m grasp:hasAttribution ?att .
+               }
                
                OPTIONAL {
                ?att rdf:value ?certainty .
                ?certainty rdf:type graspf:CertaintyValue .
                ?certainty rdfs:label ?certaintyValue .
                }
 
@@ -141,19 +148,21 @@
                 ?s rdfs:label ?slabel .
                 ?o rdfs:label ?olabel .
                }
                
                GRAPH ?g {
                    ?s ?pOriginal ?o . 
                } . 
+               
+               OPTIONAL {
                ?g gaf:denotedBy ?m . 
                ?m grasp:wasAttributedTo ?author . 
                ?author rdfs:label ?authorlabel .
-
                ?m grasp:hasAttribution ?att .
+               }
                
                OPTIONAL {
                ?att rdf:value ?certainty .
                ?certainty rdf:type graspf:CertaintyValue .
                ?certainty rdfs:label ?certaintyValue .
                }
 
@@ -183,10 +192,11 @@
            }
            """ % (utterance['subject']['uri'],
                   utterance['predicate']['uri'],
                   utterance['object']['uri'])
 
     query = self.query_prefixes + query
 
-    self._log.info(f"Triple in question: {utterance['triple']}")
+    self._log.info("Triple in question: %s", utterance['triple'])
+    # print(query)
 
     return query
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/__init__.py` & `cltl.brain-1.0.dev2/src/cltl/brain/__init__.py`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/basic_brain.py` & `cltl.brain-1.0.dev2/src/cltl/brain/basic_brain.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from cltl.brain import logger
 from cltl.brain.infrastructure import StoreConnector, RdfBuilder
 from cltl.brain.utils.helper_functions import read_query
 
 
 class BasicBrain(object):
     _ONE_TO_ONE_PREDICATES = [
-        'be-from',
-        'born_in',
-        'favorite',
+        'be-from', 'be-at'
         'live-in',
-        'work-at'
+        'work-at',
+        'be-father-of', 'be-mother-of', 'be-husband-of', 'be-wife-of'
     ]
 
     _NOT_TO_ASK_PREDICATES = ['faceID', 'name']
 
     def __init__(self, address, log_dir, clear_all=False, is_submodule=False):
         # type: (str, pathlib.Path, bool, bool) -> None
         """
@@ -74,17 +73,17 @@
 
         """
         self._log.debug("Posting query")
 
         return self._connection.query(query, ask=ask, post=post)
 
     def _brain_log(self):
-        return self.log_dir.joinpath(f"brain_log_{datetime.now().strftime('%Y-%m-%d-%H-%M-%S')}")
+        return self.log_dir.joinpath(f"brain_log_{datetime.now().strftime('%Y-%m-%d-%H-%M-%S-%f')}")
 
-    ########## brain structure exploration ##########
+    ########## brain structure_exploration ##########
     def _serialize(self, file_path):
         """
         Save graph to local file and return the serialized string
         :param file_path: path to where data will be saved
         :return: serialized data as string
         """
         # Save to file and return the string representation
@@ -114,59 +113,59 @@
 
     def ontology_is_uploaded(self):
         """
         Query the existence of the Ontology graph, thus not importing the whole Ontology every time
         :return: response status
         """
         self._log.debug("Checking if ontology is in brain")
-        query = read_query('structure exploration/ontology_uploaded')
+        query = read_query('structure_exploration/ontology_uploaded')
         response = self._submit_query(query, ask=True)
 
         return response
 
     def get_predicates(self):
         """
         Get predicates in social ontology
         :return:
         """
-        query = read_query('structure exploration/predicates')
+        query = read_query('structure_exploration/predicates')
         response = self._submit_query(query)
 
         return [elem['p']['value'].split('/')[-1] for elem in response]
 
     def get_classes(self):
         """
         Get classes or types in social ontology
         :return:
         """
-        query = read_query('structure exploration/classes')
+        query = read_query('structure_exploration/classes')
         response = self._submit_query(query)
 
         return [elem['c']['value'].split('/')[-1] for elem in response]
 
     def get_labels_and_classes(self):
         """
         Get classes in social ontology
         :return:
         """
-        query = read_query('structure exploration/labels_and_classes')
+        query = read_query('structure_exploration/labels_and_classes')
         response = self._submit_query(query)
 
         temp = dict()
         for r in response:
             temp[r['l']['value']] = r['type']['value'].split('/')[-1]
 
         return temp
 
     def get_ontology_elements(self):
         """
         Get classes, object and data properties in ontology
         :return:
         """
-        query = read_query('structure exploration/ontology_elements')
+        query = read_query('structure_exploration/ontology_elements')
         response = self._submit_query(query)
 
         temp = dict()
         for r in response:
             temp[r['name']['value']] = r['prefixedName']['value']
 
         return temp
@@ -196,24 +195,24 @@
 
     ########## learned facts exploration ##########
     def count_triples(self):
         """
         Count triples in the brain
         :return:
         """
-        query = read_query('content exploration/count_triples')
+        query = read_query('content_exploration/count_triples')
         response = self._submit_query(query)
         return float(response[0]['triples']['value'])
 
     def count_statements(self):
         """
         Count statements or 'facts' in the brain
         :return:
         """
-        query = read_query('content exploration/count_statements')
+        query = read_query('content_exploration/count_statements')
         response = self._submit_query(query)
         return float(response[0]['count']['value'])
 
     def count_statements_by(self, actor_uri):
         """
         Count statements or 'facts' in the brain by a given author
         :return:
@@ -232,24 +231,24 @@
         return [elem['statement']['value'].split('/')[-1] for elem in response]
 
     def count_perspectives(self):
         """
         Count perspectives or 'views' in the brain
         :return:
         """
-        query = read_query('content exploration/count_perspectives')
+        query = read_query('content_exploration/count_perspectives')
         response = self._submit_query(query)
         return float(response[0]['count']['value'])
 
     def get_all_negation_conflicts(self):
         """
         Count conflicts or 'facts' with opposing polarity in the brain
         :return:
         """
-        query = read_query('content exploration/all_negation_conflicts')
+        query = read_query('content_exploration/all_negation_conflicts')
         response = self._submit_query(query)
         return response
 
     def get_conflicts_by(self, actor_uri):
         """
         Return conflicts or 'facts' with opposing polarity in the brain stated by a specific actor
         :return:
@@ -260,33 +259,33 @@
         return response
 
     def count_friends(self):
         """
         Count number of people I have talked to
         :return:
         """
-        query = read_query('content exploration/count_friends')
+        query = read_query('content_exploration/count_friends')
         response = self._submit_query(query)
         return float(response[0]['count']['value'])
 
     def get_my_friends(self):
         """
         Get names of people I have talked to
         :return:
         """
-        query = read_query('content exploration/my_friends')
+        query = read_query('content_exploration/my_friends')
         response = self._submit_query(query)
         return [elem['friend']['value'].split('/')[-1] for elem in response]
 
     def get_best_friends(self):
         """
         Get names of the 5 people I have talked to the most
         :return:
         """
-        query = read_query('content exploration/best_friends')
+        query = read_query('content_exploration/best_friends')
         response = self._submit_query(query)
         return [(elem['act']['value'], elem['num_chat']['value'].split('/')[-1]) for elem in response]
 
     def when_last_chat_with(self, actor_uri):
         """
         Get time value for the last time I chatted with this person
         :param actor_uri: uri of person
@@ -309,15 +308,15 @@
         return float(response[0]['num_chats']['value'].split('/')[-1]) if response != [] else 0.0
 
     def count_instances(self):
         """
         Count instances or world entities in the brain
         :return:
         """
-        query = read_query('content exploration/count_instances')
+        query = read_query('content_exploration/count_instances')
         response = self._submit_query(query)
         return float(response[0]['count']['value'])
 
     def get_instance_of_type(self, instance_type):
         """
         Get instances of a certain class type
         :param instance_type: name of class in ontology
@@ -349,15 +348,15 @@
 
     def get_triples_with_predicate(self, predicate_uri):
         """
         Get triples that contain this predicate
         :param predicate_uri:
         :return:
         """
-        query = read_query('content exploration/triples_with_predicate') % predicate_uri
+        query = read_query('content_exploration/triples_with_predicate') % predicate_uri
         response = self._submit_query(query)
         return [(elem['s']['value'], elem['o']['value']) for elem in response]
 
     ########## WARNING deletions area ##########
 
     def clear_brain(self):
         """
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/fame_aware.py` & `cltl.brain-1.0.dev2/src/cltl/brain/fame_aware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pathlib
 
 import requests
+from cltl.commons.casefolding import casefold_text
+from iribaker import to_iri
+from rdflib import RDF, URIRef
 
 from cltl.brain.LTM_statement_processing import _link_entity, create_claim_graph
 from cltl.brain.long_term_memory import LongTermMemory
 from cltl.brain.utils.helper_functions import read_query
-from cltl.combot.backend.utils.casefolding import casefold_text
 
 
 class FameAwareMemory(LongTermMemory):
     def __init__(self, address, log_dir, clear_all=False):
         # type: (str, pathlib.Path, bool) -> None
         """
         Interact with Triple store
@@ -50,38 +52,40 @@
                 self._log.info(f"{total_triples} triples found for {comb}")
 
                 for triple in data['results']['bindings']:
                     # Add claim to the dataset
                     self.add_triple(triple)
 
                 # Finish process of uploading new knowledge to the triple store
-                data = self._serialize(self._brain_log())
+                rdf_log_path = self._brain_log()
+                data = self._serialize(rdf_log_path)
                 code = self._upload_to_brain(data)
 
-                return {'response': code, 'label': person_name, 'data': data}
+                return {'response': code, 'label': person_name, 'data': data, 'rdf_log_path': rdf_log_path}
 
         return {'response': None, 'label': person_name, 'data': None}
 
     def add_triple(self, triple):
 
         # Parse subject
         s_types = self._rdf_builder.clean_aggregated_types(triple['subjectTypesLabel']['value'])
-        s = self._rdf_builder.fill_entity(casefold_text(triple['subjectLabel']['value'], format='triple'),
-                                          s_types, uri=triple['subject']['value'])
+        s = self._rdf_builder.fill_entity(casefold_text(triple['subjectLabel']['value'], format='triple'), s_types)
         _link_entity(self, s, self.instance_graph, create_label=True)
+        self.instance_graph.add((s.id, RDF.type, URIRef(to_iri(triple['subject']['value']))))
 
         # Parse predicate
         p = self._rdf_builder.fill_predicate(casefold_text(triple['propLabel']['value'], format='triple'),
                                              uri=triple['property']['value'])
 
         # Parse object
         if 'literal' in triple['objectTypesLabel']['value']:
             o = self._rdf_builder.fill_literal(casefold_text(triple['objectLabel']['value'], format='triple'))
             self.instance_graph.add((s.id, p.id, o))
         else:
             o_types = self._rdf_builder.clean_aggregated_types(triple['objectTypesLabel']['value'])
-            o = self._rdf_builder.fill_entity(casefold_text(triple['objectLabel']['value'], format='triple'),
-                                              o_types, uri=triple['object']['value'])
+            o = self._rdf_builder.fill_entity(casefold_text(triple['objectLabel']['value'], format='triple'), o_types)
             _link_entity(self, o, self.instance_graph, create_label=True)
+            self.instance_graph.add((s.id, RDF.type, URIRef(to_iri(triple['object']['value']))))
+
             create_claim_graph(self, s, p, o)
 
         # self._log.info(f'Triple: {}')
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/api.py` & `cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import random
 from datetime import date, datetime
 from typing import List, Optional
 
-from nltk.stem import WordNetLemmatizer
+from cltl.commons.casefolding import casefold_text
+from cltl.commons.discrete import Certainty, Polarity, Sentiment, Emotion, Time
+from cltl.commons.triple_helpers import filtered_types_names
 from rdflib import Literal
 
 from cltl.brain.utils.helper_functions import hash_claim_id, is_proper_noun
-from cltl.combot.backend.api.discrete import Certainty, Polarity, Sentiment, Emotion, Time
-from cltl.combot.backend.utils.casefolding import casefold_text
-from cltl.combot.backend.utils.triple_helpers import filtered_types_names
 
 
 class RDFBase(object):
     def __init__(self, id, label, offset=None, confidence=0.0):
         # type: (str, str, Optional[slice], float) -> None
         """
         Construct RDFBase Object
@@ -94,15 +93,14 @@
             Indeces of substring where this entity was mentioned
         confidence: float
             Confidence value that this entity was mentioned
         """
         super(Entity, self).__init__(id, label, offset, confidence)
 
         self._types = [t for t in types if t != '' and t is not None]
-        self._types = list(dict.fromkeys(self._types))
 
     @property
     def types(self):
         # type: () -> List[str]
         return self._types
 
     @property
@@ -186,66 +184,18 @@
         complement_label = complement.label if complement is not None and complement.label not in ['',
                                                                                                    Literal('')] else (
             complement.types if complement is not None else '?')
 
         if format == 'triple':
             # Label
             self._label = Literal(casefold_text(self.label, format=format))
-            self._label = Literal(
-                self._fix_predicate_morphology(subject_label, str(self.label), complement_label, format=format))
 
         elif format == 'natural':
             # Label
             self._label = casefold_text(self.label, format=format)
-            self._label = self._fix_predicate_morphology(subject_label, self.label, complement_label, format=format)
-
-    @staticmethod
-    def _fix_predicate_morphology(subject, predicate, complement, format='triple'):
-        """
-        Conjugation
-        Parameters
-        ----------
-        subject
-        predicate
-
-        Returns
-        -------
-
-        """
-        # TODO revise by Lenka
-        new_predicate = ''
-        if format == 'triple':
-            if len(predicate.split()) > 1:
-                for el in predicate.split():
-                    if el == 'is':
-                        new_predicate += 'be-'
-                    else:
-                        new_predicate += el + '-'
-
-            elif predicate.endswith('s'):
-                new_predicate = WordNetLemmatizer().lemmatize(predicate)
-
-            else:
-                new_predicate = predicate
-
-        elif format == 'natural':
-            if len(predicate.split()) > 1:
-                for el in predicate.split():
-                    if el == 'be':
-                        new_predicate += 'is '
-                    else:
-                        new_predicate += el + ' '
-
-            # elif predicate == wnl.lemmatize(predicate):
-            #    new_predicate = predicate + 's' # TODO conjugate!
-
-            else:
-                new_predicate = predicate
-
-        return new_predicate.strip(' ')
 
 
 class Triple(object):
     def __init__(self, subject, predicate, complement):
         # type: (Entity, Predicate, Entity) -> None
         """
         Construct Triple Object
@@ -672,39 +622,50 @@
     def __repr__(self):
         subject = 'new' if self.subject else 'existing'
         complement = 'new' if self.complement else 'existing'
         return f'{subject} subject - {complement} object'
 
 
 class Gap(object):
-    def __init__(self, predicate, entity):
-        # type: (Predicate, Entity) -> None
+    def __init__(self, known_entity, predicate, entity):
+        # type: (Entity, Predicate, Entity) -> None
         """
         Construct Gap Object
         Parameters
         ----------
         predicate: Predicate
             Information about what can be known for the entity
         entity: Entity
             Information about the type of things that can be known
         """
+        self._known_entity = known_entity
         self._predicate = predicate
         self._entity = entity
 
     @property
+    def known_entity(self):
+        # type: () -> Entity
+        return self._known_entity
+
+    @property
     def predicate(self):
         # type: () -> Predicate
         return self._predicate
 
     @property
     def entity(self):
         # type: () -> Entity
         return self._entity
 
     @property
+    def known_entity_name(self):
+        # type: () -> str
+        return self._known_entity.label
+
+    @property
     def predicate_name(self):
         # type: () -> str
         return self._predicate.label
 
     @property
     def entity_range(self):
         # type: () -> List[str]
@@ -723,19 +684,20 @@
         ----------
         format
 
         Returns
         -------
 
         """
+        self._known_entity.casefold(format)
         self._entity.casefold(format)
         self._predicate.casefold(self.entity, None, format)
 
     def __repr__(self):
-        return f'{self.predicate_name} {self.entity_range_name}'
+        return f'{self.known_entity_name} {self.predicate_name} {self.entity_range_name}'
 
 
 class Gaps(object):
     def __init__(self, subject_gaps, complement_gaps):
         # type: (List[Gap], List[Gap]) -> None
         """
         Construct Gap Object
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/rdf_builder.py` & `cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/rdf_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 
 import importlib_resources as pkg_resources
+from cltl.commons.casefolding import casefold_text
+from cltl.commons.discrete import Certainty, Polarity, Sentiment, Emotion
+from cltl.commons.triple_helpers import fix_nlp_types
 from iribaker import to_iri
 from rdflib import Dataset, Namespace, OWL, URIRef, Literal
 
 from cltl.brain import logger
 from cltl.brain.infrastructure import Predicate, Entity, Triple, Provenance, Perspective
 from cltl.brain.utils.helper_functions import confidence_to_certainty_value, polarity_to_polarity_value, \
     sentiment_to_sentiment_value, emotion_to_emotion_value
-from cltl.combot.backend.api.discrete import Certainty, Polarity, Sentiment, Emotion
-from cltl.combot.backend.utils.casefolding import casefold_text
-from cltl.combot.backend.utils.triple_helpers import fix_nlp_types
 
 
 class RdfBuilder(object):
     def __init__(self):
         # type: () -> None
 
         self.namespaces = {}
@@ -141,15 +141,15 @@
         self.perspective_graph = self.dataset.graph(self.create_resource_uri('LTa', 'Perspectives'))
         self.interaction_graph = self.dataset.graph(self.create_resource_uri('LTa', 'Interactions'))
 
     def load_ontologies(self):
         with pkg_resources.files("cltl.brain") as pkg_root:
             ontology_root = pkg_root / 'ontologies'
             self.ontology_graph.parse(location=os.path.join(ontology_root, 'integration.ttl'), format="turtle")
-            self.ontology_graph.parse(location=os.path.join(ontology_root, 'ceo_original.ttl'), format="turtle")
+            # self.ontology_graph.parse(location=os.path.join(ontology_root, 'ceo_original.ttl'), format="turtle")
 
     ########## basic constructors ##########
     def create_resource_uri(self, namespace, resource_name):
         # type: (str, str) -> str
         """
         Create an URI for the given resource (entity, predicate, named graph, etc) in the given namespace
         Parameters
@@ -205,16 +205,17 @@
         namespace: str
             Namespace where entity belongs to
 
         Returns
         -------
             Entity object with given label
         """
+        types = [t for t in types if t not in [None, '']]
 
-        if types in [None, ''] and label != '':
+        if not types and label != '':
             self._log.warning(f'Unknown type: {label}')
             return self.fill_entity_from_label(label, namespace)
         else:
             entity_id = self.create_resource_uri(namespace, label) if not uri else URIRef(to_iri(uri))
             fixed_types = fix_nlp_types(types)
             return Entity(entity_id, Literal(label), fixed_types)
 
@@ -303,14 +304,17 @@
         perpective_dict: dict
             Dictionary with raw values for every perspective axis
 
         Returns
         -------
             Perspective object containing factuality, sentiment and emotion values
         """
+        if type(perpective_dict) == Perspective:
+            return perpective_dict
+
         certainty = perpective_dict.get('certainty', Certainty.UNDERSPECIFIED)
         polarity = perpective_dict.get('polarity', Polarity.UNDERSPECIFIED)
         sentiment = perpective_dict.get('sentiment', Sentiment.UNDERSPECIFIED)
         emotion = perpective_dict.get('emotion', Emotion.UNDERSPECIFIED)
 
         certainty_value = confidence_to_certainty_value(certainty)
         polarity_value = polarity_to_polarity_value(polarity)
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/infrastructure/store_connector.py` & `cltl.brain-1.0.dev2/src/cltl/brain/infrastructure/store_connector.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,8 +65,22 @@
         response = sparql.query().convert()
 
         if ask:
             return response['boolean']
         if post:
             return response
         else:
-            return response["results"]["bindings"]
+            return response["results"]["bindings"]
+
+    def export_repository(self):
+        """
+        Export all data in the brain
+        :param
+        :return: data in repository, as trig
+        """
+
+        # From serialized string
+        post_url = self.address + "/statements"
+        response = requests.get(post_url,
+                                 headers={'Content-Type': 'application/x-' + self.format})
+
+        return str(response.text)
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/blackbox_dataset.csv` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/blackbox_dataset.csv`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/catalog-v001.xml` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/catalog-v001.xml`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/ceo_original.owl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/ceo_original.owl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/ceo_original.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/ceo_original.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/eps.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/eps.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/gaf_extended.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/gaf_extended.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/gaf_original.rdf` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/gaf_original.rdf`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/grasp_extended.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/grasp_extended.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/grasp_original.rdf` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/grasp_original.rdf`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/integration.jsonld` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/integration.jsonld`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/integration_context.jsonld` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/integration_context.jsonld`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-dc.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-dc.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-dictionary.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-dictionary.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-links.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-links.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-o-inverses.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-o-inverses.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/prov-o.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/prov-o.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/sem_extended.ttl` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/sem_extended.ttl`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/ontologies/sem_original.rdf` & `cltl.brain-1.0.dev2/src/cltl/brain/ontologies/sem_original.rdf`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/all_negation_conflicts.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/all_negation_conflicts.rq`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 PREFIX gaf: <http://groundedannotationframework.org/gaf#>
 PREFIX grasp: <http://groundedannotationframework.org/grasp#>
 PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX graspf: <http://groundedannotationframework.org/grasp/factuality#>
 PREFIX prov: <http://www.w3.org/ns/prov#>
 PREFIX sem: <http://semanticweb.cs.vu.nl/2009/11/sem/>
+prefix leolaniFriends: <http://cltl.nl/leolani/friends/>
 
 SELECT ?g ?datePos ?authorPos ?dateNeg ?authorNeg
 
 WHERE {
     ?g gaf:denotedBy ?mPos .
     ?mPos grasp:hasAttribution ?attPos .
     ?attPos rdf:value graspf:POSITIVE .
@@ -27,13 +28,13 @@
     ?uttNeg rdf:type grasp:Utterance .
     ?contNeg sem:hasEvent / sem:hasSubEvent ?uttNeg .
     ?contNeg ?time_predNeg ?dateNeg .
     VALUES (?time_predNeg) { (sem:hasTime) (sem:hasBeginTimeStamp) } .
     ?mNeg grasp:wasAttributedTo ?authorNeg .
 
 
-    FILTER (STRSTARTS(STR(?authorPos), "http://cltl.nl/leolani/friends/")
-            && STRSTARTS(STR(?authorNeg), "http://cltl.nl/leolani/friends/")
+    FILTER (STRSTARTS(STR(?authorPos), STR(leolaniFriends:))
+            && STRSTARTS(STR(?authorNeg), STR(leolaniFriends:))
     ) .
 
 }
 GROUP BY ?g ?datePos ?authorPos ?dateNeg ?authorNeg
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/content exploration/best_friends.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/content_exploration/best_friends.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/context/detections_per_context.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/context/detections_per_context.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/context/ranked_object_ids_per_type.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/context/ranked_object_ids_per_type.rq`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+
+PREFIX n2mu: <http://cltl.nl/leolani/n2mu/>
+PREFIX xml1: <https://www.w3.org/TR/xmlschema-2/#>
 PREFIX eps: <http://cltl.nl/episodicawareness/>
 PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX sem: <http://semanticweb.cs.vu.nl/2009/11/sem/>
-PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
-PREFIX n2mu: <http://cltl.nl/leolani/n2mu/>
-PREFIX leolaniContext: <http://cltl.nl/leolani/context/>
 
-SELECT ?type  (GROUP_CONCAT(DISTINCT ?si;separator="|") as ?ids) (GROUP_CONCAT( ?num_observation;separator="|") as ?imp)
+SELECT ?type  (GROUP_CONCAT(DISTINCT ?detection_id;separator="|") as ?ids) (GROUP_CONCAT( ?num_observation;separator="|") as ?importance)
 WHERE {
 
-SELECT ?si  (COUNT(DISTINCT ?c) as ?num_observation)   (GROUP_CONCAT(DISTINCT ?stob;separator="|") as ?type)
+SELECT ?detection ?detection_id  (COUNT(DISTINCT ?context) as ?num_observation) (GROUP_CONCAT(DISTINCT ?object_type; separator="|") as ?type)
+
 WHERE {
-    ?c eps:hasDetection ?s .
-    ?s n2mu:id ?si .
-    ?s rdf:type n2mu:object, ?st, ?stob .
-    FILTER(regex(str(?stob), "n2mu")) .
-    FILTER(regex(str(?st), "n2mu")) .
-    FILTER(!regex(str(?stob), "object")) .
-    ?c sem:hasPlace leolaniContext:%s  .
+    # Identify the place where this context is taking place
+    ?seedContext n2mu:id "%s"^^xml1:string.
+    ?seedContext sem:hasPlace ?place .
+
+    # Get detections and their id
+    ?context sem:hasPlace ?place .
+    ?context eps:hasDetection ?detection .
+    ?detection n2mu:id ?detection_id .
+
+    ?detection rdf:type n2mu:object, ?object_type .
+
+    FILTER(regex(str(?object_type), "n2mu")) .
+    FILTER(!regex(str(?object_type), "object")) .
 }
-group by ?si
-    order by DESC(COUNT(DISTINCT ?c))
+group by ?detection ?detection_id
+order by DESC(COUNT(DISTINCT ?context))
+
 }
 group by ?type
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/context/rename_location.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/context/rename_location.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/famous_person.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/famous_person.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/one_to_one_conflicts.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/one_to_one_conflicts.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/prefixes.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/prefixes.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/structure exploration/ontology_elements.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/structure_exploration/ontology_elements.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/negation_conflicts.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/negation_conflicts.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/object_cardinality_conflicts.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/object_cardinality_conflicts.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/object_overlap.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/object_overlap.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/statement_novelty.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/statement_novelty.rq`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 select ?date ?authorlabel where {
     <%s> gaf:denotedBy ?m .
 
     ?m prov:wasDerivedFrom ?utt .
 
     ?context sem:hasEvent / sem:hasSubEvent ?utt .
-    ?cont ?time_pred ?d .
+    ?context ?time_pred ?d .
     ?d rdfs:label ?date .
     VALUES (?time_pred) { (sem:hasTime) (sem:hasBeginTimeStamp) } .
 
     ?m grasp:wasAttributedTo ?author .
     OPTIONAL {
         ?author rdfs:label ?authorlabel .
     }
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts/subject_overlap.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts/subject_overlap.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/negation_conflicts.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/negation_conflicts.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/object_cardinality_conflicts.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/object_cardinality_conflicts.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/object_overlap.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/object_overlap.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/statement_novelty.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/statement_novelty.rq`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 select ?date ?authorlabel where {
     <%s> gaf:denotedBy ?m .
 
     ?m prov:wasDerivedFrom ?utt .
 
     ?context sem:hasEvent / sem:hasSubEvent ?utt .
-    ?cont ?time_pred ?d .
+    ?context ?time_pred ?d .
     ?d rdfs:label ?date .
     VALUES (?time_pred) { (sem:hasTime) (sem:hasBeginTimeStamp) } .
 
     ?m grasp:wasAttributedTo ?author .
     OPTIONAL {
         ?author rdfs:label ?authorlabel .
     }
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/thoughts_subproperties/subject_overlap.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/thoughts_subproperties/subject_overlap.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/conflicts_by.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/conflicts_by.rq`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 PREFIX gaf: <http://groundedannotationframework.org/gaf#>
 PREFIX grasp: <http://groundedannotationframework.org/grasp#>
 PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX graspf: <http://groundedannotationframework.org/grasp/factuality#>
 PREFIX prov: <http://www.w3.org/ns/prov#>
 PREFIX sem: <http://semanticweb.cs.vu.nl/2009/11/sem/>
+prefix leolaniFriends: <http://cltl.nl/leolani/friends/>
 
 SELECT ?g ?datePos ?authorPos ?dateNeg ?authorNeg
 
 WHERE {
     ?g gaf:denotedBy ?mPos .
     ?mPos grasp:hasAttribution ?attPos .
     ?attPos rdf:value graspf:POSITIVE .
@@ -30,13 +31,13 @@
     ?contNeg ?time_predNeg ?dateNeg .
     VALUES (?time_predNeg) { (sem:hasTime) (sem:hasBeginTimeStamp) } .
     ?mNeg grasp:wasAttributedTo ?authorNeg .
 
 
     FILTER (?authorPos = <%s> || ?authorNeg = <%s> ) .
 
-    FILTER (STRSTARTS(STR(?authorPos), "http://cltl.nl/leolani/friends/")
-            && STRSTARTS(STR(?authorNeg), "http://cltl.nl/leolani/friends/")
+    FILTER (STRSTARTS(STR(?authorPos), STR(leolaniFriends:))
+            && STRSTARTS(STR(?authorNeg), STR(leolaniFriends:))
     ) .
 
 }
 GROUP BY ?g ?datePos ?authorPos ?dateNeg ?authorNeg
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/trust/when_last_chat_with.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/trust/when_last_chat_with.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/queries/typing/dbpedia_type_and_description.rq` & `cltl.brain-1.0.dev2/src/cltl/brain/queries/typing/dbpedia_type_and_description.rq`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/reasoners/location_reasoner.py` & `cltl.brain-1.0.dev2/src/cltl/brain/reasoners/location_reasoner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pathlib
 
+from cltl.commons.casefolding import casefold_text
+
 from cltl.brain.basic_brain import BasicBrain
 from cltl.brain.utils.helper_functions import read_query
-from cltl.combot.backend.utils.casefolding import casefold_text
 
 
 class LocationReasoner(BasicBrain):
     def __init__(self, address, log_dir, clear_all=False):
         # type: (str, pathlib.Path, bool) -> None
         """
         Interact with Triple store
@@ -78,15 +79,15 @@
         preprocessed_types = self._rdf_builder.clean_aggregated_types(raw_objects_in_location['type']['value'])
         preprocessed_ids = raw_objects_in_location['ids']['value'].split('|')
 
         return preprocessed_types, preprocessed_ids
 
     def get_location_memory(self, capsule):
         # brain object memories
-        query = read_query('context/ranked_object_ids_per_type') % casefold_text(capsule['place'], format='triple')
+        query = read_query('context/ranked_object_ids_per_type') % capsule['context_id']
         response = self._submit_query(query)
 
         location_memory = {}
         if response and response[0]['type']['value'] != '':
             for elem in response:
                 categories, ids = self._fill_location_memory_(elem)
                 # assign multiple categories (eg selene is person and agent)
@@ -108,36 +109,36 @@
         for cat, ids in list(location_memory.items()):
             all_ids = ids['brain_ids'][:]
             all_ids.extend(ids['local_ids'])
             ids['ids'] = all_ids
 
         return location_memory
 
-    def reason_location(self, capsule):
+    def reason_location(self, context_capsule, detections):
 
-        if capsule['place'] is None or capsule['place'].lower() == '':
+        if context_capsule['place'] is None or context_capsule['place'].lower() == '':
             guess = None
 
             # Query all locations and detections (through context)
             memory = self.get_episodic_memory()
 
             if memory:
                 # Generate set of current detections
                 observations = []
-                for item in capsule['objects']:
+                for item in detections['objects']:
                     if item['type'].lower() != 'person':
                         observations.append(casefold_text(item['type'], format='triple'))
-                for item in capsule['people']:
+                for item in detections['people']:
                     if item['name'].lower() != 'unknown':
                         observations.append(casefold_text(item['name'], format='triple'))
 
                 # Take geo information into account
-                observations.append(capsule['city'])
-                observations.append(capsule['country'])
-                observations.append(capsule['region'])
+                observations.append(context_capsule['city'])
+                observations.append(context_capsule['country'])
+                observations.append(context_capsule['region'])
 
                 # Compare one by one and determine most similar
                 for mem in memory:
                     memory_elements = mem['detections']
                     memory_elements.extend(mem['geo'])
                     mem['overlap'] = self._measure_detection_overlap(memory_elements, observations)
 
@@ -149,15 +150,15 @@
                     else None
 
                 self._log.info(f"Reasoned location to: {guess} with {best_guess['overlap']} overlap")
 
             return guess
 
         else:
-            return capsule['place']
+            return context_capsule['place']
 
     def set_location_label(self, context_id, label, old_label='unknown'):
         # Replace as subject, replace label, replace as object in the database (long term memory)
         query = read_query('context/rename_location') % (old_label, label, context_id, old_label, label)
         _ = self._submit_query(query, post=True)
 
         self._log.info(f"Set location to: {label}")
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/reasoners/thought_generator.py` & `cltl.brain-1.0.dev2/src/cltl/brain/reasoners/thought_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         if response and response[0] != {}:
             novelties = [self._fill_statement_novelty_(elem) for elem in response]
         else:
             novelties = []
 
         if novelties:
             n = random.choice(novelties)
-            self._log.info(f"Statement Novelty: {len(response)} times, e.g. {n.__str__()}")
+            self._log.info(f"Statement Novelty: mentioned {len(response)} times, e.g. {n.__str__()}")
 
         return novelties
 
     def _check_instance_novelty_(self, instance_url):
         """
         Query if an instance (entity) has been heard about before
         Parameters
@@ -107,33 +107,35 @@
         """
         query = read_query('thoughts/entity_novelty') % instance_url
         response = self._submit_query(query, ask=True)
 
         return response
 
     ########## gaps ##########
-    def _fill_entity_gap_(self, raw_response):
+    def _fill_entity_gap_(self, entity, raw_response):
         """
         Structure entity gap to get the predicate and range of what has been learned but not heard
         Parameters
         ----------
+        entity: Entity
+            entity for which we are getting gaps
         raw_response: dict
             standard row result from SPARQL
 
         Returns
         -------
-            Gap object containing a predicate and its range
+            Gap object containing a predicate and its range/domain
         """
 
         processed_predicate = self._rdf_builder.fill_predicate(raw_response['p']['value'].split('/')[-1],
                                                                uri=raw_response['p']['value'])
         processed_range = self._rdf_builder.fill_entity('', namespace='N2MU',
                                                         types=[raw_response['type2']['value'].split('/')[-1]])
 
-        return Gap(processed_predicate, processed_range)
+        return Gap(entity, processed_predicate, processed_range)
 
     def get_entity_gaps(self, entity, exclude=None):
         """
         Query and build gaps with regards to the range and domain of the given entity and its predicates
         Parameters
         ----------
         entity: Entity
@@ -145,27 +147,27 @@
             Gaps object containing gaps related to range and domain information that could be learned
         """
         # Role as subject
         query = read_query('thoughts/subject_gaps') % (entity.id, entity.id if exclude is None else exclude.id)
         response = self._submit_query(query)
 
         if response:
-            subject_gaps = [self._fill_entity_gap_(elem)
+            subject_gaps = [self._fill_entity_gap_(entity, elem)
                             for elem in response
                             if elem['p']['value'].split('/')[-1] not in self._NOT_TO_ASK_PREDICATES]
 
         else:
             subject_gaps = []
 
         # Role as object
         query = read_query('thoughts/object_gaps') % (entity.id, entity.id if exclude is None else exclude.id)
         response = self._submit_query(query)
 
         if response:
-            complement_gaps = [self._fill_entity_gap_(elem)
+            complement_gaps = [self._fill_entity_gap_(entity, elem)
                                for elem in response
                                if elem['p']['value'].split('/')[-1] not in self._NOT_TO_ASK_PREDICATES]
 
         else:
             complement_gaps = []
 
         gaps = Gaps(subject_gaps, complement_gaps)
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/reasoners/trust_calculator.py` & `cltl.brain-1.0.dev2/src/cltl/brain/reasoners/trust_calculator.py`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/reasoners/type_reasoner.py` & `cltl.brain-1.0.dev2/src/cltl/brain/reasoners/type_reasoner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 
 import requests
+from cltl.commons.casefolding import casefold_text
 from fuzzywuzzy import process
 
 from cltl.brain.basic_brain import BasicBrain
 from cltl.brain.utils.helper_functions import read_query, remove_articles
-from cltl.combot.backend.utils.casefolding import casefold_text
 
 
 class TypeReasoner(BasicBrain):
 
     def __init__(self, address, log_dir, clear_all=False):
         # type: (str, pathlib.Path, bool) -> None
         """
```

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/utils/constants.py` & `cltl.brain-1.0.dev2/src/cltl/brain/utils/constants.py`

 * *Files identical despite different names*

### Comparing `cltl.brain-0.0.dev8/src/cltl/brain/utils/helper_functions.py` & `cltl.brain-1.0.dev2/src/cltl/brain/utils/helper_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import enum
+import pathlib
 from datetime import date
 
 import importlib_resources as pkg_resources
 import numpy as np
+from cltl.commons.casefolding import casefold_text
+from cltl.commons.discrete import Certainty, Polarity, Sentiment, Emotion
 from rdflib import URIRef, Literal
 
 import cltl.brain
 from cltl.brain.utils.constants import CAPITALIZED_TYPES
-from cltl.combot.backend.api.discrete import Certainty, Polarity, Sentiment, Emotion
-from cltl.combot.backend.utils.casefolding import casefold_text
 
 
 def read_query(query_filename):
     """
     Read a query from file and return as a string
     Parameters
     ----------
@@ -46,57 +47,27 @@
 
 
 def hash_claim_id(triple):
     return '_'.join(triple)
 
 
 def confidence_to_certainty_value(confidence):
-    if confidence is not None and type(confidence) != Certainty:
-        confidence = float(confidence)
-
-        if confidence > .90:
-            return Certainty.CERTAIN
-        elif confidence >= .50:
-            return Certainty.PROBABLE
-        elif confidence > 0:
-            return Certainty.POSSIBLE
-
-    return Certainty.UNDERSPECIFIED
+    return Certainty.as_enum(confidence)
 
 
 def polarity_to_polarity_value(polarity):
-    if polarity is not None and type(polarity) != Polarity:
-        polarity = float(polarity)
-
-        if polarity > 0:
-            return Polarity.POSITIVE
-        elif polarity < 0:
-            return Polarity.NEGATIVE
-
-    return Polarity.UNDERSPECIFIED
+    return Polarity.as_enum(polarity)
 
 
 def sentiment_to_sentiment_value(sentiment):
-    if sentiment is not None and type(sentiment) != Sentiment:
-        sentiment = float(sentiment)
-
-        if sentiment > 0:
-            return Sentiment.POSITIVE
-        elif sentiment < 0:
-            return Sentiment.NEGATIVE
-        elif sentiment == 0:
-            return Sentiment.NEUTRAL
-
-    return Sentiment.UNDERSPECIFIED
+    return Sentiment.as_enum(sentiment)
 
 
 def emotion_to_emotion_value(emotion):
-    if emotion is not None and type(emotion) == str:
-        return Emotion[emotion.upper()]
-    return Emotion.UNDERSPECIFIED
+    return Emotion.as_enum(emotion)
 
 
 def replace_in_file(file, word, word_replacement):
     for i, line in enumerate(open(file)):
         line.replace(':%s' % word, ':%s' % word_replacement)
         line.replace('"%s' % word, '"%s' % word_replacement)
 
@@ -113,23 +84,23 @@
 
 
 def sigmoid(z, growth_rate=1):
     return 1 / (1 + np.exp(-z * growth_rate))
 
 
 def element_to_json(v):
-    if type(v) in [str, int, float] or v is None:
+    if type(v) in [str, int, float, bool] or v is None:
         pass
-    elif type(v) in [URIRef, Literal, bool]:
+    elif isinstance(v, (URIRef, Literal, pathlib.Path)):
         v = str(v)
     elif isinstance(v, date):
         v = v.isoformat()
     elif isinstance(v, enum.Enum):
         v = v.name
-    elif isinstance(v, list):
+    elif isinstance(v, list) or isinstance(v, tuple):
         v = [element_to_json(el) for el in v]
     elif isinstance(v, dict):
         v = {inner_k: element_to_json(inner_v) for inner_k, inner_v in v.items()}
     else:
         v = {inner_k: element_to_json(inner_v) for inner_k, inner_v in v.__dict__.items()}
 
     return v
```

### Comparing `cltl.brain-0.0.dev8/src/cltl.brain.egg-info/PKG-INFO` & `cltl.brain-1.0.dev2/src/cltl.brain.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cltl.brain
-Version: 0.0.dev8
+Version: 1.0.dev2
 Summary: The Leolani Brain module for knowledge representation
 Home-page: https://github.com/leolani/cltl-knowledgerepresentation
 License: MIT License
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: service
 License-File: LICENSE
 
 # cltl-knowledgerepresentation
 
 A knowledge representation service (aka Leolani's Brain). This service expects structures data and outputs an RDF graph.
 
 ## Description
@@ -49,15 +49,15 @@
     ```
 
 2. Additionally, you need to install [GraphDB Free](http://graphdb.ontotext.com/) with a repository named `sandbox`. You
    will need to launch this before running the package.
 
 ### Usage
 
-For using this repository as a package different project and on a different virtual environment, you may
+For using this repository as a package for different project and on a different virtual environment, you may
 
 - install a published version from PyPI:
 
     ```bash
     pip install cltl.brain
     ```
 
@@ -67,14 +67,24 @@
     pip install git+git://github.com/leolani/cltl-knowledgerepresentation.git@main
     ```
 
 Then you can import it in a python script as:
 
     import cltl.brain
 
+
+You can also modify the logger level as such:
+
+```python
+import logging
+
+from cltl.brain import logger as brain_logger
+
+brain_logger.setLevel(logging.ERROR)
+```
 ## Examples
 
 Please take a look at the example scripts provided to get an idea on how to run and use this package. Each example has a
 comment at the top of the script describing the behaviour of the script.
 
 For these example scripts, you need
 
@@ -103,8 +113,7 @@
 See [`LICENSE`](https://github.com/leolani/cltl-knowledgerepresentation/blob/main/LICENCE) for more information.
 
 ## Authors
 
 * [Selene Báez Santamaría](https://selbaez.github.io/)
 * [Thomas Baier](https://www.linkedin.com/in/thomas-baier-05519030/)
 * [Piek Vossen](https://github.com/piekvossen)
-
```

### Comparing `cltl.brain-0.0.dev8/src/cltl.brain.egg-info/SOURCES.txt` & `cltl.brain-1.0.dev2/src/cltl.brain.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,66 +5,72 @@
 setup.cfg
 setup.py
 src/cltl.brain.egg-info/PKG-INFO
 src/cltl.brain.egg-info/SOURCES.txt
 src/cltl.brain.egg-info/dependency_links.txt
 src/cltl.brain.egg-info/requires.txt
 src/cltl.brain.egg-info/top_level.txt
+src/cltl/brain/LTM_context_processing.py
+src/cltl/brain/LTM_experience_processing.py
+src/cltl/brain/LTM_mention_processing.py
 src/cltl/brain/LTM_question_processing.py
+src/cltl/brain/LTM_shared.py
 src/cltl/brain/LTM_statement_processing.py
 src/cltl/brain/__init__.py
 src/cltl/brain/basic_brain.py
 src/cltl/brain/fame_aware.py
 src/cltl/brain/long_term_memory.py
 src/cltl/brain/infrastructure/__init__.py
 src/cltl/brain/infrastructure/api.py
 src/cltl/brain/infrastructure/rdf_builder.py
 src/cltl/brain/infrastructure/store_connector.py
+src/cltl/brain/ontologies/BASIC-REPOSITORY-CONFIG-GRAPHDB.ttl
 src/cltl/brain/ontologies/blackbox_dataset.csv
 src/cltl/brain/ontologies/catalog-v001.xml
 src/cltl/brain/ontologies/ceo_original.owl
 src/cltl/brain/ontologies/ceo_original.ttl
 src/cltl/brain/ontologies/eps.ttl
 src/cltl/brain/ontologies/gaf_extended.ttl
 src/cltl/brain/ontologies/gaf_original.rdf
 src/cltl/brain/ontologies/grasp_extended.ttl
 src/cltl/brain/ontologies/grasp_original.rdf
 src/cltl/brain/ontologies/integration.jsonld
 src/cltl/brain/ontologies/integration.ttl
 src/cltl/brain/ontologies/integration_context.jsonld
 src/cltl/brain/ontologies/n2mu.ttl
+src/cltl/brain/ontologies/n2mu_sensory.ttl
 src/cltl/brain/ontologies/prov-dc.ttl
 src/cltl/brain/ontologies/prov-dictionary.ttl
 src/cltl/brain/ontologies/prov-links.ttl
 src/cltl/brain/ontologies/prov-o-inverses.ttl
 src/cltl/brain/ontologies/prov-o.ttl
 src/cltl/brain/ontologies/sem_extended.ttl
 src/cltl/brain/ontologies/sem_original.rdf
 src/cltl/brain/queries/count_of_type.rq
 src/cltl/brain/queries/famous_person.rq
 src/cltl/brain/queries/one_to_one_conflicts.rq
 src/cltl/brain/queries/prefixes.rq
-src/cltl/brain/queries/content exploration/all_negation_conflicts.rq
-src/cltl/brain/queries/content exploration/best_friends.rq
-src/cltl/brain/queries/content exploration/count_friends.rq
-src/cltl/brain/queries/content exploration/count_instances.rq
-src/cltl/brain/queries/content exploration/count_perspectives.rq
-src/cltl/brain/queries/content exploration/count_statements.rq
-src/cltl/brain/queries/content exploration/count_triples.rq
-src/cltl/brain/queries/content exploration/my_friends.rq
-src/cltl/brain/queries/content exploration/triples_with_predicate.rq
+src/cltl/brain/queries/content_exploration/all_negation_conflicts.rq
+src/cltl/brain/queries/content_exploration/best_friends.rq
+src/cltl/brain/queries/content_exploration/count_friends.rq
+src/cltl/brain/queries/content_exploration/count_instances.rq
+src/cltl/brain/queries/content_exploration/count_perspectives.rq
+src/cltl/brain/queries/content_exploration/count_statements.rq
+src/cltl/brain/queries/content_exploration/count_triples.rq
+src/cltl/brain/queries/content_exploration/my_friends.rq
+src/cltl/brain/queries/content_exploration/triples_with_predicate.rq
 src/cltl/brain/queries/context/detections_per_context.rq
 src/cltl/brain/queries/context/ranked_object_ids_per_type.rq
 src/cltl/brain/queries/context/rename_location.rq
 src/cltl/brain/queries/id/id_of_instance.rq
-src/cltl/brain/queries/structure exploration/classes.rq
-src/cltl/brain/queries/structure exploration/labels_and_classes.rq
-src/cltl/brain/queries/structure exploration/ontology_elements.rq
-src/cltl/brain/queries/structure exploration/ontology_uploaded.rq
-src/cltl/brain/queries/structure exploration/predicates.rq
+src/cltl/brain/queries/structure_exploration/classes.rq
+src/cltl/brain/queries/structure_exploration/labels_and_classes.rq
+src/cltl/brain/queries/structure_exploration/ontology_elements.rq
+src/cltl/brain/queries/structure_exploration/ontology_uploaded.rq
+src/cltl/brain/queries/structure_exploration/predicates.rq
 src/cltl/brain/queries/thoughts/entity_novelty.rq
 src/cltl/brain/queries/thoughts/negation_conflicts.rq
 src/cltl/brain/queries/thoughts/object_cardinality_conflicts.rq
 src/cltl/brain/queries/thoughts/object_gaps.rq
 src/cltl/brain/queries/thoughts/object_overlap.rq
 src/cltl/brain/queries/thoughts/statement_novelty.rq
 src/cltl/brain/queries/thoughts/subject_gaps.rq
@@ -93,10 +99,9 @@
 src/cltl/brain/reasoners/thought_generator.py
 src/cltl/brain/reasoners/trust_calculator.py
 src/cltl/brain/reasoners/type_reasoner.py
 src/cltl/brain/utils/__init__.py
 src/cltl/brain/utils/base_cases.py
 src/cltl/brain/utils/constants.py
 src/cltl/brain/utils/helper_functions.py
-src/cltl/combot/backend/api/discrete.py
-src/cltl/combot/backend/utils/casefolding.py
-src/cltl/combot/backend/utils/triple_helpers.py
+src/cltl_service/brain/__init__.py
+src/cltl_service/brain/service.py
```

