##  moving data to aws

- internet - potentially very slow or could be security risk
- direct connect - faster and more secure, but not always practical if no needed after migration
- physical - bundle the data and physcially send to aws

## snow family

- set of secure apllicances that provide petabyte-scale data collection and processing solutions at the edge and migrate large-scale data into and out of aws.
- offer built in computing capablities enabling customers to run their operation in remote location that do not have data ceter access or reliable network connectivity

## snowcone

- smallest device in snow family
- 8tb of storage, 4gb memory, 2 vcpu
- easily mgrate data to aws after you have processed it
- iot sensor integration
- perfec for edge computing where power and space constrained

## snowball edge

- 48tb to 81 tb in storage
- storage, compute and gpu flavors
- varying amount of cpu and ram
- perfect for off the grid computing or a migration to aws
- when slow to no internet

## snowmobile

- 100 pb of storage
- designed for exabyte scale data center migration

> pay attention to restrictions
>
> noth ways -snow fa,ilt work to get into aws as well as shipped back
>
> generally, turnaround is a week but that mistly depends on cusomter
>
> where are we going? on premise to cloud?
>
> how do we get there? snowball? DMS?
>
> all at once? increments?
>
> partial migration?
> 