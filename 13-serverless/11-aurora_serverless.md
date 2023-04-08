## surora serverless

- on demand and sutoscaling config for surora db
- automating of monitoring workloads and ajusting capacity
- based on demand
- charged only for resources consumedby db clusters, per scond billing
- budget freindly

## concepts

- aurora capacity units - measurements how your clusters scale
- set max and min of ACU
- allocated by aws managed warm pools
- combination of 3gb, matching cpu and netork caapability
- same data resiliency as aurora provisioned- 5 copies of data across 3 azs
- mutli az deployment for establishing highly available clusters

## uses

- variable workloads
- multi tenant apps - let service manage db capacity for each app
- new apps where db instance required
- dev or testing of new feature
- app might server more than one purpose with different rtraffic spoles
- easily swapped from provisioned to serverless

> on demand auto scaling version
>
> ACU
>
> variable workloads, new applications, capacity planning, development/testing needs