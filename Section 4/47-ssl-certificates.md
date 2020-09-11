## SSL/TLS - Basics

* Allows traffic between clients and LB to be encrypted in transit

## Load Balancer - SSL Certs

* X.509 certs
* Manage through ACM (AWS Certificate Manager)
* Upload certs too
* HTTPS Listener
  * Specify default cert
  * Add optional list of certs to support multiple domains
  * Clients can use SNI (Server Name Indication) to specify hostname they reach
  * Ability to specify security policy to support older version of SSL/TLS (legacy clients)

## Elastic Load Balancer

Classic Load Balancer (v1)
* Only 1 SSL cert

Application/Network Load Balancer
* Supports multiple SSL certs
* Uses SNI