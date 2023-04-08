## how comuputers communicate

* linux - ssh port 22
* windows rdp port 3389
* http web browsing port 80
* https web browsing port 443

## security groups

* virtual firewalls fro ec2 instance
* by default everything is blocked
* to let everything in 0.0.0.0/0
* to communicate to instance you need to open up correct ports

## bootstrap script

* a script that runs when the instance first runs
* adds to amount of time to boot the instance however autmates the installation of applciations
* under advanced options -> user data

> changes to sec group take places immeduiately

> any number of ec2 instances under a sec group

> multiple security groups attached to ec3 instances
>
> all inbound trraffic is blocked by default
>
> alll outbound traffice is allowed
>
> bootstrap sdcript is a script that runs when instance first runs
>
> passess user data to ec2 instance to install applications