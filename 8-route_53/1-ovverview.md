## dns

* convert domain name to ip address
* ipv4 addresses are running out - 32 bts
* ipv6 created to solve this issue - 128 bits

## top level domain

* last word in a domain name is the top level domain name
* .gov, .gov.uk etc
* controlled by internet addigned numbers authority (IANA)
* domain registrars - authortiy that assign under top level domain, registerred in internic, a service of ICANN which enforces uniqueness of domain names across the internet
* registered in the whois database

## commmon dns record types

* SOA - name of te server, administrator, current version of the data file
* NS - name server
* ns used to direct traffic to conetent dns servers that conatin the authoritative dns record

## A record

* most common
* computer uses to translate domain

## ttl

* time to live
* length of dns record is cached on the resolving server or local pc
* lower ttl - faster changes to dns records

## cname

* canoncal name
* resolve dns name to another dns name
* cannot be used for naked domain names

## alias records

* map resource record to load balancers, cloudfront distributions or d3 buckets that are configured as websites
* work like cname record
* can be used as naked domain name

## route 53

* aws dns server
* dns operates on port 53
* register domain names, create hosted zones, manage and create dns records
* named after route 66

## routing policies

* simple routing
* weighted
* latency bbased
* failover
* geolocation
* geopromiximity
* multivalue answer

> difference betwwen alias and cname : cname no naked
>
> always choose alias record over cname
>
> soa - start of authority

