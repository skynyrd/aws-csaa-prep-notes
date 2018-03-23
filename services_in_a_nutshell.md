## Compute

* __EC2 (Elastic Compute Cloud)__: Typically Virtual Machines on AWS, can contains physical machines as well.
* __EC2 Container Service__: Run and manage docker containers at scale.
* __Elastic Beanstalk__: You simply upload your application, and Elastic Beanstalk automatically handles the details of capacity provisioning, load balancing, scaling, and application health monitoring.
* __Lambda__:  Event-driven, serverless computing platform.
* __Lightsail__: VPS service.
* __Batch__: For batch computing in the cloud.


## Storage

* __S3 (Simple Storage Server)__: Files to buckets in the cloud.
* __EFS (Elastic File System)__: Network attached storage. Store files and mount to multiple VMs.
* __Glacier__: For archived data, cheap.
* __Snowball__: To bring in large amounts of data.
* __Storage Gateway__: Install in your datacenter, replicate information back to S3 (?)


## Databases

* __RDS (Relational Database Service)__: Like Postgres, MySQL etc.
* __DynamoDB__: Non relational database.
* __Elasticache__: Caching db
* __Red Shift__: Data warehousing, business intelligence.

## Migration

* __AWS Migration Hub__: Tracking service for your applications migrated to AWS
* __Application Discovery Service__: Set of automation tools for dependencies etc. (?)
* __Database Migration Service__: Migrate your databases to AWS.
* __Server Migration Service__: Migrate your servers to AWS.
* __Snowball__: Mentioned before. Also used for migrating large amounts of data into the cloud (terabytes)

## Networking & Content Delivery

* __VPC (Virtual Private Cloud)__: Virtual data centers, configure firewals, configure availability zones etc.
* __CloudFront__: Content Delivery Network
* __Route53__: DNS Service 
* __API Gateway__: Way of creating your own apis.
* __Direct Connect__: Dedicated line between you and AWS.

## Developer Tools

* __CodeStar__: Project management
* __CodeCommit__: Version management
* __CodeBuild__: Project builder
* __CodeDeploy__: Deployment service
* __CodePipeline__: CI
* __X-Ray__: Debug and analyze your serverless apps.
* __Cloud 9__: Online IDE.

## Management Tools

* __CloudWatch__: Monitoring
* __CloudFormation__: Scripting infrastructure. (e.g. take a cloud formation reusable template and deploy a wordpress site.) _IMPORTANT FOR CSAAs!_
* __CloudTrail__: Used to track logs _IMPORTANT FOR CSAAs!_
* __Config__: Monitors all the config in AWS, includes snapshot feature.
* __OpsWorks__: Similar to ElasticBeanstalk, but its a lot more robust. Uses chef and puppet.
* __Service Catalog__: Way of managing catalogs of the services, they can be VMs, images, databases etc. (Typically used by big corps.)
* __Systems Manager__: Managing AWS resources, typically used for EC2
* __Trusted Advisor__: Gives you advice about security
* __Managed Service__: Manages your services for you. (?)

## Media Services

* __Elastic Transcoder__: Takes the video, then resizes and modifies it.
* __MediaConvert__: File based video transcoding service.
* __MediaLive__: Live video processing service.
* __MediaPackage__: Prepares and protects your videos for delivery over the internet.
* __MediaStore__: Storage service built for videos
* __MediaTailor__: To do targeted advertising into video streams without sacrificing broadcast level quality of service

## Machine Learning

* __SageMaker__: Deep learning
* __Comprehend__: Sentiment analysis on data
* __DeepLens__: Deep learning enabled video camera
* __Lex__: Powers Amazon Alexa, way of communicating with customers
* __Machine Learning__: Throw a dataset and analyze.
* __Polly__: Takes text and turns it into speech
* __Rekognition__: Recognizes items and objects in the video
* __Amazon Translate__: Machine translation service (like Google Translate)
* __Amazon Transcribe__: Automatic speech recognation, speech to text. (cool usage ex: upload a video, use transcribe to get text, use translate to change its language, turn it to mp3 with polly and send it to amazon echo.)
