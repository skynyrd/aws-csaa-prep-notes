* Virtual Data Center in the cloud.
* Contains IGWs (or Vitual Private Gateways), Route tables, Network Access Control Lists, Subnets, and security groups
* 1 Subnet = 1 AZ
* Security groups are stateful, ACLs are stateless
    * stateful: Open port 80 for inbound, and outbound is also opened automatically.
* Complete control over virtual networking
    * Selection of IP from your IP range
    * Creation of subnets
    * Route tables configuration
    * Networking gateways
* You can create Hardware Virtual Private Network (VPN) connection bw your corp. data center and your VPC

`http://cidr.xyz/`: Interactive IP address and CIDR range visualizer

* 10.0.0.0 - 10.255.255.255 => 10/8 prefix (more)
* 172.16.0.0 - 172.31.255.255 => 172.16/12 prefix (mid)
* 192.168.0.0 - 192.168.255.255 => 192.168/16 prefix (less)

* Launch instances into a subnet of your choosing
* Assign custom IP address ranges in each subnet
* Configure route tables between subnets
    * You can block the connection between two subnets
* Create internet gateway and attach it to our VPC
    * 1 internet gateway - 1 VPC.
    * 1 subnet - 1 AZ
    * 1 AWS Region - 5 VPC (by default)
* Much better security control over your AWS resources.
* Instance security groups
* Subnet network access control lists (ACLS)


### Default VPC & Custom VPC

* Default => user friendly, immediately deploy instances
* Default => All subnets have a route out to the internet
* Each EC2 instance has both a public and private IP address

### VPC Peering

* Allows you to connect one VPC with another via a direct network route using private IP addresses
* Instances behave as if they were on the same private network
* You can peer VPC's with other AWS accounts as well as with other VPCs in the same acount.
* No transitive peering (If VPCA === VPCB and VPCA === VPCC, VPCB !== VPCC)