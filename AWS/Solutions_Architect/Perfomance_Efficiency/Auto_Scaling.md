* Can schedule scaling for specific times

# Launch Configuration
* Specifies EC2 instance type and AMI name

# Auto Scaling Group
* References the launch configuration
* Speciies min, max, and desired size of auto scaling group
* May reference and ELB
* Health Check type

# Auto Scaling Policy
* Specifies how to scale
* One or more may be attached to an auto scaling group