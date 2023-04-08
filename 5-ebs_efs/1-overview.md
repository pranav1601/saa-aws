## ebs volumes

* elastic block store
* attach storage volumes to ec2 instances
* virtual cloud disk
* create file system
* run db
* run os
* sotre data
* install applications

## mission critical

* designgned for mession critical workloads
* automaiticall replicated withing a asingle AZ to protect against hardware failures
* scalable -> automatically increase or decrease wihtout any downtime

## types

1. general puprose ssd(gp2) - 3 IOPS per gb, tpto max of 16000 IOPS per volume
   * volumes smaller than 1 tb burst upto 3000 IOPS
   * good for boot volumes or development and test apps that are not latency sensitive

2. gp3 - predicitable 3000 IOPS baselines performance and 125 mbps regardless f volume size
    * for applications that require high performance at a low cost such as mysql, cassandra, virtual desktops and hadoop analytics
    * can scale upto 16000 iops aand 1000 mbps for ana additional fee
    * 4 times faster than gp2

3. provisioned IOPS ssd (io1) - upto 64000iops per volume , 50 iops per gb
   * use if more than 16000 iops required
   * designed for io instensive applications, large database, latency sensitive workloads  

4. io2
   * latests generation
   * higher furability and more iops
   * 500 iops per gb, upto 64000 iops
   * 99.999% durability instead of 99.9%
   * io intensive apps, large db, latency sensitive workloads
   * apps that need high level of durability

5. throughput optmizieed hdd  - st1
   * low cost hdd volume
   * baseline throughput of 40 mbps per tb
   * ability to burst up to 250 mbps
   * max through put of 500 mbps
   * frequently accessed, throughput intensive workloads
   * big data, data warehouses, ETL and log processing
   * cost effective way to store mountains of data
   * cannot be a boot volume

6. cold hdd sc1
   * lowest cost option
   * baseline through of 12mbps
   * burst upto 80mbps per tb
   * max throughput of 250 mbps per volume
   * cold data that requires fewer scans per day
   * apps that need lowest cost and performance is not a factor
   * cannot be a boot volume

## iops vs throughput

* ops - measurs the number of read and write ops per second
* metric for wuick transactions, low latency apps, transactional workloads
* abiltiy to action reads and writes very quickly
* choose provisioned iops ss io1 or io2

### throughput

* measure the number of bits read or wtitten per second
* metric for large datasets, large io sizes, complex quieries
* ability to deal with large datasets
* choose throughput optimized hdd st1

> ebs ssd volumes -  highly available and scalable storage volumes to attach to ec2
>
> gp2 - boot disks and general apps, 16000iops per voluume, 99.9% durability
>
> gp3 - high performance appluications, 30000 iops baseline performance and 125 mbps regardless of volume size, 99.9% durability
>
> io1 - suitable for oltp and latency sentiive apps, 50 iops per gb, 64000 iops per volume, high performance and most expensive, 99.9% durability
>
> io2 - suitable for oltp and latency sesnitive apps, 5000 iops per gb, upto 64000 iops per volume, 99.999% durability, lowest gen provisioned iops volume

> hdd volumes - throughput optimized HDD st1 - sutable for big data, data warehouses and ETL, max throughput 500mb per volume, cannot be boot volume, 99.9% durability
>
> sc1 - cold hdd, max throughput of 250mb per volume, less frequently accessed data, cannot be a boot volume, lowest cost