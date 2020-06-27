# Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. 

## Sections
- [Free Tier](#Free-Tier)
- [Five Pricing Models](#Five-Pricing-Models)
- [Placement Groups](#Placement-Groups)
- [Auto Scaling Groups](#Auto-Scaling-Groups)
- [Elastic Loud Balancers](#Elastic-Load-Balancers)

## Links

https://aws.amazon.com/ec2/pricing/

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/placement-groups.html


# Free Tier
AWS Free Tier includes 750 hours of Linux and Windows t2.micro instances each month for one year. 

https://aws.amazon.com/ec2/pricing/


# Five Pricing Models

### On-Demand
With On-Demand instances, you pay for compute capacity by the hour or the second depending on which instances you run. No longer-term commitments or upfront payments are needed. 

On-Demand instances are recommended for:
* Users that prefer the low cost and flexibility of Amazon EC2 without any up-front payment or long-term commitment
* Applications with short-term, spiky, or unpredictable workloads that cannot be interrupted
* Applications being developed or tested on Amazon EC2 for the first time

### Savings Plans
Savings Plans are a flexible pricing model that offer low prices on EC2 and Fargate usage, in exchange for a commitment to a consistent amount of usage (measured in $/hour) for a 1 or 3 year term.

### Reserved Instances

Reserved Instances provide you with a significant discount (up to 75%) compared to On-Demand instance pricing. In addition, when Reserved Instances are assigned to a specific Availability Zone, they provide a capacity reservation, giving you additional confidence in your ability to launch instances when you need them.

Pricing for Reserved instances come in three options:
* AURI (All upfront reserved instance)
* PURI (Partial upfront reserved instance)
* NURI (No upfront reserved instance)

Reserved Instances are recommended for:

* Applications with steady state usage
* Applications that may require reserved capacity
* Customers that can commit to using EC2 over a 1 or 3 year term to reduce their total computing costs

### Spot Instances
Amazon EC2 Spot instances allow you to request spare Amazon EC2 computing capacity for up to 90% off the On-Demand price.

Spot instances are recommended for:
* Applications that have flexible start and end times
* Applications that are only feasible at very low compute prices
* Users with urgent computing needs for large amounts of additional capacity

### Dedicated Hosts
A Dedicated Host is a physical EC2 server dedicated for your use. Dedicated Hosts can help you reduce costs by allowing you to use your existing server-bound software licenses, including Windows Server, SQL Server, and SUSE Linux Enterprise Server (subject to your license terms), and can also help you meet compliance requirements.

* Can be purchased On-Demand (hourly).
* Can be purchased as a Reservation for up to 70% off the On-Demand price.

# Placement Groups

## Placement group strategies:
### Cluster
Packs instances close together inside an Availability Zone. This strategy enables workloads to achieve the low-latency network performance necessary for tightly-coupled node-to-node communication that is typical of HPC applications.

### Spread
Strictly places a small group of instances across distinct underlying hardware to reduce correlated failures.


### Partition
Spreads your instances across logical partitions such that groups of instances in one partition do not share the underlying hardware with groups of instances in different partitions. This strategy is typically used by large distributed and replicated workloads, such as Hadoop, Cassandra, and Kafka.

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/placement-groups.html


# Auto Scaling Groups


# Elastic Load Balancers

### Classic Load Balancer

### Network load balancer (operate at layer 4)

### Application load balancer (operates on level 7 only)