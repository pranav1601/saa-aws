## classic load balancer

* legacy
* http https
* layer 7 specific features lie x forwarded and sticky sessions
* you can use striict layer 4 load balancing for application that rely purely on tcp protocol

## x forwarded for header

* when traffic is sent from load balancer only ip of load balancer is visible
* this is used to see origiinal ip of client

## gateway timeouts

* if app stops responsing, classic load balancer responds with 504
* means app is having issues either at server layer or database layer

> 504 means gateway has timed out means app has stopped
>
> need ipv4? look for x-forwarded for header