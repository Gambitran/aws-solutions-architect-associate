## EC2 Spot Instance Requests

* Can get discount up to 90% compared to On-Demand
* Set <b>max spot price</b> and get instance while <b>current spot price < max</b>
  * Varies based on offer and capacity
  * If current spot price > max, can choose to stop or terminate instance within 2 minute grace period

* Spot Block
  * Specify during specified time frame (1 to 6 hours) without interruptions

* Recommend for batch jobs, data analysis, or workloads that are resilient to failure

## Terminate Spot Instances

* Can only cancel requests that are open, active, or disabled
* Does not terminate current instances
* Must first cancel Spot Request, then terminate associated Spot instances

## Spot Fleets

* Set of Spot Instances + (optional) On-Demand Instances
* Try to meet target capacity with price constraints
  * Define multiple launch pools: instance type, OS, AZ
  * Spot Fleet stops launching instances when reaching capacity or max cost
* Strategies:
  * lowestPrice: from pool with lowest price
  * diversified: distributed across all pools
  * capacityOptimized: pool with optimal capacity for number of instances