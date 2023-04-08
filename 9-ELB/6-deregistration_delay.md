## dregistration delay

* connection draining
* allows load balancer to keep existing connections open if ec2 instance are deregistered or become unhealthy
* enables load balancer to complete in flight requests made to instances that are de registering or unhealthy
* disable this if you want your load balancer to close the connection immediately

> enable deregistration to keep the connection open
>
> disable to remove connection