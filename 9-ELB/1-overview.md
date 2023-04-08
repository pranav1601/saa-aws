## elb

* distributes traffic automatically across multiple tarrgets like ec2 instances
* can be done across multiple AZs
* 3 load baclancers:
* 1. application load  balancer - balancing of http and https traffic, layer 7, application awaare, intelligent load balancer
* 2. network load balancer - connection level layer 4, hadnling millions of requests per seconds while maintaining ultra low latencies, performance load balancer
* 3. classic load balancer - legacy, balance http/https applications, between layer 4 and layer 7 , x-forwarded sticky session features, calssic tests, dev load balancer
* all load balancer can be configured with health checks