## weighted routing

* splits traffic based on weights

## health checks

* set health checks on ec2, load balancers, weights
* if record set fails health check, it is removed from route 53 until it passes
* sns notification to alrert you about failed health checks

> percentage amount of traffic to particular region - weighted routing