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