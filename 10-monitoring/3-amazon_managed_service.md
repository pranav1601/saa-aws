## amazon managed grafana

* grafana - visualize data for instantly querying, correlating and nd visualizing your operational metrics, logs and traces from different sources
* easil deploy operate and scare grafana
* workspaces allow for separation of data visualuisations
* completely aws managed, only worry about tasks
* secureity freatures help meet corporate governance and compliant requirements
* pricising is based per active user in a workspace
* data sources - integrate with serveral sources including cloudwatch, prometheus, opensearch, timestream

## uses

* container metric vis - promethus for visualie eks,ecs or kubernetes
* IOT - vast plugins make the service perfect for monitoring IOT and edge device data
* troubleshooting - centralised dashboard allows for morte efficient operational issue troubleshooting

## service for promotheuus

* serverless, promotheus compatible service used for securely monitoring container metrics at scale
* leerage open source promotheus data model wuth aws managed scaling anad availability
* automatic scaaling - aws manages automatic scaling based on ingestion, storage and querying of metrics
* high availabiltiy - replicates data scross 3 AZs. designed for availability
* works with AMazon eks or self managed kuberntes clusters
* PromQL - leverage open soyrce promql query language for exploring and extracting data
* data is stpred in workspaces for 150 days and then automatically deleted

> both services let aws manage high availability and automatic scaling. leverage vpc endpoint for secure vpc access
>
> several built in sourcescloudwatch, promotheus, X-ra
