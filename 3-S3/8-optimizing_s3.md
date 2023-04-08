## s3 prefix

* bucketname/folder/subfolfer/myfile.jpg

## s3 performance

* extremely low latency
* first byte with 100-200 milliseconds
* 3500 put copy post delete and 5500 get head requests per second
* spread read across diferent prefied -> 2 prefixes -> 11000 requests per second
* 4 prefix -> 22000
* basically more folders and sub folder, better performance

## s3 limitations with kms

* kms has limits for encryption
* when upload a file to a bucket, generatedatakey is called in kms api
* when download a file you will call decrypt in kmks api
* uploading / downloading will count to kms quota
* region specific -> 5500 , 10000 or 30000 requests per second
* cannot request a quota increase for kms
* encryption question in exam -> prefer s3  native encryption

## multipart uplaods

* recommended for files over 100mb
* required for files over 5 gb
* parallelize uploads
* better performance for uploads -> multipart uploads

## s3 bute ranges fetch
* parallize downloads by specifying byte ranges
* if there is a failure, only specific byte range will fail

> prefixes are folders and subfolders
>
> 3500 out copy paste post delete and 5500 get requests per second
>
> multipart uploads to increase performance
>
> kms has limitations
>
> s3 byte range fetches to increase performance when downloading files