To Connect to your EC2 instance:

* download your private key, *.pem
* chmod 400 your_private_key.pem
* ssh ec2-user@EC2_IP -i your_private_key.pem


### System Status Check

* Verifies your instance is reachable.
* Tests it via sending network packages
* If fails, there may be an issue with the infrastructure hosting, may be restart is required.
* Status Check Alarm can be set.

### Instance Status Check

* Verifies that your instance's operating system is accepting traffic.
* If fails, you may need to reboot instance.

`Basic Monitoring` : Checks every 5 min.
`Detailed Monitoring` : Checks every 1 min.

### Monitoring metrics

* CPU, Disk etc.
* Status Check Counts
* Network