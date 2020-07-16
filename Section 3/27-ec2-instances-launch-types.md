## EC2 Instance Launch Types

* On Demand Instances: short workload, predictable pricing
* Reserved: MINIMUM 1 year
  * Reserved Instances: long workloads
  * Convertible Reserved Instances: long workloads with flexible instances
  * Scheduled Reserved Instances: run at a certain schedule
* Spot Instances: short workloads, for cheap, can lose instances (less reliable)
* Dedicated Instances: no other customers will share hardware
* Dedicated Hosts: book an entire physical server, control instance placement

## EC2 On Demand

* Pay for what you use (billing/second, after first minute)
* High cost, but no upfront payment
* No long term commitment

* Recommend for short-term and un-interrupted workloads

## EC2 Reserved Instances

* Up to 75% discount compared to On-Demand
* Pay upfront for long term commitment
* Period of 1-3 years
* Reserve specific instance type

* Recommend for steady state usage applications (think database)

## Convertible Reserved Instance

* Can change EC2 instance type
* Up to 54% discount

## Scheduled Reserved Instances

* Launch within time you reserve
* Recommend for when you require fraction of day/week/month

## Spot Instances

* Can get up to 90% discount
* Can lose at anytime if max price is less than current spot price
* Recommend for workloads that resilient to failure

## Dedicated Hosts

* Physical dedicated server
* Full control of instance placement
* Visibility into underlying sockets/physical cores of hardware
* Allocated for 3 year period reservation
* $$$
* Recommend for software with complicated licensing model or security reasons

## Dedicated Instances

* Runnning on hardware that's dedicated to you
* May share hardware with other instances in same account
* No control of instance placement