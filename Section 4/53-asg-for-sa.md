## ASG Default Termination Policy

* Find AZ which has most instances
* Multiple instances in AZ to choose from, delete one with old launch configuration

## Lifecycle Hooks

* As soon as instance is launched, it's in service
* Ability to perform extra steps (Pending state)
* Ability to perform actions before termination (Terminating state)

## Launch Template vs Launch Configuration

* Both
  * Spcify ID of AMI, type, key pair, SG, and other parameters

* Launch Configuration (Legacy)
  * Re-create every time to modify

* Launch Template (Newer)
  * Multiple versions
  * Parameter subsets (partial config for re-use/inteheritance)
  * Provision both On-Demand and Spot
  * Can use T2

