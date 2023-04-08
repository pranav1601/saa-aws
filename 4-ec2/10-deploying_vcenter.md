## VMware on AWS

* used by orgs for private cloud deployment
* opt for hybrid cloud strategy nd would like to leverage AWS services.

## uses

* hybrid cloud -> connect on premise to AWS cloud and manage hybrid cloud
* migrate existing cloud env to AWS using VMwasre built in tools
* using hybridd cloud you can have inexpensive disaster recovery environemet on AWS
* use aws services to upadate apps or use new ones

## deployment

* runs on dedicated hardware hosted in AWS using single AWS account
* each host has two sockets with 18 cores per socket, 512 GB RAM and 15.2 raw ssd storage
* each host caapable of running muiltiple VMware instances(ipto hundreds)
* clusters can start with two hosts up to maximum 16 hosts per cluster

> you can deploy vCenter on the AWS using VMware
>
> perfect solutouiin for extetending your private VMwware cloud into the AWS public cloud