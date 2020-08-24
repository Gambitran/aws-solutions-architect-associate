## Application Load Balancer (v2)

* Layer 7 (HTTP)
* Multiple HTTP apps across machines (target groups)
* Multiple applications on same machine (containers)
* Support for HTTP/2 and WebSocket
* Supports redirects from HTTP to HTTPS

## HTTP-based traffic
* Routing tables to different target groups
  * Based on path (e.g. /users and /posts)
  * Based on hosntame (e.g. one.example.com and two.example.com)
  * Based on Query String/Headers (e.g. /users?id=123&order=false)
* Great fit for micro services & container-based application
* Port mapping feature to redirect to dynamic port in ECS

## Target Groups
* EC2 instances
* ECS tasks
* Lambda functions - http requrest translated into JSON event
* IP Addresses - must be private IPs

* Health checks are at target group level

## Good to know

* Fixed hostname (xxx.region.elb.amazonaws.com)
* Application services don't see IP of client directly
  * True IP of client is inserted in header X-Forwarded-For
  * Can also get Port (X-Forwarded-Port) and protocol (X-Forwarded-Proto)