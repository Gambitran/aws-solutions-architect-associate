## What is EC2?

* Elastic Compute Cloud
* Capability of:
  * Launching virtual machines
  * Data on virtual drives (EBS Volumes)
  * Distribute load (ELB/ALB)
  * Auto-scaling services (ASG)

## Hands-on

* Choose Amazon Machine Image (AMI) like OS
* Instance type
  * Specs like cpu and memory
* Configure Instance
  * Number of instances, network, roles, etc.
* Add storage
  * Set size
* Add tags
  * Like key/value pairs descriptors for the machine(s)
* Configure Security Group
  * Firewall around instance
  * Set service/ports/protocols from source IPs (e.g. SSH from 0.0.0.0/0)
* Launch
  * Create/import keypair for access to VM