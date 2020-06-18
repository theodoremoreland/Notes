"Cloud computing is the on-demand delivery of compute power, database storage, applications, and other IT resources through a cloud services platform via the Internet with pay-as-you-go pricing." - AWS

## Sections
- [Six Advantages of Cloud Computing](#Six-Advantages-of-Cloud-Computing)
- [Types of Cloud Computing / Computing Deployment](#Types-of-Cloud-Computing-Computing)
- [Cloud Computing Models](#Cloud-Computing-Models)
- [AWS Global Infrastructure](#AWS-Global-Infrastructure)
- [AWS Well-Architected Framework](#AWS-Well-Architected-Framewor)
- [AWS Cloud Adoption Framework](#AWS-Cloud-Adoption-Framework)

# Six Advantages of Cloud Computing

### Trade capital expense for variable expense

Instead of having to invest heavily in data centers and servers before you know how you’re going to use them, you can pay only when you consume computing resources, and pay only for how much you consume.

### Benefit from massive economies of scale

By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers is aggregated in the cloud, providers such as AWS can achieve higher economies of scale, which translates into lower pay as-you-go prices.

### Stop guessing capacity

Eliminate guessing on your infrastructure capacity needs. When you make a capacity decision prior to deploying an application, you often end up either sitting on expensive idle resources or dealing with limited capacity. With cloud computing, these problems go away. You can access as much or as little capacity as you need, and scale up and down as required with only a few minutes’ notice.

### Increase speed and agility

In a cloud computing environment, new IT resources are only a click away, which means that you reduce the time to make those resources available to your developers from weeks to just minutes. This results in a dramatic increase in agility for the organization, since the cost and time it takes to experiment and develop is significantly lower.

### Stop spending money running and maintaining data centers

Focus on projects that differentiate your business, not the infrastructure. Cloud computing lets you focus on your own customers, rather than on the heavy lifting of racking, stacking, and powering servers.

### Go global in minutes

Easily deploy your application in multiple regions around the world with just a few clicks. This means you can provide lower latency and a better experience for your customers at minimal cost.

# Types of Cloud Computing

### Public

AWS (Amazon Web Services), Azure, GCP (Google Cloud Platform), IBM Bluemix, Alibaba Cloud, etc.

### Hybrid

A combination of Public and Private.

### Private (On premise)
You manage in personal data center.

https://docs.aws.amazon.com/whitepapers/latest/aws-overview/types-of-cloud-computing.html
    

# Cloud Computing Models

### IAAS (Infastructure as a service)

Choose the hardware, operating system, network (e.g. VPC, EC2, EBS)

### PAAS (Platform as a service)

Manage application.
(e.g. RDS, EMR, ElasticSearch, Elastic Beanstalk)

### FAAS (Function as a service /  Abstract services)

Provides server functionality without having to manage server.
Examples: Lambda, S3, DynamoDB, SNS

### SAAS (Software as a service)

A complete application for end users (e.g. gmail, salesforce.com, creative cloud).

# AWS Global Infrastructure

### Geographic Regions (24)

A physical location around the world where we cluster data centers.

Example: AWS GovCloud (US-West, Secret)

Each AWS Region consists of multiple (2 or more), isolated, and physically separate AZ's within a geographic area. 

Choose based on needs. Consider latency, costs, regulations, and services.

Largest region is/ was US-East N. Virginia (seven AZs)

### Availability Zones (76)

An Availability Zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity in an AWS Region.

AZ’s give customers the ability to operate production applications and databases that are more highly available, fault tolerant, and scalable than would be possible from a single data center.

All AZ’s in an AWS Region are interconnected with high-bandwidth, low-latency networking, over fully redundant, dedicated metro fiber providing high-throughput, low-latency networking between AZ’s.

If an application is partitioned across AZ’s, companies are better isolated and protected from issues such as power outages, lightning strikes, tornadoes, earthquakes, and more. AZ’s are physically separated by a meaningful distance, many kilometers, from any other AZ, although all are within 100 km (60 miles) of each other

### Edge Locations (205)

Caches content for high speed delivery to users
Provides DDOS protection

### Local Zones (1)

AWS Local Zones are a new type of AWS infrastructure deployment that places AWS compute, storage, database, and other select services closer to large population, industry, and IT centers where no AWS Region exists today. With AWS Local Zones, you can easily run latency-sensitive portions of applications local to end-users and resources in a specific geography, delivering single-digit millisecond latency for use cases such as media & entertainment content creation, real-time gaming, reservoir simulations, electronic design automation, and machine learning.

Each AWS Local Zone location is an extension of an AWS Region where you can run your latency-sensitive applications in geographic proximity to end-users. AWS Local Zones provide a high-bandwidth, secure connection between local workloads and those running in the AWS Region, allowing you to seamlessly connect back to your other workloads running in AWS and to the full range of in-region services through the same APIs and tool sets.

AWS Local Zones are managed and supported by AWS.

The Los Angeles AWS Local Zone is generally available and you can expect more Local Zones to come.

https://aws.amazon.com/about-aws/global-infrastructure/

# AWS Well-Architected Framework


__"The Well-Architected Framework has been developed to help cloud architects build secure, high-performing, resilient, and efficient infrastructure for their applications. Based on five pillars, the Framework provides a consistent approach for customers and partners to evaluate architectures, and implement designs that will scale over time." - AWS__


## The pillars of the AWS Well-Architected Framework

### Operational Excellence

The ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures.

### Security

The ability to protect information, systems, and assets while delivering business value through risk assessments and mitigation strategies.

### Reliability

The ability of a system to recover from infrastructure or service disruptions, dynamically acquire computing resources to meet demand, and mitigate disruptions such as misconfigurations or transient network issues.

### Performance Efficiency

The ability to use computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve.

### Cost Optimization

The ability to run systems to deliver business value at the lowest price point.

https://aws.amazon.com/architecture/well-architected/


# AWS Cloud Adoption Framework

__"AWS Professional Services created the AWS Cloud Adoption Framework (AWS CAF) to help organizations design and travel an accelerated path to successful cloud adoption. The guidance and best practices provided by the framework help you build a comprehensive approach to cloud computing across your organization, and throughout your IT lifecycle. Using the AWS CAF helps you realize measurable business benefits from cloud adoption faster and with less risk." - AWS__

## The Six AWS CAF Perspectives

### Business Perspective

Common roles: Business Managers, Finance
Managers, Budget Owners, and Strategy Stakeholders.
Helps stakeholders understand how to update the staff skills and
organizational processes they will need to optimize business value as
they move their operations to the cloud.

### People Perspective

Common roles: Human Resources, Staffing, and
People Managers.
Provides guidance for stakeholders responsible for people development,
training, and communications. Helps stakeholders understand how to 
Amazon Web Services – An Overview of the AWS Cloud Adoption Framework
Page 3
update the staff skills and organizational processes they will use to
optimize and maintain their workforce, and ensure competencies are in
place at the appropriate time.

### Governance Perspective

Common roles: CIO, Program Managers,
Project Managers, Enterprise Architects, Business Analysts, and
Portfolio Managers.
Provides guidance for stakeholders responsible for supporting business
processes with technology. Helps stakeholders understand how to
update the staff skills and organizational processes that are necessary to
ensure business governance in the cloud, and manage and measure
cloud investments to evaluate their business outcomes.

### Platform Perspective

Common roles: CTO, IT Managers, and
Solution Architects.
Helps stakeholders understand how to update the staff skills and
organizational processes that are necessary to deliver and optimize cloud
solutions and services.

### Security Perspective

Common roles: CISO, IT Security Managers,
and IT Security Analysts.
Helps stakeholders understand how to update the staff skills and
organizational processes that are necessary to ensure that the
architecture deployed in the cloud aligns to the organization’s security
control requirements, resiliency, and compliance requirements.

### Operations Perspective

Common roles: IT Operations Managers
and IT Support Managers.
Helps stakeholders understand how to update the staff skills and
organizational processes that are necessary to ensure system health and
reliability during the move of operations to the cloud and then to operate
using agile, ongoing, cloud computing best practices.

