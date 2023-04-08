## aws batch

- run batch computing workloads (run on ec2 or ecs/fargate)
- removes heavy lifting for configuration and managements of infrastructurure
- automatically provision and scaled - based on number of jobs submitted and optimizes the distribution of workloads
- allows you to skip installatoin and maintenance of batch computing software, so you can focus on obtaining and analyzing the results

## components

1. jobs - units of work submitted to AWS batch eg shell scripts, executables, docker images
2. job definintions - how your jobs are to be run - blueprint for the resources
3. job queues - jobs get submiited to specific queus where they wait to be done according to the schedule
4. compute environment - managed or munmanaged compute resources used to run your jobs

## fargate/ecs ec2 env

* fargate recommended way of laumnching most batch jobs
* sometimes ec2 best choce - custom AMI
* - needing more that 4 vxpu
* - more than 30 gb of memory
* - if jobs require a GPU, arm based gravitation CPU can only be leveraged via EC2 for aws batch
* - linux parameters
* - when large number of jobs , dispatched at higher rate

## aws batch/lambda

- time limits - lambda has 15 mins
- disk space - limited disk space and efs requires funcitons live within a vpc in lambda
- runtime limitations - fully serverless but it has nativelly limited rntimes
- batch runtimes - batch uses odcker, so any runtime can be used 

## managed vs unmanaged compute environments

![managed vs umanaged](../images/managed_unmanaged.png)

> long running and event driver workloads, more than 15 mins - aws batch
>
> managed service