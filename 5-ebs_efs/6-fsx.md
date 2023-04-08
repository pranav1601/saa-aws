## fsx for windows

* fully managed native microsoft windows file system
* easyily move windows based applications that require file storage to aws 

## how different from EFS

![fsx vs efs](../images/fsxVSefs.png)

## fsx for lustre

* hpc
* ml
* media data processing workflows
* electronic design automation
* launch and run a lustre file for massive datasets upto 100 gb per second of throughput, million iops, sub millisecond latencies

## efs vs fsx for windows vs fsx for lustre

* efs - distribueted, highly resilient storage for linux instance and linux based apps
* fsx for windows - centralised storage for windows based appplications such as share point, sql server, workspaces, iis web server or any another native windows apllications
* fsc for luster - high speed, high caacity distribured storage. hpc, financial modeling, fsx for lustre can store data directly on s3

