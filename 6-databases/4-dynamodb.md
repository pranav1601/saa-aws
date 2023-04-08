## dynamodb

* non relational db
* nosql db
* single digit millisecond latency
* both document and key value data bodel
* mobile, we, gaming, ad tech, IoT

* stored on ssd
* spread in 3 geo distinct data center
* eventual consistent read(default) - consistency in copies of all data copies usually reached within a second, best read performance
* strong consistent read can be chosen - returns a result that reflects all writes that received a successful response prior to read

## dynambodb accelarator dax

* fully managed , highly available, in memory cache
* 10x performance   
* reduced request time from millisecond to microseconds even under load
* no need for developers to manage caching logic
* compatibel with dynamodb api calls

## on demand capacity

* pay per request
* balance cost and performance
* no min capacity
* no charge for read/wite, only sotrage and backups
* pay more per request than provisioned capacity
* use for new product launches

## security

* KMS
* site to site vpn
* direct connect
* IAM policies
* fine grained access\
* cloudwatch and cloudtrail
* vpc endpoints

> stored on ssd 
>
> 3 geo datacetner
>
> 