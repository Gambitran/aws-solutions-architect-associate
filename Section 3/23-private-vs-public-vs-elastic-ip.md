## Private vs Public IP (IPv4)

## Elastic IPs

* When you stop/start EC2 instance, it can change its public IP
* If need static, use Elastic IP
* Elastic IP is public IPv4 that you can use as long as you don't delete it
* Can attach to one instance at a time
* Can mask failure of an instance by rapidly remapping the address to another instance in account
* Can only have 5 EIP in account (but can be increased by support)