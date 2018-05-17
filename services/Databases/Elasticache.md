* In memory cache. 

### Types

* Memcached, single AZ
* Redis, multi AZ capability

### Exam tips

* Elasticache is a good choice if your db is particularly read heavy and not prone to frequent changing.
* Redshift is a good answer if the reason your db is feeling stress is because management keep running OLAP transactions on it etc.