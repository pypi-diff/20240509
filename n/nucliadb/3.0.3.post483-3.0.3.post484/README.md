# Comparing `tmp/nucliadb-3.0.3.post483-py3-none-any.whl.zip` & `tmp/nucliadb-3.0.3.post484-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,455 +1,457 @@
-Zip file size: 748263 bytes, number of entries: 453
--rw-r--r--  2.0 unx     1135 b- defN 24-May-09 09:28 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-09 09:28 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-09 09:28 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-09 09:28 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-09 09:28 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-09 09:28 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-09 09:28 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-09 09:28 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-09 09:28 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-09 09:28 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-09 09:28 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-09 09:28 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-09 09:28 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-09 09:28 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-09 09:28 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-09 09:28 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-09 09:28 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-09 09:28 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-09 09:28 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-09 09:28 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-May-09 09:28 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-09 09:28 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-09 09:28 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 09:28 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-09 09:28 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4971 b- defN 24-May-09 09:28 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-09 09:28 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3790 b- defN 24-May-09 09:28 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-09 09:28 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    21584 b- defN 24-May-09 09:28 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8490 b- defN 24-May-09 09:28 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    19549 b- defN 24-May-09 09:28 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2713 b- defN 24-May-09 09:28 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5494 b- defN 24-May-09 09:28 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-09 09:28 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-May-09 09:28 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-09 09:28 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-09 09:28 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-09 09:28 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-09 09:28 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-May-09 09:28 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-09 09:28 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-09 09:28 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3386 b- defN 24-May-09 09:28 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3498 b- defN 24-May-09 09:28 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-09 09:28 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5633 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-09 09:28 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-09 09:28 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-09 09:28 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-09 09:28 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-09 09:28 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-09 09:28 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-09 09:28 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-09 09:28 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-09 09:28 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-09 09:28 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-09 09:28 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-09 09:28 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-May-09 09:28 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-09 09:28 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-09 09:28 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-09 09:28 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-09 09:28 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-09 09:28 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-09 09:28 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-09 09:28 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-09 09:28 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-09 09:28 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-09 09:28 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-09 09:28 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-09 09:28 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-May-09 09:28 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-09 09:28 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-May-09 09:28 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-09 09:28 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12159 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-09 09:28 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-May-09 09:28 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-09 09:28 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-09 09:28 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-09 09:28 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-09 09:28 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-09 09:28 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-09 09:28 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-09 09:28 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4531 b- defN 24-May-09 09:28 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-09 09:28 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28367 b- defN 24-May-09 09:28 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-09 09:28 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-09 09:28 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-May-09 09:28 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-09 09:28 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-May-09 09:28 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-May-09 09:28 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-09 09:28 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26423 b- defN 24-May-09 09:28 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-09 09:28 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-09 09:28 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33196 b- defN 24-May-09 09:28 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-09 09:28 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-09 09:28 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-09 09:28 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27325 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-09 09:28 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3981 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4075 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-09 09:28 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-09 09:28 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-09 09:28 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-09 09:28 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-09 09:28 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-09 09:28 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-09 09:28 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9237 b- defN 24-May-09 09:28 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-09 09:28 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-09 09:28 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-09 09:28 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-09 09:28 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-09 09:28 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-09 09:28 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-09 09:28 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-09 09:28 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-09 09:28 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-09 09:28 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-09 09:28 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-09 09:28 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-May-09 09:28 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12368 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6450 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3632 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2093 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4454 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13928 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12378 b- defN 24-May-09 09:28 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-May-09 09:28 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-09 09:28 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-09 09:28 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-09 09:28 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-09 09:28 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-09 09:28 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-09 09:28 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-09 09:28 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-09 09:28 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-09 09:28 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-09 09:28 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    17332 b- defN 24-May-09 09:28 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-09 09:28 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-09 09:28 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-09 09:28 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1222 b- defN 24-May-09 09:28 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 24-May-09 09:28 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2665 b- defN 24-May-09 09:28 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8804 b- defN 24-May-09 09:28 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-09 09:28 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3041 b- defN 24-May-09 09:28 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-09 09:28 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18325 b- defN 24-May-09 09:28 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5928 b- defN 24-May-09 09:28 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2536 b- defN 24-May-09 09:28 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1433 b- defN 24-May-09 09:28 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     5887 b- defN 24-May-09 09:28 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5293 b- defN 24-May-09 09:28 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9070 b- defN 24-May-09 09:28 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-09 09:28 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-09 09:28 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-09 09:28 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-09 09:28 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-09 09:28 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-09 09:28 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-09 09:28 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-09 09:28 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-09 09:28 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-09 09:28 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31127 b- defN 24-May-09 09:28 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-09 09:28 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-09 09:28 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-09 09:28 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-09 09:28 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-09 09:28 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    15347 b- defN 24-May-09 09:28 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-09 09:28 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-09 09:28 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-09 09:28 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    13101 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8567 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-09 09:28 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-09 09:28 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-09 09:28 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-09 09:28 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-May-09 09:28 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-May-09 09:28 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-09 09:28 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-09 09:28 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5336 b- defN 24-May-09 09:28 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-May-09 09:28 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-09 09:28 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-09 09:28 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-09 09:28 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-09 09:28 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-09 09:28 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-09 09:28 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-09 09:28 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-09 09:28 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-09 09:28 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1472 b- defN 24-May-09 09:28 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-09 09:28 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-09 09:28 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-09 09:28 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-09 09:28 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-09 09:28 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-09 09:28 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-09 09:28 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-09 09:28 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-09 09:28 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-09 09:28 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-09 09:28 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-09 09:28 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-09 09:28 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-09 09:28 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-09 09:28 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-09 09:28 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-09 09:28 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3625 b- defN 24-May-09 09:28 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-09 09:28 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2758 b- defN 24-May-09 09:28 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-09 09:28 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-09 09:28 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-09 09:28 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-09 09:28 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3656 b- defN 24-May-09 09:28 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    11955 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9470 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5584 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3750 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2114 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     2998 b- defN 24-May-09 09:28 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-09 09:28 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-09 09:28 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-09 09:28 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-09 09:28 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-09 09:28 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-09 09:28 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-09 09:28 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-09 09:28 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-09 09:28 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-09 09:28 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-09 09:28 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-09 09:28 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-09 09:28 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-09 09:28 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-09 09:28 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-09 09:28 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-09 09:28 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-09 09:28 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-09 09:28 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-09 09:28 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-09 09:28 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-09 09:28 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-09 09:28 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-09 09:28 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-09 09:28 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-09 09:28 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-09 09:28 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-09 09:28 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2065 b- defN 24-May-09 09:28 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-09 09:28 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1905 b- defN 24-May-09 09:28 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2129 b- defN 24-May-09 09:28 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-09 09:28 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-09 09:28 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-09 09:28 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-09 09:28 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-09 09:28 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-09 09:28 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-09 09:28 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-09 09:28 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-09 09:28 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-09 09:28 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-09 09:28 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-09 09:28 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-09 09:28 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-09 09:28 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-09 09:28 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-09 09:28 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-09 09:28 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-09 09:28 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-09 09:28 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-09 09:28 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-09 09:28 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-09 09:28 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-09 09:28 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-09 09:28 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-09 09:28 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-09 09:28 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-09 09:28 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-09 09:28 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19495 b- defN 24-May-09 09:28 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-09 09:28 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-09 09:28 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-09 09:28 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-09 09:28 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-May-09 09:28 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-09 09:28 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-09 09:28 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6565 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24419 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5239 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2052 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18869 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10726 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30722 b- defN 24-May-09 09:28 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-09 09:28 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-09 09:28 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-09 09:28 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-09 09:28 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-May-09 09:28 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-09 09:28 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-09 09:28 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:28 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-09 09:28 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-09 09:28 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-09 09:28 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-09 09:28 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-09 09:28 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-09 09:28 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-09 09:28 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-09 09:28 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-09 09:28 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-09 09:28 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-09 09:28 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-09 09:28 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-09 09:28 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-09 09:28 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-09 09:28 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-09 09:28 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-09 09:28 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-09 09:28 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-09 09:28 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4399 b- defN 24-May-09 09:29 nucliadb-3.0.3.post483.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 09:29 nucliadb-3.0.3.post483.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-09 09:29 nucliadb-3.0.3.post483.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-09 09:29 nucliadb-3.0.3.post483.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-09 09:29 nucliadb-3.0.3.post483.dist-info/zip-safe
--rw-rw-r--  2.0 unx    42473 b- defN 24-May-09 09:29 nucliadb-3.0.3.post483.dist-info/RECORD
-453 files, 2212385 bytes uncompressed, 680347 bytes compressed:  69.3%
+Zip file size: 750489 bytes, number of entries: 455
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-09 09:42 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-09 09:42 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-09 09:42 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-09 09:42 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-09 09:42 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-09 09:42 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-09 09:42 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-09 09:42 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-09 09:42 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-09 09:42 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-09 09:42 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-09 09:42 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-09 09:42 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-09 09:42 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-09 09:42 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-09 09:42 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-09 09:42 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-09 09:42 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-09 09:42 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-09 09:42 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-May-09 09:42 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-09 09:42 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-09 09:42 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 09:42 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5022 b- defN 24-May-09 09:42 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-May-09 09:42 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-09 09:42 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3790 b- defN 24-May-09 09:42 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-09 09:42 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    21584 b- defN 24-May-09 09:42 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8490 b- defN 24-May-09 09:42 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    19549 b- defN 24-May-09 09:42 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2713 b- defN 24-May-09 09:42 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5494 b- defN 24-May-09 09:42 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-09 09:42 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12518 b- defN 24-May-09 09:42 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-09 09:42 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-09 09:42 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-09 09:42 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-09 09:42 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-May-09 09:42 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-09 09:42 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-09 09:42 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-09 09:42 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-09 09:42 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-09 09:42 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5633 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-09 09:42 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-09 09:42 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-09 09:42 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-09 09:42 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-09 09:42 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-09 09:42 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-09 09:42 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-09 09:42 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-09 09:42 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-09 09:42 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-09 09:42 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-09 09:42 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-May-09 09:42 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-09 09:42 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-09 09:42 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-09 09:42 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-09 09:42 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-09 09:42 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-09 09:42 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-09 09:42 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-09 09:42 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-09 09:42 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-09 09:42 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-09 09:42 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-09 09:42 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-May-09 09:42 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-09 09:42 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-May-09 09:42 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-09 09:42 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12159 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-09 09:42 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-09 09:42 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-09 09:42 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-09 09:42 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-09 09:42 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-09 09:42 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-09 09:42 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-09 09:42 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-09 09:42 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4531 b- defN 24-May-09 09:42 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-09 09:42 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28367 b- defN 24-May-09 09:42 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-09 09:42 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-09 09:42 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17167 b- defN 24-May-09 09:42 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-09 09:42 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-09 09:42 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-May-09 09:42 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-09 09:42 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26423 b- defN 24-May-09 09:42 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-09 09:42 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-09 09:42 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    33196 b- defN 24-May-09 09:42 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-09 09:42 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-09 09:42 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-09 09:42 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27325 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-09 09:42 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3981 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4075 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-09 09:42 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-09 09:42 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-09 09:42 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-09 09:42 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-09 09:42 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-09 09:42 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-09 09:42 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9249 b- defN 24-May-09 09:42 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-09 09:42 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-09 09:42 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-09 09:42 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-09 09:42 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-09 09:42 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-09 09:42 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-09 09:42 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-09 09:42 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-09 09:42 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-09 09:42 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-09 09:42 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-09 09:42 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-May-09 09:42 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12368 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6450 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3632 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2093 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4454 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13928 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12378 b- defN 24-May-09 09:42 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-May-09 09:42 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-09 09:42 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-09 09:42 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-09 09:42 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-09 09:42 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-09 09:42 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-09 09:42 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-09 09:42 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-09 09:42 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-09 09:42 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-09 09:42 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    17332 b- defN 24-May-09 09:42 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-09 09:42 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-09 09:42 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-09 09:42 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1222 b- defN 24-May-09 09:42 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 24-May-09 09:42 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2665 b- defN 24-May-09 09:42 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8804 b- defN 24-May-09 09:42 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-09 09:42 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3041 b- defN 24-May-09 09:42 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-09 09:42 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18325 b- defN 24-May-09 09:42 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5928 b- defN 24-May-09 09:42 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2536 b- defN 24-May-09 09:42 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1433 b- defN 24-May-09 09:42 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     5887 b- defN 24-May-09 09:42 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5293 b- defN 24-May-09 09:42 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9070 b- defN 24-May-09 09:42 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-09 09:42 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-09 09:42 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-09 09:42 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-09 09:42 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-09 09:42 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-09 09:42 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-09 09:42 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-09 09:42 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-09 09:42 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-09 09:42 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31127 b- defN 24-May-09 09:42 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-09 09:42 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-09 09:42 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-09 09:42 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-09 09:42 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-09 09:42 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    15347 b- defN 24-May-09 09:42 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-09 09:42 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-09 09:42 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-09 09:42 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    13101 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8567 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-09 09:42 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-09 09:42 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-09 09:42 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-09 09:42 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-May-09 09:42 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-May-09 09:42 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-09 09:42 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1963 b- defN 24-May-09 09:42 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-09 09:42 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5415 b- defN 24-May-09 09:42 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-May-09 09:42 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-09 09:42 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-09 09:42 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-09 09:42 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-09 09:42 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-09 09:42 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-09 09:42 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-09 09:42 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-09 09:42 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-09 09:42 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-May-09 09:42 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1572 b- defN 24-May-09 09:42 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-09 09:42 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-09 09:42 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-09 09:42 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-09 09:42 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-09 09:42 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-09 09:42 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-09 09:42 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-09 09:42 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-09 09:42 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-09 09:42 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-09 09:42 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-09 09:42 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-09 09:42 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-09 09:42 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-09 09:42 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-09 09:42 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-09 09:42 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3625 b- defN 24-May-09 09:42 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-09 09:42 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2758 b- defN 24-May-09 09:42 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-09 09:42 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-09 09:42 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-09 09:42 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-09 09:42 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3656 b- defN 24-May-09 09:42 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    11955 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9470 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2114 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     2998 b- defN 24-May-09 09:42 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-09 09:42 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-09 09:42 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-09 09:42 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-09 09:42 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-09 09:42 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-09 09:42 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-09 09:42 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-09 09:42 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-09 09:42 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-09 09:42 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-09 09:42 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-09 09:42 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-09 09:42 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-09 09:42 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-09 09:42 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-09 09:42 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-09 09:42 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-09 09:42 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-09 09:42 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-09 09:42 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-09 09:42 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-09 09:42 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-09 09:42 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-09 09:42 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-09 09:42 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-09 09:42 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-09 09:42 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-09 09:42 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2065 b- defN 24-May-09 09:42 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-09 09:42 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1905 b- defN 24-May-09 09:42 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2129 b- defN 24-May-09 09:42 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-09 09:42 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-09 09:42 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-09 09:42 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-09 09:42 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-09 09:42 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-09 09:42 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-09 09:42 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-09 09:42 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-09 09:42 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-09 09:42 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-09 09:42 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-09 09:42 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-09 09:42 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-09 09:42 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-09 09:42 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-09 09:42 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-09 09:42 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-09 09:42 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-09 09:42 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-09 09:42 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-09 09:42 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-09 09:42 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-09 09:42 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-09 09:42 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-09 09:42 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-09 09:42 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-09 09:42 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-09 09:42 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19495 b- defN 24-May-09 09:42 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-09 09:42 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-09 09:42 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-09 09:42 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-09 09:42 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-09 09:42 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-09 09:42 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-09 09:42 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6565 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24419 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5239 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2052 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18869 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10726 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30722 b- defN 24-May-09 09:42 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-09 09:42 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-09 09:42 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-09 09:42 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-09 09:42 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-09 09:42 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-09 09:42 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-09 09:42 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-09 09:42 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-09 09:42 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-09 09:42 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-09 09:42 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-09 09:42 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-09 09:42 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-09 09:42 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-09 09:42 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-09 09:42 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-09 09:42 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-09 09:42 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-09 09:42 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-09 09:42 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-09 09:42 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-09 09:42 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-09 09:42 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-09 09:42 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-09 09:42 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-09 09:42 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-09 09:42 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4399 b- defN 24-May-09 09:43 nucliadb-3.0.3.post484.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 09:43 nucliadb-3.0.3.post484.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-09 09:43 nucliadb-3.0.3.post484.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-09 09:43 nucliadb-3.0.3.post484.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-09 09:43 nucliadb-3.0.3.post484.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    42669 b- defN 24-May-09 09:43 nucliadb-3.0.3.post484.dist-info/RECORD
+455 files, 2216798 bytes uncompressed, 682257 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -825,14 +825,17 @@
 
 Filename: nucliadb/standalone/introspect.py
 Comment: 
 
 Filename: nucliadb/standalone/lifecycle.py
 Comment: 
 
+Filename: nucliadb/standalone/migrations.py
+Comment: 
+
 Filename: nucliadb/standalone/purge.py
 Comment: 
 
 Filename: nucliadb/standalone/run.py
 Comment: 
 
 Filename: nucliadb/standalone/settings.py
@@ -867,14 +870,17 @@
 
 Filename: nucliadb/standalone/tests/unit/test_auth.py
 Comment: 
 
 Filename: nucliadb/standalone/tests/unit/test_introspect.py
 Comment: 
 
+Filename: nucliadb/standalone/tests/unit/test_migrations.py
+Comment: 
+
 Filename: nucliadb/standalone/tests/unit/test_run.py
 Comment: 
 
 Filename: nucliadb/standalone/tests/unit/test_versions.py
 Comment: 
 
 Filename: nucliadb/tasks/__init__.py
@@ -1335,26 +1341,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.0.3.post483.dist-info/METADATA
+Filename: nucliadb-3.0.3.post484.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.0.3.post483.dist-info/WHEEL
+Filename: nucliadb-3.0.3.post484.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.0.3.post483.dist-info/entry_points.txt
+Filename: nucliadb-3.0.3.post484.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post483.dist-info/top_level.txt
+Filename: nucliadb-3.0.3.post484.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.0.3.post483.dist-info/zip-safe
+Filename: nucliadb-3.0.3.post484.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.0.3.post483.dist-info/RECORD
+Filename: nucliadb-3.0.3.post484.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/locking.py

```diff
@@ -32,14 +32,15 @@
 from .maindb.utils import get_driver
 
 logger = logging.getLogger(__name__)
 
 NEW_SHARD_LOCK = "new-shard-{kbid}"
 RESOURCE_INDEX_LOCK = "resource-index-{kbid}-{resource_id}"
 KB_SHARDS_LOCK = "shards-kb-{kbid}"
+MIGRATIONS_LOCK = "migration"
 
 
 class ResourceLocked(Exception): ...
 
 
 @dataclass
 class LockValue:
@@ -120,25 +121,29 @@
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
         self.task.cancel()
         async with self.driver.transaction() as txn:
             await txn.delete(self.key)
             await txn.commit()
 
-    async def is_locked(self, key: str) -> bool:
+    async def is_locked(self) -> bool:
         async with get_driver().transaction(read_only=True) as txn:
             lock_data = await self.get_lock_data(txn)
-        return lock_data is None or time.time() > lock_data.expires_at
+        return lock_data is not None and time.time() < lock_data.expires_at
 
 
 def distributed_lock(
     key: str,
     lock_timeout: float = 60.0,  # max time to wait for lock
     expire_timeout: float = 30.0,  # how long by default the lock will be held without a refresh
     refresh_timeout: float = 10.0,  # how often to refresh
 ) -> _Lock:
     return _Lock(
         key,
         lock_timeout=lock_timeout,
         expire_timeout=expire_timeout,
         refresh_timeout=refresh_timeout,
     )
+
+
+async def is_locked(key: str) -> bool:
+    return await distributed_lock(key).is_locked()
```

## nucliadb/common/cluster/standalone/utils.py

```diff
@@ -91,7 +91,14 @@
 
 
 def is_index_node() -> bool:
     return cluster_settings.standalone_node_role in (
         StandaloneNodeRole.ALL,
         StandaloneNodeRole.INDEX,
     )
+
+
+def is_worker_node() -> bool:
+    return cluster_settings.standalone_node_role in (
+        StandaloneNodeRole.ALL,
+        StandaloneNodeRole.WORKER,
+    )
```

## nucliadb/common/context/__init__.py

```diff
@@ -26,25 +26,24 @@
 from nucliadb.common.maindb.utils import setup_driver, teardown_driver
 from nucliadb_utils.indexing import IndexingUtility
 from nucliadb_utils.nats import NatsConnectionManager
 from nucliadb_utils.partition import PartitionUtility
 from nucliadb_utils.settings import indexing_settings
 from nucliadb_utils.storages.storage import Storage
 from nucliadb_utils.utilities import (
-    Utility,
-    clean_utility,
     get_storage,
     start_indexing_utility,
     start_nats_manager,
     start_partitioning_utility,
     start_transaction_utility,
     stop_indexing_utility,
     stop_nats_manager,
     stop_partitioning_utility,
     stop_transaction_utility,
+    teardown_storage,
 )
 
 
 class ApplicationContext:
     kv_driver: Driver
     shard_manager: KBShardManager
     blob_storage: Storage
@@ -84,13 +83,13 @@
         if not self._initialized:
             return
 
         await stop_transaction_utility()
         if not in_standalone_mode():
             await stop_indexing_utility()
             await stop_nats_manager()
+
         stop_partitioning_utility()
         await teardown_cluster()
         await teardown_driver()
-        await self.blob_storage.finalize()
-        clean_utility(Utility.STORAGE)
+        await teardown_storage()
         self._initialized = False
```

## nucliadb/migrator/migrator.py

```diff
@@ -215,15 +215,15 @@
             failures += 1
 
     if failures > 0:
         raise Exception(f"Failed to migrate KBs. Failures: {failures}")
 
 
 async def run(context: ExecutionContext, target_version: Optional[int] = None) -> None:
-    async with locking.distributed_lock("migration"):
+    async with locking.distributed_lock(locking.MIGRATIONS_LOCK):
         # before we move to managed migrations, see if there are any rollovers
         # scheduled and run them
         await run_rollovers(context)
 
         # everything should be in a global lock
         # only 1 migration should be running at a time
         global_info = await context.data_manager.get_global_info()
```

## nucliadb/standalone/run.py

```diff
@@ -27,14 +27,15 @@
 import uvicorn  # type: ignore
 from fastapi import FastAPI
 
 from nucliadb.common.cluster.settings import settings as cluster_settings
 from nucliadb.ingest.settings import settings as ingest_settings
 from nucliadb.standalone import versions
 from nucliadb.standalone.config import config_nucliadb
+from nucliadb.standalone.migrations import run_migrations
 from nucliadb.standalone.settings import Settings
 from nucliadb_telemetry import errors
 from nucliadb_telemetry.fastapi import instrument_app
 from nucliadb_telemetry.logs import setup_logging
 from nucliadb_telemetry.settings import LogOutputType, LogSettings
 from nucliadb_utils.settings import nuclia_settings, storage_settings
 
@@ -76,14 +77,15 @@
     server.lifespan = config.lifespan_class(config)
 
     return application, server
 
 
 def run():
     settings = setup()
+    run_migrations()
     app, server = get_server(settings)
     instrument_app(app, excluded_urls=["/"], metrics=True)
 
     if settings.fork:  # pragma: no cover
         pid = os.fork()
         if pid != 0:
             sys.stdout.write(f"Server forked and running on pid {pid}.")
```

## nucliadb/standalone/tests/unit/test_run.py

```diff
@@ -20,23 +20,27 @@
 from unittest import mock
 
 import pytest
 
 from nucliadb.standalone.run import run, run_async_nucliadb
 from nucliadb.standalone.settings import Settings
 
+STANDALONE_RUN = "nucliadb.standalone.run"
+
 
 @pytest.fixture(scope="function", autouse=True)
 def mocked_deps():
     with mock.patch("uvicorn.Server.run"), mock.patch(
         "pydantic_argparse.ArgumentParser.parse_typed_args", return_value=Settings()
     ), mock.patch(
-        "nucliadb.standalone.run.get_latest_nucliadb", return_value="1.0.0"
+        f"{STANDALONE_RUN}.get_latest_nucliadb", return_value="1.0.0"
     ), mock.patch(
         "uvicorn.Server.startup"
+    ), mock.patch(
+        f"{STANDALONE_RUN}.run_migrations"
     ):
         yield
 
 
 def test_run():
     run()
```

## Comparing `nucliadb-3.0.3.post483.dist-info/METADATA` & `nucliadb-3.0.3.post484.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.0.3.post483
+Version: 3.0.3.post484
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
-Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post483
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post483
-Requires-Dist: nucliadb-protos >=3.0.3.post483
-Requires-Dist: nucliadb-models >=3.0.3.post483
+Requires-Dist: nucliadb-telemetry[all] >=3.0.3.post484
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.0.3.post484
+Requires-Dist: nucliadb-protos >=3.0.3.post484
+Requires-Dist: nucliadb-models >=3.0.3.post484
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.0.3.post483.dist-info/entry_points.txt` & `nucliadb-3.0.3.post484.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.0.3.post483.dist-info/RECORD` & `nucliadb-3.0.3.post484.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 nucliadb/__init__.py,sha256=_abCmDJ_0ku483Os4UAjPX7Nywm39cQgAV_DiyjsKeQ,891
 nucliadb/health.py,sha256=zPwd3CAFJf9owhbadtyGLvHekOjX9ykvxLYWYxnD5eo,3733
 nucliadb/learning_proxy.py,sha256=6r_fFgE662yEFgNpgGNxc3KTfFiR78yiEN95Qir6ctI,11626
 nucliadb/metrics_exporter.py,sha256=PummIqtRLdpcONPIpRKBj_jGYnX7B9XZ2IO048bu2pM,4806
 nucliadb/openapi.py,sha256=wDiw0dVEvTpJvbatkJ0JZLkKm9RItZT5PWRHjqRfqTA,2272
 nucliadb/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/common/locking.py,sha256=_168BClwNyXVentC7mk4_on0qof5G2y5VgTpOWvzJGk,4905
+nucliadb/common/locking.py,sha256=M9ODhLZUfCyrtx3qaCE7282L2Nkga1mcFUsXhh0cV50,5022
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/base.py,sha256=z_JD-xNVPB6-6O_u8YMpyOPP3fRmimwq7LbA3EGqDnE,4971
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=10OWSt-k2198cvaQtm12gjdsjyfjEY0laXcVcaz7gyc,3790
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
 nucliadb/common/cluster/manager.py,sha256=rs2nujx6_avXC4y_6zGlHw2g22NLO6MJzU9-9T6rHl0,21584
 nucliadb/common/cluster/rebalance.py,sha256=RC5Q9Uic0__QHeukd2ANlWyd6AYKBzRm3FXhvwcwxCo,8490
@@ -42,16 +42,16 @@
 nucliadb/common/cluster/discovery/single.py,sha256=2BhcencPKQQIfVitmTPJZm3TkBHyY9ZMcr-Clh8k2tM,1737
 nucliadb/common/cluster/discovery/types.py,sha256=vs-K790rofjZ4FWYaMkgjkZZqMvIvd_0eSw3shuiLwA,1139
 nucliadb/common/cluster/discovery/utils.py,sha256=A3DhpM3ExTSxtIo0Wh8ZIFARq2GW2OM1GPX967gyRbk,2548
 nucliadb/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/common/cluster/standalone/grpc_node_binding.py,sha256=52U0TCREO4CcCOC9ctrxmx6xno2M8t01QbI8MIcw3Qc,13707
 nucliadb/common/cluster/standalone/index_node.py,sha256=aKpkAEosp9qbd-77fYgE1AAnDc-6ER05cA_HJtkeBT0,4683
 nucliadb/common/cluster/standalone/service.py,sha256=tJI5Gc-cu4uprC84bcLQr4CMW0hBS9T2YX_Ex6zeyuI,3444
-nucliadb/common/cluster/standalone/utils.py,sha256=S5aSK18CVLCd7YR4CImEK9Skz7d_xSH63eQkHOYdHK8,3386
-nucliadb/common/context/__init__.py,sha256=DaiW_oYiAprzYWaabIJdQ3kh-b99fleHKC7Xg8CaqD0,3498
+nucliadb/common/cluster/standalone/utils.py,sha256=Y6Ni9P5piE9EeacQb4L5-o_TisAk2fl4btLwAV3tt8g,3545
+nucliadb/common/context/__init__.py,sha256=BuPPLOpTTzgD4oRb6mgmjPu-gRIaq4NeZTjx8FxAIV0,3440
 nucliadb/common/context/fastapi.py,sha256=qsxQ8s5dl67uCATrwdJCXA9JDfVn3DqxgsiWf6MUJhE,1628
 nucliadb/common/datamanagers/__init__.py,sha256=nr-HLFp_3u3SZeVYMvi5ew_VGGLYNO1cQWWAXfB9b1Y,1813
 nucliadb/common/datamanagers/cluster.py,sha256=Rc_gWufL-Fx3zQ7WlgCFYBPQD9fPjUvHkyW0QK6hBSg,1451
 nucliadb/common/datamanagers/entities.py,sha256=vQe_xdyqqsII0wmqKWp1yxVTFmB67Tc6bnVxezRUVK0,5383
 nucliadb/common/datamanagers/exceptions.py,sha256=Atz_PP_GGq4jgJaWcAkcRbHBoBaGcC9yJvFteylKtTE,883
 nucliadb/common/datamanagers/kb.py,sha256=zkG3lVbGFFLtjcTlJvJDtTY6S55xdty1nSlwI4xDEQ4,3994
 nucliadb/common/datamanagers/labels.py,sha256=2pN8RrFNTXLitDo44CS3AApjCjbv-2ALkqjwHVR_Mb0,5389
@@ -158,15 +158,15 @@
 nucliadb/middleware/__init__.py,sha256=knHBrVD30vfAWxn1RdRYEloSpIqakY3Ch9-NQzqKxk4,2216
 nucliadb/middleware/transaction.py,sha256=BjLGePAUnGAtpYIfv9lXKRFI1fB6lrseVeYzY-ckiFY,3912
 nucliadb/migrator/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/migrator/command.py,sha256=MgDruKOYpLuUMoO8aAE86vPflfOt7pAbW8QZQSZTFQQ,2119
 nucliadb/migrator/context.py,sha256=3h6M_AG2HFjTYtQC2XDmKps7wywdUduT1RM3C30S_S0,1334
 nucliadb/migrator/datamanager.py,sha256=5CLt1_fA3hXCBwUr1ltfmN3o69AzbweyiP42FkOqqV0,5104
 nucliadb/migrator/exceptions.py,sha256=jTj3YhKmFwUyjjgoKUNoCAiGrpEbB64X1Um212nSNQ8,889
-nucliadb/migrator/migrator.py,sha256=p1K-gNlzBnzxd73RtoI_qbvoDNJhoSZfd7VlDAA2wQI,9237
+nucliadb/migrator/migrator.py,sha256=SrR-Z_N5PuCTY6igPi-0hY9ZLfja4hNWLdza9_4OKqk,9249
 nucliadb/migrator/models.py,sha256=3PJkL2PGvKgIG0KIBv4H5XCsOVmwWMlRV3m0ntDj10Q,1145
 nucliadb/migrator/settings.py,sha256=_by-e5oYmaX4ZTOIQl4dJufJDv78fuUMwIj9RTe1APs,1110
 nucliadb/migrator/utils.py,sha256=7Y2zJZWB2qM0PcmS5G20g5EEwSdRVeHyR4_1wWNbl6Q,2346
 nucliadb/models/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/models/responses.py,sha256=qnuOoc7TrVSUnpikfTwHLKez47_DE4mSFzpxrwtqijA,1599
 nucliadb/purge/__init__.py,sha256=IHnoGcbASPUQ74ewbPtHiOnUbRXfB92-aDH4sUYALTQ,6041
 nucliadb/purge/orphan_shards.py,sha256=tGFlF7-RLDHv2XPc5J_1lgBvBCM5UjUtUNUmpodGqBc,9364
@@ -271,29 +271,31 @@
 nucliadb/standalone/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/standalone/api_router.py,sha256=DtB9uoMmT8NWjqZy-iEolHkM6sn-KzrykWVEmeTKM80,6746
 nucliadb/standalone/app.py,sha256=AVojB5tQE3K2I9hPxHgd06At2ofyclJti4JS1g5_Y5c,5763
 nucliadb/standalone/auth.py,sha256=bglXXYH7F3TWR5d8qrJq0VgVYb63mQCJJU4vQy8hMdQ,7800
 nucliadb/standalone/config.py,sha256=SPB6fWNda14nfF-lF0FYccyRLcytp9e24lQwDrA84EY,5309
 nucliadb/standalone/introspect.py,sha256=PMXk0krDHR3rUHVzeV1VImXxofyMckpTXVRYasWOqQw,6930
 nucliadb/standalone/lifecycle.py,sha256=6cCkiXwom7LppzKoG_vRuW5Ubw_YsLuVChHlCqnhts8,2488
+nucliadb/standalone/migrations.py,sha256=Hr0NskM67Va9MbrsKKd4ggV5V04LlwFuPAJxRDH61Eg,1963
 nucliadb/standalone/purge.py,sha256=1gMeKtQgwelwvGZBzAOpmqKmJBxaswJx2GG39BI50RU,1317
-nucliadb/standalone/run.py,sha256=F-qE5n7QDzgjtdBYIe6eSJe2Zi9a_GjHy2-NnFtFZZY,5336
+nucliadb/standalone/run.py,sha256=3ObfEos_e8XQCoqt2PdD2K56UwDVr4-4mR0QsFThipc,5415
 nucliadb/standalone/settings.py,sha256=_b-dXXOs6zFYyv00HMvYp33WNLFDRagL3uIkHZfT8ec,5781
 nucliadb/standalone/versions.py,sha256=uA_jIpdu4gPM04kPx6C8xNL9d-uaItlMjCxXNzQ_1_k,3132
 nucliadb/standalone/static/favicon.ico,sha256=96pKGp6Sx457JkTfjy1dtApMhkitixfU6invCUGAYOU,2285
 nucliadb/standalone/static/index.html,sha256=PEZfuEQFYnYACAL1ceN8xC0im8lBrUx838RkE8tbvgA,3833
 nucliadb/standalone/static/logo.svg,sha256=-wQqSvPGTdlKjUP6pHE6kiq005pgYjDzp9nPl0X71Mk,2639
 nucliadb/standalone/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/standalone/tests/conftest.py,sha256=8NudI1bKtRG7tEHn5uCFi_bwMk2xnSqch9C3avbRaQE,1294
 nucliadb/standalone/tests/fixtures.py,sha256=PH9M_13lVQT37hKZJ2WWO3Fws9eQPRA6jqVtMq_KfZk,1319
 nucliadb/standalone/tests/unit/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/standalone/tests/unit/test_api_router.py,sha256=PJcnBlx0RAQxeKL74GRfi9PXAYbgII1VFgu82iyiDZU,1722
 nucliadb/standalone/tests/unit/test_auth.py,sha256=xsP4bif-_ISvI9Ilm1kbYxFupz2vYm1lKmqAtJvUE8k,5509
 nucliadb/standalone/tests/unit/test_introspect.py,sha256=XGZG31RChB2VoGNmDZfa4icswSR8nAmN0jaxS_KJHNs,1334
-nucliadb/standalone/tests/unit/test_run.py,sha256=P9IJZZdSJ0EFrOdmirJnCnOdDvnR_P2vMWlleKcEb-w,1472
+nucliadb/standalone/tests/unit/test_migrations.py,sha256=p49E0hyHgkstq0AfnlxWxqRTd9MUvB-RvYUXEH2JVPM,1845
+nucliadb/standalone/tests/unit/test_run.py,sha256=TmZqjXZohZet2RhOseJ9-q3q3Ltz3ky-EpvuhyUIZVw,1572
 nucliadb/standalone/tests/unit/test_versions.py,sha256=E7a8zzhLOwnrCidmrf-F4GkagmRhh4eKsYpx7pN0glY,1972
 nucliadb/tasks/__init__.py,sha256=ie5S4LUZ3Pu16FKOva9CM3JLwHqT7g41y4n1-sJ_oB4,1037
 nucliadb/tasks/consumer.py,sha256=aEcQ70K1JoT5O-h_QcMw5psOVRVka7yQoXCW6h5w6Wo,7655
 nucliadb/tasks/logger.py,sha256=C7keOEO_mjLVp5VbqAZ2QXfqVB2Hot7NgBlUP_SDSMw,924
 nucliadb/tasks/models.py,sha256=hzbPqaq-SZUz4cTRSgIy0G8hBOYBaYBCNgH2KtLibVg,1378
 nucliadb/tasks/producer.py,sha256=CbJbZ2qHYoFRiy6ILPFMoMO7YmfYAYOWEnmKORjkFFQ,3457
 nucliadb/tasks/registry.py,sha256=tKvv_Py_O3peuLshq4bB3w197E33O7P7B63_6loLMrA,1753
@@ -441,13 +443,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.0.3.post483.dist-info/METADATA,sha256=AehVvBdtUoQvIOVEWcnBhkLJWfP89c1XqAhRETlDGL0,4399
-nucliadb-3.0.3.post483.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.0.3.post483.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.0.3.post483.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.0.3.post483.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.0.3.post483.dist-info/RECORD,,
+nucliadb-3.0.3.post484.dist-info/METADATA,sha256=f-pLGxPTP0LTV3Faw8bAZjgenWAaSQuwlGXcjPrjIuE,4399
+nucliadb-3.0.3.post484.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.0.3.post484.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.0.3.post484.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.0.3.post484.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.0.3.post484.dist-info/RECORD,,
```

