* Relational DB Engine
* MySQL compatible
* Five times better performance than MySQL
* Price is one tenth that of a commercial db for a similar performance and availability

### Scaling

* Start with 10Gb, scales in 10Gb increments to 64TB (Storage autoscaling)
* Compute resources can scale up to 32vCPUs and 244GB of Memory.
* 2 copies of your data is contained in each AZ, min 3. So 6 copies of your data.
* Designed to transparently handle the loss of up to two copies of data withour affecting db write availability and up to three copies without affecting read availability.
* Storage is self-healing. Data blocks and disks are continuously scanned for disk failures.

### Replicas

* Aurora Replicas (currently 15)
* MySQL Read Replicas (currently 5)