*** Legacy System: `Import/Export` service, which you are sending your hardware to `Amazon` and they transfer data to `AWS` using the internal network ***

`Your local <=> Physical hardware (ready to be posted to...) <=> Amazon <=> AWS Cloud`

### Types

* Snowball
* Snowball Edge
* Snowmobile


### Snowball

* Petabyte-scale data transport solution
* can be as little as one-fifth the cost of high speed internet
* 80TB snowball in all regions.
* uses multiple layers of security designed to protect the data
    * tamper resistant enclosures
    * 256 bit encryption
    * trusted platform module (TPM) 
* Once the data transfer job has been processed and verified, AWS performs a software erasure of the snowball applience.
* You can track where is your snowball
* 80TB on board storage
* Import/Export from S3

### Snowball Edge

* Similar looking to `Snowball`
* 100GB on board storage
* Compute capability e.g. lambda
* Little AWS datacenter
* use case: Can be used in the airplane to collect and compute data, then data can be transferred to AWS.

### Snowmobile

* Exabyte(!) scale data transfer service
* You can transfer up to 100PB per Snowmobile, __a 45 foot long ruggedized shipping container pulled by a semi-trailer truck!__
* Can be used for massive video, image repos, or even a complete data center migration.
* Secure, fast and cost effective

### Regular snowball request steps

`Job created => Prepared Appliance => Prepared shipment => Shipped to you => In transit to AWS => At AWS => Importing => Completed`

### Usage

* Built-in display => Kindle on Snowball
* Download client tool
* Connect via `RJ45`, `SFP + Copper` or `SFP Optical`
* Power up.
* Get credentials from AWS Console.
* `./snowball start -i XXX.XXX.XXX.XXX -m SOMERANDOMGUID_manifest.bin -u GUID`
* `./snowball cp YOUR_LOCAL_FILE s3://yourusername-snowball`