## Scaling Policies

* Target Tracking Scaling
  * Simple
  * E.g. Want average ASG CPU to stay around 40%

* Simple/Step Scaling
  * When CloudWatch alarm is triggered (e.g CPU > 70%), then add 2 units
  * When CloudWatch alarm is triggered (e.g. CPU < 30%), then remove 1 unit

* Scheduled Actions
  * Anticipate scaling based on patterns
  * E.g. increase min capacity to 10 at 5PM on Fridays

## Scaling Cooldowns

* Period to ensure ASG doesn't launch/term additional instances before previous scaling takes effect
* Can create cooldowns that apply to specific simple scaling policy
* Overrides default cooldown period
* Common use case - terms instances based on specific criteria or metric. Because it terms instances, Auto Scaling needs less time to determine whether to terminate additional instances.
* Default is 300 seconds, if too long, can reduce costs by applying scaling-specific cooldown period of 180 seconds to scale-in policy
* If app is scaling up/down multiple times each hour, modify ASG cool-down timers and CloudWatch Alarm period that triggers scale-in