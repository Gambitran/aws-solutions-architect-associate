## ASG

* Scale out to match an increased load
* Scale in to match a decreased load
* Ensure min/max number of machines running
* Automatically register new instances to LB

## Following attributes

Launch configuration:
  * AMI/Instance type
  * EC2 User Data
  * EBS Volumes
  * SG
  * SSH keypair

* Min/Max/Initial capacity
* Network/Subnet information
* LB information
* Scaling policies

## Auto Scaling Alarms

* Can scale ASG based on CloudWatch alarms
* can create scale in/out policies

## Auto Scaling New Rules

* Target Average CPU usage
* Number of requests on ELB per instance
* Average Network In/Out

## Custom Metric

* Send custom metric from app on EC2 to CloudWatch (PutMetric API)
* Create alarm to react to values
* Use alarm as scaling policy for ASG

## Brain Dump

* To update ASG, must create new launch configuration/template
* IAM roles attached to ASG will be assigned to EC2
* ASG is free - pay for resources that are being launched
* If instances get terminated, ASG will automatically create new ones
* ASG can terminate unhealthy instances