# Comparing `tmp/faststream-0.5.4.tar.gz` & `tmp/faststream-0.5.5.tar.gz`

## Comparing `faststream-0.5.4.tar` & `faststream-0.5.5.tar`

### file list

```diff
@@ -1,322 +1,322 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.4/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.4/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.4/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.4/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.4/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.4/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.4/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/annotations.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/security.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/__init__.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/types.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/message.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/security.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    18815 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    64951 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/message.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/parser.py
--rw-r--r--   0        0        0    20346 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/security.py
--rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    28954 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    71638 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   117854 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10959 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/message.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/parser.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/security.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/message.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/parser.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/security.py
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/testing/app.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.4/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.4/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.4/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.4/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.4/README.md
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 faststream-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 faststream-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.5/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.5/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.5/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.5/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.5/SECURITY.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.5/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.5/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/security.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/types.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    18973 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    65013 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    22297 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/security.py
+-rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    29045 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    72613 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   118913 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/message.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/security.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    27053 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    19596 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/message.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/security.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/testing/app.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.5/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.5/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.5/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.5/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.5/README.md
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 faststream-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 faststream-0.5.5/PKG-INFO
```

### Comparing `faststream-0.5.4/.pre-commit-config.yaml` & `faststream-0.5.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.secrets.baseline` & `faststream-0.5.5/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/CITATION.cff` & `faststream-0.5.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/CODE_OF_CONDUCT.md` & `faststream-0.5.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/CONTRIBUTING.md` & `faststream-0.5.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/SECURITY.md` & `faststream-0.5.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/dependabot.yml` & `faststream-0.5.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.5/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/codeql.yml` & `faststream-0.5.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/dependency-review.yaml` & `faststream-0.5.5/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/deploy-docs.yaml` & `faststream-0.5.5/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/publish_coverage.yml` & `faststream-0.5.5/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/publish_pypi.yml` & `faststream-0.5.5/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/test.yaml` & `faststream-0.5.5/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/.github/workflows/update_release_notes.yaml` & `faststream-0.5.5/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e02_1_basic_publisher.py` & `faststream-0.5.5/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e02_2_basic_publisher.py` & `faststream-0.5.5/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e02_3_basic_publisher.py` & `faststream-0.5.5/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e03_miltiple_pubsub.py` & `faststream-0.5.5/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e04_msg_filter.py` & `faststream-0.5.5/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e07_ack_immediately.py` & `faststream-0.5.5/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e09_testing_mocks.py` & `faststream-0.5.5/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e10_middlewares.py` & `faststream-0.5.5/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/e11_settings.py` & `faststream-0.5.5/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/fastapi_integration/testing.py` & `faststream-0.5.5/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/howto/structlogs.py` & `faststream-0.5.5/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/kafka/testing.py` & `faststream-0.5.5/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/nats/e03_publisher.py` & `faststream-0.5.5/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/nats/e04_js_basic.py` & `faststream-0.5.5/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/nats/e05_basic_and_js.py` & `faststream-0.5.5/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/nats/e06_key_value.py` & `faststream-0.5.5/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/nats/e07_object_storage.py` & `faststream-0.5.5/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/rabbit/direct.py` & `faststream-0.5.5/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/rabbit/fanout.py` & `faststream-0.5.5/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/rabbit/header.py` & `faststream-0.5.5/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/rabbit/topic.py` & `faststream-0.5.5/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/redis/channel_sub_pattern.py` & `faststream-0.5.5/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/redis/rpc.py` & `faststream-0.5.5/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/router/basic_publish.py` & `faststream-0.5.5/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/serialization/avro/avro.py` & `faststream-0.5.5/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/serialization/msgpack/pack.py` & `faststream-0.5.5/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.5/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/__init__.py` & `faststream-0.5.5/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/_compat.py` & `faststream-0.5.5/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/app.py` & `faststream-0.5.5/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/exceptions.py` & `faststream-0.5.5/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/security.py` & `faststream-0.5.5/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/types.py` & `faststream-0.5.5/faststream/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/abc.py` & `faststream-0.5.5/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/generate.py` & `faststream-0.5.5/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/message.py` & `faststream-0.5.5/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/proto.py` & `faststream-0.5.5/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/site.py` & `faststream-0.5.5/faststream/asyncapi/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 def serve_app(
     schema: "Schema",
     host: str,
     port: int,
 ) -> None:
     """Serve the HTTPServer with AsyncAPI schema."""
     logger.info(f"HTTPServer running on http://{host}:{port} (Press CTRL+C to quit)")
-    logger.warn("Please, do not use it in production.")
+    logger.warning("Please, do not use it in production.")
 
     server.HTTPServer(
         (host, port),
         partial(_Handler, schema=schema),
     ).serve_forever()
```

### Comparing `faststream-0.5.4/faststream/asyncapi/utils.py` & `faststream-0.5.5/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.5/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/channels.py` & `faststream-0.5.5/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/info.py` & `faststream-0.5.5/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/main.py` & `faststream-0.5.5/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/message.py` & `faststream-0.5.5/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/operations.py` & `faststream-0.5.5/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/security.py` & `faststream-0.5.5/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/servers.py` & `faststream-0.5.5/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/utils.py` & `faststream-0.5.5/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.5/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.5/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.5/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.5/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.5/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.5/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.5/faststream/broker/acknowledgement_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,43 +174,31 @@
         return not is_test_env()
 
     async def __ack(self) -> None:
         try:
             await self.message.ack(**self.extra_options)
         except Exception as er:
             if self.logger is not None:
-                self.logger.log(
-                    logging.ERROR,
-                    er,
-                    exc_info=er
-                )
+                self.logger.log(logging.ERROR, er, exc_info=er)
         else:
             self.watcher.remove(self.message.message_id)
 
     async def __nack(self) -> None:
         try:
             await self.message.nack(**self.extra_options)
         except Exception as er:
             if self.logger is not None:
-                self.logger.log(
-                    logging.ERROR,
-                    er,
-                    exc_info=er
-                )
+                self.logger.log(logging.ERROR, er, exc_info=er)
 
     async def __reject(self) -> None:
         try:
             await self.message.reject(**self.extra_options)
         except Exception as er:
             if self.logger is not None:
-                self.logger.log(
-                    logging.ERROR,
-                    er,
-                    exc_info=er
-                )
+                self.logger.log(logging.ERROR, er, exc_info=er)
         else:
             self.watcher.remove(self.message.message_id)
 
 
 def get_watcher(
     logger: Optional["LoggerProto"],
     try_number: Union[bool, int],
```

### Comparing `faststream-0.5.4/faststream/broker/message.py` & `faststream-0.5.5/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/router.py` & `faststream-0.5.5/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/schemas.py` & `faststream-0.5.5/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/types.py` & `faststream-0.5.5/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/utils.py` & `faststream-0.5.5/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/core/abc.py` & `faststream-0.5.5/faststream/broker/core/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/core/logging.py` & `faststream-0.5.5/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/core/usecase.py` & `faststream-0.5.5/faststream/broker/core/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/fastapi/context.py` & `faststream-0.5.5/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.5/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/fastapi/route.py` & `faststream-0.5.5/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/fastapi/router.py` & `faststream-0.5.5/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/middlewares/base.py` & `faststream-0.5.5/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/middlewares/logging.py` & `faststream-0.5.5/faststream/broker/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/publisher/fake.py` & `faststream-0.5.5/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/publisher/proto.py` & `faststream-0.5.5/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/publisher/usecase.py` & `faststream-0.5.5/faststream/broker/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/subscriber/call_item.py` & `faststream-0.5.5/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/subscriber/proto.py` & `faststream-0.5.5/faststream/broker/subscriber/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/subscriber/usecase.py` & `faststream-0.5.5/faststream/broker/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/wrapper/call.py` & `faststream-0.5.5/faststream/broker/wrapper/call.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/broker/wrapper/proto.py` & `faststream-0.5.5/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/main.py` & `faststream-0.5.5/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/docs/app.py` & `faststream-0.5.5/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/supervisors/basereload.py` & `faststream-0.5.5/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.5/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/supervisors/utils.py` & `faststream-0.5.5/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.5/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/utils/imports.py` & `faststream-0.5.5/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/utils/logs.py` & `faststream-0.5.5/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/cli/utils/parser.py` & `faststream-0.5.5/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/annotations.py` & `faststream-0.5.5/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/client.py` & `faststream-0.5.5/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/message.py` & `faststream-0.5.5/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/parser.py` & `faststream-0.5.5/faststream/confluent/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/router.py` & `faststream-0.5.5/faststream/confluent/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/security.py` & `faststream-0.5.5/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/testing.py` & `faststream-0.5.5/faststream/confluent/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
+from unittest.mock import AsyncMock, MagicMock
 
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
 from faststream.confluent.broker import KafkaBroker
 from faststream.confluent.publisher.asyncapi import AsyncAPIBatchPublisher
 from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
@@ -18,16 +19,21 @@
 __all__ = ("TestKafkaBroker",)
 
 
 class TestKafkaBroker(TestBroker[KafkaBroker]):
     """A class to test Kafka brokers."""
 
     @staticmethod
-    async def _fake_connect(broker: KafkaBroker, *args: Any, **kwargs: Any) -> None:
+    async def _fake_connect(  # type: ignore[override]
+        broker: KafkaBroker,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Callable[..., AsyncMock]:
         broker._producer = FakeProducer(broker)
+        return _fake_connection
 
     @staticmethod
     def create_publisher_fake_subscriber(
         broker: KafkaBroker,
         publisher: "AsyncAPIPublisher[Any]",
     ) -> "HandlerCallWrapper[Any, Any, Any]":
         sub = broker.subscriber(  # type: ignore[call-overload,misc]
@@ -227,7 +233,14 @@
         key=k,
         headers=[(i, j.encode()) for i, j in headers.items()],
         offset=0,
         partition=partition or 0,
         timestamp_type=0 + 1,
         timestamp_ms=timestamp_ms or int(datetime.now().timestamp()),
     )
+
+
+def _fake_connection(*args: Any, **kwargs: Any) -> AsyncMock:
+    mock = AsyncMock()
+    mock.getone.return_value = MagicMock()
+    mock.getmany.return_value = [MagicMock()]
+    return mock
```

### Comparing `faststream-0.5.4/faststream/confluent/broker/broker.py` & `faststream-0.5.5/faststream/confluent/broker/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 
 from typing_extensions import Annotated, Doc, override
 
 from faststream.__about__ import SERVICE_NAME
 from faststream.broker.message import gen_cor_id
 from faststream.confluent.broker.logging import KafkaLoggingBroker
 from faststream.confluent.broker.registrator import KafkaRegistrator
-from faststream.confluent.client import AsyncConfluentProducer, _missing
+from faststream.confluent.client import (
+    AsyncConfluentConsumer,
+    AsyncConfluentProducer,
+    _missing,
+)
 from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
 from faststream.confluent.schemas.params import ConsumerConnectionParams
 from faststream.confluent.security import parse_security
 from faststream.exceptions import NOT_CONNECTED_YET
 from faststream.utils.data import filter_by_dict
 
 if TYPE_CHECKING:
@@ -421,54 +425,60 @@
     async def connect(
         self,
         bootstrap_servers: Annotated[
             Union[str, Iterable[str], object],
             Doc("Kafka addresses to connect."),
         ] = Parameter.empty,
         **kwargs: Any,
-    ) -> ConsumerConnectionParams:
+    ) -> Callable[..., AsyncConfluentConsumer]:
         if bootstrap_servers is not Parameter.empty:
             kwargs["bootstrap_servers"] = bootstrap_servers
 
         return await super().connect(**kwargs)
 
     @override
     async def _connect(  # type: ignore[override]
         self,
         *,
         client_id: str,
         **kwargs: Any,
-    ) -> ConsumerConnectionParams:
+    ) -> Callable[..., AsyncConfluentConsumer]:
         security_params = parse_security(self.security)
         kwargs.update(security_params)
 
         producer = AsyncConfluentProducer(
             **kwargs,
             client_id=client_id,
         )
 
         self._producer = AsyncConfluentFastProducer(
             producer=producer,
         )
 
-        return filter_by_dict(ConsumerConnectionParams, kwargs)
+        return partial(
+            AsyncConfluentConsumer,
+            **filter_by_dict(ConsumerConnectionParams, kwargs),
+        )
 
     async def start(self) -> None:
         await super().start()
 
         for handler in self._subscribers.values():
             self._log(
                 f"`{handler.call_name}` waiting for messages",
                 extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @property
     def _subscriber_setup_extra(self) -> "AnyDict":
-        return {"client_id": self.client_id, "connection_data": self._connection or {}}
+        return {
+            "client_id": self.client_id,
+            "builder": self._connection,
+        }
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: "SendableMessage",
         topic: str,
         key: Optional[bytes] = None,
```

### Comparing `faststream-0.5.4/faststream/confluent/broker/logging.py` & `faststream-0.5.5/faststream/confluent/broker/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 from inspect import Parameter
-from typing import TYPE_CHECKING, Any, ClassVar, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Optional, Tuple, Union
 
 from faststream.broker.core.usecase import BrokerUsecase
-from faststream.confluent.schemas.params import ConsumerConnectionParams
+from faststream.confluent.client import AsyncConfluentConsumer
 from faststream.log.logging import get_broker_logger
 
 if TYPE_CHECKING:
     import confluent_kafka
 
     from faststream.types import LoggerProto
 
 
 class KafkaLoggingBroker(
     BrokerUsecase[
         Union["confluent_kafka.Message", Tuple["confluent_kafka.Message", ...]],
-        ConsumerConnectionParams,
+        Callable[..., AsyncConfluentConsumer],
     ]
 ):
     """A class that extends the LoggingMixin class and adds additional functionality for logging Kafka related information."""
 
     _max_topic_len: int
     _max_group_len: int
     __max_msg_id_ln: ClassVar[int] = 10
```

### Comparing `faststream-0.5.4/faststream/confluent/broker/registrator.py` & `faststream-0.5.5/faststream/confluent/broker/registrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from functools import partial
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Literal,
@@ -14,15 +13,14 @@
     overload,
 )
 
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
-from faststream.confluent.client import AsyncConfluentConsumer
 from faststream.confluent.publisher.asyncapi import AsyncAPIPublisher
 from faststream.confluent.subscriber.asyncapi import AsyncAPISubscriber
 from faststream.exceptions import SetupError
 
 if TYPE_CHECKING:
     from confluent_kafka import Message
     from fast_depends.dependencies import Depends
@@ -1231,45 +1229,42 @@
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
     ]:
         if not auto_commit and not group_id:
             raise SetupError("You should install `group_id` with manual commit mode")
 
-        builder = partial(
-            AsyncConfluentConsumer,
-            key_deserializer=key_deserializer,
-            value_deserializer=value_deserializer,
-            fetch_max_wait_ms=fetch_max_wait_ms,
-            fetch_max_bytes=fetch_max_bytes,
-            fetch_min_bytes=fetch_min_bytes,
-            max_partition_fetch_bytes=max_partition_fetch_bytes,
-            auto_offset_reset=auto_offset_reset,
-            enable_auto_commit=auto_commit,
-            auto_commit_interval_ms=auto_commit_interval_ms,
-            check_crcs=check_crcs,
-            partition_assignment_strategy=partition_assignment_strategy,
-            max_poll_interval_ms=max_poll_interval_ms,
-            rebalance_timeout_ms=rebalance_timeout_ms,
-            session_timeout_ms=session_timeout_ms,
-            heartbeat_interval_ms=heartbeat_interval_ms,
-            consumer_timeout_ms=consumer_timeout_ms,
-            max_poll_records=max_poll_records,
-            exclude_internal_topics=exclude_internal_topics,
-            isolation_level=isolation_level,
-        )
-
         subscriber = super().subscriber(
             AsyncAPISubscriber.create(
                 *topics,
                 batch=batch,
                 batch_timeout_ms=batch_timeout_ms,
                 max_records=max_records,
                 group_id=group_id,
-                builder=builder,
+                connection_data={
+                    "key_deserializer": key_deserializer,
+                    "value_deserializer": value_deserializer,
+                    "fetch_max_wait_ms": fetch_max_wait_ms,
+                    "fetch_max_bytes": fetch_max_bytes,
+                    "fetch_min_bytes": fetch_min_bytes,
+                    "max_partition_fetch_bytes": max_partition_fetch_bytes,
+                    "auto_offset_reset": auto_offset_reset,
+                    "enable_auto_commit": auto_commit,
+                    "auto_commit_interval_ms": auto_commit_interval_ms,
+                    "check_crcs": check_crcs,
+                    "partition_assignment_strategy": partition_assignment_strategy,
+                    "max_poll_interval_ms": max_poll_interval_ms,
+                    "rebalance_timeout_ms": rebalance_timeout_ms,
+                    "session_timeout_ms": session_timeout_ms,
+                    "heartbeat_interval_ms": heartbeat_interval_ms,
+                    "consumer_timeout_ms": consumer_timeout_ms,
+                    "max_poll_records": max_poll_records,
+                    "exclude_internal_topics": exclude_internal_topics,
+                    "isolation_level": isolation_level,
+                },
                 is_manual=not auto_commit,
                 # subscriber args
                 no_ack=no_ack,
                 retry=retry,
                 broker_middlewares=self._middlewares,
                 broker_dependencies=self._dependencies,
                 # AsyncAPI
```

### Comparing `faststream-0.5.4/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.5/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.5/faststream/confluent/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.5/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/publisher/producer.py` & `faststream-0.5.5/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/publisher/usecase.py` & `faststream-0.5.5/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/schemas/params.py` & `faststream-0.5.5/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.5/faststream/confluent/subscriber/asyncapi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import (
     TYPE_CHECKING,
-    Callable,
     Dict,
     Iterable,
     Literal,
     Optional,
     Tuple,
     Union,
     overload,
@@ -29,15 +28,15 @@
 )
 
 if TYPE_CHECKING:
     from confluent_kafka import Message as ConfluentMsg
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import BrokerMiddleware
-    from faststream.confluent.client import AsyncConfluentConsumer
+    from faststream.types import AnyDict
 
 
 class AsyncAPISubscriber(LogicSubscriber[MsgType]):
     """A class to handle logic and async API operations."""
 
     def get_name(self) -> str:
         return f'{",".join(self.topics)}:{self.call_name}'
@@ -73,15 +72,15 @@
     def create(
         *topics: str,
         batch: Literal[True],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AsyncConfluentConsumer"],
+        connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConfluentMsg, ...]]"],
         # AsyncAPI args
@@ -95,15 +94,15 @@
     def create(
         *topics: str,
         batch: Literal[False],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AsyncConfluentConsumer"],
+        connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[ConfluentMsg]"],
         # AsyncAPI args
@@ -117,15 +116,15 @@
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AsyncConfluentConsumer"],
+        connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable[
             "BrokerMiddleware[Union[ConfluentMsg, Tuple[ConfluentMsg, ...]]]"
@@ -144,15 +143,15 @@
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AsyncConfluentConsumer"],
+        connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable[
             "BrokerMiddleware[Union[ConfluentMsg, Tuple[ConfluentMsg, ...]]]"
@@ -167,29 +166,29 @@
     ]:
         if batch:
             return AsyncAPIBatchSubscriber(
                 *topics,
                 batch_timeout_ms=batch_timeout_ms,
                 max_records=max_records,
                 group_id=group_id,
-                builder=builder,
+                connection_data=connection_data,
                 is_manual=is_manual,
                 no_ack=no_ack,
                 retry=retry,
                 broker_dependencies=broker_dependencies,
                 broker_middlewares=broker_middlewares,
                 title_=title_,
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
         else:
             return AsyncAPIDefaultSubscriber(
                 *topics,
                 group_id=group_id,
-                builder=builder,
+                connection_data=connection_data,
                 is_manual=is_manual,
                 no_ack=no_ack,
                 retry=retry,
                 broker_dependencies=broker_dependencies,
                 broker_middlewares=broker_middlewares,
                 title_=title_,
                 description_=description_,
```

### Comparing `faststream-0.5.4/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.5/faststream/kafka/subscriber/usecase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,69 @@
 import asyncio
 from abc import ABC, abstractmethod
+from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
+    List,
     Optional,
     Sequence,
     Tuple,
 )
 
 import anyio
-from confluent_kafka import KafkaException, Message
+from aiokafka import TopicPartition
+from aiokafka.errors import ConsumerStoppedError, KafkaError
 from typing_extensions import override
 
 from faststream.broker.publisher.fake import FakePublisher
 from faststream.broker.subscriber.usecase import SubscriberUsecase
-from faststream.broker.types import MsgType
-from faststream.confluent.parser import AsyncConfluentParser
-from faststream.confluent.schemas.params import ConsumerConnectionParams
+from faststream.broker.types import (
+    AsyncCallable,
+    BrokerMiddleware,
+    CustomCallable,
+    MsgType,
+)
+from faststream.kafka.parser import AioKafkaParser
 
 if TYPE_CHECKING:
+    from aiokafka import AIOKafkaConsumer, ConsumerRecord
+    from aiokafka.abc import ConsumerRebalanceListener
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.publisher.proto import ProducerProto
-    from faststream.broker.types import (
-        AsyncCallable,
-        BrokerMiddleware,
-        CustomCallable,
-    )
-    from faststream.confluent.client import AsyncConfluentConsumer
     from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
     """A class to handle logic for consuming messages from Kafka."""
 
     topics: Sequence[str]
     group_id: Optional[str]
 
-    consumer: Optional["AsyncConfluentConsumer"]
+    builder: Optional[Callable[..., "AIOKafkaConsumer"]]
+    consumer: Optional["AIOKafkaConsumer"]
+
     task: Optional["asyncio.Task[None]"]
     client_id: Optional[str]
+    batch: bool
 
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AsyncConfluentConsumer"],
+        connection_args: "AnyDict",
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
+        partitions: Iterable["TopicPartition"],
         is_manual: bool,
         # Subscriber args
         default_parser: "AsyncCallable",
         default_decoder: "AsyncCallable",
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
@@ -74,31 +83,35 @@
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-        self.group_id = group_id
         self.topics = topics
+        self.partitions = partitions
+        self.group_id = group_id
+
         self.is_manual = is_manual
-        self.builder = builder
+        self.builder = None
         self.consumer = None
         self.task = None
 
         # Setup it later
         self.client_id = ""
-        self.__connection_data = ConsumerConnectionParams()
+        self.__pattern = pattern
+        self.__listener = listener
+        self.__connection_args = connection_args
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         client_id: Optional[str],
-        connection_data: "ConsumerConnectionParams",
+        builder: Callable[..., "AIOKafkaConsumer"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
         extra_context: Optional["AnyDict"],
         # broker options
         broker_parser: Optional["CustomCallable"],
@@ -106,40 +119,50 @@
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
         _call_decorators: Iterable["Decorator"],
     ) -> None:
         self.client_id = client_id
-        self.__connection_data = connection_data
+        self.builder = builder
 
         super().setup(
             logger=logger,
             producer=producer,
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
             _call_decorators=_call_decorators,
         )
 
-    @override
     async def start(self) -> None:
         """Start the consumer."""
+        assert self.builder, "You should setup subscriber at first."  # nosec B101
+
         self.consumer = consumer = self.builder(
-            *self.topics,
             group_id=self.group_id,
             client_id=self.client_id,
-            **self.__connection_data,
+            **self.__connection_args,
         )
-        await consumer.start()
 
+        if self.topics:
+            consumer.subscribe(
+                topics=self.topics,
+                pattern=self.__pattern,
+                listener=self.__listener,
+            )
+
+        elif self.partitions:
+            consumer.assign(partitions=self.partitions)
+
+        await consumer.start()
         await super().start()
 
         self.task = asyncio.create_task(self._consume())
 
     async def close(self) -> None:
         await super().close()
 
@@ -149,194 +172,224 @@
 
         if self.task is not None and not self.task.done():
             self.task.cancel()
 
         self.task = None
 
     def _make_response_publisher(
-        self, message: "StreamMessage[Any]"
+        self,
+        message: "StreamMessage[Any]",
     ) -> Sequence[FakePublisher]:
         if not message.reply_to or self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
                 publish_kwargs={
                     "topic": message.reply_to,
                 },
             ),
         )
 
     @abstractmethod
-    async def get_msg(self) -> Optional[MsgType]:
+    async def get_msg(self) -> MsgType:
         raise NotImplementedError()
 
     async def _consume(self) -> None:
-        assert self.consumer, "You need to start handler first"  # nosec B101
+        assert self.consumer, "You should start subscriber at first."  # nosec B101
 
         connected = True
         while self.running:
             try:
                 msg = await self.get_msg()
-            except KafkaException:  # pragma: no cover  # noqa: PERF203
+
+            # pragma: no cover
+            except KafkaError:  # noqa: PERF203
                 if connected:
                     connected = False
                 await anyio.sleep(5)
 
+            except ConsumerStoppedError:
+                return
+
             else:
                 if not connected:  # pragma: no cover
                     connected = True
 
-                if msg is not None:
-                    await self.consume(msg)  # type: ignore[arg-type]
+                if msg:
+                    await self.consume(msg)
 
     @staticmethod
-    def get_routing_hash(topics: Iterable[str], group_id: Optional[str] = None) -> int:
+    def get_routing_hash(
+        topics: Iterable[str],
+        group_id: Optional[str] = None,
+    ) -> int:
         return hash("".join((*topics, group_id or "")))
 
+    @property
+    def topic_names(self) -> List[str]:
+        if self.__pattern:
+            return [self.__pattern]
+        elif self.topics:
+            return list(self.topics)
+        else:
+            return [f"{p.topic}-{p.partition}" for p in self.partitions]
+
     def __hash__(self) -> int:
-        return self.get_routing_hash(self.topics, self.group_id)
+        return self.get_routing_hash(
+            topics=self.topic_names,
+            group_id=self.group_id,
+        )
 
     @staticmethod
     def build_log_context(
         message: Optional["StreamMessage[Any]"],
         topic: str,
         group_id: Optional[str] = None,
     ) -> Dict[str, str]:
         return {
             "topic": topic,
             "group_id": group_id or "",
             "message_id": getattr(message, "message_id", ""),
         }
 
+    def get_log_context(
+        self,
+        message: Optional["StreamMessage[ConsumerRecord]"],
+    ) -> Dict[str, str]:
+        if message is None:
+            topic = ",".join(self.topic_names)
+        elif isinstance(message.raw_message, Sequence):
+            topic = message.raw_message[0].topic
+        else:
+            topic = message.raw_message.topic
+
+        return self.build_log_context(
+            message=message,
+            topic=topic,
+            group_id=self.group_id,
+        )
+
     def add_prefix(self, prefix: str) -> None:
         self.topics = tuple("".join((prefix, t)) for t in self.topics)
 
+        self.partitions = [
+            TopicPartition(
+                topic="".join((prefix, p.topic)),
+                partition=p.partition,
+            )
+            for p in self.partitions
+        ]
+
 
-class DefaultSubscriber(LogicSubscriber[Message]):
+class DefaultSubscriber(LogicSubscriber["ConsumerRecord"]):
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AsyncConfluentConsumer"],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
+        connection_args: "AnyDict",
+        partitions: Iterable["TopicPartition"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[Message]"],
+        broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             *topics,
             group_id=group_id,
-            builder=builder,
+            listener=listener,
+            pattern=pattern,
+            connection_args=connection_args,
+            partitions=partitions,
             is_manual=is_manual,
             # subscriber args
-            default_parser=AsyncConfluentParser.parse_message,
-            default_decoder=AsyncConfluentParser.decode_message,
+            default_parser=AioKafkaParser.parse_message,
+            default_decoder=AioKafkaParser.decode_message,
             # Propagated args
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> Optional["Message"]:
+    async def get_msg(self) -> "ConsumerRecord":
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
         return await self.consumer.getone()
 
-    def get_log_context(
-        self,
-        message: Optional["StreamMessage[Message]"],
-    ) -> Dict[str, str]:
-        if message is None:
-            topic = ",".join(self.topics)
-        else:
-            topic = message.raw_message.topic() or ",".join(self.topics)
-
-        return self.build_log_context(
-            message=message,
-            topic=topic,
-            group_id=self.group_id,
-        )
 
-
-class BatchSubscriber(LogicSubscriber[Tuple[Message, ...]]):
+class BatchSubscriber(LogicSubscriber[Tuple["ConsumerRecord", ...]]):
     def __init__(
         self,
         *topics: str,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AsyncConfluentConsumer"],
+        listener: Optional["ConsumerRebalanceListener"],
+        pattern: Optional[str],
+        connection_args: "AnyDict",
+        partitions: Iterable["TopicPartition"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[Tuple[Message, ...]]"],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Sequence[Tuple[ConsumerRecord, ...]]]"
+        ],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         self.batch_timeout_ms = batch_timeout_ms
         self.max_records = max_records
 
         super().__init__(
             *topics,
             group_id=group_id,
-            builder=builder,
+            listener=listener,
+            pattern=pattern,
+            connection_args=connection_args,
+            partitions=partitions,
             is_manual=is_manual,
             # subscriber args
-            default_parser=AsyncConfluentParser.parse_message_batch,
-            default_decoder=AsyncConfluentParser.decode_message_batch,
+            default_parser=AioKafkaParser.parse_message_batch,
+            default_decoder=AioKafkaParser.decode_message_batch,
             # Propagated args
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> Optional[Tuple["Message", ...]]:
+    async def get_msg(self) -> Tuple["ConsumerRecord", ...]:
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
 
         messages = await self.consumer.getmany(
             timeout_ms=self.batch_timeout_ms,
             max_records=self.max_records,
         )
 
         if not messages:  # pragma: no cover
             await anyio.sleep(self.batch_timeout_ms / 1000)
-            return None
-
-        return messages
-
-    def get_log_context(
-        self,
-        message: Optional["StreamMessage[Tuple[Message, ...]]"],
-    ) -> Dict[str, str]:
-        if message is None:
-            topic = ",".join(self.topics)
-        else:
-            topic = message.raw_message[0].topic() or ",".join(self.topics)
+            return ()
 
-        return self.build_log_context(
-            message=message,
-            topic=topic,
-            group_id=self.group_id,
-        )
+        return tuple(chain(*messages.values()))
```

### Comparing `faststream-0.5.4/faststream/kafka/annotations.py` & `faststream-0.5.5/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/message.py` & `faststream-0.5.5/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/parser.py` & `faststream-0.5.5/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/router.py` & `faststream-0.5.5/faststream/kafka/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from typing_extensions import Annotated, Doc, deprecated
 
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
 from faststream.kafka.broker.registrator import KafkaRegistrator
 
 if TYPE_CHECKING:
-    from aiokafka import ConsumerRecord
+    from aiokafka import ConsumerRecord, TopicPartition
+    from aiokafka.abc import ConsumerRebalanceListener
     from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
         BrokerMiddleware,
         CustomCallable,
         Filter,
@@ -372,14 +373,52 @@
             else returns empty.
             """),
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
+        listener: Annotated[
+            Optional["ConsumerRebalanceListener"],
+            Doc("""
+            Optionally include listener
+               callback, which will be called before and after each rebalance
+               operation.
+               As part of group management, the consumer will keep track of
+               the list of consumers that belong to a particular group and
+               will trigger a rebalance operation if one of the following
+               events trigger:
+
+               * Number of partitions change for any of the subscribed topics
+               * Topic is created or deleted
+               * An existing member of the consumer group dies
+               * A new member is added to the consumer group
+
+               When any of these events are triggered, the provided listener
+               will be invoked first to indicate that the consumer's
+               assignment has been revoked, and then again when the new
+               assignment has been received. Note that this listener will
+               immediately override any listener set in a previous call
+               to subscribe. It is guaranteed, however, that the partitions
+               revoked/assigned
+               through this interface are from topics subscribed in this call.
+            """),
+        ] = None,
+        pattern: Annotated[
+            Optional[str],
+            Doc("""
+            Pattern to match available topics. You must provide either topics or pattern, but not both.
+            """),
+        ] = None,
+        partitions: Annotated[
+            Optional[Iterable["TopicPartition"]],
+            Doc("""
+            A topic and partition tuple. You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -452,14 +491,17 @@
             consumer_timeout_ms=consumer_timeout_ms,
             max_poll_records=max_poll_records,
             exclude_internal_topics=exclude_internal_topics,
             isolation_level=isolation_level,
             max_records=max_records,
             batch_timeout_ms=batch_timeout_ms,
             batch=batch,
+            listener=listener,
+            pattern=pattern,
+            partitions=partitions,
             # basic args
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             # AsyncAPI args
```

### Comparing `faststream-0.5.4/faststream/kafka/security.py` & `faststream-0.5.5/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/testing.py` & `faststream-0.5.5/faststream/kafka/testing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
+from unittest.mock import AsyncMock, MagicMock
 
 from aiokafka import ConsumerRecord
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
+from faststream.kafka import TopicPartition
 from faststream.kafka.broker import KafkaBroker
 from faststream.kafka.publisher.asyncapi import AsyncAPIBatchPublisher
 from faststream.kafka.publisher.producer import AioKafkaFastProducer
 from faststream.kafka.subscriber.asyncapi import AsyncAPIBatchSubscriber
 from faststream.testing.broker import TestBroker, call_handler
 
 if TYPE_CHECKING:
@@ -19,26 +21,38 @@
 __all__ = ("TestKafkaBroker",)
 
 
 class TestKafkaBroker(TestBroker[KafkaBroker]):
     """A class to test Kafka brokers."""
 
     @staticmethod
-    async def _fake_connect(broker: KafkaBroker, *args: Any, **kwargs: Any) -> None:
+    async def _fake_connect(  # type: ignore[override]
+        broker: KafkaBroker,
+        *args: Any,
+        **kwargs: Any,
+    ) -> Callable[..., AsyncMock]:
         broker._producer = FakeProducer(broker)
+        return _fake_connection
 
     @staticmethod
     def create_publisher_fake_subscriber(
         broker: KafkaBroker,
         publisher: "AsyncAPIPublisher[Any]",
     ) -> "HandlerCallWrapper[Any, Any, Any]":
-        sub = broker.subscriber(
-            publisher.topic,
-            batch=isinstance(publisher, AsyncAPIBatchPublisher),
-        )
+        if publisher.partition:
+            tp = TopicPartition(topic=publisher.topic, partition=publisher.partition)
+            sub = broker.subscriber(
+                partitions=[tp],
+                batch=isinstance(publisher, AsyncAPIBatchPublisher),
+            )
+        else:
+            sub = broker.subscriber(
+                publisher.topic,
+                batch=isinstance(publisher, AsyncAPIBatchPublisher),
+            )
 
         if not sub.calls:
 
             @sub  # type: ignore[misc]
             def f(msg: Any) -> None:
                 pass
 
@@ -88,15 +102,24 @@
             timestamp_ms=timestamp_ms,
             headers=headers,
             correlation_id=correlation_id,
             reply_to=reply_to,
         )
 
         for handler in self.broker._subscribers.values():  # pragma: no branch
-            if topic in handler.topics:
+            call: bool = False
+
+            for p in handler.partitions:
+                if p.topic == topic and (partition is None or p.partition == partition):
+                    call = True
+
+            if not call and topic in handler.topics:
+                call = True
+
+            if call:
                 return await call_handler(
                     handler=handler,
                     message=[incoming]
                     if isinstance(handler, AsyncAPIBatchSubscriber)
                     else incoming,
                     rpc=rpc,
                     rpc_timeout=rpc_timeout,
@@ -180,7 +203,14 @@
         key=k,
         serialized_key_size=len(k),
         serialized_value_size=len(msg),
         checksum=sum(msg),
         offset=0,
         headers=[(i, j.encode()) for i, j in headers.items()],
     )
+
+
+def _fake_connection(*args: Any, **kwargs: Any) -> AsyncMock:
+    mock = AsyncMock()
+    mock.subscribe = MagicMock
+    mock.assign = MagicMock
+    return mock
```

### Comparing `faststream-0.5.4/faststream/kafka/broker/broker.py` & `faststream-0.5.5/faststream/kafka/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,15 +553,15 @@
     async def connect(  # type: ignore[override]
         self,
         bootstrap_servers: Annotated[
             Union[str, Iterable[str], object],
             Doc("Kafka addresses to connect."),
         ] = Parameter.empty,
         **kwargs: "Unpack[KafkaInitKwargs]",
-    ) -> ConsumerConnectionParams:
+    ) -> Callable[..., aiokafka.AIOKafkaConsumer]:
         """Connect to Kafka servers manually.
 
         Consumes the same with `KafkaBroker.__init__` arguments and overrides them.
         To startup subscribers too you should use `broker.start()` after/instead this method.
         """
         if bootstrap_servers is not Parameter.empty:
             connect_kwargs: "AnyDict" = {
@@ -575,29 +575,32 @@
 
     @override
     async def _connect(  # type: ignore[override]
         self,
         *,
         client_id: str,
         **kwargs: Any,
-    ) -> ConsumerConnectionParams:
+    ) -> Callable[..., aiokafka.AIOKafkaConsumer]:
         security_params = parse_security(self.security)
         kwargs.update(security_params)
 
         producer = aiokafka.AIOKafkaProducer(
             **kwargs,
             client_id=client_id,
         )
 
         await producer.start()
         self._producer = AioKafkaFastProducer(
             producer=producer,
         )
 
-        return filter_by_dict(ConsumerConnectionParams, kwargs)
+        return partial(
+            aiokafka.AIOKafkaConsumer,
+            **filter_by_dict(ConsumerConnectionParams, kwargs),
+        )
 
     async def start(self) -> None:
         """Connect broker to Kafka and startup all subscribers."""
         await super().start()
 
         for handler in self._subscribers.values():
             self._log(
@@ -606,15 +609,15 @@
             )
             await handler.start()
 
     @property
     def _subscriber_setup_extra(self) -> "AnyDict":
         return {
             "client_id": self.client_id,
-            "connection_args": self._connection or {},
+            "builder": self._connection,
         }
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
             "SendableMessage",
```

### Comparing `faststream-0.5.4/faststream/kafka/broker/logging.py` & `faststream-0.5.5/faststream/kafka/broker/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import logging
 from inspect import Parameter
-from typing import TYPE_CHECKING, Any, ClassVar, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Optional, Tuple, Union
 
 from faststream.broker.core.usecase import BrokerUsecase
-from faststream.kafka.schemas.params import ConsumerConnectionParams
 from faststream.log.logging import get_broker_logger
 
 if TYPE_CHECKING:
     import aiokafka
 
     from faststream.types import LoggerProto
 
 
 class KafkaLoggingBroker(
     BrokerUsecase[
         Union["aiokafka.ConsumerRecord", Tuple["aiokafka.ConsumerRecord", ...]],
-        ConsumerConnectionParams,
+        Callable[..., "aiokafka.AIOKafkaConsumer"],
     ]
 ):
     """A class that extends the LoggingMixin class and adds additional functionality for logging Kafka related information."""
 
     _max_topic_len: int
     _max_group_len: int
     __max_msg_id_ln: ClassVar[int] = 10
```

### Comparing `faststream-0.5.4/faststream/kafka/broker/registrator.py` & `faststream-0.5.5/faststream/kafka/broker/registrator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from functools import partial
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Literal,
@@ -10,26 +9,25 @@
     Sequence,
     Tuple,
     Union,
     cast,
     overload,
 )
 
-from aiokafka import AIOKafkaConsumer, ConsumerRecord
+from aiokafka import ConsumerRecord
 from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
-from faststream.exceptions import SetupError
 from faststream.kafka.publisher.asyncapi import AsyncAPIPublisher
 from faststream.kafka.subscriber.asyncapi import AsyncAPISubscriber
 
 if TYPE_CHECKING:
-    from aiokafka import ConsumerRecord
+    from aiokafka import ConsumerRecord, TopicPartition
     from aiokafka.abc import ConsumerRebalanceListener
     from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
     from fast_depends.dependencies import Depends
 
     from faststream.broker.types import (
         CustomCallable,
         Filter,
@@ -332,14 +330,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -656,14 +661,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -980,14 +992,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1307,14 +1326,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1363,50 +1389,45 @@
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
     ]:
-        if not auto_commit and not group_id:
-            raise SetupError("You should install `group_id` with manual commit mode")
-
-        builder = partial(
-            AIOKafkaConsumer,
-            key_deserializer=key_deserializer,
-            value_deserializer=value_deserializer,
-            fetch_max_wait_ms=fetch_max_wait_ms,
-            fetch_max_bytes=fetch_max_bytes,
-            fetch_min_bytes=fetch_min_bytes,
-            max_partition_fetch_bytes=max_partition_fetch_bytes,
-            auto_offset_reset=auto_offset_reset,
-            enable_auto_commit=auto_commit,
-            auto_commit_interval_ms=auto_commit_interval_ms,
-            check_crcs=check_crcs,
-            partition_assignment_strategy=partition_assignment_strategy,
-            max_poll_interval_ms=max_poll_interval_ms,
-            rebalance_timeout_ms=rebalance_timeout_ms,
-            session_timeout_ms=session_timeout_ms,
-            heartbeat_interval_ms=heartbeat_interval_ms,
-            consumer_timeout_ms=consumer_timeout_ms,
-            max_poll_records=max_poll_records,
-            exclude_internal_topics=exclude_internal_topics,
-            isolation_level=isolation_level,
-        )
-
         subscriber = super().subscriber(
             AsyncAPISubscriber.create(
                 *topics,
                 batch=batch,
                 batch_timeout_ms=batch_timeout_ms,
                 max_records=max_records,
                 group_id=group_id,
                 listener=listener,
                 pattern=pattern,
-                builder=builder,
+                connection_args={
+                    "key_deserializer": key_deserializer,
+                    "value_deserializer": value_deserializer,
+                    "fetch_max_wait_ms": fetch_max_wait_ms,
+                    "fetch_max_bytes": fetch_max_bytes,
+                    "fetch_min_bytes": fetch_min_bytes,
+                    "max_partition_fetch_bytes": max_partition_fetch_bytes,
+                    "auto_offset_reset": auto_offset_reset,
+                    "enable_auto_commit": auto_commit,
+                    "auto_commit_interval_ms": auto_commit_interval_ms,
+                    "check_crcs": check_crcs,
+                    "partition_assignment_strategy": partition_assignment_strategy,
+                    "max_poll_interval_ms": max_poll_interval_ms,
+                    "rebalance_timeout_ms": rebalance_timeout_ms,
+                    "session_timeout_ms": session_timeout_ms,
+                    "heartbeat_interval_ms": heartbeat_interval_ms,
+                    "consumer_timeout_ms": consumer_timeout_ms,
+                    "max_poll_records": max_poll_records,
+                    "exclude_internal_topics": exclude_internal_topics,
+                    "isolation_level": isolation_level,
+                },
+                partitions=partitions,
                 is_manual=not auto_commit,
                 # subscriber args
                 no_ack=no_ack,
                 retry=retry,
                 broker_middlewares=self._middlewares,
                 broker_dependencies=self._dependencies,
                 # AsyncAPI
```

### Comparing `faststream-0.5.4/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.5/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.5/faststream/kafka/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from faststream.broker.utils import default_filter
 from faststream.kafka.broker.broker import KafkaBroker as KB
 
 if TYPE_CHECKING:
     from asyncio import AbstractEventLoop
     from enum import Enum
 
+    from aiokafka import TopicPartition
     from aiokafka.abc import AbstractTokenProvider, ConsumerRebalanceListener
     from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
     from fastapi import params
     from fastapi.types import IncEx
     from starlette.types import ASGIApp, Lifespan
 
     from faststream.asyncapi import schema as asyncapi
@@ -915,14 +916,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1397,14 +1405,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -1879,14 +1894,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -2364,14 +2386,21 @@
         ] = None,
         pattern: Annotated[
             Optional[str],
             Doc("""
             Pattern to match available topics. You must provide either topics or pattern, but not both.
             """),
         ] = None,
+        partitions: Annotated[
+            Iterable["TopicPartition"],
+            Doc("""
+            An explicit partitions list to assign.
+            You can't use 'topics' and 'partitions' in the same time.
+            """),
+        ] = (),
         # broker args
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
             Optional["CustomCallable"],
@@ -2571,14 +2600,15 @@
             exclude_internal_topics=exclude_internal_topics,
             isolation_level=isolation_level,
             batch=batch,
             max_records=max_records,
             batch_timeout_ms=batch_timeout_ms,
             listener=listener,
             pattern=pattern,
+            partitions=partitions,
             # broker args
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
             retry=retry,
```

### Comparing `faststream-0.5.4/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.5/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/publisher/producer.py` & `faststream-0.5.5/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/publisher/usecase.py` & `faststream-0.5.5/faststream/kafka/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/schemas/params.py` & `faststream-0.5.5/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.5/faststream/nats/subscriber/asyncapi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,223 +1,196 @@
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    Iterable,
-    Literal,
-    Optional,
-    Tuple,
-    Union,
-    overload,
-)
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
 
+from nats.aio.subscription import (
+    DEFAULT_SUB_PENDING_BYTES_LIMIT,
+    DEFAULT_SUB_PENDING_MSGS_LIMIT,
+)
+from nats.js.client import (
+    DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
+    DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
+)
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
-from faststream.asyncapi.schema.bindings import kafka
+from faststream.asyncapi.schema.bindings import nats
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import MsgType
-from faststream.kafka.subscriber.usecase import (
-    BatchSubscriber,
-    DefaultSubscriber,
+from faststream.exceptions import SetupError
+from faststream.nats.helpers import stream_builder
+from faststream.nats.subscriber.usecase import (
+    BatchHandler,
+    DefaultHandler,
     LogicSubscriber,
 )
 
 if TYPE_CHECKING:
-    from aiokafka import AIOKafkaConsumer, ConsumerRecord
-    from aiokafka.abc import ConsumerRebalanceListener
     from fast_depends.dependencies import Depends
+    from nats.js import api
 
     from faststream.broker.types import BrokerMiddleware
+    from faststream.nats.schemas import JStream, PullSub
+    from faststream.types import AnyDict
 
 
-class AsyncAPISubscriber(LogicSubscriber[MsgType]):
-    """A class to handle logic and async API operations."""
+class AsyncAPISubscriber(LogicSubscriber[Any]):
+    """A class to represent a NATS handler."""
 
     def get_name(self) -> str:
-        return f'{",".join(self.topics)}:{self.call_name}'
+        return f"{self.subject}:{self.call_name}"
 
     def get_schema(self) -> Dict[str, Channel]:
-        channels = {}
-
         payloads = self.get_payloads()
 
-        for t in self.topics:
-            handler_name = self.title_ or f"{t}:{self.call_name}"
-
-            channels[handler_name] = Channel(
+        return {
+            self.name: Channel(
                 description=self.description,
                 subscribe=Operation(
                     message=Message(
-                        title=f"{handler_name}:Message",
+                        title=f"{self.name}:Message",
                         payload=resolve_payloads(payloads),
                         correlationId=CorrelationId(
                             location="$message.header#/correlation_id"
                         ),
                     ),
                 ),
                 bindings=ChannelBinding(
-                    kafka=kafka.ChannelBinding(topic=t),
+                    nats=nats.ChannelBinding(
+                        subject=self.subject,
+                        queue=self.queue or None,
+                    )
                 ),
             )
-
-        return channels
-
-    @overload  # type: ignore[override]
-    @staticmethod
-    def create(
-        *topics: str,
-        batch: Literal[True],
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        listener: Optional["ConsumerRebalanceListener"],
-        pattern: Optional[str],
-        builder: Callable[..., "AIOKafkaConsumer"],
-        is_manual: bool,
-        # Subscriber args
-        no_ack: bool,
-        retry: bool,
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConsumerRecord, ...]]"],
-        # AsyncAPI args
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> "AsyncAPIBatchSubscriber": ...
-
-    @overload
-    @staticmethod
-    def create(
-        *topics: str,
-        batch: Literal[False],
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        listener: Optional["ConsumerRebalanceListener"],
-        pattern: Optional[str],
-        builder: Callable[..., "AIOKafkaConsumer"],
-        is_manual: bool,
-        # Subscriber args
-        no_ack: bool,
-        retry: bool,
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
-        # AsyncAPI args
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> "AsyncAPIDefaultSubscriber": ...
-
-    @overload
-    @staticmethod
-    def create(
-        *topics: str,
-        batch: bool,
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        listener: Optional["ConsumerRebalanceListener"],
-        pattern: Optional[str],
-        builder: Callable[..., "AIOKafkaConsumer"],
-        is_manual: bool,
-        # Subscriber args
-        no_ack: bool,
-        retry: bool,
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable[
-            "BrokerMiddleware[Union[ConsumerRecord, Tuple[ConsumerRecord, ...]]]"
-        ],
-        # AsyncAPI args
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> Union[
-        "AsyncAPIDefaultSubscriber",
-        "AsyncAPIBatchSubscriber",
-    ]: ...
+        }
 
     @override
     @staticmethod
-    def create(
-        *topics: str,
-        batch: bool,
-        batch_timeout_ms: int,
-        max_records: Optional[int],
-        # Kafka information
-        group_id: Optional[str],
-        listener: Optional["ConsumerRebalanceListener"],
-        pattern: Optional[str],
-        builder: Callable[..., "AIOKafkaConsumer"],
-        is_manual: bool,
+    def create(  # type: ignore[override]
+        *,
+        subject: str,
+        queue: str,
+        pending_msgs_limit: Optional[int],
+        pending_bytes_limit: Optional[int],
+        # Core args
+        max_msgs: int,
+        # JS args
+        durable: Optional[str],
+        config: Optional["api.ConsumerConfig"],
+        ordered_consumer: bool,
+        idle_heartbeat: Optional[float],
+        flow_control: bool,
+        deliver_policy: Optional["api.DeliverPolicy"],
+        headers_only: Optional[bool],
+        # pull args
+        pull_sub: Optional["PullSub"],
+        inbox_prefix: bytes,
+        # custom args
+        ack_first: bool,
+        max_workers: int,
+        stream: Union[str, "JStream", None],
         # Subscriber args
         no_ack: bool,
-        retry: bool,
+        retry: Union[bool, int],
         broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable[
-            "BrokerMiddleware[Union[ConsumerRecord, Tuple[ConsumerRecord, ...]]]"
-        ],
-        # AsyncAPI args
+        broker_middlewares: Iterable["BrokerMiddleware[Any]"],
+        # AsyncAPI information
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
     ]:
-        if batch:
+        if stream := stream_builder.stream(stream):
+            stream.add_subject(subject)
+
+        if pull_sub is not None and stream is None:
+            raise SetupError("Pull subscriber can be used only with a stream")
+
+        if stream:
+            # TODO: pull & queue warning
+            # TODO: push & durable warning
+
+            extra_options: AnyDict = {
+                "pending_msgs_limit": pending_msgs_limit
+                or DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
+                "pending_bytes_limit": pending_bytes_limit
+                or DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
+                "durable": durable,
+                "stream": stream.name,
+                "config": config,
+            }
+
+            if pull_sub is not None:
+                extra_options.update({"inbox_prefix": inbox_prefix})
+
+            else:
+                extra_options.update(
+                    {
+                        "ordered_consumer": ordered_consumer,
+                        "idle_heartbeat": idle_heartbeat,
+                        "flow_control": flow_control,
+                        "deliver_policy": deliver_policy,
+                        "headers_only": headers_only,
+                        "manual_ack": not ack_first,
+                    }
+                )
+
+        else:
+            extra_options = {
+                "pending_msgs_limit": pending_msgs_limit
+                or DEFAULT_SUB_PENDING_MSGS_LIMIT,
+                "pending_bytes_limit": pending_bytes_limit
+                or DEFAULT_SUB_PENDING_BYTES_LIMIT,
+                "max_msgs": max_msgs,
+            }
+
+        if getattr(pull_sub, "batch", False):
             return AsyncAPIBatchSubscriber(
-                *topics,
-                batch_timeout_ms=batch_timeout_ms,
-                max_records=max_records,
-                group_id=group_id,
-                listener=listener,
-                pattern=pattern,
-                builder=builder,
-                is_manual=is_manual,
+                extra_options=extra_options,
+                # basic args
+                pull_sub=pull_sub,
+                subject=subject,
+                queue=queue,
+                stream=stream,
+                # Subscriber args
                 no_ack=no_ack,
                 retry=retry,
                 broker_dependencies=broker_dependencies,
                 broker_middlewares=broker_middlewares,
+                # AsyncAPI information
                 title_=title_,
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
+
         else:
             return AsyncAPIDefaultSubscriber(
-                *topics,
-                group_id=group_id,
-                listener=listener,
-                pattern=pattern,
-                builder=builder,
-                is_manual=is_manual,
+                max_workers=max_workers,
+                extra_options=extra_options,
+                # basic args
+                pull_sub=pull_sub,
+                subject=subject,
+                queue=queue,
+                stream=stream,
+                # Subscriber args
                 no_ack=no_ack,
                 retry=retry,
                 broker_dependencies=broker_dependencies,
                 broker_middlewares=broker_middlewares,
+                # AsyncAPI information
                 title_=title_,
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
 
 
-class AsyncAPIDefaultSubscriber(
-    DefaultSubscriber,
-    AsyncAPISubscriber["ConsumerRecord"],
-):
-    pass
+class AsyncAPIDefaultSubscriber(AsyncAPISubscriber, DefaultHandler):
+    """One-message consumer with AsyncAPI methods."""
 
 
-class AsyncAPIBatchSubscriber(
-    BatchSubscriber,
-    AsyncAPISubscriber[Tuple["ConsumerRecord", ...]],
-):
-    pass
+class AsyncAPIBatchSubscriber(AsyncAPISubscriber, BatchHandler):
+    """Batch-message consumer with AsyncAPI methods."""
```

### Comparing `faststream-0.5.4/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.5/faststream/confluent/subscriber/usecase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,61 @@
 import asyncio
 from abc import ABC, abstractmethod
-from itertools import chain
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Optional,
     Sequence,
     Tuple,
 )
 
 import anyio
-from aiokafka.errors import ConsumerStoppedError, KafkaError
+from confluent_kafka import KafkaException, Message
 from typing_extensions import override
 
 from faststream.broker.publisher.fake import FakePublisher
 from faststream.broker.subscriber.usecase import SubscriberUsecase
-from faststream.broker.types import (
-    AsyncCallable,
-    BrokerMiddleware,
-    CustomCallable,
-    MsgType,
-)
-from faststream.kafka.parser import AioKafkaParser
+from faststream.broker.types import MsgType
+from faststream.confluent.parser import AsyncConfluentParser
 
 if TYPE_CHECKING:
-    from aiokafka import AIOKafkaConsumer, ConsumerRecord
-    from aiokafka.abc import ConsumerRebalanceListener
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.publisher.proto import ProducerProto
-    from faststream.kafka.schemas.params import ConsumerConnectionParams
+    from faststream.broker.types import (
+        AsyncCallable,
+        BrokerMiddleware,
+        CustomCallable,
+    )
+    from faststream.confluent.client import AsyncConfluentConsumer
     from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
     """A class to handle logic for consuming messages from Kafka."""
 
     topics: Sequence[str]
     group_id: Optional[str]
 
-    consumer: Optional["AIOKafkaConsumer"]
+    builder: Optional[Callable[..., "AsyncConfluentConsumer"]]
+    consumer: Optional["AsyncConfluentConsumer"]
+
     task: Optional["asyncio.Task[None]"]
     client_id: Optional[str]
-    batch: bool
 
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., "AIOKafkaConsumer"],
-        listener: Optional["ConsumerRebalanceListener"],
-        pattern: Optional[str],
+        connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         default_parser: "AsyncCallable",
         default_decoder: "AsyncCallable",
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
@@ -82,30 +78,28 @@
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
         self.group_id = group_id
         self.topics = topics
         self.is_manual = is_manual
-        self.builder = builder
+        self.builder = None
         self.consumer = None
         self.task = None
 
         # Setup it later
         self.client_id = ""
-        self.__pattern = pattern
-        self.__listener = listener
-        self.__connection_args: "ConsumerConnectionParams" = {}
+        self.__connection_data = connection_data
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         client_id: Optional[str],
-        connection_args: "ConsumerConnectionParams",
+        builder: Callable[..., "AsyncConfluentConsumer"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
         extra_context: Optional["AnyDict"],
         # broker options
         broker_parser: Optional["CustomCallable"],
@@ -113,40 +107,39 @@
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
         _call_decorators: Iterable["Decorator"],
     ) -> None:
         self.client_id = client_id
-        self.__connection_args = connection_args
+        self.builder = builder
 
         super().setup(
             logger=logger,
             producer=producer,
             graceful_timeout=graceful_timeout,
             extra_context=extra_context,
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
             _call_decorators=_call_decorators,
         )
 
+    @override
     async def start(self) -> None:
         """Start the consumer."""
+        assert self.builder, "You should setup subscriber at first."  # nosec B101
+
         self.consumer = consumer = self.builder(
+            *self.topics,
             group_id=self.group_id,
             client_id=self.client_id,
-            **self.__connection_args,
-        )
-        consumer.subscribe(
-            topics=self.topics,
-            pattern=self.__pattern,
-            listener=self.__listener,
+            **self.__connection_data,
         )
         await consumer.start()
 
         await super().start()
 
         self.task = asyncio.create_task(self._consume())
 
@@ -159,203 +152,194 @@
 
         if self.task is not None and not self.task.done():
             self.task.cancel()
 
         self.task = None
 
     def _make_response_publisher(
-        self,
-        message: "StreamMessage[Any]",
+        self, message: "StreamMessage[Any]"
     ) -> Sequence[FakePublisher]:
         if not message.reply_to or self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
                 publish_kwargs={
                     "topic": message.reply_to,
                 },
             ),
         )
 
     @abstractmethod
-    async def get_msg(self) -> MsgType:
+    async def get_msg(self) -> Optional[MsgType]:
         raise NotImplementedError()
 
     async def _consume(self) -> None:
-        assert self.consumer, "You should setup subscriber at first."  # nosec B101
+        assert self.consumer, "You should start subscriber at first."  # nosec B101
 
         connected = True
         while self.running:
             try:
                 msg = await self.get_msg()
-
-            # pragma: no cover
-            except KafkaError:  # noqa: PERF203
+            except KafkaException:  # pragma: no cover  # noqa: PERF203
                 if connected:
                     connected = False
                 await anyio.sleep(5)
 
-            except ConsumerStoppedError:
-                return
-
             else:
                 if not connected:  # pragma: no cover
                     connected = True
 
-                if msg:
-                    await self.consume(msg)
+                if msg is not None:
+                    await self.consume(msg)  # type: ignore[arg-type]
 
     @staticmethod
-    def get_routing_hash(
-        topics: Iterable[str],
-        group_id: Optional[str] = None,
-    ) -> int:
+    def get_routing_hash(topics: Iterable[str], group_id: Optional[str] = None) -> int:
         return hash("".join((*topics, group_id or "")))
 
     def __hash__(self) -> int:
-        return self.get_routing_hash(
-            topics=(*self.topics, self.__pattern or ""),
-            group_id=self.group_id,
-        )
+        return self.get_routing_hash(self.topics, self.group_id)
 
     @staticmethod
     def build_log_context(
         message: Optional["StreamMessage[Any]"],
         topic: str,
         group_id: Optional[str] = None,
     ) -> Dict[str, str]:
         return {
             "topic": topic,
             "group_id": group_id or "",
             "message_id": getattr(message, "message_id", ""),
         }
 
-    def get_log_context(
-        self,
-        message: Optional["StreamMessage[ConsumerRecord]"],
-    ) -> Dict[str, str]:
-        if message is None:
-            topic = ",".join(self.topics)
-        elif isinstance(message.raw_message, Sequence):
-            topic = message.raw_message[0].topic
-        else:
-            topic = message.raw_message.topic
-
-        return self.build_log_context(
-            message=message,
-            topic=topic,
-            group_id=self.group_id,
-        )
-
     def add_prefix(self, prefix: str) -> None:
         self.topics = tuple("".join((prefix, t)) for t in self.topics)
 
 
-class DefaultSubscriber(LogicSubscriber["ConsumerRecord"]):
+class DefaultSubscriber(LogicSubscriber[Message]):
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        listener: Optional["ConsumerRebalanceListener"],
-        pattern: Optional[str],
-        builder: Callable[..., "AIOKafkaConsumer"],
+        connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
+        broker_middlewares: Iterable["BrokerMiddleware[Message]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             *topics,
             group_id=group_id,
-            listener=listener,
-            pattern=pattern,
-            builder=builder,
+            connection_data=connection_data,
             is_manual=is_manual,
             # subscriber args
-            default_parser=AioKafkaParser.parse_message,
-            default_decoder=AioKafkaParser.decode_message,
+            default_parser=AsyncConfluentParser.parse_message,
+            default_decoder=AsyncConfluentParser.decode_message,
             # Propagated args
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> "ConsumerRecord":
+    async def get_msg(self) -> Optional["Message"]:
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
         return await self.consumer.getone()
 
+    def get_log_context(
+        self,
+        message: Optional["StreamMessage[Message]"],
+    ) -> Dict[str, str]:
+        if message is None:
+            topic = ",".join(self.topics)
+        else:
+            topic = message.raw_message.topic() or ",".join(self.topics)
+
+        return self.build_log_context(
+            message=message,
+            topic=topic,
+            group_id=self.group_id,
+        )
+
 
-class BatchSubscriber(LogicSubscriber[Tuple["ConsumerRecord", ...]]):
+class BatchSubscriber(LogicSubscriber[Tuple[Message, ...]]):
     def __init__(
         self,
         *topics: str,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        listener: Optional["ConsumerRebalanceListener"],
-        pattern: Optional[str],
-        builder: Callable[..., "AIOKafkaConsumer"],
+        connection_data: "AnyDict",
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
         broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable[
-            "BrokerMiddleware[Sequence[Tuple[ConsumerRecord, ...]]]"
-        ],
+        broker_middlewares: Iterable["BrokerMiddleware[Tuple[Message, ...]]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         self.batch_timeout_ms = batch_timeout_ms
         self.max_records = max_records
 
         super().__init__(
             *topics,
             group_id=group_id,
-            listener=listener,
-            pattern=pattern,
-            builder=builder,
+            connection_data=connection_data,
             is_manual=is_manual,
             # subscriber args
-            default_parser=AioKafkaParser.parse_message_batch,
-            default_decoder=AioKafkaParser.decode_message_batch,
+            default_parser=AsyncConfluentParser.parse_message_batch,
+            default_decoder=AsyncConfluentParser.decode_message_batch,
             # Propagated args
             no_ack=no_ack,
             retry=retry,
             broker_middlewares=broker_middlewares,
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> Tuple["ConsumerRecord", ...]:
+    async def get_msg(self) -> Optional[Tuple["Message", ...]]:
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
 
         messages = await self.consumer.getmany(
             timeout_ms=self.batch_timeout_ms,
             max_records=self.max_records,
         )
 
         if not messages:  # pragma: no cover
             await anyio.sleep(self.batch_timeout_ms / 1000)
-            return ()
+            return None
 
-        return tuple(chain(*messages.values()))
+        return messages
+
+    def get_log_context(
+        self,
+        message: Optional["StreamMessage[Tuple[Message, ...]]"],
+    ) -> Dict[str, str]:
+        if message is None:
+            topic = ",".join(self.topics)
+        else:
+            topic = message.raw_message[0].topic() or ",".join(self.topics)
+
+        return self.build_log_context(
+            message=message,
+            topic=topic,
+            group_id=self.group_id,
+        )
```

### Comparing `faststream-0.5.4/faststream/log/formatter.py` & `faststream-0.5.5/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/log/logging.py` & `faststream-0.5.5/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/__init__.py` & `faststream-0.5.5/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/annotations.py` & `faststream-0.5.5/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/helpers.py` & `faststream-0.5.5/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/message.py` & `faststream-0.5.5/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/parser.py` & `faststream-0.5.5/faststream/nats/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/router.py` & `faststream-0.5.5/faststream/nats/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/security.py` & `faststream-0.5.5/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/testing.py` & `faststream-0.5.5/faststream/nats/testing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from unittest.mock import AsyncMock
 
 from nats.aio.msg import Msg
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
 from faststream.exceptions import WRONG_PUBLISH_ARGS
 from faststream.nats.broker import NatsBroker
@@ -36,16 +37,22 @@
                 pass
 
             broker.setup_subscriber(sub)
 
         return sub.calls[0].handler
 
     @staticmethod
-    async def _fake_connect(broker: NatsBroker, *args: Any, **kwargs: Any) -> None:
+    async def _fake_connect(  # type: ignore[override]
+        broker: NatsBroker,
+        *args: Any,
+        **kwargs: Any,
+    ) -> AsyncMock:
+        broker.stream = AsyncMock()  # type: ignore[assignment]
         broker._js_producer = broker._producer = FakeProducer(broker)  # type: ignore[assignment]
+        return AsyncMock()
 
     @staticmethod
     def remove_publisher_fake_subscriber(
         broker: NatsBroker, publisher: "AsyncAPIPublisher"
     ) -> None:
         broker._subscribers.pop(
             AsyncAPISubscriber.get_routing_hash(publisher.subject), None
```

### Comparing `faststream-0.5.4/faststream/nats/broker/broker.py` & `faststream-0.5.5/faststream/nats/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/broker/logging.py` & `faststream-0.5.5/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/broker/registrator.py` & `faststream-0.5.5/faststream/nats/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/fastapi/__init__.py` & `faststream-0.5.5/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.5/faststream/nats/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.5/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/publisher/producer.py` & `faststream-0.5.5/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/publisher/usecase.py` & `faststream-0.5.5/faststream/nats/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/schemas/js_stream.py` & `faststream-0.5.5/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.5/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.5/faststream/redis/testing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,196 +1,225 @@
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
+import re
+from typing import TYPE_CHECKING, Any, Optional, Sequence, Union
+from unittest.mock import AsyncMock, MagicMock
 
-from nats.aio.subscription import (
-    DEFAULT_SUB_PENDING_BYTES_LIMIT,
-    DEFAULT_SUB_PENDING_MSGS_LIMIT,
-)
-from nats.js.client import (
-    DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-    DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-)
 from typing_extensions import override
 
-from faststream.asyncapi.schema import (
-    Channel,
-    ChannelBinding,
-    CorrelationId,
-    Message,
-    Operation,
-)
-from faststream.asyncapi.schema.bindings import nats
-from faststream.asyncapi.utils import resolve_payloads
-from faststream.exceptions import SetupError
-from faststream.nats.helpers import stream_builder
-from faststream.nats.subscriber.usecase import (
-    BatchHandler,
-    DefaultHandler,
-    LogicSubscriber,
+from faststream.broker.message import gen_cor_id
+from faststream.exceptions import WRONG_PUBLISH_ARGS, SetupError
+from faststream.redis.broker.broker import RedisBroker
+from faststream.redis.message import (
+    BatchListMessage,
+    BatchStreamMessage,
+    DefaultListMessage,
+    DefaultStreamMessage,
+    PubSubMessage,
+    bDATA_KEY,
 )
+from faststream.redis.parser import RawMessage
+from faststream.redis.publisher.producer import RedisFastProducer
+from faststream.redis.schemas import INCORRECT_SETUP_MSG
+from faststream.redis.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.testing.broker import TestBroker, call_handler
 
 if TYPE_CHECKING:
-    from fast_depends.dependencies import Depends
-    from nats.js import api
+    from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.redis.publisher.asyncapi import AsyncAPIPublisher
+    from faststream.types import AnyDict, SendableMessage
 
-    from faststream.broker.types import BrokerMiddleware
-    from faststream.nats.schemas import JStream, PullSub
-    from faststream.types import AnyDict
-
-
-class AsyncAPISubscriber(LogicSubscriber[Any]):
-    """A class to represent a NATS handler."""
-
-    def get_name(self) -> str:
-        return f"{self.subject}:{self.call_name}"
-
-    def get_schema(self) -> Dict[str, Channel]:
-        payloads = self.get_payloads()
-
-        return {
-            self.name: Channel(
-                description=self.description,
-                subscribe=Operation(
-                    message=Message(
-                        title=f"{self.name}:Message",
-                        payload=resolve_payloads(payloads),
-                        correlationId=CorrelationId(
-                            location="$message.header#/correlation_id"
-                        ),
-                    ),
-                ),
-                bindings=ChannelBinding(
-                    nats=nats.ChannelBinding(
-                        subject=self.subject,
-                        queue=self.queue or None,
-                    )
-                ),
-            )
-        }
+__all__ = ("TestRedisBroker",)
+
+
+class TestRedisBroker(TestBroker[RedisBroker]):
+    """A class to test Redis brokers."""
 
-    @override
     @staticmethod
-    def create(  # type: ignore[override]
+    def create_publisher_fake_subscriber(
+        broker: RedisBroker,
+        publisher: "AsyncAPIPublisher",
+    ) -> "HandlerCallWrapper[Any, Any, Any]":
+        sub = broker.subscriber(**publisher.subscriber_property)
+
+        if not sub.calls:
+
+            @sub
+            def f(msg: Any) -> None:
+                pass
+
+            broker.setup_subscriber(sub)
+
+        return sub.calls[0].handler
+
+    @staticmethod
+    async def _fake_connect(  # type: ignore[override]
+        broker: RedisBroker,
+        *args: Any,
+        **kwargs: Any,
+    ) -> AsyncMock:
+        broker._producer = FakeProducer(broker)  # type: ignore[assignment]
+        connection = MagicMock()
+        connection.pubsub.side_effect = AsyncMock
+        return connection
+
+    @staticmethod
+    def remove_publisher_fake_subscriber(
+        broker: RedisBroker,
+        publisher: "AsyncAPIPublisher",
+    ) -> None:
+        broker._subscribers.pop(
+            hash(AsyncAPISubscriber.create(**publisher.subscriber_property)),
+            None,
+        )
+
+
+class FakeProducer(RedisFastProducer):
+    def __init__(self, broker: RedisBroker) -> None:
+        self.broker = broker
+
+    @override
+    async def publish(  # type: ignore[override]
+        self,
+        message: "SendableMessage",
         *,
-        subject: str,
-        queue: str,
-        pending_msgs_limit: Optional[int],
-        pending_bytes_limit: Optional[int],
-        # Core args
-        max_msgs: int,
-        # JS args
-        durable: Optional[str],
-        config: Optional["api.ConsumerConfig"],
-        ordered_consumer: bool,
-        idle_heartbeat: Optional[float],
-        flow_control: bool,
-        deliver_policy: Optional["api.DeliverPolicy"],
-        headers_only: Optional[bool],
-        # pull args
-        pull_sub: Optional["PullSub"],
-        inbox_prefix: bytes,
-        # custom args
-        ack_first: bool,
-        max_workers: int,
-        stream: Union[str, "JStream", None],
-        # Subscriber args
-        no_ack: bool,
-        retry: Union[bool, int],
-        broker_dependencies: Iterable["Depends"],
-        broker_middlewares: Iterable["BrokerMiddleware[Any]"],
-        # AsyncAPI information
-        title_: Optional[str],
-        description_: Optional[str],
-        include_in_schema: bool,
-    ) -> Union[
-        "AsyncAPIDefaultSubscriber",
-        "AsyncAPIBatchSubscriber",
-    ]:
-        if stream := stream_builder.stream(stream):
-            stream.add_subject(subject)
-
-        if pull_sub is not None and stream is None:
-            raise SetupError("Pull subscriber can be used only with a stream")
-
-        if stream:
-            # TODO: pull & queue warning
-            # TODO: push & durable warning
-
-            extra_options: AnyDict = {
-                "pending_msgs_limit": pending_msgs_limit
-                or DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-                "pending_bytes_limit": pending_bytes_limit
-                or DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
-                "durable": durable,
-                "stream": stream.name,
-                "config": config,
-            }
-
-            if pull_sub is not None:
-                extra_options.update({"inbox_prefix": inbox_prefix})
-
-            else:
-                extra_options.update(
-                    {
-                        "ordered_consumer": ordered_consumer,
-                        "idle_heartbeat": idle_heartbeat,
-                        "flow_control": flow_control,
-                        "deliver_policy": deliver_policy,
-                        "headers_only": headers_only,
-                        "manual_ack": not ack_first,
-                    }
+        channel: Optional[str] = None,
+        list: Optional[str] = None,
+        stream: Optional[str] = None,
+        maxlen: Optional[int] = None,
+        headers: Optional["AnyDict"] = None,
+        reply_to: str = "",
+        correlation_id: Optional[str] = None,
+        rpc: bool = False,
+        rpc_timeout: Optional[float] = 30.0,
+        raise_timeout: bool = False,
+    ) -> Optional[Any]:
+        if rpc and reply_to:
+            raise WRONG_PUBLISH_ARGS
+
+        correlation_id = correlation_id or gen_cor_id()
+
+        body = build_message(
+            message=message,
+            reply_to=reply_to,
+            correlation_id=correlation_id,
+            headers=headers,
+        )
+
+        any_of = channel or list or stream
+        if any_of is None:
+            raise SetupError(INCORRECT_SETUP_MSG)
+
+        msg: Any = None
+        for handler in self.broker._subscribers.values():  # pragma: no branch
+            call = False
+
+            if channel and (ch := getattr(handler, "channel", None)) is not None:
+                call = bool(
+                    (not ch.pattern and ch.name == channel)
+                    or (
+                        ch.pattern
+                        and re.match(
+                            ch.name.replace(".", "\\.").replace("*", ".*"),
+                            channel,
+                        )
+                    )
+                )
+
+                msg = PubSubMessage(
+                    type="message",
+                    data=body,
+                    channel=channel,
+                    pattern=ch.pattern,
+                )
+
+            elif list and (ls := getattr(handler, "list_sub", None)) is not None:
+                if ls.batch:
+                    msg = BatchListMessage(
+                        type="blist",
+                        channel=list,
+                        data=[body],
+                    )
+
+                else:
+                    msg = DefaultListMessage(
+                        type="list",
+                        channel=list,
+                        data=body,
+                    )
+
+                call = list == ls.name
+
+            elif stream and (st := getattr(handler, "stream_sub", None)) is not None:
+                if st.batch:
+                    msg = BatchStreamMessage(
+                        type="bstream",
+                        channel=stream,
+                        data=[{bDATA_KEY: body}],
+                        message_ids=[],
+                    )
+                else:
+                    msg = DefaultStreamMessage(
+                        type="stream",
+                        channel=stream,
+                        data={bDATA_KEY: body},
+                        message_ids=[],
+                    )
+
+                call = stream == st.name
+
+            if call:
+                r = await call_handler(
+                    handler=handler,
+                    message=msg,
+                    rpc=rpc,
+                    rpc_timeout=rpc_timeout,
+                    raise_timeout=raise_timeout,
                 )
 
-        else:
-            extra_options = {
-                "pending_msgs_limit": pending_msgs_limit
-                or DEFAULT_SUB_PENDING_MSGS_LIMIT,
-                "pending_bytes_limit": pending_bytes_limit
-                or DEFAULT_SUB_PENDING_BYTES_LIMIT,
-                "max_msgs": max_msgs,
-            }
-
-        if getattr(pull_sub, "batch", False):
-            return AsyncAPIBatchSubscriber(
-                extra_options=extra_options,
-                # basic args
-                pull_sub=pull_sub,
-                subject=subject,
-                queue=queue,
-                stream=stream,
-                # Subscriber args
-                no_ack=no_ack,
-                retry=retry,
-                broker_dependencies=broker_dependencies,
-                broker_middlewares=broker_middlewares,
-                # AsyncAPI information
-                title_=title_,
-                description_=description_,
-                include_in_schema=include_in_schema,
-            )
-
-        else:
-            return AsyncAPIDefaultSubscriber(
-                max_workers=max_workers,
-                extra_options=extra_options,
-                # basic args
-                pull_sub=pull_sub,
-                subject=subject,
-                queue=queue,
-                stream=stream,
-                # Subscriber args
-                no_ack=no_ack,
-                retry=retry,
-                broker_dependencies=broker_dependencies,
-                broker_middlewares=broker_middlewares,
-                # AsyncAPI information
-                title_=title_,
-                description_=description_,
-                include_in_schema=include_in_schema,
-            )
+                if rpc:  # pragma: no branch
+                    return r
+
+        return None
 
+    async def publish_batch(
+        self,
+        *msgs: "SendableMessage",
+        list: str,
+        correlation_id: Optional[str] = None,
+    ) -> None:
+        correlation_id = correlation_id or gen_cor_id()
+
+        for handler in self.broker._subscribers.values():  # pragma: no branch
+            if (
+                list_sub := getattr(handler, "list_sub", None)
+            ) and list_sub.name == list:
+                await call_handler(
+                    handler=handler,
+                    message=BatchListMessage(
+                        type="blist",
+                        channel=list,
+                        data=[
+                            build_message(
+                                m,
+                                correlation_id=correlation_id,
+                            )
+                            for m in msgs
+                        ],
+                    ),
+                )
 
-class AsyncAPIDefaultSubscriber(AsyncAPISubscriber, DefaultHandler):
-    """One-message consumer with AsyncAPI methods."""
+        return None
 
 
-class AsyncAPIBatchSubscriber(AsyncAPISubscriber, BatchHandler):
-    """Batch-message consumer with AsyncAPI methods."""
+def build_message(
+    message: Union[Sequence["SendableMessage"], "SendableMessage"],
+    *,
+    correlation_id: str,
+    reply_to: str = "",
+    headers: Optional["AnyDict"] = None,
+) -> bytes:
+    data = RawMessage.encode(
+        message=message,
+        reply_to=reply_to,
+        headers=headers,
+        correlation_id=correlation_id,
+    )
+    return data
```

### Comparing `faststream-0.5.4/faststream/nats/subscriber/usecase.py` & `faststream-0.5.5/faststream/nats/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/__init__.py` & `faststream-0.5.5/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/annotations.py` & `faststream-0.5.5/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/message.py` & `faststream-0.5.5/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/parser.py` & `faststream-0.5.5/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/router.py` & `faststream-0.5.5/faststream/rabbit/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/security.py` & `faststream-0.5.5/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/testing.py` & `faststream-0.5.5/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/utils.py` & `faststream-0.5.5/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/broker/broker.py` & `faststream-0.5.5/faststream/rabbit/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/broker/logging.py` & `faststream-0.5.5/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/broker/registrator.py` & `faststream-0.5.5/faststream/rabbit/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.5/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/fastapi/router.py` & `faststream-0.5.5/faststream/rabbit/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.5/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/publisher/producer.py` & `faststream-0.5.5/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.5/faststream/rabbit/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/schemas/constants.py` & `faststream-0.5.5/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.5/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/schemas/queue.py` & `faststream-0.5.5/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/schemas/reply.py` & `faststream-0.5.5/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.5/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.5/faststream/rabbit/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/__init__.py` & `faststream-0.5.5/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/annotations.py` & `faststream-0.5.5/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/message.py` & `faststream-0.5.5/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/parser.py` & `faststream-0.5.5/faststream/redis/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/router.py` & `faststream-0.5.5/faststream/redis/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/security.py` & `faststream-0.5.5/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/broker/broker.py` & `faststream-0.5.5/faststream/redis/broker/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/broker/logging.py` & `faststream-0.5.5/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/broker/registrator.py` & `faststream-0.5.5/faststream/redis/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/fastapi/__init__.py` & `faststream-0.5.5/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.5/faststream/redis/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.5/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/publisher/producer.py` & `faststream-0.5.5/faststream/redis/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/publisher/usecase.py` & `faststream-0.5.5/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/schemas/list_sub.py` & `faststream-0.5.5/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/schemas/proto.py` & `faststream-0.5.5/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.5/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.5/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.5/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/redis/subscriber/usecase.py` & `faststream-0.5.5/faststream/redis/subscriber/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/testing/app.py` & `faststream-0.5.5/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/testing/broker.py` & `faststream-0.5.5/faststream/testing/broker.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/ast.py` & `faststream-0.5.5/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/classes.py` & `faststream-0.5.5/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/data.py` & `faststream-0.5.5/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/functions.py` & `faststream-0.5.5/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/no_cast.py` & `faststream-0.5.5/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/path.py` & `faststream-0.5.5/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/context/builders.py` & `faststream-0.5.5/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/context/repository.py` & `faststream-0.5.5/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/faststream/utils/context/types.py` & `faststream-0.5.5/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/scripts/build-docs-pre-commit.sh` & `faststream-0.5.5/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/scripts/lint-pre-commit.sh` & `faststream-0.5.5/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/scripts/set_variables.sh` & `faststream-0.5.5/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/scripts/static-pre-commit.sh` & `faststream-0.5.5/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/LICENSE` & `faststream-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/README.md` & `faststream-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.4/pyproject.toml` & `faststream-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -71,21 +71,21 @@
 
 nats = ["nats-py>=2.3.1,<=3.0.0"]
 
 redis = ["redis>=5.0.0,<6.0.0"]
 
 # dev dependencies
 devdocs = [
-    "mkdocs-material==9.5.18",
+    "mkdocs-material==9.5.21",
     "mkdocs-static-i18n==1.2.2",
     "mdx-include==1.4.2",
     "mkdocstrings[python]==0.25.0",
     "mkdocs-literate-nav==0.6.1",
-    "mkdocs-git-revision-date-localized-plugin==1.2.4",
-    "mike==2.0.0",                                      # versioning
+    "mkdocs-git-revision-date-localized-plugin==1.2.5",
+    "mike==2.1.1",                                      # versioning
     "mkdocs-minify-plugin==0.8.0",
     "mkdocs-macros-plugin==1.0.5",                      # includes with variables
     "mkdocs-glightbox==0.3.7",                          # img zoom
     "pillow",                                           # required for mkdocs-glightbo
     "cairosvg",                                         # required for mkdocs-glightbo
     "requests",                                         # using in CI, do not pin it
     "griffe-typingdoc==0.2.5",                          # Annotated[..., Doc("")] support
@@ -102,30 +102,30 @@
     "types-Pygments",
     "types-docutils",
     "confluent-kafka-stubs; python_version >= '3.11'",
 ]
 
 lint = [
     "faststream[types]",
-    "ruff==0.4.2",
+    "ruff==0.4.3",
     "bandit==1.7.8",
     "semgrep==1.70.0",
     "codespell==2.2.6",
 ]
 
 test-core = [
     "coverage[toml]==7.4.4",
     "pytest==8.2.0",
     "pytest-asyncio==0.23.6",
     "dirty-equals==0.7.1.post0",
 ]
 
 testing = [
     "faststream[test-core]",
-    "fastapi==0.110.2",
+    "fastapi==0.111.0",
     "pydantic-settings>=2.0.0,<3.0.0",
     "httpx==0.27.0",
     "PyYAML==6.0.1",
     "watchfiles==0.21.0",
     "email-validator==2.1.1",
 ]
```

### Comparing `faststream-0.5.4/PKG-INFO` & `faststream-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.4
+Version: 0.5.5
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -52,57 +52,57 @@
 Requires-Dist: codespell==2.2.6; extra == 'dev'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'dev'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'dev'
 Requires-Dist: coverage[toml]==7.4.4; extra == 'dev'
 Requires-Dist: detect-secrets==1.4.0; extra == 'dev'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'dev'
 Requires-Dist: email-validator==2.1.1; extra == 'dev'
-Requires-Dist: fastapi==0.110.2; extra == 'dev'
+Requires-Dist: fastapi==0.111.0; extra == 'dev'
 Requires-Dist: griffe-typingdoc==0.2.5; extra == 'dev'
 Requires-Dist: httpx==0.27.0; extra == 'dev'
 Requires-Dist: mdx-include==1.4.2; extra == 'dev'
-Requires-Dist: mike==2.0.0; extra == 'dev'
-Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'dev'
+Requires-Dist: mike==2.1.1; extra == 'dev'
+Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.5; extra == 'dev'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'dev'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'dev'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'dev'
-Requires-Dist: mkdocs-material==9.5.18; extra == 'dev'
+Requires-Dist: mkdocs-material==9.5.21; extra == 'dev'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'dev'
 Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'dev'
 Requires-Dist: mkdocstrings[python]==0.25.0; extra == 'dev'
 Requires-Dist: mypy==1.10.0; extra == 'dev'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'dev'
 Requires-Dist: pillow; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
 Requires-Dist: pre-commit==3.7.0; (python_version >= '3.9') and extra == 'dev'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'dev'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'dev'
 Requires-Dist: pytest==8.2.0; extra == 'dev'
 Requires-Dist: pyyaml==6.0.1; extra == 'dev'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'dev'
 Requires-Dist: requests; extra == 'dev'
-Requires-Dist: ruff==0.4.2; extra == 'dev'
+Requires-Dist: ruff==0.4.3; extra == 'dev'
 Requires-Dist: semgrep==1.70.0; extra == 'dev'
 Requires-Dist: types-docutils; extra == 'dev'
 Requires-Dist: types-pygments; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
 Requires-Dist: types-redis; extra == 'dev'
 Requires-Dist: types-setuptools; extra == 'dev'
 Requires-Dist: types-ujson; extra == 'dev'
 Requires-Dist: watchfiles==0.21.0; extra == 'dev'
 Provides-Extra: devdocs
 Requires-Dist: cairosvg; extra == 'devdocs'
 Requires-Dist: griffe-typingdoc==0.2.5; extra == 'devdocs'
 Requires-Dist: mdx-include==1.4.2; extra == 'devdocs'
-Requires-Dist: mike==2.0.0; extra == 'devdocs'
-Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'devdocs'
+Requires-Dist: mike==2.1.1; extra == 'devdocs'
+Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.5; extra == 'devdocs'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
-Requires-Dist: mkdocs-material==9.5.18; extra == 'devdocs'
+Requires-Dist: mkdocs-material==9.5.21; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
 Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'devdocs'
 Requires-Dist: mkdocstrings[python]==0.25.0; extra == 'devdocs'
 Requires-Dist: pillow; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
@@ -112,15 +112,15 @@
 Requires-Dist: bandit==1.7.8; extra == 'lint'
 Requires-Dist: codespell==2.2.6; extra == 'lint'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'lint'
 Requires-Dist: mypy==1.10.0; extra == 'lint'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'lint'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'lint'
-Requires-Dist: ruff==0.4.2; extra == 'lint'
+Requires-Dist: ruff==0.4.3; extra == 'lint'
 Requires-Dist: semgrep==1.70.0; extra == 'lint'
 Requires-Dist: types-docutils; extra == 'lint'
 Requires-Dist: types-pygments; extra == 'lint'
 Requires-Dist: types-pyyaml; extra == 'lint'
 Requires-Dist: types-redis; extra == 'lint'
 Requires-Dist: types-setuptools; extra == 'lint'
 Requires-Dist: types-ujson; extra == 'lint'
@@ -135,15 +135,15 @@
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'test-core'
 Requires-Dist: pytest==8.2.0; extra == 'test-core'
 Provides-Extra: testing
 Requires-Dist: coverage[toml]==7.4.4; extra == 'testing'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'testing'
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
-Requires-Dist: fastapi==0.110.2; extra == 'testing'
+Requires-Dist: fastapi==0.111.0; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'testing'
 Requires-Dist: pytest==8.2.0; extra == 'testing'
 Requires-Dist: pyyaml==6.0.1; extra == 'testing'
 Requires-Dist: watchfiles==0.21.0; extra == 'testing'
 Provides-Extra: types
```

