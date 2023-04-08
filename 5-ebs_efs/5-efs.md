## efs

* amazon elastic fles systen
* managed nfs that can be mounted to many ec 2 instances
* efs works with ec2 in multi AXs
* hihgly available and scalable but it is expensive

## uses

* content management - easily share content between ec2 instances
* web servers - have just a single folder structure for your website

* uses nfsv4 protocol
* compatibel with linux, not windows
* encryption at rest using kms
* file system scales automatically
* pay per use
* 1000s of concurrent connections
* 10gbps throughput
* scaled to petabytes

## controlling performance

* general purpros - web server
* max io - big data, media processing

## sotrage tiers

* comes with storage tiers and lifecycle managementma allowing to move data from one tier to another after x number of days
1. standard - frequently accessed
2. infrequently accessed - not frequently accessed

> supports nfs v5 protocol
>
> pay for storage you use
>
> scale to petabytes
>
> 1000s of concurrent connections
>
> data stored across multiple AZs
>
> read after write consistency
>
> highly scalable shared storage using nfs -> efs