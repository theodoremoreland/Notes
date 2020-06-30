* A change porpogates immediately
* All traffic (ports, IP addresses) are blocked / denied by default
* All outbound traffic is allowed by default
* Can only allow traffic (certain ports, IP addresses)
* Can attach multiple security groups to server, meaning the allowed traffic is compounded (assuming each group has different inbound/outbound access)
* Can have any number of servers attached to a single security group

# Stateful
When you apply an inboud rule, a symmetric outbound rule is automatically created.


# Extra 

from acloudguru forums @ https://acloud.guru/forums/aws-csa-2019/discussion/-LuWv1R2IdRlVMCpgtSR/important_to_remember,_securit

* Security groups (SG) control inbound and outbound traffic for your instances (SG = Firewall for EC2 Instances)

* NACLs control inbound and outbound traffic for your subnets (NACL = Firewall for Subnets)

There are Layers of Security, like an Onion. This is a Great Link that explain that:
https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Security.html

