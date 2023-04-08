## networking with ec2

* you can attach 3 different types of cirtaul networking cards
* ENI -> elastic network interface, for basic day to day networking
* EN -> enhanced networking, uses single root IO virtualization to provide high performance
* EFA -> elastic fabric adapter -> accelarates high performance computing and machine learning applications

## ENI

* private ipv4 address
* public ipv4 address
* many ipv6 addresses
* MAC address
* 1 more security groups
* create a management network
* use network and security appliances in your vpc
* create dual home instances with workloads/roles on distinct subnets
* create a low budget high availablity solution
  
## enhanced network

* single root IO virtualization -> SR IOV provides higher IO performance and lower CPU utilization
* performance -> higher bandwidth, higher packet per second performance, and consistently lower inter instance latencies
* for higher performance networking betwwen 10gbps and 100 gbps
* can be used using: 
* 1. elastic network adapter(ENA) -> supports network speeds of up to 100 gbps for supported instance types
* 2. intel 82599 virtual funciton interface -> supports network sppeds of up to 10gbps for supported instance types. Typically used for older instances 
* choose ENA over VF because faster and more modern

## EFA

* accelarate HPC and machine learning apps
* lower and more consistent latency and higher throughput than the tcp transport traditionally used in HPC systems
* lot faster with much lower latency
* os bypass enables HPC and machine learning apps to bypass the os kernel and communicate directly with EFA device, not supoorted with windows - only linux

> eni for basic networing, separata management network from your prod network or separate logging network, at low cost, multple ENIs for each network
>
> EN -> speed between 10 gbps, reliable, high throughput 
>
> EFA - for when you need to accelarate hpc and ml apps or if need to do os bypass. if hpc or ml mentioned in question choose EFA