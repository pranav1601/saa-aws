## EBS behaviors reviews

* if instance stopped data is kept on the disk with EBS and will remain until ec2 is started
* if instance is terminated, root device volume will be terminated


## start ec2

* os boots up
* user data script is run
* app starts

## ec2 hibernation

* saves the content f instance RAM to ebs volume
* start from instance volume:
* evs root volume restored to prev state
* ram content reloaded
* processes that were running previouslly are resumed
* previously attached data volumes are attached
* instance boots much faster
* used for long running processes of apps that take time to initialize

> preserves in memory ram in ebs
> 
> donot need to reload the os, hence faster
> 
> ram less than 150 gb
> 
> instance family for c3, c4, c5 , m3, m4, m5, r3, r4, r5
>
> available for windows, AL2, ubunut
>
> cant be hibernated for more than 60 days
>
> available for on demand instance and reserved instances