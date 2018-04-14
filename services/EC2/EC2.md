# EC2 (Elastic Compute Cloud)

```
Web service that provides resizable compute capacity in the cloud. Reduces the time required to obtain and boot new server instances to minutes,
allowing to quicklyscale capasity, both up and down, as computing reqs change.
```
* Pay only for capacity that you actually use
* Provides devs the tools to build failure resilient apps
* Isolates devs from common failure scenarios

### EC2 Options

* __On Demand__: Pay a fixed rate by the hour (or by the second - linux only) with no commitment. Most popular.
* __Reserved__: Capacity reservation, 1 year or 3 year terms. Significant discount on the hourly charge.
* __Spot__: Bid whatever price you want for instance capacity, providing for even greater savings if your apps have flexible start and end times.
* __Dedicated Hosts__: Physical EC2 server dedicated for your use. Dedicated Hosts can help you reduce costs by allowing to use your existing server-bound software licences.

#### On Demand

* Low cost and flexibility of EC2 without up-front payment or long-term commitment
* Apps with short term, spiky or unpredictable workloads that cannot be interrupted
* Apps being developed or tested on EC2 for the first time

#### Reserved

* Apps with steady state or predictable usage
* Apps that require reserved capacity
* Users able to make upfront payments to reduce their total computing costs even further
    * __Standard RI (Reserved Instance)__: Up to 75% off on demand
    * __Convertible RI's__: Up to 54% off on demand. Capability to change the attributes of the RI as long as the exchange results in the creation of Reserved Instances of equal or greater value. (Change attribute e.g. Windows -> Linux, General purpose -> CPU optimized)
    * __Scheduled RI's__: Match your capacity reservation to a predictable recurring schedule that only requires a fraction of a day, a week or a month

#### Spot

* Apps that have flexible start and end times
* Apps that are only feasible at very low compute prices
* Users with urgent computing needs for large amount of additional capacity.