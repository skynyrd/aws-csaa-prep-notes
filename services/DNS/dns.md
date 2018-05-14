* Kinda Phone book.

* `IPv4` => 32 bit field and has over 4 billion different addresses.
* `IPv6` => 128 bits address, 340 undecillion addresses in theory.
* VPC and EC2 supports IPv6
* `Top level domain names` => .com, .edu, .gov, .net and etc. controlled by Internet Assigned Numbers Authority (IANA)
* Domain registration is done by registrars, authority that can assign domain names directly under one or more top level domains.
*  Domain names registered by InterNIC, service of ICANN
* Stored in central db: WhoIS
* Popular domain registrars include GoDaddy.com, 123-reg.co.uk
* Amazon is domain registrar too.

`SOA Records (Authoritative record)` 

* The name of the server that supplied the data for the zone.
* The admin of the zone.
* Current version of the data file...

`NS Records`

Name Server records are used by Top Level Domain servers to direct traffic to the Content DNS server which contains the authoritative DNS records.

`A Records`

Fundamental type of DNS record, meaning `Adress`, used by a computer to translate the name of the domin to the IP address.

`TTL`

The length that a DNS record is cached on either the Resolving Server or the users' own local PC. `Time to Live` in seconds.

`CNAMES (Canonical Names)`

Can be used to resolve one domain name to another. ex: `m.mysite.com ===A===> mobile.mysite.com ===B===> IP Address` (A is CNAME)

`Alias Records`

* Term in AWS world.
* Similar to CNAME
* Difference: CNAME can't be used for naked domain names (domain name without `www`) (zone apex record)
* Route 53 automatically recognizes changes in the DNS record sets that the alies resource record set refers to.
    * e.g. `example.com` binded to ELB `lb1-1234.us-east-1.elb.amazonaws.com`, if IP address of the load balancer changes, Route 53 automatically reflect those changes in DNS.


#### Exam Tips

* ELB's do not have pre defined IPv4 addresses, you resolve to them using a DNS name.
* Understand the difference between an Alias Record and a CNAME. `CNAME is charged, Alias is not`
* Always choose an Alias Record over a CNAME