* Data warehouse service in the cloud.
* Start for $0.25 per hour with no commitments to a petabyte or more for $1000 terabyte per year
* Less than a tenth of most other data warehousing solutions.
* OLAP

### Redshift Configuration

* Single Node (160Gb)
* Multi Node
    * Leader Node (manages client connections and receives queries)
    * Compute Node (store data and perform queries). Up to 128 Compute Nodes

 #### Columnar Data Storage

 * Instead of storing data as a series of rows, Redshift organizes the data by column
 * Queries often involve aggregates performed over large data sets.
 * Columnar data is stored sequentially on the storage media.
 * Requires far fewer I/Os, greatly improving query performance.


 #### Advanced Compression

 * Columnar data stores can be compressed much more than row based data stores as similar data is stored sequentially on disk.
 * Multiple compression techniques
 * Redshift doesn't require indexes or materialized views, so uses less space.
 * When loading data into an empty table, Redshift automatically samples your data and selects the most appropriate compression scheme.

 #### Massively Parallel Processing (MPP)

 * Redshift automatically distributes data and query load across all nodes.
 * Makes it easy to add nodes to your data warehouse
 * Enables you to maintain fast query performance as your data warehouse grows.

 #### Pricing

 * Compute Node Hours
 * Backup
 * Data Transfer (only within a VPC)

 #### Security

 * Encrypted in transit using SSL
 * Encrypted at rest using AES-256 encryption
 * By default Redshift takes care of key management
    * Manage your own keys thru HSM
    * AWS Key Management Service

#### Availability

* Currently only available in 1 AZ
* Can restore snapshots to new AZs in the event of an outage.