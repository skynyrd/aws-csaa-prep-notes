* Virtual Firewall
* 1 security group can have multiple instances.
* 1 instance can have multiple security groups, groups are joined.
* Changes to security groups take effect immediately.
* All inbound traffic is blocked by default.
* All outbound traffic is allowed by default.
* Security groups are stateful.
    * If you set an `inbound` rule, `outbound` rule is also set automatically.
* You can't block specific IP addresses using sec groups, instead use Network Access Control Lists. (see VPC section for further details)
* You can specify allow rules, but not deny rules.