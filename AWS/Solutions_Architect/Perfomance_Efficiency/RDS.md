# Read Replicas

*supported by MySQL, PostgreSQL, Maria, Aurora* NOT Oracle, nor SQL Server


# Storage types
## General Purpose SSD Storage
cost-effective storage that is acceptable for most database workloads
## Provisioned IOPS SSD Storage
Provisioned IOPS storage is a storage type that delivers predictable performance, and consistently low latency. Provisioned IOPS storage is optimized for online transaction processing (OLTP) workloads that have consistent performance requirements.
## Magnetic Storage
for backward compatibility. We recommend that you use General Purpose SSD or Provisioned IOPS SSD for any new storage needs.
    Doesn't allow you to scale storage when using the SQL Server database engine.

    Doesn't support storage autoscaling.

    Doesn't support elastic volumes.

    Limited to a maximum size of 3 TiB.

    Limited to a maximum of 1,000 IOPS.

# Aurora
With Aurora MySQL you can configure cross-region Aurora Replicas using logical replication to up to five secondary AWS regions. Aurora PostgreSQL currently does not support cross-region replicas. Aurora Replica physical replication can only replicate to one secondary region. Using Aurora over RDS provides multiple read replicas in the deployment region and other benefits automatically without having to configure them.

* Aurora storage limit is not an adjustable quota

https://aws.amazon.com/rds/faqs/