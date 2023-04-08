## eks anywhere

- run and manage on premise eks
- eks distro - allows deployment, usage and mgmnt methods for cluster in data centers
- lifecycle offer full lifecycle management of multiple k8s cluster, operates independently of AWS

## concepts

- control pane - k8s plane management managed by customer
- location - control plane location is entirely wiithin a customer data center or operations center
- upates - cluster updates are done entirely via manual cli or flux
- curated packages - offer core functionalities of k8s clusters
- enterprise subs- curated packages require an enterprise subscription

## ecs anywhere

- allows the management of container based apps on premise
- no need to install and operate local container orchestration, meaning more operationaly efficeicny
- completely managed solution enabling standardization of container management across environments
- no elb support makes inbound traffic requirements less efficient
- external - new launch type noted as external for creating services or running tasks

## ecs anywhere requirements

- ssm agent, ecs agent, docker
- register external instances as ssm managed instances
- easily create an installation script within the ecs console
- scripts contain ssm activation keys and commands for required software
- execute scripts on you on premise vm or bare metal servers
- deploy containers using the external launc type

![ecs anywhere](../images/ecs_anywhere.png)

> eks anwyhere- based on eks distro
>
> > distro allows customer to maintain efficiency of eks
>
> > everything managed by user
>
> ecs anywhere - service within ecs
> > allows aws managed cintainer orchestration anywhere on premises
>
> > requiremetns - must have ssm agent,ecs docker installed
>
> > execute scruptis containing required steps and use the external launch type