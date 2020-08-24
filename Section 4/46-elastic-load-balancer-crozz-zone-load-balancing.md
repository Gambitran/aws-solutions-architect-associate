## Cross-Zone Load Balanceing

* Each LB instance distributes evenly across all registered instances in all AZ
* If not enabled, each LB only distributes requests in its AZ

## CLB

* Disabled by default
* No charges for inter AZ data if enabled

## ALB

* Always on, cannot disable
* No charges for inter AZ data

## NLB

* Disabled by default
* Pay charges for inter AZ data if enabled