## EBS (Elastic Block Storage)

* Disk in the cloud
* Allows you to create storage volumes and attach them to EC2 instances.
* Once attached, you can:
    * Create a file system
    * Run a db
    * Use them any other way you would use a block device.
* EBS volumes are placed in a specific Availability Zone, where they are automatically replicated to protect you from the failure of a single component.
* EC2 instances and their EBS volumes must be in the same availability zone.

### Types

* General Purpose SSD (GP2)
    * Balances price and performance
    * Ratio of 3 IOPS per GB with up to 10000 IOPS and ability to burst up to 3000 IOPS for extended periods of time for volumes at 3334 GB and above.

`If you have <10000 IOPS, you probably want GP2`

* Provisioned IOPS SSD (IO1)
    * Very high performance
    * Designed for I/O intensive apps such as large relational SQL or NoSQL Dbs
    * If you need more than 10000 IOPS
    * Can be provisioned to 20000 IOPS per volume

### EBS Volume Types

* Thruput Optimized HDD (ST1)
    * Big data
    * Data warehouses
    * Log processing
    * Cannot be a boot volume
* Cold HDD (SC1)
    * Lowest cost
    * Infreq. accessed workloads
    * File Server
    * Cannot be a boot volume
* Magnetic (Standard)
    * Lowest cost per gb of all EBS volume types that is bootable.
    * Ideal for workloads where data is accessed infreq.
    * For Apps where the lowest storage cost is important
    * Legacy.
