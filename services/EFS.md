* ~ FTP
* Amazon Elastic File System (EFS) is a file storage service for EC2.
* Storage capacity is elastic, growing and shrinking automatically as you add and remove files.
* Supports NFSv4 protocol.
* You only pay for the storage you use.
* Can scale up to petabytes.
* ==> __Can support thousands of concurrent NFS connections.__ (Connect hundreds of EC2 instances to the same volume. EBS can connect to one.)
* Data is stored across multiple AZ's with a region.
* Block based, not object based.
* Read after write consistency.
