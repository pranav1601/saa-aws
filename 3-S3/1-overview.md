## what is s3

* simple storage service
* store and retrive any amount of data at very low cost
* object based storage
* any file type
* can not run OS or DB
* static files
* unlimited storage
* object 5tb in size
* stores in s3 buckets(folders)
* universal namespace - globally unique
* url - https://bucket-namee.s3.region.amazonaws.com/key-name
* when upload a file -200 status code returned
* key - name of the object 
* version id - multiple versions of same object
* value- data itself
* metadata
* safe place to store file 
* higly available and highly surable
* 99.95-99.99 service availaility
* 99.999999999 11 9s durability for data stored

## s3 standard

* stored redundantly -> multiple facilities >= 3 AZs
* 99.99 % availability
* 99.99.. 11 9s durability
* perfect for frequent aaccessed data
* default storage class
* webiste, content distribution, mobile and gaming applications, big data analytics.

## tired storages
> lifecycle manageent - automatically transition to cheaper storage version
> with versioning all version of an object are stored and can be retireved including deleted objects

## securing data

* server side encryption - able to set default encryption to encrypt all new objects
* ACLs - define which AWS accounts or groups are granted access and type of access. can attach S3 ACLs to individual objects within a bucket
* s3 bucket policies are also definable

> strong read over write consistency
* after a successful write, any subsequent read request immediately receives the latest version
* listing also able to be done immediately
  
> object based
> 
> files upto 5 TB
> 
> not os or db storage
> 
> unilimited storage
> 
> s3 universal namespace
> 
> successful cli or api uploads will generate 200 status code