"Cloud computing is the on-demand delivery of compute power, database storage, applications, and other IT resources through a cloud services platform via the Internet with pay-as-you-go pricing." - AWS

## Sections
- [Six Advantages of Cloud Computing](#Six-Advantages-of-Cloud-Computing)
- [Types of Cloud Computing / Computing Deployment](#Types-of-Cloud-Computing)
- [Cloud Computing Models](#Cloud-Computing-Service-Models)
- [AWS Global Infrastructure](#AWS-Global-Infrastructure)
- [AWS Well-Architected Framework](#AWS-Well-Architected-Framewor)
- [AWS Cloud Adoption Framework](#AWS-Cloud-Adoption-Framework)

## Links

https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html

https://aws.amazon.com/types-of-cloud-computing/

https://docs.aws.amazon.com/whitepapers/latest/aws-overview/types-of-cloud-computing.html

https://aws.amazon.com/about-aws/global-infrastructure/

https://aws.amazon.com/architecture/well-architected/

https://aws.amazon.com/professional-services/CAF/


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

https://docs.aws.amazon.com/whitepapers/latest/aws-overview/six-advantages-of-cloud-computing.html

# Types of Cloud Computing

### Public

AWS (Amazon Web Services), Azure, GCP (Google Cloud Platform), IBM Bluemix, Alibaba Cloud, etc.

### Hybrid

A combination of Public and Private.

### Private (On premise)
You manage in personal data center.

https://docs.aws.amazon.com/whitepapers/latest/aws-overview/types-of-cloud-computing.html
    

# Cloud Computing Service Models

### IAAS (Infastructure as a service)

Choose / provision the hardware, operating system, network (e.g. VPC, EC2, EBS)

### PAAS (Platform as a service)

A platform for allowing end user to develop, run, and manage applications without the complexity of building and maintaining the infrastructure (e.g. servers).

(e.g. RDS, EMR, ElasticSearch, Elastic Beanstalk)


### SAAS (Software as a service)

A complete application for end users.


### Others

* FAAS (Function as a service /  Abstract services)

Examples: Lambda

* CaaS (Container as a Service)

Examples: ECS

* DaaS (Desktop-as-a-Service)

Examples: Workspaces

* DBaaS (Database-as-a-Service)

Examples: RDS, Dynamo, Aurora, ElastiCache, DocumentDB, Neptune, Timestream, QLDB

* mBaaS (Mobile-Backend-as-a-Service)

Example: Amplify

etc...

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

A site that CloudFront uses to cache copies of your content for faster delivery to users at any location.

Provides DDOS protection ???

### Local Zones (1)

AWS Local Zones are a new type of AWS infrastructure deployment that places AWS compute, storage, database, and other select services closer to large population, industry, and IT centers where no AWS Region exists today. With AWS Local Zones, you can easily run latency-sensitive portions of applications local to end-users and resources in a specific geography, delivering single-digit millisecond latency for use cases such as media & entertainment content creation, real-time gaming, reservoir simulations, electronic design automation, and machine learning.

Each AWS Local Zone location is an extension of an AWS Region where you can run your latency-sensitive applications in geographic proximity to end-users. AWS Local Zones provide a high-bandwidth, secure connection between local workloads and those running in the AWS Region, allowing you to seamlessly connect back to your other workloads running in AWS and to the full range of in-region services through the same APIs and tool sets.

AWS Local Zones are managed and supported by AWS.

The Los Angeles AWS Local Zone is generally available and you can expect more Local Zones to come.

### AWS Wavelength

AWS Wavelength enables developers to build applications that deliver single-digit millisecond latencies to mobile devices and end-users. AWS developers can deploy their applications to Wavelength Zones, AWS infrastructure deployments that embed AWS compute and storage services within the telecommunications providers’ datacenters at the edge of the 5G networks, and seamlessly access the breadth of AWS services in the region. This enables developers to deliver applications that require single-digit millisecond latencies such as game and live video streaming, machine learning inference at the edge, and augmented and virtual reality (AR/VR). AWS Wavelength brings AWS services to the edge of the 5G network, minimizing the latency to connect to an application from a mobile device. Application traffic can reach application servers running in Wavelength Zones without leaving the mobile provider’s network. This reduces the extra network hops to the Internet that can result in latencies of more than 100 milliseconds, preventing customers from taking full advantage of the bandwidth and latency advancements of 5G.


### AWS Outposts

AWS Outposts bring native AWS services, infrastructure, and operating models to virtually any data center, co-location space, or on-premises facility. You can use the same AWS APIs, tools, and infrastructure across on-premises and the AWS cloud to deliver a truly consistent hybrid experience. AWS Outposts is designed for connected environments and can be used to support workloads that need to remain on-premises due to low latency or local data processing needs.

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

"The Business Perspective helps you move from separate strategies for business and IT to a business model that integrates IT strategy. Agile IT strategies are aligned to support your business outcomes, and they can adjust to business needs or technical capabilities as they change.

Common Roles: Business Managers; Finance Managers; Budget Owners; Strategy Stakeholders.

Capabilities:

IT Finance addresses your capacity to plan, allocate, and manage the budget for IT expenses with the use-based cost model of cloud services.

IT Strategy helps you take advantage of cloud-based IT approach to deliver value and end-user adoption.

Benefits Realization helps you to measure the benefits of your IT investments using methods for a cloud-based IT operating model.

Business Risk Management helps you estimate the potential business impact of preventable, strategic, and/or external risks." - AWS

### People Perspective

"The People Perspective helps Human Resources (HR) and personnel management prepare their teams for cloud adoption by updating staff skills and organizational processes to include cloud-based competencies.

Common Roles: Human Resources; Staffing; People Managers.

Capabilities:

Resource Management helps you understand and forecast new personnel needs for a cloud-based model.

Incentive Management helps you implement a compensation program that will attract and retain the personnel required to operate a cloud-based IT model.

Career Management helps you identify, acquire, and retain the skills needed for your cloud migration and ongoing operating model.

Training Management provides guidance on how to develop or acquire training for your employees so they can perform their roles in a cloud environment.

Organizational Change Management helps you manage the impact of business, structural, and cultural changes caused by cloud adoption." - AWS

### Governance Perspective

"The Governance Perspective integrates IT Governance and Organizational Governance. It provides guidance on identifying and implementing best practices for IT Governance, and on supporting business processes with technology.

Common Roles: CIO; Program Managers; Project Managers; Enterprise Architects; Business Analysts; Portfolio Managers.

Capabilities:

Portfolio Management provides a mechanism to manage it based on desired business outcomes. It can help to determine cloud-eligibility for workloads when prioritizing which services to move to the cloud.

Program and Project Management helps you manage technology projects using methodologies that take advantage of the agility and cost management benefits inherent to cloud services.

Business Performance Measurement helps you measure the impact of the cloud on business objectives.

License Management defines methods to procure, distribute, and manage the licenses needed for IT systems, services, and software." - AWS

### Platform Perspective

"The Platform Perspective helps you design, implement, and optimize the architecture of AWS technology based on business goals and objectives. It helps provide strategic guidance for the design, principles, tools, and policies you will use to define AWS infrastructure. The Platform perspective also includes principles and patterns for communicating your target state environment, implementing new solutions on the cloud, and migrating on-premises workloads to the cloud.
Common Roles: CTO; IT Managers; Solution Architects.

Capabilities:

Systems and Solution Architecture helps you define and describe the system design and your architectural standards.

Compute, Network, Storage, and Database Provisioning helps you develop new processes for provisioning infrastructure in a cloud environment. Provisioning shifts from an operational focus aligning supply with demand, to an architectural focus aligning services with requirements.

Application Development addresses your ability to support business goals with new or updated applications, and helps implement new skills and processes for software development that take advantage of the agility gained by cloud computing." - AWS

### Security Perspective

"The Security Perspective helps you structure the selection and implementation of controls. Following this guidance can make it easier to identify areas of non-compliance and plan ongoing security initiatives.

For more information on the AWS CAF Security Perspective, download the AWS CAF Security Perspective White Paper.
Common Roles: CISO; IT Security Managers; IT Security Analysts.

Capabilities:

Identity and Access Management (IAM) helps you integrate AWS into your identity management lifecycle, and sources of authentication and authorization.

Detective Control provides guidance to help identify potential security incidents within your AWS environment.

Infrastructure Security helps you implement control methodologies necessary to comply with best practices as well as meet industry or regulatory obligations.

Data Protection helps you to implement appropriate safeguards that protect data in transit and at rest.

Incident Response helps you define and execute a response to security incidents." - AWS

### Operations Perspective

"The Operations Perspective helps you to run, use, operate, and recover IT workloads to levels that meet the requirements of your business stakeholders. Insights gained through the Operations Perspective define your current operating procedures as well as process changes and training needed for successful cloud adoption. Well-managed IT operations support the operations of the business from planning and sustaining, through change and incident management.
Common Roles: IT Operations Managers; IT Support Managers.

Capabilities:

Service Monitoring focuses on detecting and responding to IT operations health indicators, to meet your service level agreements and operating level agreements.

Application Performance Monitoring (APM) provides you with new approaches for monitoring application performance in a cloud environment to ensure that application health meets defined requirements.

Resource Inventory Management helps you manage virtual IT assets to provide services that are both high performing and cost efficient.

Release/Change Management helps your teams adopt software development best practices such as automation and Continuous Integration/Continuous Delivery (CI/CD) techniques, increasing the pace of your innovations.

Reporting and Analytics helps you monitor the health of cloud assets and provide insights to help you reach the desired level of performance.

Business Continuity/Disaster Recovery helps you implement processes to keep your business running during a catastrophic event.

IT Service Catalog helps you to offer cloud services to the business using a model that can help to improve efficiency of providing IT services as well as the productivity of consuming them." - AWS

https://aws.amazon.com/professional-services/CAF/
