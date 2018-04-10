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

#### Notes

* Edge locations are not just READ only, you can write to them too!
* Objects are cached for the life of the TTL (Time to live)
* You can clear cached objects, but you will be charged
* Bucket address can be restricted over CloudFront configuration
* Path pattern takes RegEx

For cache:

* Protocol policy can be configured (HTTP, HTTPS, both or redirection etc.)
* Allowed HTTP methods can be configured (GET, HEAD, OPTIONS, PUT, DELETE...)
* Time to live (TTL) can be configured for minimum, max and default (unit: sec)
* Viewer access can be restricted (with signed URLs and cookies)
* Alternate domain names can be configured
* Geo-Restriction can be enabled (Whitelist/Blacklist of countries)
* Can be invalidated any time from the CloudFront web console.