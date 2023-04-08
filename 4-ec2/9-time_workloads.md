## spot instances

* unused ec2 capacity in the AWS cloud.
* 90% discount on on demand

## use case

* stateless, fault tolerant, felxible. Wont use in web servers cuz they run all the time. used in big data appps, cicd, other test and devleopmnent workloads

## how

* decie max spot price. the instanve will be provisioned so long as the spot price is below the maximum spot price
* depends on capacity and region
* when it goes above max, you have 2 min s to stop/terminate the instance
* spot block - stop your spot instanves from being terminated even in if the price goes above max spot price
* set it to 1-6 hours

## pricing history

* you can check princing history on the console

## uses

* big data and analytics
* containerized workloads
* cicd testing
* image and media rendering
* High perforance computing

## not uses

* persistent workloads
* critical jobs
* databases

## terminating spot instances

* spot request -> one time or persistent
* one time -> request is served if price below max spot price and instance created
* persistent -> everytime it is below the price instance is created -> loop goes on. to terminate stop the request and manually terminate the instance

## spot fleets

* collection of spot instance and optinally on demand instances
* attempts to launch the numer of spot instance s and on demand instances to meeting the target capacity specified in the spot fleet request.
* request is fulfilled if there is available capacity and max price specified is high thean the curent spot price.
* attempts to maintain its target capacity fleet if your spot instances are interrupted.
* setup different launch pools -> define ec2 instance type, os, AZ
* can have multiple pools and fleet will choose the best way to implement depending on the strategy you define
* will stop launching instances once you reach your price threshold or capacity desire

## different strategies

1. capacityoptimized -> spot instances come from the pool with optimal capacity for the number of instances launching
2. lowestprice -> the spot instances come from the pool witht the lowest price. this is default strategy
3. diversifeied -> spot instances are distributed across all pools
4. instancepoolsto usecount -> distributed across number of spot instance pools you specify. Parameter is valid only when used in combination with lowestprice

> save upto 90% of on demand
>
> wheer you dont need persistent storage
>
> block spot instances from terminating using spot block
>
> a spot fleet is a collection of spot instances and on demand instances