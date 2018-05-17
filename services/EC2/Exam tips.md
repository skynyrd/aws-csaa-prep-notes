* Learn On Demand
* Learn Reserved
* Learn Spot
* Learn Dedicated Hosts
* `If a spot instance is terminated by Amazon EC2, you will not be charged for a partial hour of usage. However, if you terminate the instance yourself, you will be charged for the complete hour in which instance ran.`
* FIGHT PC DR MX
* Check EBS Hard disk drive types
* When creating an instance:
    * 1 subnet = 1 availability zone
    * A port can be restricted to your ip address or a custom ip block
* If you delete EC2 instance, what will be to the EBS?
    * Default behaviour => It will be deleted as well.
    * You can choose the option when creating an instance.
* Termination protection is turned off by default, you must turn it on.
* EBS Root Volumes of your DEFAULT AMI's cannot be encrypted. You can use a 3rd party tool to encrypt the root volume, or this can be done when creating AMI's in the AWS console or using the API.
* Additional volumes can be encrypted.
* When terminating an EC2 instance, only root volume is terminated, other volumes binded to that EC2 are not terminated by default.
* Snapshots exists on S3, even you can't see them.
* Snapshots are incremental.
* You can take create a snapshot from running instance but you should stop it if you are creating a snapshot of a root volume.
* Amazon Machine Images (AMIs) can be generated from volumes or snaps.
* You can change EBS volume sizes and types of an EC2 instance when it is running, but stop is recommended.
* Snapshots of encrypted volumes are encrypted automatically.
* Volumes restored from encrypted snaps are encrypted automatically.
* Snapshots can be shared with other AWS accounts/publicl if they are not encrypted.


* How can we copy the EBS volume in another availability
zone?
    * We can take a snapshot of an EBS volume, then create another volume with that snap. (Btw we can change the type and availability zone in this step) then we can bind it to a new EC2 instance.
    * Or take an image of it then copy it to another availability zone.

* How can we move an EC2 instance one region to another?
    * Create a snapshot of the EBS volume.
    * Copy the snapshot to another region
    * Create an image with that snap
    * Boot new EC2 instance with that snapshot.

* How to create encrypted AMI?
    * Stop the EC2 instance (recommended)
    * Take a snapshot
    * Copy the snapshot (optional: to another region) with checking encryption option
    * Create an AMI (Amazon Machine Image) from that instance
    * Go to `AMIs` from dashboard
    * Launch an EC2 instance with image

* You can rent/buy AMI from `AWS Marketplace`, or you can use `Community AMIs`

`Instance Store`

* You cannot attach instance store volumes to your instance once after creating it.
* You cannot stop the instance store, you can stop EBS
* If the underlying host fails, you will lose your data.

`EBS Backed Instance`

* Can be stopped
* Will not lose data on this instance if it is stopped.

`For Instance Store and EBS Backed Instance`

* Will not lose your data after reboot
* By default, both ROOT volumes will be deleted on termination, however with EBS volumes, you can tell AWS to keep the root device volume.

`Getting meta data/user data of an instance`

* ssh to the instance
* `curl http://169.254.169.254/latest/meta-data`
* `curl http://169.254.169.254/latest/user-data`
