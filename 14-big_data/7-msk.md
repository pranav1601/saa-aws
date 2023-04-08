## msk

- fully mnanaged service for running data steaming applications that leverage apache kafka
- control pane - creates, updates, deletes clusters as required
- data plane - leverage kafka data-plane operations for produincg and consuiming streaming data
- existing apps - open source version of apache kafka allow support for existing apps, tools and plugins

## compnnents

- broker nods - amount of broker nodes per az
- zookeeper nodes - createed for you
- producers, consumers and topics - kafka data-plane operations allow creation of topics and ability to produce/consume data
- flexible cluster operations - perform cluster operations with the console, aws cli or APIs within SDK

## resilience

- autoamtic recovery - automatic detection and recovery
- detections- detect broker failures resulting n mitigation/replacement of unhealthy nodes
- reduce data - tries to reuse storage from older brokers suring failures to redce data needing replication
- time required - impact time is limited to however long it takes amazon msk to complete detection and recovery
- after recovery - after successful recovery, producer and consumer aps continue to communicate with the same broker ip as before

## features

- msk serverless - within msk offering serverless cluster management
- fully compatible - fully compatible with apache kafka. use the same client apps for producing and consuming data
- msk connect - allows developers to asily stream data to and from apache kafka clusters

## security and logging

- uintegrate with kms for see requirements
- encryption at rest by default
- tls 1.2 for encryption in transit between brokers in clusters
- deliver broker logs to cloudwatch, s3, kinesissis data firehose
- metrics are gatheererd and sent to CW
- all msk api calls are logged to cloudtrail

> runnning and building kfka data stereaming apps
>
> kafka - msk