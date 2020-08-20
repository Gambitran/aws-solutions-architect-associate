## EC2 Hibernate

* Can stop/terminate instances
  * Stop: data is kept intact in next start
  * Terminate: EBS volumes will be lost

* On start, the following happens:
  * First start: OS boots, EC2 user data script run
  * Following starts: OS boots up
  * Application then starts, caches get warmed up, this can take time

* Hibernate:
  * In-memory (RAM) state is preserved
  * Instance boot is much faster
  * OS not stopped/restarted
  * Under hood, RAM state is written to file in root EBS volume
  * Root EBS volume must be encrypted

* Use cases:
  * Long-running processing
  * Saving RAM state
  * Services that take time to initialize

* Supported families - C3, C4, C5, M3, M4, M5, R3, R4, R5
* RAM size - must be less than 150 GB
* Instance size - not supported for bare metal
* AMI - Amazon Linux 2, Linux AMI, Ubuntu, Windows
* Root Volume - must be EBS, encrypted, not instance store, and large
* Available for On-Demand and RI
* Cannot be hibernated more than 60 days