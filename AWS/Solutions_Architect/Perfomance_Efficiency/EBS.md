# Amazon Elastic Block Store (EBS) is an easy to use, high performance block storage service designed for use with Amazon Elastic Compute Cloud (EC2) for both throughput and transaction intensive workloads at any scale. A broad range of workloads, such as relational and non-relational databases, enterprise applications, containerized applications, big data analytics engines, file systems, and media workflows are widely deployed on Amazon EBS.

**on ebs backed instance, default behavior is to delete the ebs volume upon ec2 termination, but not additional volumes by default**

**EBS Snapshots are backed up to S3 incrementally**

**EBS volumes are replicated to another AZ automatically**

To delete an EBS Snapshot attached to a registered AMI, first remove the AMI, then the snapshot can be deleted

# Five Types of Storage

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

# EBS vs Instance Store
* Instace store volumes are nicknamed "Ephemeral storage"
* Instance store volumes can not be added about provisioning
* Instance store backed EC2 instances can not be stopped (only rebooted or terminated)
* Because they can not be stopped, if the host fails, the data is lost (but not when rebooted).
* Both (EBS and Instance Store) root volumes will be deleted on termination of EC2 by default, but with EBS backed instances, you can configure it such that AWS saves the EBS volume.