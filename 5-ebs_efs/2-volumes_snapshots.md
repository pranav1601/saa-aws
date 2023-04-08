## volumes

* virtual hard dsk
* 1 volume per ec2 instance atleast - call root device volume

## snapshots

* exist on s3
* photo pg virtual disk/volume
* point in time copy of a volume
* increminatal -> data that has been changed since your last snapshot is moved to s3
* first snapshot -> takes longer because their is not point in time previous snapshot

## tips

* for consistent snapshot - recommended to stop the instance and take snap
* * only captutire data that has been writteen to EBS which might exlcude data that has been locally cached by application or os.
* snapshot of encrypted ebs volume will be encrypted automatically
* snapshots can be shared only in region where it was creaed. to share to other region, you will need to copy to the desitination region firs

* ebs vol will be saame az as ec2 instance 
*  resize ebs without stopping ec2 iinstance but need to extend the filesystem in the os so the os can see the resized volume
*  you can change volume types on the fly. No need to stop or restart the instance

> volume exist in ebs, snapshots exist on s3
>
> snapshots a re point in time photos and are incremental in nature
>
> first snapshot willt ake time to create, subsequent ones easier
>
> share snapshots between aws accounts as well as between refions. but first you need to copy thaat snapshot to target region.
>
> you can resize ebs volumes on the fly as well as changing the volume types.