## launch ec2 instance from cmd

* ssh ec2-user@ip-address -i pemfile

## list s3 buckets

* aws s3 ls
* aws config -> to configure your aws creds
* if no access key then go to IAM and create access key when creating user 
* access key id and access secret key

## make bucket

* aws s3 mb s3://enterbucketname

## copy file to bucket

* aws s3 cp filename s3://bucketname

> always give user least privilege access

> use groups and not directly permission to users

> secret access key -> password

> dont share key pairs, one key pair per user
>
> supports linux, windows and macos
>
> 