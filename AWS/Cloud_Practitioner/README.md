"Cloud computing is the on-demand delivery of compute power, database storage, applications, and other IT resources through a cloud services platform via the Internet with pay-as-you-go pricing." - AWS

## Sections
- [Six Advantages of Cloud Computing](#Six-Advantages-of-Cloud-Computing)
- [Types of Cloud Computing / Computing Deployment](#Types-of-Cloud-Computing)
- [Cloud Computing Models](#Cloud-Computing-Service-Models)
- [AWS Global Infrastructure](#AWS-Global-Infrastructure)

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
