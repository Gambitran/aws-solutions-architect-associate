## AMI (Amazon Machine Image)

* AWS comes with base images like Ubuntu, Fedora, Windows, etc.
* Images can be customized at runtime using EC2 User Data

## Why create custom AMI

* Pre-install packages needed
* Faster boot time (no need for user data)
* Configured with monitoring/enterprise software
* Security concerns
* Control of maintenance/updates

Note: AMI are built for specific AWS region

## Public AMIs

* Leverage AMIs from other people
* Pay for other AMI by hour using marketplace
* Can be found on marketplace

Warnin:

* Do not use AMI you don't trust, some come with malware/not secure

## AMI Storage

* AMI take space in S3
* By default, AMI are private/locked for account/region
* Can make them public

## Pricing

* Live in S3, get charged for storage