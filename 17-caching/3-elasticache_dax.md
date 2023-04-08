## elasticache

- aws managed version of 2 oss tech memcached and redis
- allows avoiding lot of issues
- redis - non relation nosql db

![memcached vs redis](../images/memcachedvsredis.png)

## dax

- in memory cache - reduce ddb response time for milli to micro seconds
- cache is highly available and lives inside the vpc you specify
- user determines the node size, count for the cluster, ttl for data and maintencance windows for changes and updates

## whta type of cache

- dax - only for ddb
- elasticache - flexibility - any db but excels in front of rds

> favor answer that inclue db caching solution
>
> redis can be cache and a db
>
> memcache and dax are not source of truth for your data cuz cant be used as db