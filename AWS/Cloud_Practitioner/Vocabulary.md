## Sections
- [Definitions](#Definitions)
- [Acronyms](#Acronyms)
- [Initialisms](#Initialisms)

# Definitions

### Automation

"Cloud automation is the practice or discipline of using specialized software tools and methodologies to automate some or all of the manual tasks associated with managing and operating cloud-based IT infrastructure." - sumo logic

https://www.sumologic.com/glossary/cloud-automation/

### Availability

Availability refers to system uptime (i.e. the system is live and can deliver data upon request). Historically, this has been achieved through hardware redundancy so that if any component fails, access to data will prevail.

### Reliability

"Reliability is closely related to availability, however, a system can be ‘available’ but not be working properly. Reliability is the probability that a system will work as designed." - Aditya

https://medium.com/@sprinkle_twinkles/availability-vs-reliability-vs-durability-vs-resiliency-dfead8c92c58

"The ability of a system to recover from infrastructure or service disruptions, dynamically acquire computing resources to meet demand, and mitigate disruptions such as misconfigurations or transient network issues." - AWS

https://wa.aws.amazon.com/wat.pillar.reliability.en.html

### Durability

Refers to long-term data protection. Rather than focusing on hardware redundancy, it is concerned with data redundancy so that data is never lost or compromised (e.g. bit rot, degradation, corruption, etc)

### Scalability

Successful, growing, systems often see an increase in demand over time. A system that is scalable can adapt to meet this new level of demand.

https://wa.aws.amazon.com/wat.concept.scalability.en.html

### Elasticity

The ability to acquire resources as you need them and release resources when you no longer need them. In the cloud, you want to do this automatically.

https://wa.aws.amazon.com/wat.concept.elasticity.en.html


### Elastic vs Scalable

Scalable systems will accomodate increases in demand by adding resources (typically more EC2 instances). Elastic systems will both add and remove resources relative to demand (think of a rubberband; it can grow and shrink in size).

### Fault Tolerant

"Fault tolerance relies on specialized hardware to detect a hardware fault and instantaneously switch to a redundant hardware component—whether the failed component is a processor, memory board, power supply, I/O subsystem, or storage subsystem. Although this cutover is apparently seamless and offers non-stop service, a high premium is paid in both hardware cost and performance because the redundant components do no processing. More importantly, the fault tolerant model does not address software failures, by far the most common reason for downtime." - IBM

https://www.ibm.com/support/knowledgecenter/SSPHQG_7.2/concept/ha_concepts_fault.html


### Resource Group Vs Placement Group

* A resource group is a collection of AWS resources that are all in the same AWS region, and that match criteria provided in a query (e.g. a query based on tags or a query based on a CloudFormation stack). 

https://docs.aws.amazon.com/ARG/latest/userguide/welcome.html

* When you launch a new EC2 instance, the EC2 service attempts to place the instance in such a way that all of your instances are spread out across underlying hardware to minimize correlated failures. You can use placement groups to influence the placement of a group of interdependent instances to meet the needs of your workload.

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/placement-groups.html

# Acronyms

    Capex (Capital Expenditure)
    Opex (Operational Expenditure)


# Initialisms
    ACM (AWS Certificate Manager)
    AMI (Amazon Machine Image)
    ARN (Amazon Resource Name)
    CAF (Cloud Adoption Framework)
    CIDR (Classless Inter-Domain Routing)
    CMK (Customer Master Key)
    EC2 (Elastic Cloud Compute)
    ECR (Elastic Container Registry)
    ECS (Elastic Container Service)
    EFS (Elastic File System)
    EKS (Elastic Kubernetes Service)
    EMR (Elastic MapReduce)
    FSx (File system x ???)
    IAM (Identity and Access Management)
    IoT (Internet of Things)
    MSK (Managed Streaming for Kafka)
    MQ (Messaging Queue)   
    QLDB (Quantum Ledger Database)
    RDS (Relational Database Service)
    S3 (Simple Storage Service)
    SNS (Simple Notification Service)
    SQS (Simple Queue Service)
    SWF (Simple Workflow Service)
    TCO (Total Cost of Ownership)
    VPC (Virtual Private Cloud)
    WAF (Web Application Firewall)    
    
    
https://docs.aws.amazon.com/general/latest/gr/glos-chap.html