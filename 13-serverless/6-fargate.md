## Fargate

- serveerless compute engine for fargate
- works with ecs and eks
- aws managed

![ec2 vs fargate](../images/ec2vsfargate.png)

#### fargate

- select when more consistent workloads
- allows docker use across the organization and greater level of control

#### lambda

- unpredictible workloads
- perfect for applications that can be run from one function

> know the use case
>
> lambda -lightweight cases, for aws
>
> fargate - container
>
> ec2 - run for a longer time
>
> fargate doesnt work without ecs/eks
>
> fargate more xpensive than ec2 but easier to use