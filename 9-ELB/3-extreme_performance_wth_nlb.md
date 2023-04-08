## layer 4 load balancing - network load balancers

* handle millions requests per second
* select a target from the target for the feault rule
* open a tcp connection to the target on the oport specifiecd in the configuration

## listeners

* checks for connection requests on the port
* forwards the request to the target group
* no rules unlike application load balancers

## target groups

* routes requests to one or more targets in target group

## ports and protocol

* tcp
* tls
* udp
* tcp_udp
* ports - 1-65535

## encryptions

* use tls listener to offload work of encryption and decryption to your load balancer so your applications can focus on business logic
* if the listener is TLS, you must deploy exactly one ssl server certificate on the listener

## use cases

* best for load balacing of tcp traffic where ectreme performance is used
* use for extreme performance
* maintain ultra low latencies

> layer 4
>
> extreme performance
>
> use cases where protocls not supported by apllication load balancer