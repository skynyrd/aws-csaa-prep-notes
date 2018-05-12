All AMIs are categorized as either backed by Amazon EBS or backed by instance store.

`For EBS Volumes`: The root device for an instance launched from the AMI is an Amazon EBS volume created from an Amazon EBS snapshot.

`For Instance Store Volumes (Ephemeral Storage)`: The root device is an instance store volume created from a template stored in Amazon S3. Provisioning is slower.