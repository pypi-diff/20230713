# Comparing `tmp/localstack-core-2.1.1.dev20230713161930.tar.gz` & `tmp/localstack-core-2.1.1.dev20230713205536.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230713161930.tar", last modified: Thu Jul 13 16:19:38 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230713205536.tar", last modified: Thu Jul 13 20:55:44 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230713161930.tar` & `localstack-core-2.1.1.dev20230713205536.tar`

### file list

```diff
@@ -1,878 +1,878 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.916967 localstack-core-2.1.1.dev20230713161930/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-13 16:19:38.916967 localstack-core-2.1.1.dev20230713161930/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.780967 localstack-core-2.1.1.dev20230713161930/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.780967 localstack-core-2.1.1.dev20230713161930/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-13 16:19:30.000000 localstack-core-2.1.1.dev20230713161930/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4217 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    86365 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   760042 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.784967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   134355 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.788967 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9183 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29093 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8070 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.792967 localstack-core-2.1.1.dev20230713161930/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.796967 localstack-core-2.1.1.dev20230713161930/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.796967 localstack-core-2.1.1.dev20230713161930/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.832967 localstack-core-2.1.1.dev20230713161930/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.832967 localstack-core-2.1.1.dev20230713161930/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.832967 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65824 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40232 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15121 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    78643 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.836967 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.836967 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.836967 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19981 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72344 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.836967 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.836967 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.840967 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13116 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60184 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7829 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8646 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2341 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.840967 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21531 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7311 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2283 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5756 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21650 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9484 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27850 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3365 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4684 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5007 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2735 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1513 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13537 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6852 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8861 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5059 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10780 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5845 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40630 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/resource_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73285 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24178 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20375 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.844967 localstack-core-2.1.1.dev20230713161930/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.848967 localstack-core-2.1.1.dev20230713161930/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    83531 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34301 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/provider_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15011 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22742 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43100 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.852967 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16684 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.856967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.860967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.860967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.864967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.864967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.864967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.864967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.864967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.864967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.864967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.872967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.872967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.872967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.872967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.872967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.876967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.876967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.876967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.880967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3890 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.884967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.884967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10826 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.888967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2069 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.896967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4102 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5244 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7413 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3954 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4137 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.896967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.896967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.896967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.896967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.896967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.896967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.900967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.900967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.900967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.900967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.900967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.900967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.900967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13659 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13605 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69822 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.904967 localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26930 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.908967 localstack-core-2.1.1.dev20230713161930/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.912967 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.912967 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13775 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11852 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23586 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.912967 localstack-core-2.1.1.dev20230713161930/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.912967 localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    46654 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33137 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33236 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.912967 localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.912967 localstack-core-2.1.1.dev20230713161930/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23661 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 16:19:38.916967 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-13 16:19:38.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39252 2023-07-13 16:19:38.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-13 16:19:38.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-13 16:19:38.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-13 16:19:34.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-13 16:19:34.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-13 16:19:38.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-13 16:19:38.000000 localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-13 16:19:38.916967 localstack-core-2.1.1.dev20230713161930/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-13 15:44:08.000000 localstack-core-2.1.1.dev20230713161930/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11768 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-07-13 20:55:36.000000 localstack-core-2.1.1.dev20230713205536/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4217 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    86365 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.439746 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   127167 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.455744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    82279 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   760042 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   103613 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50222 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72128 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    38483 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68386 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   133756 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   134355 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18818 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.459744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39472 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9183 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10074 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7199 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5983 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49984 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29093 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.463744 localstack-core-2.1.1.dev20230713205536/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28010 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51172 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8070 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.467744 localstack-core-2.1.1.dev20230713205536/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11533 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.467744 localstack-core-2.1.1.dev20230713205536/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.467744 localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.467744 localstack-core-2.1.1.dev20230713205536/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14626 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6161 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5159 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.467744 localstack-core-2.1.1.dev20230713205536/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.467744 localstack-core-2.1.1.dev20230713205536/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.467744 localstack-core-2.1.1.dev20230713205536/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.471743 localstack-core-2.1.1.dev20230713205536/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.471743 localstack-core-2.1.1.dev20230713205536/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5625 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.471743 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65824 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40232 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15121 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    78643 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5717 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11435 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.471743 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24315 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.471743 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11079 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3046 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3999 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12154 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19280 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.475743 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18173 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19981 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28442 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72344 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17450 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.475743 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155061 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.475743 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2083 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8503 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.475743 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12364 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8428 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61886 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7957 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9733 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2483 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.479743 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33411 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21531 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7311 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2283 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5756 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21650 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2890 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9484 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27850 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3365 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4684 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5007 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2735 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1267 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1513 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13537 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6852 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8861 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5059 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10780 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5845 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41308 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3154 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26015 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/resource_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5571 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.479743 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.479743 localstack-core-2.1.1.dev20230713205536/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.479743 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1435 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73285 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.479743 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17407 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24178 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20375 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4824 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28575 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60349 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.483743 localstack-core-2.1.1.dev20230713205536/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7546 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24475 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27010 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7817 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11819 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29389 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    83531 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34301 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/provider_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15011 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.487743 localstack-core-2.1.1.dev20230713205536/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22742 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43100 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39491 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54686 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7517 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16684 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4257 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.491742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3706 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.495742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.495742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.495742 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      767 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.527740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.527740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.527740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.527740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1246 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.527740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.527740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.527740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.535740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1560 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2054 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.535740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.535740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.535740 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.539739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.539739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.539739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.539739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.543739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3890 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.547739 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.555738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.555738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.555738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10826 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.555738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.555738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2938 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.555738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.555738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2069 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.559738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4102 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5244 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7413 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3954 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4137 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.559738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2524 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1575 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1697 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5029 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1366 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5122 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.563738 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.567737 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.567737 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.567737 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32336 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.567737 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.567737 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13659 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      629 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.571737 localstack-core-2.1.1.dev20230713205536/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.571737 localstack-core-2.1.1.dev20230713205536/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.571737 localstack-core-2.1.1.dev20230713205536/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.571737 localstack-core-2.1.1.dev20230713205536/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13605 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.571737 localstack-core-2.1.1.dev20230713205536/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.571737 localstack-core-2.1.1.dev20230713205536/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.571737 localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.575737 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2847 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69822 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.575737 localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26930 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.575737 localstack-core-2.1.1.dev20230713205536/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5239 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13775 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13571 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11852 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7927 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7353 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23586 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46654 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33137 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33236 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9032 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9890 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16615 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12451 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3776 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23661 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-13 20:55:44.583736 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-07-13 20:55:44.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39252 2023-07-13 20:55:44.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-13 20:55:44.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5340 2023-07-13 20:55:44.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-13 20:55:40.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5433 2023-07-13 20:55:40.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2851 2023-07-13 20:55:44.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-07-13 20:55:44.000000 localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3230 2023-07-13 20:55:44.587736 localstack-core-2.1.1.dev20230713205536/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-07-13 20:18:21.000000 localstack-core-2.1.1.dev20230713205536/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230713161930/LICENSE.txt` & `localstack-core-2.1.1.dev20230713205536/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/Makefile` & `localstack-core-2.1.1.dev20230713205536/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/PKG-INFO` & `localstack-core-2.1.1.dev20230713205536/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230713161930
+Version: 2.1.1.dev20230713205536
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230713161930/README.md` & `localstack-core-2.1.1.dev20230713205536/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/bin/localstack` & `localstack-core-2.1.1.dev20230713205536/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230713205536/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230713205536/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230713205536/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230713205536/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230713205536/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230713205536/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230713205536/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/config.py` & `localstack-core-2.1.1.dev20230713205536/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/constants.py` & `localstack-core-2.1.1.dev20230713205536/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230713205536/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230713205536/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/client.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/request.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/response.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/http/router.py` & `localstack-core-2.1.1.dev20230713205536/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230713205536/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230713205536/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230713205536/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230713205536/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230713205536/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230713205536/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230713205536/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230713205536/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/plugins.py` & `localstack-core-2.1.1.dev20230713205536/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230713205536/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230713205536/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230713205536/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230713205536/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230713205536/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from typing import Optional, TypedDict
 
 from localstack.aws.api.cloudformation import Capability, ChangeSetType, Parameter
 from localstack.services.cloudformation.engine.parameters import (
     StackParameter,
     convert_stack_parameters_to_list,
-    map_to_legacy_structure,
     strip_parameter_type,
 )
 from localstack.utils.aws import arns
 from localstack.utils.collections import select_attributes
 from localstack.utils.json import clone_safe
 from localstack.utils.objects import recurse_object
 from localstack.utils.strings import long_uid, short_uid
@@ -240,34 +239,18 @@
     def stack_name(self):
         return self.metadata["StackName"]
 
     @property
     def stack_id(self):
         return self.metadata["StackId"]
 
-    # TODO: potential performance issues due to many stack_parameters calls (cache or limit actual invocations)
     @property
-    def resources(self):  # TODO: not actually resources, split apart
-        """Return dict of resources, parameters, conditions, and other stack metadata."""
-        result = dict(self.template_resources)
-
-        result.update(
-            {k: map_to_legacy_structure(k, v) for k, v in self.resolved_parameters.items()}
-        )
-
-        # TODO: conditions don't really belong here and should be handled separately
-        for name, value in self.conditions.items():
-            if name not in result:
-                result[name] = {
-                    "Type": "Parameter",
-                    "LogicalResourceId": name,
-                    "Properties": {"Value": value},
-                }
-
-        return result
+    def resources(self):
+        """Return dict of resources"""
+        return dict(self.template_resources)
 
     @property
     def template_resources(self):
         return self.template.setdefault("Resources", {})
 
     @property
     def tags(self):
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/quirks.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 import uuid
 from typing import Any, Callable, Literal, Optional, Type, TypedDict
 
 import botocore
 
 from localstack import config
 from localstack.aws.accounts import get_aws_account_id
-from localstack.constants import FALSE_STRINGS
 from localstack.services.cloudformation import usage
 from localstack.services.cloudformation.deployment_utils import (
     PLACEHOLDER_AWS_NO_VALUE,
     dump_resource_as_json,
     fix_boto_parameters_based_on_report,
     get_action_name_for_resource_change,
-    is_none_or_empty_value,
     log_not_available_message,
     remove_none_values,
 )
 from localstack.services.cloudformation.engine.entities import Stack, StackChangeSet
+from localstack.services.cloudformation.engine.parameters import StackParameter
 from localstack.services.cloudformation.engine.template_utils import (
     fn_equals_type_conversion,
     get_deps_for_resource,
 )
 from localstack.services.cloudformation.engine.types import DeployTemplates, FuncDetails
 from localstack.services.cloudformation.resource_provider import (
     Credentials,
@@ -105,18 +104,14 @@
         # TODO(srw): assign resource objects rather than fetching state all the time
         # convert resource props to resource entity
         instance = get_resource_model_instance(resource_id, resources)
         if instance:
             state = instance.fetch_and_update_state(stack_name=stack_name, resources=resources)
             return state
 
-        # special case for stack parameters
-        if resource_type == "Parameter":
-            return resource_props
-
         message = (
             f"Unexpected resource type {resource_type} when resolving "
             f"references of resource {resource_id}: {dump_resource_as_json(resource)}"
         )
         log_not_available_message(resource_type=resource_type, message=message)
 
     except DependencyNotYetSatisfied:
@@ -139,15 +134,14 @@
     resource_id=None,
     resource=None,
     resources=None,
     stack_name=None,
 ):
     LOG.debug("Extract resource attribute: %s %s", resource_type, attribute)
     is_ref_attribute = attribute in ["PhysicalResourceId", "Ref"]
-    is_ref_attr_or_arn = is_ref_attribute or attribute == "Arn"
     resource = resource or {}
     if not resource and resources:
         resource = resources[resource_id]
 
     if not resource_state:
         resource_state = retrieve_resource_details(resource_id, {}, resources, stack_name)
         if not resource_state:
@@ -167,27 +161,14 @@
             f'Unable to extract attribute "{attribute}" from "{resource_type}" model class {type(resource_state)}'
         )
 
     # extract resource specific attributes
     # TODO: remove the code below - move into resource model classes!
 
     resource_props = resource.get("Properties", {})
-    if resource_type == "Parameter":
-        result = None
-        param_value = resource_props.get(
-            "Value",
-            resource.get("Value", resource_props.get("Properties", {}).get("Value")),
-        )
-        if is_ref_attr_or_arn:
-            result = param_value
-        elif isinstance(param_value, dict):
-            result = param_value.get(attribute)
-        if result is not None:
-            return result
-        return ""
     attribute_lower = first_char_to_lower(attribute)
     result = resource_state.get(attribute) or resource_state.get(attribute_lower)
     if result is None and isinstance(resource, dict):
         result = resource_props.get(attribute) or resource_props.get(attribute_lower)
         if result is None:
             result = get_attr_from_model_instance(
                 resource,
@@ -205,17 +186,15 @@
 
 
 def get_attr_from_model_instance(
     resource: dict, attribute: str, resource_type: str, resource_id: Optional[str] = None
 ):
     model_class = RESOURCE_MODELS.get(resource_type)
     if not model_class:
-        if resource_type not in ["AWS::Parameter", "Parameter"]:
-            LOG.debug('Unable to find model class for resource type "%s"', resource_type)
-        return
+        LOG.debug('Unable to find model class for resource type "%s"', resource_type)
     try:
         inst = model_class(resource_name=resource_id, resource_json=resource)
         return inst.get_cfn_attribute(attribute)
     except Exception:
         log_method = getattr(LOG, "debug")
         if config.CFN_VERBOSE_ERRORS:
             log_method = getattr(LOG, "exception")
@@ -228,15 +207,23 @@
     model_class = RESOURCE_MODELS.get(resource_type)
     if model_class:
         return model_class(resource_name=logical_resource_id, resource_json=resource).get_ref()
 
     LOG.error("Unsupported resource type: %s", resource_type)
 
 
-def resolve_ref(stack_name: str, resources: dict, mappings: dict, ref: str, attribute: str):
+def resolve_ref(
+    stack_name: str,
+    resources: dict,
+    mappings: dict,
+    conditions: dict[str, bool],
+    parameters: dict[str, StackParameter],
+    ref: str,
+    attribute: str,
+):
     # pseudo parameters
     if ref == "AWS::Region":
         return aws_stack.get_region()
     if ref == "AWS::Partition":
         return "aws"
     if ref == "AWS::StackName":
         return stack_name
@@ -256,49 +243,38 @@
     if attribute == "Ref":
         # ref always needs to be a static string
         # ref can be one of these:
         # 1. a parameter
         # 2. a pseudo-parameter (e.g. AWS::Region)
         # 3. the "value" of a resource
 
-        resource = resources.get(ref)
-        if not resource:
-            raise Exception("Should be detected earlier")
+        if parameter := parameters.get(ref):
+            parameter_type: str = parameter["ParameterType"]
+            parameter_value = parameter.get("ResolvedValue") or parameter.get("ParameterValue")
 
-        # TODO: remove after refactoring parameter resolution
-        # TODO: split this apart in parameter resource types and stack parameter handling
-        if resource["Type"] == "Parameter":
-            # https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/parameters-section-structure.html
-            # TODO: extract this into a util function and extend type support
-            parameter_type = resource.get("Properties", {}).get("ParameterType")
-            if not parameter_type:
-                # assuming this is an actual resource type now
-                return resource["Properties"]["Value"]
+            if parameter_type in ["CommaDelimitedList"] or parameter_type.startswith("List<"):
+                return [p.strip() for p in parameter_value.split(",")]
             else:
-                parameter_type: str = resource["Properties"]["ParameterType"]
-                if parameter_type in ["CommaDelimitedList"] or parameter_type.startswith("List<"):
-                    return [p.strip() for p in resource["Properties"]["Value"].split(",")]
-                else:
-                    return resource["Properties"]["Value"]
-        else:
-            # TODO: this shouldn't be needed when dependency graph and deployment status is honored
-            resolve_refs_recursively(stack_name, resources, mappings, resources.get(ref))
-            return get_ref_from_model(resources, ref)
+                return parameter_value
 
-    # TODO: remove if tests pass
-    is_ref_attribute = attribute in ["Arn"]
-    if is_ref_attribute:
-        raise Exception("invalid")
+        resource = resources.get(ref)
+        if not resource:
+            raise Exception("Should be detected earlier.")
+
+        # TODO: this shouldn't be needed when dependency graph and deployment status is honored
+        resolve_refs_recursively(
+            stack_name, resources, mappings, conditions, parameters, resources.get(ref)
+        )
+        return get_ref_from_model(resources, ref)
 
     if resources.get(ref):
         if isinstance(resources[ref].get(attribute), (str, int, float, bool, dict)):
             return resources[ref][attribute]
 
     # TODO: when do we go into the branch below?
-
     # TODO(ds): remove all below next
     # fetch resource details
     resource_new = retrieve_resource_details(ref, {}, resources, stack_name)
     if not resource_new:
         raise DependencyNotYetSatisfied(
             resource_ids=ref,
             message='Unable to fetch details for resource "%s" (resolving attribute "%s")'
@@ -326,16 +302,25 @@
     return result
 
 
 # Using a @prevent_stack_overflow decorator here to avoid infinite recursion
 # in case we load stack exports that have circular dependencies (see issue 3438)
 # TODO: Potentially think about a better approach in the future
 @prevent_stack_overflow(match_parameters=True)
-def resolve_refs_recursively(stack_name: str, resources: dict, mappings: dict, value):
-    result = _resolve_refs_recursively(stack_name, resources, mappings, value)
+def resolve_refs_recursively(
+    stack_name: str,
+    resources: dict,
+    mappings: dict,
+    conditions: dict[str, bool],
+    parameters: dict,
+    value,
+):
+    result = _resolve_refs_recursively(
+        stack_name, resources, mappings, conditions, parameters, value
+    )
 
     # localstack specific patches
     if isinstance(result, str):
         # we're trying to filter constructed API urls here (e.g. via Join in the template)
         api_match = REGEX_OUTPUT_APIGATEWAY.match(result)
         if api_match:
             prefix = api_match[1]
@@ -402,39 +387,54 @@
                 LOG.warning(f"Unsupported service for dynamic parameter: {service_name=}")
 
     return result
 
 
 @prevent_stack_overflow(match_parameters=True)
 def _resolve_refs_recursively(
-    stack_name: str, resources: dict, mappings: dict, value: dict | list | str | bytes | None
+    stack_name: str,
+    resources: dict,
+    mappings: dict,
+    conditions: dict,
+    parameters: dict,
+    value: dict | list | str | bytes | None,
 ):
     if isinstance(value, dict):
         keys_list = list(value.keys())
         stripped_fn_lower = keys_list[0].lower().split("::")[-1] if len(keys_list) == 1 else None
 
         # process special operators
         if keys_list == ["Ref"]:
-            ref = resolve_ref(stack_name, resources, mappings, value["Ref"], attribute="Ref")
+            ref = resolve_ref(
+                stack_name,
+                resources,
+                mappings,
+                conditions,
+                parameters,
+                value["Ref"],
+                attribute="Ref",
+            )
             if ref is None:
                 msg = 'Unable to resolve Ref for resource "%s" (yet)' % value["Ref"]
                 LOG.debug("%s - %s", msg, resources.get(value["Ref"]) or set(resources.keys()))
                 raise DependencyNotYetSatisfied(resource_ids=value["Ref"], message=msg)
-            ref = resolve_refs_recursively(stack_name, resources, mappings, ref)
+            ref = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, ref
+            )
             return ref
 
         if stripped_fn_lower == "getatt":
             attr_ref = value[keys_list[0]]
             attr_ref = attr_ref.split(".") if isinstance(attr_ref, str) else attr_ref
             resource_logical_id = attr_ref[0]
             attribute_name = attr_ref[1]
 
             # the attribute name can be a Ref
             attribute_name = resolve_refs_recursively(
-                stack_name, resources, mappings, attribute_name
+                stack_name, resources, mappings, conditions, parameters, attribute_name
             )
             resource = resources.get(resource_logical_id)
 
             resolved_getatt = get_attr_from_model_instance(
                 resource, attribute_name, get_resource_type(resource)
             )
             # TODO: we should check the deployment state and not try to GetAtt from a resource that is still IN_PROGRESS or hasn't started yet.
@@ -443,18 +443,21 @@
             return resolved_getatt
 
         if stripped_fn_lower == "join":
             join_values = value[keys_list[0]][1]
 
             # this can actually be another ref that produces a list as output
             if isinstance(join_values, dict):
-                join_values = resolve_refs_recursively(stack_name, resources, mappings, join_values)
+                join_values = resolve_refs_recursively(
+                    stack_name, resources, mappings, conditions, parameters, join_values
+                )
 
             join_values = [
-                resolve_refs_recursively(stack_name, resources, mappings, v) for v in join_values
+                resolve_refs_recursively(stack_name, resources, mappings, conditions, parameters, v)
+                for v in join_values
             ]
 
             none_values = [v for v in join_values if v is None]
             if none_values:
                 raise Exception(
                     "Cannot resolve CF fn::Join %s due to null values: %s" % (value, join_values)
                 )
@@ -466,51 +469,63 @@
             attr_refs = {r: {"Ref": r} for r in STATIC_REFS}
             if not isinstance(item_to_sub, list):
                 item_to_sub = [item_to_sub, {}]
             result = item_to_sub[0]
             item_to_sub[1].update(attr_refs)
 
             for key, val in item_to_sub[1].items():
-                val = resolve_refs_recursively(stack_name, resources, mappings, val)
+                val = resolve_refs_recursively(
+                    stack_name, resources, mappings, conditions, parameters, val
+                )
                 result = result.replace("${%s}" % key, val)
 
             # resolve placeholders
-            result = resolve_placeholders_in_string(result, stack_name, resources, mappings)
+            result = resolve_placeholders_in_string(
+                result, stack_name, resources, mappings, conditions, parameters
+            )
             return result
 
         if stripped_fn_lower == "findinmap":
             # "Fn::FindInMap"
             mapping_id = value[keys_list[0]][0]
 
             if isinstance(mapping_id, dict) and "Ref" in mapping_id:
                 # TODO: ??
-                mapping_id = resolve_ref(stack_name, resources, mappings, mapping_id["Ref"], "Ref")
+                mapping_id = resolve_ref(
+                    stack_name,
+                    resources,
+                    mappings,
+                    conditions,
+                    parameters,
+                    mapping_id["Ref"],
+                    "Ref",
+                )
 
             selected_map = mappings.get(mapping_id)
             if not selected_map:
                 raise Exception(
                     f"Cannot find Mapping with ID {mapping_id} for Fn::FindInMap: {value[keys_list[0]]} {list(resources.keys())}"  # TODO: verify
                 )
 
             first_level_attribute = value[keys_list[0]][1]
             first_level_attribute = resolve_refs_recursively(
-                stack_name, resources, mappings, first_level_attribute
+                stack_name, resources, mappings, conditions, parameters, first_level_attribute
             )
 
             second_level_attribute = value[keys_list[0]][2]
             if not isinstance(second_level_attribute, str):
                 second_level_attribute = resolve_refs_recursively(
-                    stack_name, resources, mappings, second_level_attribute
+                    stack_name, resources, mappings, conditions, parameters, second_level_attribute
                 )
 
             return selected_map.get(first_level_attribute).get(second_level_attribute)
 
         if stripped_fn_lower == "importvalue":
             import_value_key = resolve_refs_recursively(
-                stack_name, resources, mappings, value[keys_list[0]]
+                stack_name, resources, mappings, conditions, parameters, value[keys_list[0]]
             )
             exports = exports_map()
             stack_export = exports.get(import_value_key) or {}
             if not stack_export.get("Value"):
                 LOG.info(
                     'Unable to find export "%s" in stack "%s", existing export names: %s',
                     import_value_key,
@@ -518,99 +533,137 @@
                     list(exports.keys()),
                 )
                 return None
             return stack_export["Value"]
 
         if stripped_fn_lower == "if":
             condition, option1, option2 = value[keys_list[0]]
-            condition = evaluate_condition(stack_name, resources, mappings, condition)
+            condition = conditions[condition]
             result = resolve_refs_recursively(
-                stack_name, resources, mappings, option1 if condition else option2
+                stack_name,
+                resources,
+                mappings,
+                conditions,
+                parameters,
+                option1 if condition else option2,
             )
             return result
 
         if stripped_fn_lower == "condition":
             # FIXME: this should only allow strings, no evaluation should be performed here
             #   see https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-condition.html
-            result = evaluate_condition(stack_name, resources, mappings, value[keys_list[0]])
-            return result
+            return conditions[value[keys_list[0]]]
 
         if stripped_fn_lower == "not":
             condition = value[keys_list[0]][0]
-            condition = resolve_refs_recursively(stack_name, resources, mappings, condition)
+            condition = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, condition
+            )
             return not condition
 
         if stripped_fn_lower in ["and", "or"]:
             conditions = value[keys_list[0]]
             results = [
-                resolve_refs_recursively(stack_name, resources, mappings, cond)
+                resolve_refs_recursively(
+                    stack_name, resources, mappings, conditions, parameters, cond
+                )
                 for cond in conditions
             ]
             result = all(results) if stripped_fn_lower == "and" else any(results)
             return result
 
         if stripped_fn_lower == "equals":
             operand1, operand2 = value[keys_list[0]]
-            operand1 = resolve_refs_recursively(stack_name, resources, mappings, operand1)
-            operand2 = resolve_refs_recursively(stack_name, resources, mappings, operand2)
+            operand1 = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, operand1
+            )
+            operand2 = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, operand2
+            )
             # TODO: investigate type coercion here
             return fn_equals_type_conversion(operand1) == fn_equals_type_conversion(operand2)
 
         if stripped_fn_lower == "select":
             index, values = value[keys_list[0]]
-            index = resolve_refs_recursively(stack_name, resources, mappings, index)
-            values = resolve_refs_recursively(stack_name, resources, mappings, values)
+            index = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, index
+            )
+            values = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, values
+            )
             try:
                 return values[index]
             except TypeError:
                 return values[int(index)]
 
         if stripped_fn_lower == "split":
             delimiter, string = value[keys_list[0]]
-            delimiter = resolve_refs_recursively(stack_name, resources, mappings, delimiter)
-            string = resolve_refs_recursively(stack_name, resources, mappings, string)
+            delimiter = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, delimiter
+            )
+            string = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, string
+            )
             return string.split(delimiter)
 
         if stripped_fn_lower == "getazs":
             region = (
-                resolve_refs_recursively(stack_name, resources, mappings, value["Fn::GetAZs"])
+                resolve_refs_recursively(
+                    stack_name, resources, mappings, conditions, parameters, value["Fn::GetAZs"]
+                )
                 or aws_stack.get_region()
             )
             azs = []
             for az in ("a", "b", "c", "d"):
                 azs.append("%s%s" % (region, az))
 
             return azs
 
         if stripped_fn_lower == "base64":
             value_to_encode = value[keys_list[0]]
             value_to_encode = resolve_refs_recursively(
-                stack_name, resources, mappings, value_to_encode
+                stack_name, resources, mappings, conditions, parameters, value_to_encode
             )
             return to_str(base64.b64encode(to_bytes(value_to_encode)))
 
         for key, val in dict(value).items():
-            value[key] = resolve_refs_recursively(stack_name, resources, mappings, val)
+            value[key] = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, val
+            )
 
     if isinstance(value, list):
         # in some cases, intrinsic functions are passed in as, e.g., `[['Fn::Sub', '${MyRef}']]`
         if len(value) == 1 and isinstance(value[0], list) and len(value[0]) == 2:
             inner_list = value[0]
             if str(inner_list[0]).lower().startswith("fn::"):
                 return resolve_refs_recursively(
-                    stack_name, resources, mappings, {inner_list[0]: inner_list[1]}
+                    stack_name,
+                    resources,
+                    mappings,
+                    conditions,
+                    parameters,
+                    {inner_list[0]: inner_list[1]},
                 )
 
         for i in range(len(value)):
-            value[i] = resolve_refs_recursively(stack_name, resources, mappings, value[i])
+            value[i] = resolve_refs_recursively(
+                stack_name, resources, mappings, conditions, parameters, value[i]
+            )
 
     return value
 
 
-def resolve_placeholders_in_string(result, stack_name: str, resources: dict, mappings: dict):
+def resolve_placeholders_in_string(
+    result,
+    stack_name: str,
+    resources: dict,
+    mappings: dict,
+    conditions: dict[str, bool],
+    parameters: dict,
+):
     """
     Resolve individual Fn::Sub variable replacements
 
     Variables can be template parameter names, resource logical IDs, resource attributes, or a variable in a key-value map
     """
 
     def _replace(match):
@@ -629,52 +682,63 @@
                 raise DependencyNotYetSatisfied(
                     resource_ids=resource_name,
                     message=f"Unable to resolve attribute ref {ref_expression}",
                 )
             if not isinstance(resolved, str):
                 resolved = str(resolved)
             return resolved
-        if len(parts) == 1 and parts[0] in resources:
-            # Logical resource ID or parameter name specified => Use Ref for lookup
-            result = resolve_ref(stack_name, resources, mappings, parts[0], "Ref")
+        if len(parts) == 1:
+            if parts[0] in resources:
+                # Logical resource ID or parameter name specified => Use Ref for lookup
+                result = resolve_ref(
+                    stack_name, resources, mappings, conditions, parameters, parts[0], "Ref"
+                )
 
-            if result is None:
+                if result is None:
+                    raise DependencyNotYetSatisfied(
+                        resource_ids=parts[0],
+                        message=f"Unable to resolve attribute ref {ref_expression}",
+                    )
+                # TODO: is this valid?
+                # make sure we resolve any functions/placeholders in the extracted string
+                result = resolve_refs_recursively(
+                    stack_name, resources, mappings, conditions, parameters, result
+                )
+                # make sure we convert the result to string
+                # TODO: do this more systematically
+                result = "" if result is None else str(result)
+                return result
+            elif parts[0] in parameters:
+                parameter = parameters[parts[0]]
+                parameter_type: str = parameter["ParameterType"]
+                parameter_value = parameter.get("ResolvedValue") or parameter.get("ParameterValue")
+
+                if parameter_type in ["CommaDelimitedList"] or parameter_type.startswith("List<"):
+                    return [p.strip() for p in parameter_value.split(",")]
+                else:
+                    return parameter_value
+            else:
                 raise DependencyNotYetSatisfied(
                     resource_ids=parts[0],
                     message=f"Unable to resolve attribute ref {ref_expression}",
                 )
-            # TODO: is this valid?
-            # make sure we resolve any functions/placeholders in the extracted string
-            result = resolve_refs_recursively(stack_name, resources, mappings, result)
-            # make sure we convert the result to string
-            result = "" if result is None else str(result)
-            return result
         # TODO raise exception here?
         return match.group(0)
 
     regex = r"\$\{([^\}]+)\}"
     result = re.sub(regex, _replace, result)
     return result
 
 
-def evaluate_condition(stack_name: str, resources: dict, mappings: dict, condition: str) -> bool:
-    condition = resolve_refs_recursively(stack_name, resources, mappings, condition)
-    condition = resolve_ref(stack_name, resources, mappings, condition, attribute="Ref")
-    condition = resolve_refs_recursively(stack_name, resources, mappings, condition)
-    return condition
-
-
 def evaluate_resource_condition(
-    stack_name: str, resources: dict, mappings: dict, resource: dict
+    stack_name: str, resources: dict, mappings: dict, conditions: dict[str, bool], resource: dict
 ) -> bool:
     condition = resource.get("Condition")
     if condition:
-        condition = evaluate_condition(stack_name, resources, mappings, condition)
-        if condition is False or condition in FALSE_STRINGS or is_none_or_empty_value(condition):
-            return False
+        return conditions.get(condition, True)
     return True
 
 
 # TODO: move (registry/util)
 def get_resource_model_instance(resource_id: str, resources) -> Optional[GenericBaseModel]:
     """Obtain a typed resource entity instance representing the given stack resource."""
     resource = resources[resource_id]
@@ -896,15 +960,19 @@
             }
             if len(resources) == 0:
                 break
             for resource_id, resource in resources.items():
                 try:
                     # TODO: cache condition value in resource details on deployment and use cached value here
                     if evaluate_resource_condition(
-                        self.stack_name, self.resources, self.mappings, resource
+                        self.stack_name,
+                        self.resources,
+                        self.mappings,
+                        self.stack.resolved_conditions,
+                        resource,
                     ):
                         executor = self.create_resource_provider_executor()
                         resource_provider_payload = self.create_resource_provider_payload(
                             "Remove", logical_resource_id=resource_id
                         )
                         executor.deploy_loop(resource_provider_payload)  # noqa
                         self.stack.set_resource_status(resource_id, "DELETE_COMPLETE")
@@ -932,15 +1000,15 @@
     # ----------------------------
     # DEPENDENCY RESOLUTION UTILS
     # ----------------------------
 
     def is_deployable_resource(self, resource):
         resource_type = get_resource_type(resource)
         entry = get_deployment_config(resource_type)
-        if entry is None and resource_type not in ["Parameter", None]:
+        if entry is None:
             resource_str = dump_resource_as_json(resource)
             LOG.warning(f'Unable to deploy resource type "{resource_type}": {resource_str}')
         return bool(entry and entry.get(ACTION_CREATE))
 
     def is_deployed(self, resource):
         # TODO: make this a check on the actual resource status instead(!)
         resource_status = {}
@@ -960,16 +1028,20 @@
         return resource_instance.is_updatable()
 
     def all_resource_dependencies_satisfied(self, resource) -> bool:
         unsatisfied = self.get_unsatisfied_dependencies(resource)
         return not unsatisfied
 
     def get_unsatisfied_dependencies(self, resource):
-        res_deps = self.get_resource_dependencies(resource)
-        res_deps_mapped = {v: self.stack.resources.get(v) for v in res_deps}
+        res_deps = self.get_resource_dependencies(
+            resource
+        )  # the output here is currently a set of merged IDs from both resources and parameters
+        parameter_deps = {d for d in res_deps if d in self.stack.resolved_parameters}
+        resource_deps = res_deps.difference(parameter_deps)
+        res_deps_mapped = {v: self.stack.resources.get(v) for v in resource_deps}
         return self.get_unsatisfied_dependencies_for_resources(res_deps_mapped, resource)
 
     def get_unsatisfied_dependencies_for_resources(
         self, resources, depending_resource=None, return_first=True
     ):
         result = {}
         for resource_id, resource in resources.items():
@@ -1318,23 +1390,30 @@
         resource = new_resources[resource_id]
         res_change = change["ResourceChange"]
         action = res_change["Action"]
 
         # TODO: this needs to happen much earlier
         # check resource condition, if present
         if not evaluate_resource_condition(
-            stack.stack_name, stack.resources, stack.mappings, resource
+            stack.stack_name, stack.resources, stack.mappings, stack.resolved_conditions, resource
         ):
             LOG.debug(
                 'Skipping deployment of "%s", as resource condition evaluates to false', resource_id
             )
             return
 
         # resolve refs in resource details
-        resolve_refs_recursively(stack.stack_name, stack.resources, stack.mappings, resource)
+        resolve_refs_recursively(
+            stack.stack_name,
+            stack.resources,
+            stack.mappings,
+            stack.resolved_conditions,
+            stack.resolved_parameters,
+            resource,
+        )
 
         if action in ["Add", "Modify"]:
             if action == "Add" and not self.is_deployable_resource(resource):
                 return False
             is_deployed = self.is_deployed(resource)
             # TODO: Attaching the cached _deployed info here, as we should not change the "Add"/"Modify" attribute
             #  here, which is used further down the line to determine the resource action CREATE/UPDATE. This is a
@@ -1365,15 +1444,17 @@
         action = change_details["Action"]
         resource_id = change_details["LogicalResourceId"]
         resources = stack.resources
         resource = resources[resource_id]
 
         # TODO: this should not be needed as resources are filtered out if the
         # condition evaluates to False.
-        if not evaluate_resource_condition(stack.stack_name, resources, stack.mappings, resource):
+        if not evaluate_resource_condition(
+            stack.stack_name, resources, stack.mappings, stack.resolved_conditions, resource
+        ):
             return
 
         # remove AWS::NoValue entries
         resource_props = resource.get("Properties")
         if resource_props:
             resource["Properties"] = remove_none_values(resource_props)
 
@@ -1438,24 +1519,38 @@
 
 # FIXME: resolve_refs_recursively should not be needed, the resources themselves should have those values available already
 def resolve_outputs(stack) -> list[dict]:
     result = []
     for k, details in stack.outputs.items():
         value = None
         try:
-            resolve_refs_recursively(stack.stack_name, stack.resources, stack.mappings, details)
+            resolve_refs_recursively(
+                stack.stack_name,
+                stack.resources,
+                stack.mappings,
+                stack.resolved_conditions,
+                stack.resolved_parameters,
+                details,
+            )
             value = details["Value"]
         except Exception as e:
             log_method = getattr(LOG, "debug")
             if config.CFN_VERBOSE_ERRORS:
                 log_method = getattr(LOG, "exception")
             log_method("Unable to resolve references in stack outputs: %s - %s", details, e)
         exports = details.get("Export") or {}
         export = exports.get("Name")
-        export = resolve_refs_recursively(stack.stack_name, stack.resources, stack.mappings, export)
+        export = resolve_refs_recursively(
+            stack.stack_name,
+            stack.resources,
+            stack.mappings,
+            stack.resolved_conditions,
+            stack.resolved_parameters,
+            export,
+        )
         description = details.get("Description")
         entry = {
             "OutputKey": k,
             "OutputValue": value,
             "Description": description,
             "ExportName": export,
         }
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,29 @@
 def template_to_json(template: str) -> str:
     template = parse_template(template)
     return json.dumps(template)
 
 
 # TODO: consider moving to transformers.py as well
 def transform_template(
-    template: dict, parameters: list, stack_name: str, resources: dict, mappings: dict
+    template: dict,
+    parameters: list,
+    stack_name: str,
+    resources: dict,
+    mappings: dict,
+    conditions: dict[str, bool],
+    resolved_parameters: dict,
 ) -> dict:
     result = dict(template)
 
     # apply 'Fn::Transform' intrinsic functions (note: needs to be applied before global
     #  transforms below, as some utils - incl samtransformer - expect them to be resolved already)
-    result = apply_transform_intrinsic_functions(result, stack_name, resources, mappings)
+    result = apply_transform_intrinsic_functions(
+        result, stack_name, resources, mappings, conditions, resolved_parameters
+    )
 
     # apply global transforms
     transformations = format_transforms(result.get("Transform", []))
     for transformation in transformations:
         if not isinstance(transformation["Name"], str):
             # TODO this should be done during template validation
             raise CommonServiceException(
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/template_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/template_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,18 +146,28 @@
                         )  # TODO: this pseudo parameter resolving needs context(!)
                     # TODO: add util function for resolving individual refs (e.g. one util for resolving pseudo parameters)
                     # TODO: pseudo-parameters like AWS::Region
                     # can only really be a parameter here
                     # TODO: how are conditions references written here? as {"Condition": "ConditionA"} or via Ref?
                     # TODO: test for a boolean parameter?
                     param = parameters[v]
-                    return param[
-                        "ParameterValue"
-                    ]  # TODO: extend this logic, e.g. what about lists, other types, ... why is string interpreted as a boolean?
-                    # return parameters[v]
+                    parameter_type: str = param["ParameterType"]
+                    parameter_value = param.get("ResolvedValue") or param.get("ParameterValue")
+
+                    if parameter_type in ["CommaDelimitedList"] or parameter_type.startswith(
+                        "List<"
+                    ):
+                        return [p.strip() for p in parameter_value.split(",")]
+                    else:
+                        return parameter_value
+
+                case "Condition":
+                    return resolve_condition(
+                        conditions[v], conditions, parameters, mappings, stack_name
+                    )
                 case "Fn::FindInMap":
                     map_name, top_level_key, second_level_key = v
                     return mappings[map_name][top_level_key][second_level_key]
                 case "Fn::If":
                     if_condition_name, true_branch, false_branch = v
                     if resolve_condition(
                         if_condition_name, conditions, parameters, mappings, stack_name
@@ -180,14 +190,29 @@
                     return resolve_condition(
                         v[0], conditions, parameters, mappings, stack_name
                     ) or resolve_condition(v[1], conditions, parameters, mappings, stack_name)
                 case "Fn::Equals":
                     left = resolve_condition(v[0], conditions, parameters, mappings, stack_name)
                     right = resolve_condition(v[1], conditions, parameters, mappings, stack_name)
                     return fn_equals_type_conversion(left) == fn_equals_type_conversion(right)
+                case "Fn::Join":
+                    join_list = v[1]
+                    if isinstance(v[1], dict):
+                        join_list = resolve_condition(
+                            v[1], conditions, parameters, mappings, stack_name
+                        )
+                    result = v[0].join(
+                        [
+                            resolve_condition(x, conditions, parameters, mappings, stack_name)
+                            for x in join_list
+                        ]
+                    )
+                    return result
+                case _:
+                    raise Exception(f"Invalid condition structure encountered: {condition=}")
     else:
         return condition
 
 
 def fn_equals_type_conversion(value) -> str:
     if isinstance(value, str):
         return value
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/transformers.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,25 +36,32 @@
 
 
 # maps transformer names to implementing classes
 transformers: Dict[str, Type] = {"AWS::Include": AwsIncludeTransformer}
 
 
 def apply_transform_intrinsic_functions(
-    template: dict, stack_name: str, resources: dict, mappings: dict
+    template: dict,
+    stack_name: str,
+    resources: dict,
+    mappings: dict,
+    conditions: dict[str, bool],
+    stack_parameters: dict,
 ) -> dict:
     """Resolve constructs using the 'Fn::Transform' intrinsic function."""
     from localstack.services.cloudformation.engine.template_deployer import resolve_refs_recursively
 
     def _visit(obj, **_):
         if isinstance(obj, dict) and obj.keys() == {"Fn::Transform"}:
             transform = obj["Fn::Transform"]
             transform_name = transform.get("Name")
             transformer_class = transformers.get(transform_name)
             if transformer_class:
                 transformer = transformer_class()
                 parameters = transform.get("Parameters") or {}
-                parameters = resolve_refs_recursively(stack_name, resources, mappings, parameters)
+                parameters = resolve_refs_recursively(
+                    stack_name, resources, mappings, conditions, stack_parameters, parameters
+                )
                 return transformer.transform(parameters)
         return obj
 
     return recurse_object(template, _visit)
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/types.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,16 @@
         try:
             template = template_preparer.transform_template(
                 template,
                 list(resolved_parameters.values()),
                 stack.stack_name,
                 stack.resources,
                 stack.mappings,
+                {},  # TODO
+                resolved_parameters,
             )
         except FailedTransformationException as e:
             stack.add_stack_event(
                 stack.stack_name,
                 stack.stack_id,
                 status="ROLLBACK_IN_PROGRESS",
                 status_reason=e.message,
@@ -294,21 +296,30 @@
         parameter_declarations = param_resolver.extract_stack_parameter_declarations(template)
         resolved_parameters = param_resolver.resolve_parameters(
             parameter_declarations=parameter_declarations,
             new_parameters=new_parameters,
             old_parameters=stack.resolved_parameters,
         )
 
+        resolved_stack_conditions = resolve_stack_conditions(
+            conditions=template.get("Conditions", {}),
+            parameters=resolved_parameters,
+            mappings=template.get("Mappings", {}),
+            stack_name=stack_name,
+        )
+
         try:
             template = template_preparer.transform_template(
                 template,
                 list(resolved_parameters.values()),
                 stack.stack_name,
                 stack.resources,
                 stack.mappings,
+                resolved_stack_conditions,
+                resolved_parameters,
             )
         except FailedTransformationException as e:
             stack.add_stack_event(
                 stack.stack_name,
                 stack.stack_id,
                 status="ROLLBACK_IN_PROGRESS",
                 status_reason=e.message,
@@ -317,14 +328,15 @@
             return CreateStackOutput(StackId=stack.stack_id)
 
         deployer = template_deployer.TemplateDeployer(stack)
         # TODO: there shouldn't be a "new" stack on update
         new_stack = Stack(request, template)
         new_stack.set_resolved_parameters(resolved_parameters)
         stack.set_resolved_parameters(resolved_parameters)
+        stack.set_resolved_stack_conditions(resolved_stack_conditions)
         try:
             deployer.update_stack(new_stack)
         except Exception as e:
             stack.set_stack_status("UPDATE_FAILED")
             msg = f'Unable to update stack "{stack_name}": {e}'
             LOG.exception("%s", msg)
             raise ValidationError(msg) from e
@@ -553,14 +565,16 @@
         # apply template transformations
         transformed_template = template_preparer.transform_template(
             template,
             parameters,
             stack_name=temp_stack.stack_name,
             resources=temp_stack.resources,
             mappings=temp_stack.mappings,
+            conditions={},  # TODO: we don't have any resolved conditions yet at this point but we need the conditions because of the samtranslator...
+            resolved_parameters=resolved_parameters,
         )
 
         # create change set for the stack and apply changes
         change_set = StackChangeSet(stack, req_params, transformed_template)
         # only set parameters for the changeset, then switch to stack on execute_change_set
         change_set.set_resolved_parameters(resolved_parameters)
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/provider_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/resource_provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack-core-2.1.1.dev20230713205536/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/provider_stream.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/provider_stream.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack-core-2.1.1.dev20230713205536/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230713205536/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/state/core.py` & `localstack-core-2.1.1.dev20230713205536/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230713205536/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230713205536/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230713205536/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230713205536/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230713205536/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230713161930
+Version: 2.1.1.dev20230713205536
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8516569200779727%*

 * *Differences: {"'localstack.hooks.configure_localstack_container'": '{insert: [(1, '*

 * *                                                      "'_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file')], "*

 * *                                                      'delete: [0]}',*

 * * "'localstack.hooks.on_infra_ready'": '{insert: [(1, '*

 * *                                      "'_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready')], "*

 * *                                      'delete: [0]}',*

 * * […]*

```diff
@@ -47,48 +47,48 @@
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.cloudformation.resource_providers": [
         "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user:IAMUserProviderPlugin",
         "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter:SSMParameterProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
-        "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file",
-        "configure_edge_port=localstack.plugins:configure_edge_port"
+        "configure_edge_port=localstack.plugins:configure_edge_port",
+        "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
     ],
     "localstack.hooks.on_infra_ready": [
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
+        "terraform/community=localstack.packages.plugins:terraform_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package"
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230713161930/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230713205536/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/pyproject.toml` & `localstack-core-2.1.1.dev20230713205536/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230713161930/setup.cfg` & `localstack-core-2.1.1.dev20230713205536/setup.cfg`

 * *Files identical despite different names*

