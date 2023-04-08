## encryption

* encrypt volume using aes 256.
* using AWS KMS customer master keys
* data at rest is encrypted in the volume
* data in transit is encrypted
* snapshots are encyrpted
* all volumes created from the snapshot are envrypted

* handled transparently
* no impact on latency
* copying an unencrypted snapshot allows encryption
* snapshot of encrypted volmes are envcrypted
* encrypt root device volumes upon creation

## steps to encrypt unencypted volume

* create a snapshot of unencrypted
* create copy pf snapshot and encrypt it
* create ami from encrypted snapshot
* use ami to launch new encrypted instances

> data at rest is encrypteed inside the volume
>
> all data in flight is encrypted
>
> all snapshots are encrypted
>
> all volumes created from snapshot are encrypted
>
> 