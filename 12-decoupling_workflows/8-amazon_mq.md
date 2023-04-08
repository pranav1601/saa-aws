## MQ

- mamanged messaging broker
- message broker - allowing easier migration of existing apps to cloud
- variety - leverages multiple programming languages, operating systems and messaging protocols
- engine types - supports both apache activemq or rabbitmq
- managed service

## sqs with sns vs MQ

- both have topics and quesus. allows one to one and one to many
- if migrate consider MQ
- if new application, use sns with sqs. simple, scalable 
- MQ - private networking like VPC, direect connect or VPN. SNS and SQS are publicly accessible by default
- MS has no default AWS integrations

## configuring brokers

- one brokerin 1 AZ, dev environments, Rabbit MQ has NLB in front
- highly available arch to minimize downtimes. arch depends on broker engine type
- with active.standby deployoments, one instance will remain available at all times.
- MQ fro RabbitMQ- cluster deplpoyments are logical grouping s of three roerker nodes across multiple AXz sitting behind a network load balancer

> managed broker service for easily migrating message roker systems to the AWS cloud
>
> anything specific to JMS or messaging protocols like AMQP 091, AMQP 1, MQTT, openwire and stomp (cant be handled by sns/sqs)
>
> apachemq or rabbit mq -  AWS MQ