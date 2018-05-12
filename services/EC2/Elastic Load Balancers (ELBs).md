* Instances monitored by ELB are reported as;
    * InService
    * OutOfService

* Health Check checks the instance health by talking to it.
* Have their own DNS name. You are never given an IP address.
* Read the ELB FAQ, concentrate on `Classic Load Balancers`

`Application Load Balancers`

* When you need a flexible feature set for your web apps with HTTP and HTTPS traffic.
* Advanced routing, TLS termination and visibility features targeted at microservices and containers and other architectures.

`Classic Load Balancers`

* When you have an existing application running in the EC2 Classic network