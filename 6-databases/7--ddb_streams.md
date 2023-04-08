## streams

* time ordered sequence of item level changes in table
* stored  for 24 hours
* inserts, updates, deletes
* combine with lambda for funcitonality like stored procedure

## global tables

* globall distributed applications
* mutli master, multi region replication
* based on ddb streeams
* multi region redundancy for disaster recover/ high availability
* no application rewrites
* replication latency udner 1 second

> if global table not turning on then need to enable ddb stream