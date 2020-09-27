## EBS Volume

* Network drive you can attach to instances while they run
  * Uses network to communicate, can introduce latency
* Persist data
* Can be detached/attached
* Locked to AZ
  * Need to snapshot first to move across
* Have provisioned capacity (size in GBs, and IOPS)
  * Get billed for ALL provisioned capacity
  * Can increase capacity over time

## EBS Volume Types

* 4 Types
  * GP2 (SSD) - General purpose
  * IO1 (SSD) - Highest performance
  * ST1 (HDD) - Low cost for high performance
  * SC1 (HDD) - Lowest cost for less performance

* Characterized in size, throughput, IOPS

* Only GP2 and IO1 can be used as boot volumes
