## Scalability & High Availability

* Scalability means app/system can handle greater loads by adapting
  * Vertical scalability
  * Horizontal scalability (=elasticity)
* Scalability linked but different to HA

## Vertical Scalability

* Increase size of the instance
  * App runs on t2.micro
  * Scaling up means changing it to t2.large
  * Common for non-distributed systems, such as database
  * RDS/ElastiCache can scale vertically
  * Usually limit how much can scale upwards (hardware limit)

## Horizontal Scalability

* Increase number of instances/systems for app
  * Implies distributed systems
  * Common for web applications

## High Availability

* Usually goes hand in hand with horizontal
* Running app/system in at least 2 data centers (AZ)
* Goal is to survive data center loss

* HA can be passive (RDS Multi AZ)
* Can be active (horizontal scaling)