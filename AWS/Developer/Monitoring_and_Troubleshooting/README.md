# General
Check the error code
* 400 series = fix application
* 500 series = retry operation

Collection and analysis of log data from sources such as
* System logs
* HTTP logs

Monitoring of
* Instance health and performance
* Availability of managed services (RDS, etc)
* Networking
* Utilization for costs efficiency
* Unused or under-used instances running


# Axioms
* Always check security groups and network access control lists when troubleshooting
* Instances launched into a private subnet in a VPC can't properly communicate with the Internet unless you use NAT
* You need an IGW and a route in the route table to talk to the internet
* EBS vloumes are loosely couple to EC2 instances; can attach/detach except for the boot volume