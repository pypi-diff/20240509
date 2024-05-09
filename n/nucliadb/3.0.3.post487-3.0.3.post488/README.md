# Comparing `tmp/nucliadb-3.0.3.post487-py3-none-any.whl.zip` & `tmp/nucliadb-3.0.3.post488-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,457 +1,457 @@
-Zip file size: 750566 bytes, number of entries: 455
--rw-r--r--  2.0 unx     1135 b- defN 24-May-09 11:27 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-09 11:27 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-09 11:27 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-09 11:27 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-09 11:27 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-09 11:27 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-09 11:27 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-09 11:27 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-09 11:27 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-09 11:27 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-09 11:27 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-09 11:27 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-09 11:27 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-09 11:27 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-09 11:27 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-09 11:27 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-09 11:27 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-09 11:27 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-09 11:27 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-09 11:27 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-May-09 11:27 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-09 11:27 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-09 11:27 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 11:27 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5022 b- defN 24-May-09 11:27 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4971 b- defN 24-May-09 11:27 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-09 11:27 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3790 b- defN 24-May-09 11:27 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-09 11:27 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21584 b- defN 24-May-09 11:27 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8490 b- defN 24-May-09 11:27 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19549 b- defN 24-May-09 11:27 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-May-09 11:27 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5686 b- defN 24-May-09 11:27 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-09 11:27 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-May-09 11:27 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-09 11:27 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-09 11:27 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-09 11:27 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-09 11:27 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-May-09 11:27 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-09 11:27 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-09 11:27 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-09 11:27 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-09 11:27 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-09 11:27 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5633 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-09 11:27 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-09 11:27 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-09 11:27 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-09 11:27 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-09 11:27 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-09 11:27 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-09 11:27 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-09 11:27 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-09 11:27 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-09 11:27 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-09 11:27 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-09 11:27 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-May-09 11:27 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-09 11:27 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-09 11:27 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-09 11:27 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-09 11:27 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-09 11:27 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-09 11:27 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-09 11:27 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-09 11:27 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-09 11:27 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-09 11:27 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-09 11:27 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-09 11:27 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-May-09 11:27 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-09 11:27 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-May-09 11:27 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-09 11:27 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12159 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-09 11:27 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-May-09 11:27 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-09 11:27 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-09 11:27 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-09 11:27 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-09 11:27 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-09 11:27 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-09 11:27 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-09 11:27 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4531 b- defN 24-May-09 11:27 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-09 11:27 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28367 b- defN 24-May-09 11:27 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-09 11:27 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-09 11:27 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-May-09 11:27 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-09 11:27 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-May-09 11:27 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-May-09 11:27 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-09 11:27 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26423 b- defN 24-May-09 11:27 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-09 11:27 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-09 11:27 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33196 b- defN 24-May-09 11:27 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-09 11:27 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-09 11:27 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-09 11:27 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27325 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-09 11:27 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3981 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4075 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-09 11:27 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-09 11:27 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-09 11:27 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-09 11:27 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-09 11:27 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-09 11:27 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-09 11:27 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9249 b- defN 24-May-09 11:27 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-09 11:27 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-09 11:27 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-09 11:27 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-09 11:27 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-09 11:27 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-09 11:27 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-09 11:27 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-09 11:27 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-09 11:27 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-09 11:27 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-09 11:27 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-09 11:27 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-May-09 11:27 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12368 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6450 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3632 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2093 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4454 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13928 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12378 b- defN 24-May-09 11:27 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-May-09 11:27 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-09 11:27 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-09 11:27 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-09 11:27 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-09 11:27 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-09 11:27 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-09 11:27 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-09 11:27 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-09 11:27 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-09 11:27 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-09 11:27 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    17332 b- defN 24-May-09 11:27 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-09 11:27 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-09 11:27 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-09 11:27 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1222 b- defN 24-May-09 11:27 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 24-May-09 11:27 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2665 b- defN 24-May-09 11:27 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8804 b- defN 24-May-09 11:27 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-09 11:27 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3041 b- defN 24-May-09 11:27 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-09 11:27 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18325 b- defN 24-May-09 11:27 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5928 b- defN 24-May-09 11:27 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2536 b- defN 24-May-09 11:27 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1433 b- defN 24-May-09 11:27 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     5887 b- defN 24-May-09 11:27 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5293 b- defN 24-May-09 11:27 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9070 b- defN 24-May-09 11:27 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-09 11:27 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-09 11:27 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-09 11:27 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-09 11:27 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-09 11:27 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-09 11:27 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-09 11:27 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-09 11:27 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-09 11:27 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-09 11:27 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31127 b- defN 24-May-09 11:27 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-09 11:27 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-09 11:27 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-09 11:27 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-09 11:27 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-09 11:27 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15347 b- defN 24-May-09 11:27 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-09 11:27 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-09 11:27 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-09 11:27 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    13101 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8567 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-09 11:27 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-09 11:27 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-09 11:27 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-09 11:27 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-May-09 11:27 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-May-09 11:27 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-09 11:27 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1963 b- defN 24-May-09 11:27 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-09 11:27 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5415 b- defN 24-May-09 11:27 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-May-09 11:27 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-09 11:27 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-09 11:27 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-09 11:27 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-09 11:27 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-09 11:27 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-09 11:27 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-09 11:27 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-09 11:27 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-09 11:27 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1845 b- defN 24-May-09 11:27 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1572 b- defN 24-May-09 11:27 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-09 11:27 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-09 11:27 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-09 11:27 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-09 11:27 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-09 11:27 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-09 11:27 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-09 11:27 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-09 11:27 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-09 11:27 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-09 11:27 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-09 11:27 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-09 11:27 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-09 11:27 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-09 11:27 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-09 11:27 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-09 11:27 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-09 11:27 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3625 b- defN 24-May-09 11:27 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-09 11:27 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2758 b- defN 24-May-09 11:27 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-09 11:27 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-09 11:27 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-09 11:27 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-09 11:27 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3656 b- defN 24-May-09 11:27 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9470 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3750 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2114 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     2998 b- defN 24-May-09 11:27 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-09 11:27 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-09 11:27 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-09 11:27 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-09 11:27 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-09 11:27 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-09 11:27 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-09 11:27 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-09 11:27 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-09 11:27 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-09 11:27 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-09 11:27 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-09 11:27 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-09 11:27 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-09 11:27 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-09 11:27 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-09 11:27 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-09 11:27 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-09 11:27 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-09 11:27 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-09 11:27 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-09 11:27 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-09 11:27 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-09 11:27 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-09 11:27 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-09 11:27 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-09 11:27 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-09 11:27 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-09 11:27 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2065 b- defN 24-May-09 11:27 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-09 11:27 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1905 b- defN 24-May-09 11:27 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2129 b- defN 24-May-09 11:27 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-09 11:27 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-09 11:27 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-09 11:27 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-09 11:27 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-09 11:27 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-09 11:27 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-09 11:27 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-09 11:27 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-09 11:27 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-09 11:27 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-09 11:27 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-09 11:27 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-09 11:27 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-09 11:27 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-09 11:27 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-09 11:27 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-09 11:27 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-09 11:27 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-09 11:27 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-09 11:27 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-09 11:27 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-09 11:27 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-09 11:27 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-09 11:27 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-09 11:27 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-09 11:27 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-09 11:27 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-09 11:27 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19495 b- defN 24-May-09 11:27 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-09 11:27 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-09 11:27 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-09 11:27 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-09 11:27 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-May-09 11:27 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-09 11:27 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-09 11:27 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24419 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5239 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2052 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18869 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10726 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30722 b- defN 24-May-09 11:27 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-09 11:27 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-09 11:27 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-09 11:27 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-09 11:27 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-May-09 11:27 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-09 11:27 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-09 11:27 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 11:27 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-09 11:27 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-09 11:27 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-09 11:27 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-09 11:27 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-09 11:27 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-09 11:27 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-09 11:27 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-09 11:27 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-09 11:27 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-09 11:27 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-09 11:27 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-09 11:27 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-09 11:27 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-09 11:27 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-09 11:27 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-09 11:27 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-09 11:27 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-09 11:27 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-09 11:27 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4399 b- defN 24-May-09 11:28 nucliadb-3.0.3.post487.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 11:28 nucliadb-3.0.3.post487.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-09 11:28 nucliadb-3.0.3.post487.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-09 11:28 nucliadb-3.0.3.post487.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-09 11:28 nucliadb-3.0.3.post487.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42669 b- defN 24-May-09 11:28 nucliadb-3.0.3.post487.dist-info/RECORD
-455 files, 2216990 bytes uncompressed, 682334 bytes compressed:  69.3%
+Zip file size: 750612 bytes, number of entries: 455
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-09 12:28 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-09 12:28 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-09 12:28 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-09 12:28 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-09 12:28 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-09 12:28 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-09 12:28 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-09 12:28 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-09 12:28 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-09 12:28 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-09 12:28 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-09 12:28 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-09 12:28 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-09 12:28 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-09 12:28 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-09 12:28 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-09 12:28 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-09 12:28 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-09 12:28 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-09 12:28 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-May-09 12:28 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-09 12:28 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-09 12:28 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 12:28 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5022 b- defN 24-May-09 12:28 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-May-09 12:28 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-09 12:28 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3790 b- defN 24-May-09 12:28 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-09 12:28 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    21584 b- defN 24-May-09 12:28 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8490 b- defN 24-May-09 12:28 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    19549 b- defN 24-May-09 12:28 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2713 b- defN 24-May-09 12:28 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5686 b- defN 24-May-09 12:28 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-09 12:28 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-May-09 12:28 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-09 12:28 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-09 12:28 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-09 12:28 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-09 12:28 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-May-09 12:28 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-09 12:28 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-09 12:28 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-09 12:28 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-09 12:28 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-09 12:28 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5633 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-09 12:28 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-09 12:28 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-09 12:28 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-09 12:28 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-09 12:28 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-09 12:28 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-09 12:28 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-09 12:28 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-09 12:28 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-09 12:28 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-09 12:28 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-09 12:28 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-May-09 12:28 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-09 12:28 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-09 12:28 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-09 12:28 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-09 12:28 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-09 12:28 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-09 12:28 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-09 12:28 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-09 12:28 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-09 12:28 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-09 12:28 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-09 12:28 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-09 12:28 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-May-09 12:28 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-09 12:28 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-May-09 12:28 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-09 12:28 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12159 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-09 12:28 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-09 12:28 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-09 12:28 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-09 12:28 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-09 12:28 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-09 12:28 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-09 12:28 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-09 12:28 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-09 12:28 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4531 b- defN 24-May-09 12:28 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-09 12:28 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28367 b- defN 24-May-09 12:28 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-09 12:28 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-09 12:28 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17167 b- defN 24-May-09 12:28 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-09 12:28 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-09 12:28 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-May-09 12:28 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-09 12:28 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26423 b- defN 24-May-09 12:28 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-09 12:28 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-09 12:28 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    33196 b- defN 24-May-09 12:28 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-09 12:28 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-09 12:28 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-09 12:28 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27325 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-09 12:28 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3981 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4075 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-09 12:28 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-09 12:28 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-09 12:28 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-09 12:28 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-09 12:28 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-09 12:28 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-09 12:28 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9249 b- defN 24-May-09 12:28 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-09 12:28 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-09 12:28 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-09 12:28 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-09 12:28 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-09 12:28 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-09 12:28 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-09 12:28 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-09 12:28 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-09 12:28 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-09 12:28 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-09 12:28 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-09 12:28 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-May-09 12:28 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13940 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12399 b- defN 24-May-09 12:28 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-May-09 12:28 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-09 12:28 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-09 12:28 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-09 12:28 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-09 12:28 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-09 12:28 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-09 12:28 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-09 12:28 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-09 12:28 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-09 12:28 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-09 12:28 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    17332 b- defN 24-May-09 12:28 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-09 12:28 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-09 12:28 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-09 12:28 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1222 b- defN 24-May-09 12:28 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9882 b- defN 24-May-09 12:28 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-09 12:28 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8810 b- defN 24-May-09 12:28 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-09 12:28 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-09 12:28 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-09 12:28 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18337 b- defN 24-May-09 12:28 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-09 12:28 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-09 12:28 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1433 b- defN 24-May-09 12:28 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-09 12:28 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-09 12:28 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9070 b- defN 24-May-09 12:28 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-09 12:28 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-09 12:28 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-09 12:28 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-09 12:28 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-09 12:28 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-09 12:28 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-09 12:28 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-09 12:28 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-09 12:28 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-09 12:28 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31127 b- defN 24-May-09 12:28 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-09 12:28 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-09 12:28 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-09 12:28 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-09 12:28 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-09 12:28 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15347 b- defN 24-May-09 12:28 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-09 12:28 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-09 12:28 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-09 12:28 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    13101 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8567 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-09 12:28 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-09 12:28 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-09 12:28 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-09 12:28 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-May-09 12:28 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-May-09 12:28 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-09 12:28 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1963 b- defN 24-May-09 12:28 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-09 12:28 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5415 b- defN 24-May-09 12:28 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-May-09 12:28 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-09 12:28 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-09 12:28 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-09 12:28 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-09 12:28 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-09 12:28 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-09 12:28 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-09 12:28 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-09 12:28 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-09 12:28 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-May-09 12:28 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1572 b- defN 24-May-09 12:28 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-09 12:28 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-09 12:28 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-09 12:28 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-09 12:28 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-09 12:28 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-09 12:28 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-09 12:28 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-09 12:28 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-09 12:28 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-09 12:28 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-09 12:28 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-09 12:28 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-09 12:28 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-09 12:28 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-09 12:28 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-09 12:28 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-09 12:28 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-May-09 12:28 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-09 12:28 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-May-09 12:28 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-09 12:28 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-09 12:28 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-09 12:28 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-09 12:28 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-May-09 12:28 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9470 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-May-09 12:28 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-09 12:28 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-09 12:28 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-09 12:28 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-09 12:28 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-09 12:28 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-09 12:28 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-09 12:28 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-09 12:28 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-09 12:28 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-09 12:28 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-09 12:28 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-09 12:28 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-09 12:28 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-09 12:28 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-09 12:28 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-09 12:28 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-09 12:28 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-09 12:28 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-09 12:28 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-09 12:28 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-09 12:28 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-09 12:28 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-09 12:28 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-09 12:28 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-09 12:28 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-09 12:28 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-09 12:28 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-09 12:28 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-09 12:28 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-09 12:28 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-09 12:28 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-09 12:28 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-09 12:28 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-09 12:28 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-09 12:28 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-09 12:28 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-09 12:28 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-09 12:28 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-09 12:28 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-09 12:28 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-09 12:28 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-09 12:28 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-09 12:28 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-09 12:28 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-09 12:28 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-09 12:28 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-09 12:28 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-09 12:28 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-09 12:28 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-09 12:28 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-09 12:28 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-09 12:28 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-09 12:28 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-09 12:28 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-09 12:28 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-09 12:28 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-09 12:28 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-09 12:28 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-09 12:28 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-09 12:28 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19495 b- defN 24-May-09 12:28 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-09 12:28 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-09 12:28 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-09 12:28 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-09 12:28 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-09 12:28 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-09 12:28 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-09 12:28 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6571 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18893 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10747 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30857 b- defN 24-May-09 12:28 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-09 12:28 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-09 12:28 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-09 12:28 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-09 12:28 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-09 12:28 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-09 12:28 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-09 12:28 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 12:28 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-09 12:28 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-09 12:28 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-09 12:28 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-09 12:28 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-09 12:28 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-09 12:28 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-09 12:28 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-09 12:28 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-09 12:28 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-09 12:28 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-09 12:28 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-09 12:28 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-09 12:28 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-09 12:28 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-09 12:28 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-09 12:28 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-09 12:28 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-09 12:28 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-09 12:28 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4399 b- defN 24-May-09 12:29 nucliadb-3.0.3.post488.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 12:29 nucliadb-3.0.3.post488.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-09 12:29 nucliadb-3.0.3.post488.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-09 12:29 nucliadb-3.0.3.post488.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-09 12:29 nucliadb-3.0.3.post488.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42669 b- defN 24-May-09 12:29 nucliadb-3.0.3.post488.dist-info/RECORD
+455 files, 2217313 bytes uncompressed, 682380 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -1341,26 +1341,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.0.3.post487.dist-info/METADATA
+Filename: nucliadb-3.0.3.post488.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.0.3.post487.dist-info/WHEEL
+Filename: nucliadb-3.0.3.post488.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.0.3.post487.dist-info/entry_points.txt
+Filename: nucliadb-3.0.3.post488.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post487.dist-info/top_level.txt
+Filename: nucliadb-3.0.3.post488.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post487.dist-info/zip-safe
+Filename: nucliadb-3.0.3.post488.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.0.3.post487.dist-info/RECORD
+Filename: nucliadb-3.0.3.post488.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/reader/api/v1/download.py

```diff
@@ -46,15 +46,15 @@
     FIELD = "field"
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/{{field_type}}/{{field_id}}/download/extracted/{{download_field:path}}",  # noqa
     tags=["Resource fields"],
     status_code=200,
-    name="Download extracted binary file (by slug)",
+    summary="Download extracted binary file (by slug)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_extract_file_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
@@ -67,15 +67,15 @@
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/{{field_type}}/{{field_id}}/download/extracted/{{download_field:path}}",  # noqa
     tags=["Resource fields"],
     status_code=200,
-    name="Download extracted binary file (by id)",
+    summary="Download extracted binary file (by id)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_extract_file_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
@@ -109,15 +109,15 @@
     return await download_api(sf, request.headers)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/file/{{field_id}}/download/field",
     tags=["Resource fields"],
     status_code=200,
-    name="Download field binary field (by slug)",
+    summary="Download field binary field (by slug)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_field_file_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
@@ -129,15 +129,15 @@
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/file/{{field_id}}/download/field",
     tags=["Resource fields"],
     status_code=200,
-    name="Download field binary field (by id)",
+    summary="Download field binary field (by id)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_field_file_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
@@ -164,15 +164,15 @@
     return await download_api(sf, request.headers, inline=inline)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/layout/{{field_id}}/download/field/{{download_field}}",
     tags=["Resource fields"],
     status_code=200,
-    name="Download layout binary field (by slug)",
+    summary="Download layout binary field (by slug)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_field_layout_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
@@ -184,15 +184,15 @@
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/layout/{{field_id}}/download/field/{{download_field}}",
     tags=["Resource fields"],
     status_code=200,
-    name="Download layout binary field (by id)",
+    summary="Download layout binary field (by id)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_field_layout_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
@@ -221,15 +221,15 @@
     return await download_api(sf, request.headers)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/conversation/{{field_id}}/download/field/{{message_id}}/{{file_num}}",  # noqa
     tags=["Resource fields"],
     status_code=200,
-    name="Download conversation binary field (by slug)",
+    summary="Download conversation binary field (by slug)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_field_conversation_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
@@ -242,15 +242,15 @@
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/conversation/{{field_id}}/download/field/{{message_id}}/{{file_num}}",  # noqa
     tags=["Resource fields"],
     status_code=200,
-    name="Download conversation binary field (by id)",
+    summary="Download conversation binary field (by id)",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def download_field_conversation_rid_prefix(
     request: Request,
     kbid: str,
     rid: str,
```

## nucliadb/reader/api/v1/export_import.py

```diff
@@ -37,15 +37,15 @@
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_utils.authentication import requires_one
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/export/{{export_id}}",
     status_code=200,
-    name="Download a Knowledge Box export",
+    summary="Download a Knowledge Box export",
     tags=["Knowledge Boxes"],
     response_class=StreamingResponse,
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.READER])
 @version(1)
 async def download_export_kb_endpoint(request: Request, kbid: str, export_id: str):
     context = get_app_context(request.app)
@@ -96,15 +96,15 @@
         yield chunk
     await dm.try_delete_from_storage("export", kbid, export_id)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/export/{{export_id}}/status",
     status_code=200,
-    name="Get the status of a Knowledge Box Export",
+    summary="Get the status of a Knowledge Box Export",
     response_model=StatusResponse,
     tags=["Knowledge Boxes"],
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.READER])
 @version(1)
 async def get_export_status_endpoint(
     request: Request, kbid: str, export_id: str
@@ -115,15 +115,15 @@
 
     return await _get_status(context, "export", kbid, export_id)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/import/{{import_id}}/status",
     status_code=200,
-    name="Get the status of a Knowledge Box Import",
+    summary="Get the status of a Knowledge Box Import",
     response_model=StatusResponse,
     tags=["Knowledge Boxes"],
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.READER])
 @version(1)
 async def get_import_status_endpoint(
     request: Request, kbid: str, import_id: str
```

## nucliadb/reader/api/v1/knowledgebox.py

```diff
@@ -33,15 +33,15 @@
 )
 from nucliadb_utils.authentication import requires, requires_one
 
 
 @api.get(
     f"/{KBS_PREFIX}",
     status_code=200,
-    name="List Knowledge Boxes",
+    summary="List Knowledge Boxes",
     response_model=KnowledgeBoxList,
     tags=["Knowledge Boxes"],
     include_in_schema=False,
 )
 @requires(NucliaDBRoles.MANAGER)
 @version(1)
 async def get_kbs(request: Request, prefix: str = "") -> KnowledgeBoxList:
@@ -52,15 +52,15 @@
             response.kbs.append(KnowledgeBoxObjSummary(slug=slug or None, uuid=kbid))  # type: ignore
         return response
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}",
     status_code=200,
-    name="Get Knowledge Box",
+    summary="Get Knowledge Box",
     response_model=KnowledgeBoxObj,
     tags=["Knowledge Boxes"],
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.READER])
 @version(1)
 async def get_kb(request: Request, kbid: str) -> KnowledgeBoxObj:
     driver = get_driver()
@@ -75,15 +75,15 @@
             config=KnowledgeBoxConfig.from_message(kb_config),
         )
 
 
 @api.get(
     f"/{KB_PREFIX}/s/{{slug}}",
     status_code=200,
-    name="Get Knowledge Box (by slug)",
+    summary="Get Knowledge Box (by slug)",
     response_model=KnowledgeBoxObj,
     tags=["Knowledge Boxes"],
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.READER])
 @version(1)
 async def get_kb_by_slug(request: Request, slug: str) -> KnowledgeBoxObj:
     driver = get_driver()
```

## nucliadb/reader/api/v1/learning_collector.py

```diff
@@ -25,15 +25,15 @@
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_utils.authentication import requires
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/feedback/{{month}}",
     status_code=200,
-    name="Download feedback of a Knowledge Box",
+    summary="Download feedback of a Knowledge Box",
     description="Download the feedback of a particular month in a Knowledge Box",  # noqa
     response_model=None,
     tags=["Knowledge Boxes"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def feedback_download(
@@ -45,15 +45,15 @@
         request, "GET", f"/collect/feedback/{kbid}/{month}"
     )
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/feedback",
     status_code=200,
-    name="Feedback avalaible months",
+    summary="Feedback avalaible months",
     description="List of months within the last year with feedback data",
     response_model=None,
     tags=["Knowledge Boxes"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def feedback_list_months(
```

## nucliadb/reader/api/v1/learning_config.py

```diff
@@ -27,15 +27,15 @@
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.settings import is_onprem_nucliadb
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/models/{{model_id}}/{{filename:path}}",
     status_code=200,
-    name="Download the Knowledege Box model",
+    summary="Download the Knowledege Box model",
     description="Download the trained model or any other generated file as a result of a training task on a Knowledge Box.",  # noqa
     response_model=None,
     tags=["Models"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def download_model(
@@ -48,15 +48,15 @@
         request, "GET", f"/download/{kbid}/model/{model_id}/{filename}"
     )
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/configuration",
     status_code=200,
-    name="Get Knowledge Box models configuration",
+    summary="Get Knowledge Box models configuration",
     description="Current configuration of models assigned to a Knowledge Box",
     response_model=None,
     tags=["Models"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_configuration(
@@ -70,15 +70,15 @@
         extra_headers={"X-STF-USER": request.headers.get("X-NUCLIADB-USER", "")},
     )
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/models",
     status_code=200,
-    name="Get available models",
+    summary="Get available models",
     description="Get available models",
     response_model=None,
     tags=["Models"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_models(
@@ -87,15 +87,15 @@
 ):
     return await learning_config_proxy(request, "GET", f"/models/{kbid}")
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/model/{{model_id}}",
     status_code=200,
-    name="Get model metadata",
+    summary="Get model metadata",
     description="Get metadata for a particular model",
     response_model=None,
     tags=["Models"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_model(
@@ -110,15 +110,15 @@
         extra_headers={"X-STF-USER": request.headers.get("X-NUCLIADB-USER", "")},
     )
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/schema",
     status_code=200,
-    name="Learning configuration schema",
+    summary="Learning configuration schema",
     description="Get jsonschema definition to update the `learning_configuration` of your Knowledge Box",
     response_model=None,
     tags=["Models"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_schema_for_configuration_updates(
@@ -127,15 +127,15 @@
 ):
     return await learning_config_proxy(request, "GET", f"/schema/{kbid}")
 
 
 @api.get(
     path=f"/nua/schema",
     status_code=200,
-    name="Learning configuration schema for Knowledge Box creation",
+    summary="Learning configuration schema for Knowledge Box creation",
     description="Get jsonschema definition for `learning_configuration` field for the Knowledge Box creation payload",
     response_model=None,
     tags=["Models"],
     include_in_schema=False,
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
```

## nucliadb/reader/api/v1/resource.py

```diff
@@ -137,15 +137,15 @@
         pagination=ResourcePagination(page=page, size=size, last=is_last_page),
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}",
     status_code=200,
-    name="Get Resource (by id)",
+    summary="Get Resource (by id)",
     response_model=Resource,
     response_model_exclude_unset=True,
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_resource_by_uuid(
@@ -177,15 +177,15 @@
         x_forwarded_for=x_forwarded_for,
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}",
     status_code=200,
-    name="Get Resource (by slug)",
+    summary="Get Resource (by slug)",
     response_model=Resource,
     response_model_exclude_unset=True,
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_resource_by_slug(
@@ -250,15 +250,15 @@
         raise HTTPException(status_code=404, detail="Resource does not exist")
     return result
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/{{field_type}}/{{field_id}}",
     status_code=200,
-    name="Get Resource field (by slug)",
+    summary="Get Resource field (by slug)",
     response_model=ResourceField,
     response_model_exclude_unset=True,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_resource_field_rslug_prefix(
@@ -290,15 +290,15 @@
         page=page,
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/{{field_type}}/{{field_id}}",
     status_code=200,
-    name="Get Resource field (by id)",
+    summary="Get Resource field (by id)",
     response_model=ResourceField,
     response_model_exclude_unset=True,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_resource_field_rid_prefix(
```

## nucliadb/reader/api/v1/services.py

```diff
@@ -60,15 +60,15 @@
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.utilities import get_ingest, get_storage
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroups",
     status_code=200,
-    name="Get Knowledge Box Entities",
+    summary="Get Knowledge Box Entities",
     response_model=KnowledgeBoxEntities,
     tags=["Knowledge Box Services"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_entities(
     request: Request, kbid: str, show_entities: bool = False
@@ -104,15 +104,15 @@
             status_code=500, detail="Error on listing Knowledge box entities"
         )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroup/{{group}}",
     status_code=200,
-    name="Get a Knowledge Box Entities Group",
+    summary="Get a Knowledge Box Entities Group",
     response_model=EntitiesGroup,
     tags=["Knowledge Box Services"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_entity(request: Request, kbid: str, group: str) -> EntitiesGroup:
     ingest = get_ingest()
@@ -137,15 +137,15 @@
             status_code=500, detail="Error on getting entities group on a Knowledge box"
         )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/labelsets",
     status_code=200,
-    name="Get Knowledge Box Label Sets",
+    summary="Get Knowledge Box Label Sets",
     response_model=KnowledgeBoxLabels,
     tags=["Knowledge Box Services"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_labelsets(request: Request, kbid: str) -> KnowledgeBoxLabels:
     ingest = get_ingest()
@@ -172,15 +172,15 @@
             status_code=500, detail="Error on getting Knowledge box labels"
         )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/labelset/{{labelset}}",
     status_code=200,
-    name="Get a Knowledge Box Label Set",
+    summary="Get a Knowledge Box Label Set",
     response_model=LabelSet,
     tags=["Knowledge Box Services"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_labelset(request: Request, kbid: str, labelset: str) -> LabelSet:
     ingest = get_ingest()
@@ -205,15 +205,15 @@
             status_code=500, detail="Error on getting labelset on a Knowledge box"
         )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=200,
-    name="Get Knowledge Box Custom Synonyms",
+    summary="Get Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     response_model=KnowledgeBoxSynonyms,
     openapi_extra={"x-operation_order": 2},
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def get_custom_synonyms(request: Request, kbid: str):
@@ -229,15 +229,15 @@
             status_code=500, detail="Error getting synonyms of a Knowledge box"
         )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/notifications",
     status_code=200,
-    name="Knowledge Box Notifications Stream",
+    summary="Knowledge Box Notifications Stream",
     description="Provides a stream of activity notifications for the given Knowledge Box. The stream will be automatically closed after 2 minutes.",  # noqa: E501
     tags=["Knowledge Box Services"],
     response_description="Each line of the response is a Base64-encoded JSON object representing a notification. Refer to [the internal documentation](https://github.com/nuclia/nucliadb/blob/main/docs/tutorials/KB_NOTIFICATIONS.md) for a more detailed explanation of each notification type.",  # noqa: E501
     response_model=None,
     responses={"404": {"description": "Knowledge Box not found"}},
 )
 @requires(NucliaDBRoles.READER)
@@ -269,15 +269,15 @@
     async with datamanagers.with_transaction(read_only=True) as txn:
         return await datamanagers.kb.exists_kb(txn, kbid=kbid)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/processing-status",
     status_code=200,
-    name="Knowledge Box Processing Status",
+    summary="Knowledge Box Processing Status",
     description="Provides the status of the processing of the given Knowledge Box.",
     tags=["Knowledge Box Services"],
     response_model=processing.RequestsResults,
     responses={
         "404": {"description": "Knowledge Box not found"},
     },
 )
```

## nucliadb/search/api/v1/chat.py

```diff
@@ -87,15 +87,14 @@
     ),
 }
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/chat",
     status_code=200,
-    name="Chat Knowledge Box",
     summary="Chat on a Knowledge Box",
     description="Chat on a Knowledge Box",
     tags=["Search"],
     response_model=None,
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
```

## nucliadb/search/api/v1/feedback.py

```diff
@@ -31,15 +31,15 @@
 from nucliadb_telemetry import errors
 from nucliadb_utils.authentication import requires
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/feedback",
     status_code=200,
-    name="Send Feedback",
+    summary="Send Feedback",
     description="Send feedback for a search operation in a Knowledge Box",
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def send_feedback_endpoint(
     request: Request,
```

## nucliadb/search/api/v1/find.py

```diff
@@ -59,15 +59,15 @@
     )
 }
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/find",
     status_code=200,
-    name="Find Knowledge Box",
+    summary="Find Knowledge Box",
     description="Find on a Knowledge Box",
     response_model=KnowledgeboxFindResults,
     response_model_exclude_unset=True,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
@@ -166,15 +166,15 @@
         response, kbid, item, x_ndb_client, x_nucliadb_user, x_forwarded_for
     )
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/find",
     status_code=200,
-    name="Find Knowledge Box",
+    summary="Find Knowledge Box",
     description="Find on a Knowledge Box",
     response_model=KnowledgeboxFindResults,
     response_model_exclude_unset=True,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
```

## nucliadb/search/api/v1/predict_proxy.py

```diff
@@ -35,23 +35,23 @@
 
 DESCRIPTION = "Convenience endpoint that proxies requests to the Predict API. It adds the Knowledge Box configuration settings as headers to the predict API request. Refer to the Predict API documentation for more details about the request and response models: https://docs.nuclia.dev/docs/nua-api#tag/Predict"  # noqa: E501
 
 
 @api.get(
     path=f"/{KB_PREFIX}/{{kbid}}/predict/{{endpoint}}",
     status_code=200,
-    name="Predict API Proxy",
+    summary="Predict API Proxy",
     description=DESCRIPTION,
     response_model=None,
     tags=["Search"],
 )
 @api.post(
     path=f"/{KB_PREFIX}/{{kbid}}/predict/{{endpoint}}",
     status_code=200,
-    name="Predict API Proxy",
+    summary="Predict API Proxy",
     description=DESCRIPTION,
     response_model=None,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def predict_proxy_endpoint(
```

## nucliadb/search/api/v1/search.py

```diff
@@ -83,15 +83,15 @@
     ),
 }
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/search",
     status_code=200,
-    name="Search Knowledge Box",
+    summary="Search Knowledge Box",
     description="Search on a Knowledge Box and retrieve separate results for documents, paragraphs, and sentences. Usually, it is better to use `find`",  # noqa: E501
     response_model=KnowledgeboxSearchResults,
     response_model_exclude_unset=True,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
@@ -202,15 +202,15 @@
         response, kbid, item, x_ndb_client, x_nucliadb_user, x_forwarded_for
     )
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/catalog",
     status_code=200,
-    name="List resources of a Knowledge Box",
+    summary="List resources of a Knowledge Box",
     description="List resources of a Knowledge Box",
     response_model=KnowledgeboxSearchResults,
     response_model_exclude_unset=True,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
@@ -246,15 +246,15 @@
         item.sort = SortOptions(field=sort_field, limit=sort_limit, order=sort_order)
     return await catalog(kbid, item)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/catalog",
     status_code=200,
-    name="List resources of a Knowledge Box",
+    summary="List resources of a Knowledge Box",
     description="List resources of a Knowledge Box",
     response_model=KnowledgeboxSearchResults,
     response_model_exclude_unset=True,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
@@ -342,15 +342,15 @@
     except LimitsExceededError as exc:
         return HTTPClientError(status_code=exc.status_code, detail=exc.detail)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/search",
     status_code=200,
-    name="Search Knowledge Box",
+    summary="Search Knowledge Box",
     description="Search on a Knowledge Box and retrieve separate results for documents, paragraphs, and sentences. Usually, it is better to use `find`",  # noqa: E501
     response_model=KnowledgeboxSearchResults,
     response_model_exclude_unset=True,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
```

## nucliadb/search/api/v1/suggest.py

```diff
@@ -43,14 +43,15 @@
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.utilities import get_audit
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/suggest",
     status_code=200,
+    summary="Suggest on a knowledge box",
     description="Suggestions on a knowledge box",
     response_model=KnowledgeboxSuggestResults,
     response_model_exclude_unset=True,
     tags=["Search"],
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
```

## nucliadb/search/api/v1/summarize.py

```diff
@@ -32,16 +32,15 @@
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.exceptions import LimitsExceededError
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/summarize",
     status_code=200,
-    name="Summarize Your Documents",
-    summary="Summarize Your Documents",
+    summary="Summarize your documents",
     description="Summarize Your Documents",
     tags=["Search"],
     response_model=SummarizedResponse,
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def summarize_endpoint(
```

## nucliadb/search/api/v1/resource/chat.py

```diff
@@ -38,16 +38,15 @@
 
 from ..chat import create_chat_response
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/resource/{{rid}}/chat",
     status_code=200,
-    name="Chat with a Resource (by id)",
-    summary="Chat with a resource",
+    summary="Chat with a resource (by id)",
     description="Chat with a resource",
     tags=["Search"],
     response_model=None,
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def resource_chat_endpoint_by_uuid(
@@ -75,16 +74,15 @@
         resource_id=rid,
     )
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_SLUG_PREFIX}/{{slug}}/chat",
     status_code=200,
-    name="Chat with a Resource (by slug)",
-    summary="Chat with a resource",
+    summary="Chat with a resource (by slug)",
     description="Chat with a resource",
     tags=["Search"],
     response_model=None,
 )
 @requires(NucliaDBRoles.READER)
 @version(1)
 async def resource_chat_endpoint_by_slug(
```

## nucliadb/search/api/v1/resource/search.py

```diff
@@ -43,16 +43,16 @@
 )
 from nucliadb_utils.authentication import requires_one
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/search",
     status_code=200,
-    name="Search on Resource",
-    description="Search on a Resource",
+    summary="Search on Resource",
+    description="Search on a single resource",
     tags=["Search"],
     response_model_exclude_unset=True,
     response_model=ResourceSearchResults,
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def resource_search(
```

## nucliadb/train/api/v1/check.py

```diff
@@ -28,15 +28,15 @@
 from nucliadb_utils.authentication import requires_one
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/check/labeler/{{labelset}}",
     tags=["Train"],
     status_code=200,
-    name="Return check status of labels",
+    summary="Return check status of labels",
     response_model=TrainSetPartitions,
 )
 @version(1)
 @requires_one([NucliaDBRoles.READER])
 async def check_labeler(
     request: Request, kbid: str, labelset: str
 ) -> TrainSetPartitions:
@@ -44,15 +44,15 @@
     return TrainSetPartitions(partitions=all_keys)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/check/ner/{{entitygroup}}",
     tags=["Train"],
     status_code=200,
-    name="Return check status of entities",
+    summary="Return check status of entities",
     response_model=TrainSetPartitions,
 )
 @version(1)
 @requires_one([NucliaDBRoles.READER])
 async def check_ner(
     request: Request, kbid: str, entitygroup: str
 ) -> TrainSetPartitions:
```

## nucliadb/train/api/v1/shards.py

```diff
@@ -30,15 +30,15 @@
 from nucliadb_utils.authentication import requires_one
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/trainset/{{shard}}",
     tags=["Object Response"],
     status_code=200,
-    name="Return Train Stream",
+    summary="Return Train Stream",
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def object_get_response(
     request: Request,
     kbid: str,
     shard: str,
```

## nucliadb/train/api/v1/trainset.py

```diff
@@ -30,28 +30,28 @@
 from nucliadb_utils.authentication import requires_one
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/trainset",
     tags=["Train"],
     status_code=200,
-    name="Return Train call",
+    summary="Return Train call",
     response_model=TrainSetPartitions,
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def get_partitions_all(request: Request, kbid: str) -> TrainSetPartitions:
     return await get_partitions(kbid)
 
 
 @api.get(
     f"/{KB_PREFIX}/{{kbid}}/trainset/{{prefix}}",
     tags=["Train"],
     status_code=200,
-    name="Return Train call",
+    summary="Return Train call",
     response_model=TrainSetPartitions,
 )
 @requires_one([NucliaDBRoles.READER])
 @version(1)
 async def get_partitions_prefix(
     request: Request, kbid: str, prefix: str
 ) -> TrainSetPartitions:
```

## nucliadb/writer/api/v1/export_import.py

```diff
@@ -50,15 +50,15 @@
 from nucliadb_telemetry import errors
 from nucliadb_utils.authentication import requires_one
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/export",
     status_code=200,
-    name="Start an export of a Knowledge Box",
+    summary="Start an export of a Knowledge Box",
     tags=["Knowledge Boxes"],
     response_model=CreateExportResponse,
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.WRITER])
 @version(1)
 async def start_kb_export_endpoint(request: Request, kbid: str):
     context = get_app_context(request.app)
@@ -75,15 +75,15 @@
         await start_export_task(context, kbid, export_id)
         return CreateExportResponse(export_id=export_id)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/import",
     status_code=200,
-    name="Start an import to a Knowledge Box",
+    summary="Start an import to a Knowledge Box",
     tags=["Knowledge Boxes"],
     response_model=CreateImportResponse,
 )
 @requires_one([NucliaDBRoles.MANAGER, NucliaDBRoles.WRITER])
 @version(1)
 async def start_kb_import_endpoint(request: Request, kbid: str):
     context = get_app_context(request.app)
```

## nucliadb/writer/api/v1/field.py

```diff
@@ -326,15 +326,15 @@
 
 # API endpoints
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/text/{{field_id}}",
     status_code=201,
-    name="Add resource text field (by slug)",
+    summary="Add resource text field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_text_rslug_prefix(
     request: Request,
@@ -347,15 +347,15 @@
         request, kbid, rslug, field_id, field_payload
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/text/{{field_id}}",
     status_code=201,
-    name="Add resource text field (by id)",
+    summary="Add resource text field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_text_rid_prefix(
     request: Request,
@@ -366,15 +366,15 @@
 ) -> ResourceFieldAdded:
     return await add_field_to_resource(request, kbid, rid, field_id, field_payload)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/link/{{field_id}}",
     status_code=201,
-    name="Add resource link field (by slug)",
+    summary="Add resource link field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_link_rslug_prefix(
     request: Request,
@@ -387,15 +387,15 @@
         request, kbid, rslug, field_id, field_payload
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/link/{{field_id}}",
     status_code=201,
-    name="Add resource link field (by id)",
+    summary="Add resource link field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_link_rid_prefix(
     request: Request,
@@ -406,15 +406,15 @@
 ) -> ResourceFieldAdded:
     return await add_field_to_resource(request, kbid, rid, field_id, field_payload)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/keywordset/{{field_id}}",
     status_code=201,
-    name="Add resource keywordset field (by slug)",
+    summary="Add resource keywordset field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_keywordset_rslug_prefix(
     request: Request,
@@ -427,15 +427,15 @@
         request, kbid, rslug, field_id, field_payload
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/keywordset/{{field_id}}",
     status_code=201,
-    name="Add resource keywordset field (by id)",
+    summary="Add resource keywordset field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_keywordset_rid_prefix(
     request: Request,
@@ -446,15 +446,15 @@
 ) -> ResourceFieldAdded:
     return await add_field_to_resource(request, kbid, rid, field_id, field_payload)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/datetime/{{field_id}}",
     status_code=201,
-    name="Add resource datetime field (by slug)",
+    summary="Add resource datetime field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_datetime_rslug_prefix(
     request: Request,
@@ -467,15 +467,15 @@
         request, kbid, rslug, field_id, field_payload
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/datetime/{{field_id}}",
     status_code=201,
-    name="Add resource datetime field (by id)",
+    summary="Add resource datetime field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_datetime_rid_prefix(
     request: Request,
@@ -486,15 +486,15 @@
 ) -> ResourceFieldAdded:
     return await add_field_to_resource(request, kbid, rid, field_id, field_payload)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/layout/{{field_id}}",
     status_code=201,
-    name="Add resource layout field (by slug)",
+    summary="Add resource layout field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_layout_rslug_prefix(
     request: Request,
@@ -507,15 +507,15 @@
         request, kbid, rslug, field_id, field_payload
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/layout/{{field_id}}",
     status_code=201,
-    name="Add resource layout field (by id)",
+    summary="Add resource layout field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_layout_rid_prefix(
     request: Request,
@@ -526,15 +526,15 @@
 ) -> ResourceFieldAdded:
     return await add_field_to_resource(request, kbid, rid, field_id, field_payload)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/conversation/{{field_id}}",
     status_code=201,
-    name="Add resource conversation field (by slug)",
+    summary="Add resource conversation field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_conversation_rslug_prefix(
     request: Request,
@@ -547,15 +547,15 @@
         request, kbid, rslug, field_id, field_payload
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/conversation/{{field_id}}",
     status_code=201,
-    name="Add resource conversation field (by id)",
+    summary="Add resource conversation field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_conversation_rid_prefix(
     request: Request,
@@ -566,15 +566,15 @@
 ) -> ResourceFieldAdded:
     return await add_field_to_resource(request, kbid, rid, field_id, field_payload)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/file/{{field_id}}",
     status_code=201,
-    name="Add resource file field (by slug)",
+    summary="Add resource file field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_file_rslug_prefix(
     request: Request,
@@ -588,15 +588,15 @@
         request, kbid, rslug, field_id, field_payload, skip_store=x_skip_store
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/file/{{field_id}}",
     status_code=201,
-    name="Add resource file field (by id)",
+    summary="Add resource file field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def add_resource_field_file_rid_prefix(
     request: Request,
@@ -610,15 +610,15 @@
         request, kbid, rid, field_id, field_payload, skip_store=x_skip_store
     )
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/conversation/{{field_id}}/messages",
     status_code=200,
-    name="Append messages to conversation field (by slug)",
+    summary="Append messages to conversation field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_messages_to_conversation_field_rslug_prefix(
     request: Request,
@@ -631,15 +631,15 @@
     field.messages.extend(messages)
     return await add_field_to_resource_by_slug(request, kbid, rslug, field_id, field)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/conversation/{{field_id}}/messages",
     status_code=200,
-    name="Append messages to conversation field (by id)",
+    summary="Append messages to conversation field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_messages_to_conversation_field_rid_prefix(
     request: Request,
@@ -652,15 +652,15 @@
     field.messages.extend(messages)
     return await add_field_to_resource(request, kbid, rid, field_id, field)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/layout/{{field_id}}/blocks",
     status_code=200,
-    name="Append blocks to layout field (by slug)",
+    summary="Append blocks to layout field (by slug)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_blocks_to_layout_field_rslug_prefix(
     request: Request,
@@ -673,15 +673,15 @@
     field.body.blocks.update(blocks)
     return await add_field_to_resource_by_slug(request, kbid, rslug, field_id, field)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/layout/{{field_id}}/blocks",
     status_code=200,
-    name="Append blocks to layout field (by id)",
+    summary="Append blocks to layout field (by id)",
     response_model=ResourceFieldAdded,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def append_blocks_to_layout_field_rid_prefix(
     request: Request,
@@ -694,15 +694,15 @@
     field.body.blocks.update(blocks)
     return await add_field_to_resource(request, kbid, rid, field_id, field)
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/{{field_type}}/{{field_id}}",
     status_code=204,
-    name="Delete Resource field (by slug)",
+    summary="Delete Resource field (by slug)",
     response_model_exclude_unset=True,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_resource_field_rslug_prefix(
     request: Request,
@@ -715,15 +715,15 @@
         request, kbid, rslug, field_type, field_id
     )
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/{{field_type}}/{{field_id}}",
     status_code=204,
-    name="Delete Resource field (by id)",
+    summary="Delete Resource field (by id)",
     response_model_exclude_unset=True,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_resource_field_rid_prefix(
     request: Request,
@@ -734,15 +734,15 @@
 ):
     return await delete_resource_field(request, kbid, rid, field_type, field_id)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/file/{{field_id}}/reprocess",
     status_code=202,
-    name="Reprocess file field (by id)",
+    summary="Reprocess file field (by id)",
     response_model=models.writer.ResourceUpdated,
     tags=["Resource fields"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def reprocess_file_field(
     request: Request,
```

## nucliadb/writer/api/v1/knowledgebox.py

```diff
@@ -44,15 +44,15 @@
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.utilities import get_ingest
 
 
 @api.post(
     f"/{KBS_PREFIX}",
     status_code=201,
-    name="Create Knowledge Box",
+    summary="Create Knowledge Box",
     response_model=KnowledgeBoxObj,
     tags=["Knowledge Boxes"],
     openapi_extra={"x-hidden-operation": True},
 )
 @requires(NucliaDBRoles.MANAGER)
 @version(1)
 async def create_kb(request: Request, item: KnowledgeBoxConfig):
@@ -86,15 +86,15 @@
         requestpb.learning_config = json.dumps(item.learning_configuration)
     return requestpb
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}",
     status_code=200,
-    name="Update Knowledge Box",
+    summary="Update Knowledge Box",
     response_model=KnowledgeBoxObjID,
     tags=["Knowledge Boxes"],
     openapi_extra={"x-hidden-operation": True},
 )
 @requires(NucliaDBRoles.MANAGER)
 @version(1)
 async def update_kb(request: Request, kbid: str, item: KnowledgeBoxConfig):
@@ -114,15 +114,15 @@
     elif kbobj.status == KnowledgeBoxResponseStatus.ERROR:
         raise HTTPException(status_code=500, detail="Error on creating knowledge box")
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}",
     status_code=200,
-    name="Delete Knowledge Box",
+    summary="Delete Knowledge Box",
     response_model=KnowledgeBoxObj,
     tags=["Knowledge Boxes"],
     openapi_extra={"x-hidden-operation": True},
 )
 @requires(NucliaDBRoles.MANAGER)
 @version(1)
 async def delete_kb(request: Request, kbid: str):
```

## nucliadb/writer/api/v1/learning_config.py

```diff
@@ -25,15 +25,15 @@
 from nucliadb_models.resource import NucliaDBRoles
 from nucliadb_utils.authentication import requires
 
 
 @api.post(
     path=f"/{KB_PREFIX}/{{kbid}}/configuration",
     status_code=204,
-    name="Create Knowledge Box models configuration",
+    summary="Create Knowledge Box models configuration",
     description="Create configuration of models assigned to a Knowledge Box",
     response_model=None,
     tags=["Knowledge Boxes"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def set_configuration(
@@ -42,15 +42,15 @@
 ):
     return await learning_config_proxy(request, "POST", f"/config/{kbid}")
 
 
 @api.patch(
     path=f"/{KB_PREFIX}/{{kbid}}/configuration",
     status_code=204,
-    name="Update Knowledge Box models configuration",
+    summary="Update Knowledge Box models configuration",
     description="Update current configuration of models assigned to a Knowledge Box",
     response_model=None,
     tags=["Knowledge Boxes"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def patch_configuration(
```

## nucliadb/writer/api/v1/resource.py

```diff
@@ -160,15 +160,15 @@
 
     return ResourceCreated(seqid=seqid, uuid=uuid, elapsed=txn_time)
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}",
     status_code=200,
-    name="Modify Resource (by slug)",
+    summary="Modify Resource (by slug)",
     response_model=ResourceUpdated,
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def modify_resource_rslug_prefix(
     request: Request,
@@ -188,15 +188,15 @@
         x_nucliadb_user=x_nucliadb_user,
     )
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}",
     status_code=200,
-    name="Modify Resource (by id)",
+    summary="Modify Resource (by id)",
     response_model=ResourceUpdated,
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def modify_resource_rid_prefix(
     request: Request,
@@ -355,15 +355,15 @@
         await txn.commit()
         return old_slug
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/reprocess",
     status_code=202,
-    name="Reprocess resource (by slug)",
+    summary="Reprocess resource (by slug)",
     response_model=ResourceUpdated,
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def reprocess_resource_rslug_prefix(
     request: Request,
@@ -376,15 +376,15 @@
         request, kbid, rid, x_nucliadb_user=x_nucliadb_user
     )
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/reprocess",
     status_code=202,
-    name="Reprocess resource (by id)",
+    summary="Reprocess resource (by id)",
     response_model=ResourceUpdated,
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def reprocess_resource_rid_prefix(
     request: Request,
@@ -452,15 +452,15 @@
 
     return ResourceUpdated(seqid=processing_info.seqid)
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}",
     status_code=204,
-    name="Delete Resource (by slug)",
+    summary="Delete Resource (by slug)",
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_resource_rslug_prefix(
     request: Request,
     kbid: str,
@@ -469,15 +469,15 @@
     rid = await get_rid_from_slug_or_raise_error(kbid, rslug)
     return await _delete_resource(request, kbid, rid)
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}",
     status_code=204,
-    name="Delete Resource (by id)",
+    summary="Delete Resource (by id)",
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_resource_rid_prefix(
     request: Request,
     kbid: str,
@@ -519,15 +519,15 @@
 
     return Response(status_code=204)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/reindex",
     status_code=204,
-    name="Reindex Resource (by slug)",
+    summary="Reindex Resource (by slug)",
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def reindex_resource_rslug_prefix(
     request: Request,
     kbid: str,
@@ -537,15 +537,15 @@
     rid = await get_rid_from_slug_or_raise_error(kbid, rslug)
     return await _reindex_resource(request, kbid, rid, reindex_vectors=reindex_vectors)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/reindex",
     status_code=204,
-    name="Reindex Resource (by id)",
+    summary="Reindex Resource (by id)",
     tags=["Resources"],
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def reindex_resource_rid_prefix(
     request: Request,
     kbid: str,
```

## nucliadb/writer/api/v1/services.py

```diff
@@ -51,15 +51,15 @@
 from nucliadb_utils.authentication import requires
 from nucliadb_utils.utilities import get_ingest
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroups",
     status_code=200,
-    name="Create Knowledge Box Entities Group",
+    summary="Create Knowledge Box Entities Group",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 1},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def create_entities_group(
     request: Request, kbid: str, item: CreateEntitiesGroupPayload
@@ -96,15 +96,15 @@
             detail="Error on settings entities on a Knowledge box"
         )
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroup/{{group}}",
     status_code=200,
-    name="Update Knowledge Box Entities Group",
+    summary="Update Knowledge Box Entities Group",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 2},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def update_entities_group(
     request: Request, kbid: str, group: str, item: UpdateEntitiesGroupPayload
@@ -143,15 +143,15 @@
             detail="Error on settings entities on a Knowledge box"
         )
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/entitiesgroup/{{group}}",
     status_code=200,
-    name="Delete Knowledge Box Entities",
+    summary="Delete Knowledge Box Entities",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 3},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_entities(request: Request, kbid: str, group: str):
     ingest = get_ingest()
@@ -171,15 +171,15 @@
 
     return Response(status_code=204)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/labelset/{{labelset}}",
     status_code=200,
-    name="Set Knowledge Box Labels",
+    summary="Set Knowledge Box Labels",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 1},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def set_labels(request: Request, kbid: str, labelset: str, item: LabelSet):
     ingest = get_ingest()
@@ -217,15 +217,15 @@
             status_code=500, detail="Error on settings labels on a Knowledge box"
         )
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/labelset/{{labelset}}",
     status_code=200,
-    name="Delete Knowledge Box Label",
+    summary="Delete Knowledge Box Label",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 3},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_labels(request: Request, kbid: str, labelset: str):
     ingest = get_ingest()
@@ -243,15 +243,15 @@
         )
     return Response(status_code=204)
 
 
 @api.put(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=204,
-    name="Set Knowledge Box Custom Synonyms",
+    summary="Set Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 1},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def set_custom_synonyms(request: Request, kbid: str, item: KnowledgeBoxSynonyms):
     ingest = get_ingest()
@@ -268,15 +268,15 @@
             status_code=500, detail="Error setting synonyms of a Knowledge box"
         )
 
 
 @api.delete(
     f"/{KB_PREFIX}/{{kbid}}/custom-synonyms",
     status_code=204,
-    name="Delete Knowledge Box Custom Synonyms",
+    summary="Delete Knowledge Box Custom Synonyms",
     tags=["Knowledge Box Services"],
     openapi_extra={"x-operation_order": 3},
 )
 @requires(NucliaDBRoles.WRITER)
 @version(1)
 async def delete_custom_synonyms(request: Request, kbid: str):
     ingest = get_ingest()
```

## nucliadb/writer/api/v1/upload.py

```diff
@@ -94,22 +94,22 @@
 @api.options(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}/{{upload_id}}",
     include_in_schema=False,
 )
 @api.options(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/file/{{field}}/{TUSUPLOAD}",
     tags=["Resource field TUS uploads"],
-    name="TUS Server information",
+    summary="TUS Server information",
     openapi_extra={"x-operation-order": 4},
     include_in_schema=False,
 )
 @api.options(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}",
     tags=["Knowledge Box TUS uploads"],
-    name="TUS Server information",
+    summary="TUS Server information",
     openapi_extra={"x-operation-order": 4},
 )
 @version(1)
 def tus_options(
     request: Request,
     kbid: str,
     rid: Optional[str] = None,
@@ -127,15 +127,15 @@
     resp = Response(headers=TUS_HEADERS, status_code=204)
     return resp
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/file/{{field}}/{TUSUPLOAD}",
     tags=["Resource field TUS uploads"],
-    name="Create new upload on a Resource (by slug)",
+    summary="Create new upload on a Resource (by slug)",
     openapi_extra={"x-operation-order": 1},
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_post_rslug_prefix(
     request: Request,
     kbid: str,
@@ -146,15 +146,15 @@
     rid = await get_rid_from_slug_or_raise_error(kbid, rslug)
     return await _tus_post(request, kbid, item, path_rid=rid, field_id=field)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{path_rid}}/file/{{field}}/{TUSUPLOAD}",
     tags=["Resource field TUS uploads"],
-    name="Create new upload on a Resource (by id)",
+    summary="Create new upload on a Resource (by id)",
     openapi_extra={"x-operation-order": 1},
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_post_rid_prefix(
     request: Request,
     kbid: str,
@@ -164,15 +164,15 @@
 ) -> Response:
     return await _tus_post(request, kbid, item, path_rid=path_rid, field_id=field)
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}",
     tags=["Knowledge Box TUS uploads"],
-    name="Create new upload on a Knowledge Box",
+    summary="Create new upload on a Knowledge Box",
     openapi_extra={"x-operation-order": 1},
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_post(
     request: Request,
     kbid: str,
@@ -301,14 +301,15 @@
 
 @api.head(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/file/{{field}}/{TUSUPLOAD}/{{upload_id}}",
     tags=["Resource field TUS uploads"],
     status_code=200,
     openapi_extra={"x-operation-order": 3},
     name="Upload information",
+    summary="Upload information",
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_head_rslug_prefix(
     request: Request,
     kbid: str,
     rslug: str,
@@ -320,14 +321,15 @@
 
 @api.head(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{path_rid}}/file/{{field}}/{TUSUPLOAD}/{{upload_id}}",
     tags=["Resource field TUS uploads"],
     status_code=200,
     openapi_extra={"x-operation-order": 3},
     name="Upload information",
+    summary="Upload information",
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_head_rid_prefix(
     request: Request,
     kbid: str,
     path_rid: str,
@@ -339,14 +341,15 @@
 
 @api.head(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}/{{upload_id}}",
     tags=["Knowledge Box TUS uploads"],
     status_code=200,
     openapi_extra={"x-operation-order": 3},
     name="Upload information",
+    summary="Upload information",
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def head(
     request: Request,
     kbid: str,
     upload_id: str,
@@ -375,15 +378,15 @@
     return Response(headers=tus_head_response)
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/file/{{field}}/{TUSUPLOAD}/{{upload_id}}",
     tags=["Resource field TUS uploads"],
     status_code=200,
-    name="Upload data on a Resource (by slug)",
+    summary="Upload data on a Resource (by slug)",
     openapi_extra={"x-operation-order": 2},
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_patch_rslug_prefix(
     request: Request,
     kbid: str,
@@ -395,15 +398,15 @@
     return await tus_patch(request, kbid, upload_id, rid=rid, field=field)
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{rid}}/file/{{field}}/{TUSUPLOAD}/{{upload_id}}",
     tags=["Resource field TUS uploads"],
     status_code=200,
-    name="Upload data on a Resource (by id)",
+    summary="Upload data on a Resource (by id)",
     openapi_extra={"x-operation-order": 2},
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def tus_patch_rid_prefix(
     request: Request,
     kbid: str,
@@ -414,15 +417,15 @@
     return await tus_patch(request, kbid, upload_id, rid=rid, field=field)
 
 
 @api.patch(
     f"/{KB_PREFIX}/{{kbid}}/{TUSUPLOAD}/{{upload_id}}",
     tags=["Knowledge Box TUS uploads"],
     status_code=200,
-    name="Upload data on a Knowledge Box",
+    summary="Upload data on a Knowledge Box",
     openapi_extra={"x-operation-order": 2},
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def patch(
     request: Request,
     kbid: str,
@@ -578,15 +581,15 @@
         )
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RSLUG_PREFIX}/{{rslug}}/file/{{field}}/{UPLOAD}",
     status_code=201,
     tags=["Resource fields"],
-    name="Upload binary file on a Resource (by slug)",
+    summary="Upload binary file on a Resource (by slug)",
     description="Upload a file as a field on an existing resource, if the field exists will return a conflict (419)",
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def upload_rslug_prefix(
     request: StarletteRequest,
     kbid: str,
@@ -610,15 +613,15 @@
     )
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{RESOURCE_PREFIX}/{{path_rid}}/file/{{field}}/{UPLOAD}",
     status_code=201,
     tags=["Resource fields"],
-    name="Upload binary file on a Resource (by id)",
+    summary="Upload binary file on a Resource (by id)",
     description="Upload a file as a field on an existing resource, if the field exists will return a conflict (419)",
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def upload_rid_prefix(
     request: StarletteRequest,
     kbid: str,
@@ -641,15 +644,15 @@
     )
 
 
 @api.post(
     f"/{KB_PREFIX}/{{kbid}}/{UPLOAD}",
     status_code=201,
     tags=["Knowledge Boxes"],
-    name="Upload binary file on a Knowledge Box",
+    summary="Upload binary file on a Knowledge Box",
     description="Upload a file onto a Knowledge Box, field id will be file and rid will be autogenerated. ",
 )
 @requires_one([NucliaDBRoles.WRITER])
 @version(1)
 async def upload(
     request: StarletteRequest,
     kbid: str,
```

## Comparing `nucliadb-3.0.3.post487.dist-info/METADATA` & `nucliadb-3.0.3.post488.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.0.3.post487
+Version: 3.0.3.post488
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post487
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post487
-Requires-Dist: nucliadb-protos >=3.0.3.post487
-Requires-Dist: nucliadb-models >=3.0.3.post487
+Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post488
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post488
+Requires-Dist: nucliadb-protos >=3.0.3.post488
+Requires-Dist: nucliadb-models >=3.0.3.post488
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.0.3.post487.dist-info/entry_points.txt` & `nucliadb-3.0.3.post488.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.0.3.post487.dist-info/RECORD` & `nucliadb-3.0.3.post488.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -174,22 +174,22 @@
 nucliadb/reader/app.py,sha256=dyvTCnVwXD3gVsk09tUB63N6hL-fS9q_S-AsI3zpFkk,3709
 nucliadb/reader/lifecycle.py,sha256=45NGAjNyi01Emi14Eh5GYBScS5N7yJbs2r1R2P-usSg,1366
 nucliadb/reader/openapi.py,sha256=ZwXYXZPYpxQL68HyWI310YnmMKJMzBUtYe-r9OSbN8I,1031
 nucliadb/reader/run.py,sha256=AR-iCnON3YVXgI5-KEgg99G4KAPN1BKXDg7nr4dgoDA,1447
 nucliadb/reader/api/__init__.py,sha256=c-UD29C0FVzQDGEvslebDCKtvnyEcAbiDd-3Q_QgGN4,872
 nucliadb/reader/api/models.py,sha256=QozP_WzNdacDy8GU0O89b2kIMDYbyG85fZyan8VJ81k,2434
 nucliadb/reader/api/v1/__init__.py,sha256=81AhxhYJcni8K_a5apWfL8Dnj4Mf_EznIsFse7jN-gQ,1110
-nucliadb/reader/api/v1/download.py,sha256=g4NwOO921Ok5WU6mYUYHRW0iK0p6rz6LttuMdMfGSs0,12368
-nucliadb/reader/api/v1/export_import.py,sha256=yybMDAaut_CPotTaiBGi52mMwQtx4V2UGPJEh-2ZYsg,6450
-nucliadb/reader/api/v1/knowledgebox.py,sha256=YeIxd6hAsTTerXqukvwm8N-2L6-FrMixrtAMw7JibLM,3632
-nucliadb/reader/api/v1/learning_collector.py,sha256=9K30TSYwsPJoAWynoJm5Yl3N7__QNy2T20Tw4jAvVpw,2093
-nucliadb/reader/api/v1/learning_config.py,sha256=vAZf1taIv3p_p48RJA9J1bPP1l4S1ALjXqrVWnlH42Q,4454
-nucliadb/reader/api/v1/resource.py,sha256=IFnuftz9F0eKIYs-73wA3LazHs4m58pbMoytyyrv-e0,13928
+nucliadb/reader/api/v1/download.py,sha256=ZO_KjjF9qM4K_xcEW7c1S0ZnieGkhv3Yu2E4kSU9F_s,12392
+nucliadb/reader/api/v1/export_import.py,sha256=nBYEwFnKUJYsiXUlbfKIL_jI9Ec5UVZE-2fCbK1rfQk,6459
+nucliadb/reader/api/v1/knowledgebox.py,sha256=Pd71iqTVRgx5u_Gb2LegDTQ3gGTKbVLsAvgcZne5_lM,3641
+nucliadb/reader/api/v1/learning_collector.py,sha256=6XDrfEZffqPrFYGj9TDfWOS1wcy3n9DRu35aH6-2WRA,2099
+nucliadb/reader/api/v1/learning_config.py,sha256=T1bxwsNDnVaeW9lkO4WTO9RHjz6GhYCJwvS1_MNYTes,4472
+nucliadb/reader/api/v1/resource.py,sha256=wYw9FlYGVisdq9kNrz_ck9gJDrhV6tIfIirXu43Y9ac,13940
 nucliadb/reader/api/v1/router.py,sha256=eyNmEGSP9zHkCIG5XlAXl6sukq950B7gFT3X2peMtIE,1011
-nucliadb/reader/api/v1/services.py,sha256=rZFk7rpWlhmh5EvOzf3XFGOVPl9RbJy9do8J464PTGs,12378
+nucliadb/reader/api/v1/services.py,sha256=PssrduMSIbZuSxPBYMIvjpQpzCWZ-lzFkdjlAGQHYwE,12399
 nucliadb/reader/reader/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/reader/notifications.py,sha256=cPpcnyHr9prcsGvkq4JwZqHjbTEkpXVcPWoYA4Up5fU,8155
 nucliadb/reader/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/reader/tests/conftest.py,sha256=RH5huJVfSZ9cQgzEWC_xViGbXUelZFuHmrOnWb-FpEU,1224
 nucliadb/reader/tests/fixtures.py,sha256=pVrolKyIQaUA01Coe8WHG6OuliqREnzq8DJnnfPF8_k,4345
 nucliadb/reader/tests/test_list_resources.py,sha256=yKsG6MLh4_cB7Yhov0OoBAVCJCXnpuQmT453R1oVQ6Q,2748
 nucliadb/reader/tests/test_reader_file_download.py,sha256=V_wLTRmSlYemSPLOBo3A_jhMBluro2sJiQwSsGGBx6I,10199
@@ -201,27 +201,27 @@
 nucliadb/search/openapi.py,sha256=t3Wo_4baTrfPftg2BHsyLWNZ1MYn7ZRdW7ht-wFOgRs,1016
 nucliadb/search/predict.py,sha256=SOzMErnplx-jDTdKya1hr4LKbQt956THyzN_vVc1iiY,17332
 nucliadb/search/run.py,sha256=aFb-CXRi_C8YMpP_ivNj8KW1BYhADj88y8K9Lr_nUPI,1402
 nucliadb/search/settings.py,sha256=Nm4BkdNNdYfU1wGvvWMvlazRSlRGoae99GEdm48-bXI,1193
 nucliadb/search/utilities.py,sha256=9SsRDw0rJVXVoLBfF7rBb6q080h-thZc7u8uRcTiBeY,1037
 nucliadb/search/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/api/v1/__init__.py,sha256=tusthakDVkeiAgU-eNjLsO183KXs8Js3fdPAF3JTXP0,1222
-nucliadb/search/api/v1/chat.py,sha256=dNaU4Cfkbta9-buRsPb98s1gsfvvzVCQIoYp2yvICmk,9913
-nucliadb/search/api/v1/feedback.py,sha256=j0PGSGDSbwwS5clRDbU_iCxuISFOtf2DN9Ey-fVGpso,2665
-nucliadb/search/api/v1/find.py,sha256=TvfV-KBUT52gpAgrWTtDOEkNTcKm69qma8mKl0p9mCQ,8804
+nucliadb/search/api/v1/chat.py,sha256=6rFou6kpEPiRBw0DTpDkrud8tYhpyfrOiAifmETSzp8,9882
+nucliadb/search/api/v1/feedback.py,sha256=SFXKzqgn31TDudUYPmp8845EBwLSJtWImG-7tTc9WQM,2668
+nucliadb/search/api/v1/find.py,sha256=oHfavVeX56ipsEiTUNVyBoFu-E5-dWwP_iyaHaUqz5c,8810
 nucliadb/search/api/v1/knowledgebox.py,sha256=hQ0wdBlHJVTwiRZgVCeNVwW_6f2bay88Hs9JMHgnx9M,6938
-nucliadb/search/api/v1/predict_proxy.py,sha256=2RME4enSpVXbNzboYQT1XhFFSgakDBgg3Wxj26mQglY,3041
+nucliadb/search/api/v1/predict_proxy.py,sha256=QrGzo0hKjtmyGZ6pjlJHYAh4hxwVUIOTcVcerRCw7eE,3047
 nucliadb/search/api/v1/router.py,sha256=mtT07rBZcVfpa49doaw9b1tj3sdi3qLH0gn9Io6NYM0,988
-nucliadb/search/api/v1/search.py,sha256=M3NQ7xZDeWsEWpfZyNnivHj7NNk11K4rbbziqhj8Ihs,18325
-nucliadb/search/api/v1/suggest.py,sha256=zGNB-vFgwYUjp9vxBYr5KB2ucJhhhZJqK85tOUO6z0w,5928
-nucliadb/search/api/v1/summarize.py,sha256=-hzveoztY3Qy68V5bCbX07McG5TKFzCerA27rYOQW7o,2536
+nucliadb/search/api/v1/search.py,sha256=GbCmp_WzG-wA8oVZkXGo9TwVLOHDBE2rhPWptHplje4,18337
+nucliadb/search/api/v1/suggest.py,sha256=3Mz34gxxTtyWG45CpfXQFJ54WS7cHUVwwz7oAtmtM28,5970
+nucliadb/search/api/v1/summarize.py,sha256=VAHJvE6V3xUgEBfqNKhgoxmDqCvh30RnrEIBVhMcNLU,2499
 nucliadb/search/api/v1/utils.py,sha256=yEAuvuPXjyhCQ-rOqGajCRDp0Y6UDH8uG6QWtK-tVuc,1433
 nucliadb/search/api/v1/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/search/api/v1/resource/chat.py,sha256=y3SIyr92oMQBrc5UKWsRLDFUCK3cgAKjxM0PBsNnu5Q,5887
-nucliadb/search/api/v1/resource/search.py,sha256=xIl_w70MpvC8Aqu89h4tXWNCZYaN9hxUUV04J1wK95w,5293
+nucliadb/search/api/v1/resource/chat.py,sha256=OaU3_yivCtdF2QLosGOiCngyzp4v4cCmbSMzCDxSpog,5821
+nucliadb/search/api/v1/resource/search.py,sha256=C6Do2x0dq0lUyUg67hFYxHMJ8xtaAtJj5yPnmrGTONo,5303
 nucliadb/search/requesters/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/search/requesters/utils.py,sha256=UbWLBSIuZETkG0OoDDkL4XjC2Zmc5wWfofdJPufXmdw,9070
 nucliadb/search/search/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/search/search/cache.py,sha256=86WwnknDYI00bd-kFf5MhN8TVFS2tfHzgobUHv_fAIA,2746
 nucliadb/search/search/exceptions.py,sha256=mbToQ-ghrv8ukLEv8S_-EZrgweWaIZZ5SIpoeuGDk6s,1154
 nucliadb/search/search/fetch.py,sha256=6S6s2s0JEP2QADDesbeN3XYPvTquMsTz9l0FKqQtSKU,5465
 nucliadb/search/search/filters.py,sha256=HpTpaDjKmUZWkp5xFFqKHz3TYdKEVBk4jWb2ssIYa5g,6513
@@ -363,18 +363,18 @@
 nucliadb/train/types.py,sha256=M3olA6vBosVs7L5QpzlxiFhuF3_vQhSkdlgClQzXjaQ,1496
 nucliadb/train/upload.py,sha256=Sz8KDXqFMD8reFw-8mb11il7Ab4onKcH0MPsZ1AbYUk,3265
 nucliadb/train/uploader.py,sha256=JEdZ6ozdFuKC_DmimljKnnH0gz2Nu-HxMFzjLa3gmkg,6420
 nucliadb/train/utils.py,sha256=Xoz7LjSWRfFNSHyZF-eK9DmWf9sgjyJXdYPppc3BE_c,3179
 nucliadb/train/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/train/api/utils.py,sha256=mvxHr3A3CCwvFXJyppm8KIi8yOwGxXhK-ADyDbZOuVo,1479
 nucliadb/train/api/v1/__init__.py,sha256=P4vCIv93r_Cq1WFDDNjy_Wg7zBkzx0S4euXwfPy1LA4,928
-nucliadb/train/api/v1/check.py,sha256=B6yGpZmYNghzWQEqu1Qoqk3bxC3jcKf2r91IEDeQXKc,2065
+nucliadb/train/api/v1/check.py,sha256=VLJRvkHG8fQGnIKu27tGTY1c7HBDrYQSn3tbIvnYmms,2071
 nucliadb/train/api/v1/router.py,sha256=ukdxn5q1oMar6NSPobgJczWsSxLCHw6DYKlb3zwCiSo,910
-nucliadb/train/api/v1/shards.py,sha256=EDV7fJkF-Elzpt0MSm-KxagzpAYks64Fr9NGW1vFdpM,1905
-nucliadb/train/api/v1/trainset.py,sha256=Iq-p9yppOfYcU687KOQQ7Dg6YY-g-YdCD3KI7UVrzeE,2129
+nucliadb/train/api/v1/shards.py,sha256=4osVrNisomtTOJqY96yqn80S-BFZxFVbuDldOHZ9Wwo,1908
+nucliadb/train/api/v1/trainset.py,sha256=4Ow8i4JJ6Hgm53bXjQZeYS6JcxD9vO0TLxu-DoMtQ0Y,2135
 nucliadb/train/generators/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/train/generators/field_classifier.py,sha256=YP_FvuXlouuLZ5aBnIUR0aXN5588ddEqXU7YkoJumAw,3723
 nucliadb/train/generators/image_classifier.py,sha256=M25BhLllbZXU6MQtQPfAQB9BegOZmv5AjezhQ5qWbo8,6712
 nucliadb/train/generators/paragraph_classifier.py,sha256=Vg4FMdB-1mkQdp5I5YgbDUFApNBW2fqotRp9cbuv_Xw,2789
 nucliadb/train/generators/paragraph_streaming.py,sha256=U4d_vL_sOloFIM95UgDsWZd6tqEiWluyMRqOiFRhWGY,3590
 nucliadb/train/generators/question_answer_streaming.py,sha256=ME-rKB02xZ2JNbNEaBz8oN09FaEN_zbTQS-oOl33J5c,5372
 nucliadb/train/generators/sentence_classifier.py,sha256=K1UBebwyPngDy4pWjxZ8tTZyOo3M5WlizBLJ0DPMP1s,5160
@@ -407,22 +407,22 @@
 nucliadb/writer/openapi.py,sha256=thqCO1ht_RJgOkXs-aIsv8aXJrU5z8wo2n05l2_LqMs,1032
 nucliadb/writer/run.py,sha256=euVZ_rtHDXs-O1kB-Pt1Id8eft9CYVpWH3zJzEoEqls,1448
 nucliadb/writer/settings.py,sha256=A1JY7pFQzLPV0Vm0TSG6jPBR3dEMK76SknbeANTG4Hg,3074
 nucliadb/writer/utilities.py,sha256=AZ5qEny1Xm0IDsFtH13oJa2usvJZK8f0FdgF1LrnLCw,1036
 nucliadb/writer/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/api/constants.py,sha256=b63uWvu7_bwg51R6EL5DaJwoT550Ih4GhVXzvEYLQNQ,1429
 nucliadb/writer/api/v1/__init__.py,sha256=FVn7N9VJ6bsEoy4TRnkclr4Umd5hECiwPXVqRnJ8BME,1095
-nucliadb/writer/api/v1/export_import.py,sha256=LrGg7y5Aq8xEnoYr529HG0g9LcF2UjP1VFpk9z1pJfE,6565
-nucliadb/writer/api/v1/field.py,sha256=mxZq2tRddGKD_ezKZU0ZdUI8wtLJFr6ND_C0hJFm9e8,24419
-nucliadb/writer/api/v1/knowledgebox.py,sha256=sFPPOsB2z-ljV51JP7oHMxUjejnJXMw93Pq8i-EMRkg,5239
-nucliadb/writer/api/v1/learning_config.py,sha256=GQN2d2N2IJLPX-S7hddTgrb7fDE8gCJ1MghgsIjBPKA,2052
-nucliadb/writer/api/v1/resource.py,sha256=Pk8ot63W191xQtq6ryYZZAEaZUr95H-cjOY7iupnqDA,18869
+nucliadb/writer/api/v1/export_import.py,sha256=SucHn2UX0hKRpfs_AYv8MNq-DPu1DIlSORd_K4N-cjk,6571
+nucliadb/writer/api/v1/field.py,sha256=Yi0F1IUin2TaQXyh9QDSwwzrqfjKw7nrAVbfnhl7z3o,24482
+nucliadb/writer/api/v1/knowledgebox.py,sha256=624Uv5_UHacWLv1p2YoMAR7oFPUlM9VgmiwsuJezqWk,5248
+nucliadb/writer/api/v1/learning_config.py,sha256=GaYaagjBrVG9ZxrWQyVQfqGMQV3tAJjqJ5CStaKhktU,2058
+nucliadb/writer/api/v1/resource.py,sha256=BBgRL4pQydm1arcsRCV-Y8FB1OBDggjQ9yZzxGVWivg,18893
 nucliadb/writer/api/v1/router.py,sha256=RjuoWLpZer6Kl2BW_wznpNo6XL3BOpdTGqXZCn3QrrQ,1034
-nucliadb/writer/api/v1/services.py,sha256=vzE0ABaPHBpczxqDuDwpcUIF4OyOKIVhWZMtYDPEAo0,10726
-nucliadb/writer/api/v1/upload.py,sha256=z8JYfT1qJvLMZ2JkZpZJk8nKvPQ9VhulX9FVqN4qiMU,30722
+nucliadb/writer/api/v1/services.py,sha256=jzgAck-Y9IsF8mSyPqFjV2TFqlt2Ccr9kn7tX5HuF7Q,10747
+nucliadb/writer/api/v1/upload.py,sha256=hkyXA_YlvH5j9jdf48rdmUuSf8T29hUXwBD0DNgLUP0,30857
 nucliadb/writer/layouts/__init__.py,sha256=Siod9W963CG5gJa20GSTw9VemAFgsMmJDbUspbrYAyE,1612
 nucliadb/writer/layouts/v1.py,sha256=Yc2idmfrpCS8js_XJByNWA_tmt2WeKoWvidLHoTPXoo,2115
 nucliadb/writer/resource/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/writer/resource/audit.py,sha256=SXPu_hdNBlm9uCSl666UQL7hzMx9zYVbBLT_U7ro8Gs,1425
 nucliadb/writer/resource/basic.py,sha256=eSWW6u6U3e0KjjdFwp9YQokojoDepl5vmJfbE2MQACM,10968
 nucliadb/writer/resource/field.py,sha256=7Y1vfuKDv1b3e7NCjEvDg8mktGR1rnzHaC5_qNj-3YQ,16319
 nucliadb/writer/resource/origin.py,sha256=3Y2zVtG_v0U6uMbDhW9Yl7KKHKt5V3T5_v3iCpqdBEk,2022
@@ -443,13 +443,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.0.3.post487.dist-info/METADATA,sha256=Er6MTvMP3RcSHCQoMT-NhgGe753hKK3ClOlk5UEq71o,4399
-nucliadb-3.0.3.post487.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.0.3.post487.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.0.3.post487.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.0.3.post487.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.0.3.post487.dist-info/RECORD,,
+nucliadb-3.0.3.post488.dist-info/METADATA,sha256=66J3_5UO-vtRcDjwr5U6V41OSi3U09jk8pARTWpZXE8,4399
+nucliadb-3.0.3.post488.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.0.3.post488.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.0.3.post488.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.0.3.post488.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.0.3.post488.dist-info/RECORD,,
```

