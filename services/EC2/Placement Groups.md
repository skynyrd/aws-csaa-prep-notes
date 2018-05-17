* Logical grouping of instances within a single Availability Zone.
* Enables applications to participate in a low latency, 10Gbps network.
* Ideal for low network latency, high network thruput or both.
* Can't span a multiple availability zones.
* The name of the placement group must be unique.
* Only certain types of instances can be launched. (Compute optimized, GPU, Memory Optimized, Storage optimized)
* AWS recommends homogenous groups. (same size same type etc)
* You can't merge placement groups.
* You can't move an existing instance into a placement group. You can create an AMI from you existing instance, and then start a new instance from that AMI into a placement group.