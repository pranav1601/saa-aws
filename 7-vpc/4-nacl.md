## nacl 

* layer of security for vpc that acts as a firewall for cvonyrtolling traffic in and out of one or more subnets
* rules similiar to security groups
* first line of dedense
* vpc comes with default nacls, by default allows everything
* custommnetwork acl - by deafult denies all inobund and outbound traffic
* subnet assocaiations - each subnet must be associated with nacl. If dont explicity associate, it is associated with default nacl
* block ip addresses using nacl not sec groups

* 1 nacl to many subnets but 1 subnet to only 1 nacl
* numbered list of rules and evaluated in order
* separate inbound and outbound rules, and each can either allow or deny traffic
* stateless - response to allowed inbound traffic are subject to the rules for outbound traffic
* open ephemeral ports for clients 1024-65535

* if block ip - make sure add that rule before any other rule

> when associate network ACL with a subnet, the previous association is removed