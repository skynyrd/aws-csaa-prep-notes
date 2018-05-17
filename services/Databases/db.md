* You need to specify a port number or protocol when you add a rule to an RDS security group.
* If you use RDS provisioned IOPS storage with MySQL or Oracle engines, max volume can have 6TB.
* By default, the maximum provisioned IOPS capacity on an Oracle and MySQL RDS instance (using provisioned IOPS) is 30,000 IOPS.

#### Relational DB

* Since 70s
* Traditional spreadsheet
* Database, Tables, Row, Fields
* SQL Server, Oracle, MySQL, PostgreSQL, Amazon Aurora, MariaDB

#### Non Relational DB

* Collection
* Document
* Key Value Pairs
* JSON
* DynamoDB

#### Data Warehousing

* Used for business intelligence
* Jaspersoft, SQL Server Reporting Service, SAP NetWeaver
* Used to pull in very large and complex data sets.

* `OLTP - Online Transaction Processing` - Short online transactions (Insert, Update, Delete etc.)
* `OLAP - Online Analytics Processing` - deals with Historical/Archival Data. Queries are complex, involve aggregations. e.g. Sum of radios sold in EMEA


#### Elasticache

* Web service that makes it easy to deploy, operate, and scale an in memory cache in the cloud.
* Supports two open source in memory caching engines: `Memcached` and `Redis`


#### AWS Database Types

* RDS - OLTP
    * SQL (MySQL, PostgreSQL, Oracle, Aurora, MariaDB)
* DynamoDB - No SQL
* RedShift - OLAP
* Elasticache - In Memory Caching

#### Read Replicas

* Allow you to have a read only copy of your prod db.
* Archived by using async replication from primary RDS instance to the read replica.
* For read heavy workloads.
* Available for MySQL, PostgreSQL, MariaDB and Aurora
* Used for scale out (horizontal scale)
* Must have auto backup turned on to deploy a read replica
* You can have up to 5 read replica.
* You can have read replicas of read replicas (but watch for latency.)
* Each read replica will have its own DNS end point.
* You can have read replicas that have Multi AZ
* You can create read replicas of Multi AZ source dbs.
* Can be promoted to be their own databases. This breaks the replication.
* You can have a read replica in a second region.
* Replicating data from primary RDS instance to secondary RDS instance is free.