## aurora

* amazon propriety db
* mysql and postgresql compatible db engine that combnines speed and availability of high end commercial db with simplicity and const effectiveness of open source db
* 5x performance than mysql and 3x than postgre at lower price with same performane
* starts with 10gb and increments 10gb upto 128 tb
* compute resourcrs scale upto 96vcpu and 768 gb of memory
* 2 copies contained in each AZ with min of 3 AZs, hance 6 copies of data
* handle loss up to 2 copies of data without affecting write availability and 3 copies without affecting read availability
* storage is self healing - data blocks and disks are continuously scanned for error and repaired automatically
* aurora replicas - 15 read replicas with aurora
* mysql replicas - 5 read replicas with aurora mysql
* postgresql - 5 read replicas with aurora postgresql

![aurora replicas](../images/aurorua_replicas.png)

* backups are always enabled. donot impact performance
* able to take snapshots with aurora, no impact on performance
* share aurora snapshots wih other aws accounts

## aurora serverless

* on demand, auto scalin for mysql, postgresql compatible
* automatically start, shuts, scales up or down based on app needs
* infrequent, intermittent, unpredictible workloads

> 2 copies in each AZ, 3 az, 6 copies
>
> share snapshot with other aws acount
>
> automated failover onlyy on aurora replica
>
> aururoa serverless for infreqnent workloads
>
> automatic backup enabled by default