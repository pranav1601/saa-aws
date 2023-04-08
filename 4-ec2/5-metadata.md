## metadata

* data about your ec2 instance
* curl http://169.254.169.254/latest/meta-data
* curl http://169.254.169.254/latest/meta-data/local-ipv4 > myip.txt (add to user data)

> user data is bootstrapped text
>
> metadata is about your ec2 instances
>
> use bootsrap scripts to acceess metadata