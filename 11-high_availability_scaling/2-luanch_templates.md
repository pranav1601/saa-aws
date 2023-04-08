## launch template

* setting that go into building ec2
* collection of etting you can configyre with going through the ec2 wizard again and again

## template vs configurations

![launch template vs confugrations](../images/launchtemplatevsconfig.png)

> template - AMI, instance size, sec groups
>
> if we provide networking configs in the launch template, cant be used for autoscaling
>
> launchtemplates most up to data, flexible way
>
> configuration old way
>
> user data included in the template or configruyration
>
> templates can be versioned
>
> configs dont include netwokring information