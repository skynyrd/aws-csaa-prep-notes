## Identity Access Management

* Manage users and their levels to the AWS Console
* Centralised control
* Granular Permissions
* Identity Federation e.g. Active dir, Facebook, Linked In...
* Multifactor Auth
* Temp access for users/devices and services if necessary
* Configurable pass rotation policy
* Integration to many AWS services
* Supports PCI DSS

__IAM Service is available in all regions. (Top right: Global)__

Users sign in link: https://YOUR_AWS_ACCOUNT_NUMBER.signin.aws.amazon.com/console, you can alias your aws account number with some string with `Customize` section.

* At first, root access keys should be deleted, IAM users should be created instead.
* Multi factor auth should be enabled for the root acount. (Google authenticator)

`There are 2 access types, programmatic allows your apis to connect AWS and management console allows you to log in to the AWS management console.`

Policy files are in JSON format.

`Access key ID` & `Secret access key` for programmatic access.

User Permissions can be from the group of the user or direct.

#### Roles (Different than user permissions)

* Secure way to grant permissions to entities that you trust.
* Application code running on an EC2 instance that needs to perform actions on AWS resources
* IAM user in another account
* An AWS service that needs to act on resources in your account to provide its features
* Users from a corporate directory who use identity federation with SAML

### To Conclude

* IAM => Global region
* Root acount (got Administrator Access) is simply the account created when first setup your AWS account. Has complete Admin access.
* New users have NO permissions when first created.
* New users are assigned Access Key ID & Secret Access Keys when first created. And these are for programmatic access.
* These keys only get to view once. If you lose them, you have to regenerate them. So it must be saved in a secure location when first created.
* Multifactor Auth should be set up.
* Password rotation policy should be set.
* Power user access allows access to all AWS services except for management of groups and users within IAM

