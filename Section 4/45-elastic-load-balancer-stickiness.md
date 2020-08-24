## Load Balancer Stickiness

* Same client always redirected to the same instance behind LB
* Works for CLB and ALB
* "Cookie" is used for stickness has an expiration date that we control
* Use case: user doesn't lose session data
* May bring imbalance to laod over the backend EC2 instances

* Set at target group level