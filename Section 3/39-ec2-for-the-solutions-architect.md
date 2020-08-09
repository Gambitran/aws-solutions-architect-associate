## EC2 for the Solutions Architects

* EC2 instances are billed by the second
* Use SSH terminal
* Lock down security group to your IP
* Timeout issues, look at SG issues
* SSH private key chmod 400
* SG can reference other SGs instead of IPs
* Know difference between private, public, and elastic IP
* Customize EC2 instance at boot using EC2 User Data
* 4 EC2 launch nodes:
  * On Demand, Reserved, Spot, Dedicated Hosts
* Basic instance types: R, C, M, I, G, T2/T3
* Create AMIs to pre-install software on EC2, means faster boot
* AMI can be copied across regions and accounts
* Can be started in placement groups:
  * Cluster, Spread