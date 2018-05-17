* Fast and flexible NoSQL db service.
* Single digit ms latency.
* Flexible data model and reliable performance.
* Stored on SSD storage.
* Spread across 3 geographically distinct data centres.
* Eventual consistent reads (default)
    * Best performance
* Strong consistent reads
* Cheap for reads, can be expensive for rights
* __Push button scaling, no downtime__

### Pricing

* Provisioned Throughput Capacity
    * Write thruput $0.0065 per hour for every 10 units
    * Read thruput $0.0065 per hour for every 50 units
    * Storage $0.25 per GB/month

e.g. `1 million write and read per day, 3GB data`

1000000/24 hours/60 minutes/60 seconds = 11.6 writes per second