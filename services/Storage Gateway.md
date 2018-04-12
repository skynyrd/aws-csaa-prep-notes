* Connects an on-premises software appliance with cloud based storage.
* Async replication to AWS (S3, Glacier etc.)

```
Your Data Center ====== Storage Gateway (VM) ======= AWS
```

* Can be downloaded as a VM image that you install on a host in your datacenter.
* Supports VMware ESXi or Microsoft Hyper-V
* After configured, create storage gateway option from AWS Management Console.
* Don't have to be on-premise. Can be EC2 or as it is in Amazon VPC (Virtual Private Cloud)

### Types

* File Gateway (NFS) (Store flat files)
* Volume Gateway (iSCSI) (Block based storage, images etc.)
    * Stored Volumes
    * Cached Volumes
* Tape Gateway (VTL) (Backup/Archive solution)

#### File Gateway (NFS)

* User API Server => Storage Gateway (via NFS)
* Storage Gateaway => AWS Services (S3, S3-IA, Glacier) via
    * `Direct Connect`
    * Internet (most common)
    * `Amazon VPC`

#### Volume Gateway

* Presents disk volumes, virtual harddisk (operating systems, images, sql server etc.)
* iSCSI block protocol
* Can be async backed up as point-in-time snapshots of the volumes.
* Backed up volumes are stored in the cloud as `Amazon EBS (Elastic Block Store)` snapshots
* `Snapshot`: Incremental backup that capture only changed blocks
* All snapshots are compressed.

__Volume Gateway - Stored Volumes__

* Store your primary data locally, async. backups to AWS.
* Virtual harddisk
* 1GB - 16 TB

__Volume Gateway - Cached Volumes__

* S3 - Primary data storage
* Frequently accessed data - on prem. (local)
* Storage volumes -> up to 32 TB

__Tape Gateway__

* durable, cost effective solution to archive data in AWS.
* Supported by NetBackup, Backup Exec, Veeam etc.
* Virtual Tape to AWS

