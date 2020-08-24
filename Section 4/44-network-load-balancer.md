## Network Load Balancer

* Layer 4
  * Forward TCP/UDP traffic
  * Handle millions of request/seconds
  * Less latency ~100ms (vs 400ms for ALB)

* Has 1 static IP per AZ, supports assigning EIP (helpful for whitelisting specific IP)
* Extreme performance