## elastic compute cloud

* secure, resizable compute capacity in cloud
* like a VM
* web-scale cloud comouting for developers
* capacity you want when you want it
* all under the user's control
* pay for what you use 
* select the capacity and grow and shrink on the way
* on premise - > long term investment 3-5 years
* avg time to provision server on premise -> 10-20 days

## pricing models

* on demand -> hour/second depending on type of instance
* reserved-> reserved for 1-3 yearrs, upto 72% discount on hourly charge
* spot-> unused capacity at a discount of upto 90% -> prices fluctuate with supply and demand
* dedicated -> physcial ec2 server dedicated for your use, most expensive option

## on demand instances

* flexibe -> low cost and flexible without any upfront payment
* short term, unpredictible work loads, cannot be interrupted
* app being deeveloped and trying ec2 for first time

## reserved instanced(RI)

* app with steady state or predictable usage
* require reserved capacity
* pay upfront to reduce total computing costs even further
* standard RI up to 72% off on  on demand price
* convertible RI -> option to change ec2 instance type to >= cost instance. 54% off on on demand price
* scheduled RI -> launch within the time you want -> predicitbele recurring schedule that only requires a fraction of day, week or month
* operate in regional level
* save upto 72% depending on contract length
* commit t 1 or 3 years
* super flexible with lambda fargate etc

## spot instances

* app with flexibele start and end price
* feasible at very low compute prices
* urgent need for large amounts of additional computing capacity

* image rrendering
* genomic sequencing
*  algrithmic trading engines

## dedicated hosts

* compliance -> requirement that may not support multi tenant virtualization -> no sharing of RAM/storage with different companies
* licensing -> does not require multi tenacy support or cloud deployments
* can be purchased on demand(hourly)
* can be purchased as a reservation for upto 70% off of the on demand price

> like a VM, hosted in Aws instead of data enter

> select capacity you need right now

> grow and shrink when you need
>
> provisioned in muites
>
> on demand -> pay by hour / second for flexibility

> reserved -> 1 to 3 years, 72% disci=ount upto 72%. known, fixed requirements.
>
> spot -> purchase unused capacity upto 90% -> fluxtuate with supply and demand
>
> dedicated -> physcial ec2 sererf dedicated for use. server boundaries
