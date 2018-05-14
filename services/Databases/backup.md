### Automated Backups

* Allow you to recover your db to any point in time within a `retention period`. (RP can be between 1-35 day.)
* AWS chooses the most recent daily back up, and then apply transaction logs relevant to that day. This allows you to do a point in time recovery down to a second, within the retention period.
* Enabled by default
* Stored in S3
* You have a free storage space equal to the size of your db.


### Snapshots

* They are stored even after you delete the original RDS instance, unlike automated backups.

### Restoring Backups

* Restored to new RDS instance
* new DNS

### Encryption

* Supported for MySQL, Oracle, SQL Server, PostgreSQL, MariaDB and Aurora.
* Done by AWS Key Management Service (KMS)
* Once encrypted, automated backups, read replicas, snapshots, data stored at rest are also encrypted.
* At present time, encrypting an existing DB Instance is not supported. To do that, you must first create a snapshot, make a copy of that snapshot and encrypt the copy.

### Multi-AZ RDS

* Allows you to have an exact copy of your prod db in another AZ.
* AWS handles the replication for you.
* If DB instance or AZ failure happens, Amazon RDS will automatically failover to the standby so that db operations can resume quickly without admin. intervention.
* For ONLY DISASTER RECOVERY.
* You want performance improvement? You need read replicas.