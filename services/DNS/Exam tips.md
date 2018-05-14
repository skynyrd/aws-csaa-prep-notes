* ELB's don't have pre-defined IPv4 addresses, you resolve to them using a DNS name.
* Understand difference between Alias Record and a CNAME.
* Given the choice, always choose Alias Record.
* Route 53 support MX Records
* Route53 => Port 53 is DNS
* There is a limit of 50 domain names however this limit can be raised by contacting AWS support.

### Routing Policies

* `Simple`: Stupid Round-Robin, single web server.
* `Weighted`: e.g. A-B test, %10 to new web site, %90 to old web site.
* `Latency`: Based on end users.
* `Failover`
* `Geolocation`: Europeans => London Server, Rest of the world => Sydney server.
