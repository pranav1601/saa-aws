## global accelarator

- networking service that sends users traffi through aws global netowwkr infra. it can increase performance and help deal with ip caching
- gives 2 ip addresses to users
- even ip of elb changes, then user will not have problem

## features

- masks cmplex arch - as deployments happen, users wont notice since they will use same ip
- sppedy since traffic is routed through aws gloabal network infrastructutre
- weighted pools - can create weighted groups behinf the IPs to test out new features or handle failure in your env

> ip caching - global accelarator
>
> uses edge location to speed everything up
>
> can set up wights between different endpoints
>
> 2 static IPs that dont change