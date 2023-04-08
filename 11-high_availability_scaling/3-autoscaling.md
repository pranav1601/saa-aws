## sutoscaling groups

* collection of ec2 considered as a collectibe group for scaling and management
* template - settins to create the EC2
*  - networking and purchasing - pick networking space and purchasing options. Using multiple AZs for high availability
*  - ELB - EC2 can be registered behing ELB.the ASG can be set to repect the lad balancer health check
*  - scaling policies - minimimum, maximum and desired cpacity needs to be set to ensire you dont have too many or too few resources
*  - setup SNS to notify when scaling done

## restricitons

- minimum - lowest ec2 instances you'll ever have online. generally 2
- maximum - highest ec2 instance sthat youl will provision
- desired - how many you want this instant

* can use sopt instances to save money

> autoscalisng is vital to creating a highly available application
>
> select answers that spread resources out over multi AZs and utilise ELB
>
> networking - contan the location of where instances will live
>
> ELB - select a load balances for the instances to live behind
>
> autoscaling groups only for ec2
>
> favor solutions that are predictive than reactive
>
> bake AMI to reduce build times. avoid long prvisioning times bu putting everthing in AMI. this is better than user data
>
> spread out autoscaling groups over multi AZ