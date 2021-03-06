Cloud computing is the on-demand delivery of compute power, database storage, applications, and other IT resources through a cloud services platform via the Internet with pay-as-you-go pricing.

Six Advantages of Cloud Computing
    Trade capital expense for variable expense
        Instead of having to invest heavily in data centers and servers before you know how you’re going to use them, you can pay only when you consume computing resources, and pay only for how much you consume.

    Benefit from massive economies of scale
        By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers is aggregated in the cloud, providers such as AWS can achieve higher economies of scale, which translates into lower pay as-you-go prices.

    Stop guessing capacity
        Eliminate guessing on your infrastructure capacity needs. When you make a capacity decision prior to deploying an application, you often end up either sitting on expensive idle resources or dealing with limited capacity. With cloud computing, these problems go away. You can access as much or as little capacity as you need, and scale up and down as required with only a few minutes’ notice.

    Increase speed and agility
        In a cloud computing environment, new IT resources are only a click away, which means that you reduce the time to make those resources available to your developers from weeks to just minutes. This results in a dramatic increase in agility for the organization, since the cost and time it takes to experiment and develop is significantly lower.

    Stop spending money running and maintaining data centers
        Focus on projects that differentiate your business, not the infrastructure. Cloud computing lets you focus on your own customers, rather than on the heavy lifting of racking, stacking, and powering servers.

    Go global in minutes
        Easily deploy your application in multiple regions around the world with just a few clicks. This means you can provide lower latency and a better experience for your customers at minimal cost.

Types of Cloud Computing / Computing Deployment:
    (Cloud computing is processing over the internet where the exact location of the servers is unknown).
    https://docs.aws.amazon.com/whitepapers/latest/aws-overview/types-of-cloud-computing.html

    Public
        AWS, Azure, GCP
    Hybrid

    Private (On premise)
        You manage in personal data center
    

Cloud Computing Model(s)
    IAAS (Infastructure as a service)
        Choose the hardware, operating system, network (e.g. VPC, Ec2, EBS)

    PAAS (Platform as a service)
        Manage application
        (e.g. RDS, EMR, ElasticSearch)

    FAAS (Function as a service /  Abstract services)
        Provides server functionality without having to manage server
        Examples: Lambda, S3, DynamoDB, SNS

    SAAS (Software as a service)
        A complete application for end users (e.g. gmail, salesforce.com, creative cloud)


Geographic Regions ?+
    Example: AWS GovCloud (US-West, Secret)
    Choose based on needs. Consider latency, costs, regulations, and services.
    Broken up into at least two Availability Zones
    Largest region is/ was US-East N. Virginia (seven AZs)

Availability Zones ?+
    Example: TBD
    Physically isolated server locations
    Connected via high speed fiber optics
    If one location fails, AWS will connect to another (Fault tolerance)

Edge Locations 100+
    100+ locations
    Caches content for high speed delivery to users
    Provides DDOS protection


The pillars of the AWS Well-Architected Framework
    Operational Excellence
        The ability to run and monitor systems to deliver business value and to continually improve supporting processes and procedures.

    Security
        The ability to protect information, systems, and assets while delivering business value through risk assessments and mitigation strategies.

    Reliability
        The ability of a system to recover from infrastructure or service disruptions, dynamically acquire computing resources to meet demand, and mitigate disruptions such as misconfigurations or transient network issues.

    Performance Efficiency
        The ability to use computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve.

    Cost Optimization
        The ability to run systems to deliver business value at the lowest price point.


Each AWS CAF Perspective is made up of a set of CAF Capabilities, which is a
composite of responsibilities typically owned or managed by one or more
functionally related stakeholders. Each Capability describes “what” a
stakeholder owns or manages in the cloud adoption journey. The Capabilities
are a standard used within the CAF. Each Capability consists of a set of CAF
Skills and Processes that provide structure to identify gaps in your existing skills
and processes. For example, the People Perspective provides guidance for
stakeholders who own or manage human resources (HR), staffing functions,
and people management responsibilities. The guidance in this Perspective
focuses on people development, training, and communications to assess how
stakeholder-owned or -managed capabilities will transform with cloud
adoption.
In general, the Business, People, and Governance Perspectives focus on
business capabilities, and the Platform, Security, and Operations Perspectives
focus on technical capabilities. A brief description of each AWS CAF Perspective
is provided here, with more detailed descriptions later in this whitepaper.
 Business Perspective – Common roles: Business Managers, Finance
Managers, Budget Owners, and Strategy Stakeholders.
Helps stakeholders understand how to update the staff skills and
organizational processes they will need to optimize business value as
they move their operations to the cloud.
 People Perspective – Common roles: Human Resources, Staffing, and
People Managers.
Provides guidance for stakeholders responsible for people development,
training, and communications. Helps stakeholders understand how to 
Amazon Web Services – An Overview of the AWS Cloud Adoption Framework
Page 3
update the staff skills and organizational processes they will use to
optimize and maintain their workforce, and ensure competencies are in
place at the appropriate time.
 Governance Perspective – Common roles: CIO, Program Managers,
Project Managers, Enterprise Architects, Business Analysts, and
Portfolio Managers.
Provides guidance for stakeholders responsible for supporting business
processes with technology. Helps stakeholders understand how to
update the staff skills and organizational processes that are necessary to
ensure business governance in the cloud, and manage and measure
cloud investments to evaluate their business outcomes.
 Platform Perspective – Common roles: CTO, IT Managers, and
Solution Architects.
Helps stakeholders understand how to update the staff skills and
organizational processes that are necessary to deliver and optimize cloud
solutions and services.
 Security Perspective – Common roles: CISO, IT Security Managers,
and IT Security Analysts.
Helps stakeholders understand how to update the staff skills and
organizational processes that are necessary to ensure that the
architecture deployed in the cloud aligns to the organization’s security
control requirements, resiliency, and compliance requirements.
 Operations Perspective – Common roles: IT Operations Managers
and IT Support Managers.
Helps stakeholders understand how to update the staff skills and
organizational processes that are necessary to ensure system health and
reliability during the move of operations to the cloud and then to operate
using agile, ongoing, cloud computing best practices.

