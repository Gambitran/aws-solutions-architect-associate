## Elastic Network Interfaces (ENI)

* Logical component in VPC that represents virtual network card
* ENI can have:
  * Primary private IPv4 (one or more secondary IPv4)
  * One Elastic IP (IPv4) per private IPv4
  * One public IPv4
  * One or more security groups
  * A MAC address
* Can create ENI indepedently and attach on fly on EC2 instances for failover
* Bound to specific AZ