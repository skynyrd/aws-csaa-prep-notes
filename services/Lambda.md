`Compute service where you can upload your code and create a Lambda function`

Two typical use case:

* Event driven compute service where Lambda runs your code in response to events such as change data in S3 bucket etc.
* Compute service to run your code in response to HTTP requests using Amazon API Gateway or API calls made using AWS SDKs.
* No servers.
* Continuous Scaling.
* Cheap

Lambda encapsulates

* Data Centers,
* Hardware,
* Assembly Code / Protocols,
* Application Layer / AWS APIs
* Operating systems

Everytime user invokes e.g. API Gateway, a lambda function is invoked.

`Supported Languages`

* NodeJS
* Java
* Python
* C#

`Pricing`

* __Number of requests__: First 1 million requests are free. After that, $0.20 per 1 million requests.
* __Duration__: Time your code begins executing until it returns or terminates, rounded up to the nearest 100ms. $0.00001667 for every GB-second used.

`Exam Tips`

* Lambda scales out (not up) automatically.
* Indpendant 