## nat

* network address trtransaltor
* allow instance in vpc to connect to internet without allowing internet to connect
* provision nat gateway in public subnet
* allow instance in private subnet to access nat gateway
* redudndant inside the availability zone
* starts at 5 gbps and scales currently to 45 gbps
* no need to patch
* not associated with sec groups
* automatically assigned a public ip

> high availability with nat gateway  - if resources in multi AZ and share a nat gateway, if nat gateway az is down, resource in other AZ will lose internet access
>
> * to create az independent architecture, create a nat in each az and configure routing to ensure resources use the nat gateway in the same az