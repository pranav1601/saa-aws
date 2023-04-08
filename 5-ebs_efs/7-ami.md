## ami

* provides the info required to launch instance
* region, os, architecture, launch permissions, storage for root device
* ebs or instance store

## ebs 

* root devices is an amazon ebs volume created from ebs snapshot

## instance store

* root device is an instance store volume created from a template stored in s3
* instance store volumes cannot be stopped

* instance store volume - ephemeral - cannot be stopped - if instance stopped no data
* if you delete instance then instance store volume lost
* root device deleted on termintion

* ebs volume can be stoppped
* donot lose data if instance is stopped
* reboot ebs and not lose your data
* by default root device volume deleted on termination. However, can tell AWS to keep the root device volume with ebs volumes