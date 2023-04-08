## placement groups

* 3 types

### cluster placement groups

* grouping instances within a single AZ
* apps that need low network latency, high network throughput or both
* only certain instance types can be launched into a cluster placement group


## spread placement grroup

* each placed on distinct underlying hardware
* apps that have a small number of critical instances that should be kept separate from eachother
* used for individual instances

### partition placement groups

* each partition has its own set of racks.
* each rack has its own network and power source
* no two partitions within a placement group share same racks, allowing to isolate imapact of hardware failurte within your application
* ec3 divides each group into logical segments called partitions
* used for multiple instances 

> cluster -> low lnetwork latency, high network throughput
>
> spread -> individual critical ec2 instances
>
> partition -> multiple ec2 instances, HDFS, HBase, Cassandra
>
> a cluster placement group cant span across multiple AZs but a spread and partition can
>
> only certain types of instances can be launched in aplacement group (compute optimizded, gpu, memory optimized, storage optimized)
>
> aws recommends homogenuous instances within cluster placement groups
>
> cant merge placement groups
>
> move an existing instance into a placemenent group. but before you move instance bust be in stopped state. you can move or remove using AWS cLI or AWS SDJ+K but not via the console yet