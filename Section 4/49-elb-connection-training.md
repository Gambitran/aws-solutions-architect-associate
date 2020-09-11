## ELB - Connection Draining

Feature naming:
* CLB: Connection Draining
* Target Group: Deregistration Delay (ALB/NLB)

* Time to complete "in-flight" requests while instance is de-registering or unhealthy
* Stops sending new requests to instance that is de-registering

* 300 seconds is default, can check between 1-3600 seconds
* Can be disabled by setting to 0
* Set low value if requests are short