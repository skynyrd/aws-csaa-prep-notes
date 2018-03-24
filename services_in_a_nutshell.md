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

## Analytics

* __Athena__: SQL queries against things in S3 buckets.
* __EMR (Elastic Map Reduce)__: For processing large amounts of data.
* __CloudSearch & ElasticSearch__: Search services
* __Kinesis__: Ingesting large amounts of data into AWS, e.g. social media feeds, hashtags
* __Kinesis Video Streams__: For video
* __QuickSight__: Business Intelligence Tool
* __Data Pipeline__: Move data between AWS services
* __Glue__: For ETL

## Security & Identity & Compliance

* __IAM__: Identity Access Management.
* __Cognito__: Way of device authentication, e.g. mobile apps.
* __GuardDuty__: Monitors malicious activities on your AWS account.
* __Inspector__: Agent. e.g. For testing your VMs, can be scheduled.
* __Macie__: Scans your S3 buckets for personal identifiable information, e.g. passport no, addresses, phone numbers.
* __Certificate Manager__: Manages SSL ceritificates. (SSL certificate is free for AWS users registered their domains to Route53)
* __CloudHSM (Hardware Security Module)__: Generate and use your own encryption keys on the AWS Cloud.
* __Directory Services__: Integrate Microsoft Active Directory.
* __WAF (Web Application Firewall)__: Firewall
* __Shield__: To prevent DDOS attacks.
* __Artifact__: Provides on-demand downloads of AWS security and compliance documents e.g.  ISO certifications, Payment Card Industry (PCI), and Service Organization Control (SOC) reports

## Mobile Services

* __Mobile Hub__: Management console for mobile services, generates config file etc.
* __Pinpoint__: For push notifications
* __AWS AppSync__: Auto updates web and mobile apps
* __Device Farm__: For testing apps
* __Mobile Analytics__: Can understand from its name.

## AR / VR (Augmented Reality / Virtual Reality)

* __Sumerian__: To create VR, AR, and 3D experiences

## Application Integration

* __Step Functions__: Managing lambda functions and step functions
* __Amazon MQ__: Message Queue
* __SNS__: Notification Service (Email, SMS etc.)
* __SQS__: Decoupling the infrastructure
* __SWF__: Simple Work Flow

## Customer Engagement

* __Connect__: Contact center as a service (call center)
* __Simple Email Service__: Can understand from its name.

## Business Productivity

* __Alexa For Business__: Use it to dial into a meeting room, to inform IT when printer is broken etc...
* __Chime__: Like Google hangouts or Zoom. Online meeting.
* __Work Docs__: Kinda Dropbox
* __WorkMail__: Kinda Office 365

## Desktop && App Streaming

* __Workspaces__: Desktop envs being running in the cloud streamed to your device
* __AppStream 2.0__: Apps runnning in the cloud streamed to your device

## Internet of Things

* __iOT__: Ubiquitous devices connecting the physical world to the cloud 
* __iOT Device Management__: Service that makes it easy to securely onboard, organize, monitor, and remotely manage IoT devices at scale
* __Amazon FreeRTOS__: Operating System for your microcontrollers
* __Greengrass__: Software that lets you run local compute, messaging & data caching for connected devices in a secure way

## Game Development

* __GameLift__: Dedicated game server hosting