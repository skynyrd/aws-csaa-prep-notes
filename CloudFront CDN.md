`A content delivery network (CDN) is a system of distributed servers that deliver webpages and other content to a user based on the geo locations of the user, the origin of the webpage and a content delivery server.`


* __Edge Location__: Location where content will be cached, seperate to an AWS Region/AZ
* __Origin__: Origin of all the files that CDN will distribute. Can be S3 bucket, EC2 instance, Elastic Load Balancer or Route53 or non AWS origin server.
* __Distribution__: Name given the CDN consisting collection of Edge Locations.

__CloudFront can be used for:__

* Entire website,
* Dynamic,
* Static,
* Streaming,
* Interactive content.

__Terminology__

* Web distribution: Website
* RTMP: Used for media streaming

__Edge locations are not just READ only, you can write to them too!__

__Objects are cached for the life of the TTL (Time to live)__

__You can clear cached objects, but you will be charged__