# Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers. 

## Sections
- [Free Tier](#Free-Tier)
- [Five Pricing Models](#Five-Pricing-Models)
- [Placement Groups](#Placement-Groups)
- [Auto Scaling Groups](#Auto-Scaling-Groups)
- [Elastic Loud Balancers](#Elastic-Load-Balancers)
- [EBS](#EBS)

## Links

https://aws.amazon.com/ec2/pricing/

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/placement-groups.html

https://aws.amazon.com/elasticloadbalancing/

https://aws.amazon.com/ebs/?ebs-whats-new.sort-by=item.additionalFields.postDateTime&ebs-whats-new.sort-order=desc

https://aws.amazon.com/ebs/volume-types/

**can encrpyt root ebs volumes during lauch / config**
**termination protection is turned off by default, must be manually turned on**
**on ebs backed instance, default behavior is to delete the ebs volume upon ec2 termination, but not additional volumes by default**

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

Reserved Instance Types:
* **Standard** (Up to 75% off, the more you pay upfront and the longer the contract, the less you pay)
* **Convertible** (Up to 54% off, allows flexbility of instance types of equal or greater value)
* **Scheduled** (Reserve a fraction of a day/week/month)

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

**Elastic Load Balancing automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, and Lambda functions. It can handle the varying load of your application traffic in a single Availability Zone or across multiple Availability Zones.**

* 504 Error = Application timed out (i.e. didn't respond within the idle time out peroid).
* X-Forwarded-For header contains IP Address of end users.

## Classic Load Balancer

Classic Load Balancer provides basic load balancing across multiple Amazon EC2 instances and operates at both the request level and connection level. 

Classic Load Balancer is intended for applications that were built within the EC2-Classic network.

## Network load balancer

Network Load Balancer is best suited for load balancing of Transmission Control Protocol (TCP), User Datagram Protocol (UDP) and Transport Layer Security (TLS) traffic where extreme performance is required.

Operating at the connection level (Layer 4), Network Load Balancer routes traffic to targets within Amazon Virtual Private Cloud (Amazon VPC) and is capable of handling millions of requests per second while maintaining ultra-low latencies. 

Network Load Balancer is also optimized to handle sudden and volatile traffic patterns.

## Application load balancer

Application Load Balancer is best suited for load balancing of HTTP and HTTPS traffic and provides advanced request routing targeted at the delivery of modern application architectures, including microservices and containers.

Operating at the individual request level (Layer 7), Application Load Balancer routes traffic to targets within Amazon Virtual Private Cloud (Amazon VPC) based on the content of the request.

# EBS
Amazon Elastic Block Store (EBS) is an easy to use, high performance block storage service designed for use with Amazon Elastic Compute Cloud (EC2) for both throughput and transaction intensive workloads at any scale. A broad range of workloads, such as relational and non-relational databases, enterprise applications, containerized applications, big data analytics engines, file systems, and media workflows are widely deployed on Amazon EBS.

## Five Types of Storage

### General Purpose SSD (gp2)
General Purpose SSD volume that balances price performance for a wide variety of transactional workloads

* **Use Cases:** Boot volumes, low-latency interactive apps, dev & test
* **Volume Size:** 1 GB – 16 TB
* **Max IOPS**/Volume:** 16,000

### Provisioned IOPS SSD (io1)
High performance SSD volume designed for latency-sensitive transactional workloads

* **Use Cases:** I/O-intensive NoSQL & relational databases
* **Volume Size:** 4 GB – 16 TB
* **Max IOPS*/Volume:** 64,000

### Throughput Optimized Hard Disk Drive (st1)
Low cost HDD volume designed for frequently accessed, throughput-intensive workloads

* **Use Cases:** Big data, data warehouses, log processing
* **Volume Size:** 500 GB – 16 TB
* **Max IOPS**/Volume:** 500

### Cold Hard Disk Drive (sc1)
Lowest cost HDD volume designed for less frequently accessed workloads

* **Use Cases:** Colder data requiring fewer scans per day
* **Volume Size:** 500 GB – 16 TB
* **Max IOPS**/Volume:** 250

### Magnetic (Standard)
Previous generation SSD

* **Use Cases:** Workloads where data is infrequently accessed
* **Volume Size:** 1 GiB - 1 TiB
* **Max IOPS**/Volume:** 40-200

https://aws.amazon.com/ebs/volume-types/


Elastic Fabric Adapter

https://aws.amazon.com/ec2/faqs/