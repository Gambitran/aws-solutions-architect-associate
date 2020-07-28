## EC2 Instance Types - Main Ones

Applications that need:

* R - RAM - in-memory caches
* C - CPU - compute/databases
* M - balanced - general/webapp
* I - local I/O - databases
* G - GPU - video rendering/maching learning

* T2/T3 - burstable instances (up to capacity)
* T2/T3 Unlimited - unlimited bursts

https://www.ec2instances.info

## Burstable Instances (T2/T3)

* OK CPU performance, but when spike, performance can be very good
* If machine bursts, utilizes "burst credits"
* If credits are gone, CPU becomes bad
* If machine stops bursting, credits are accumulated over time

## T2/T3 Unlimited

* Burst as long as you want, but pay extra if over credit balance
