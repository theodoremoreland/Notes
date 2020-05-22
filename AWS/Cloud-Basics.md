Cloud computing is the on-demand delivery of compute power, database storage, applications, and other IT resources through a cloud services platform via the Internet with pay-as-you-go pricing.

Six Advantages of Cloud Computing
    Trade capital expense for variable expense – Instead of having to invest heavily in data centers and servers before you know how you’re going to use them, you can pay only when you consume computing resources, and pay only for how much you consume.

    Benefit from massive economies of scale – By using cloud computing, you can achieve a lower variable cost than you can get on your own. Because usage from hundreds of thousands of customers is aggregated in the cloud, providers such as AWS can achieve higher economies of scale, which translates into lower pay as-you-go prices.

    Stop guessing capacity – Eliminate guessing on your infrastructure capacity needs. When you make a capacity decision prior to deploying an application, you often end up either sitting on expensive idle resources or dealing with limited capacity. With cloud computing, these problems go away. You can access as much or as little capacity as you need, and scale up and down as required with only a few minutes’ notice.

    Increase speed and agility – In a cloud computing environment, new IT resources are only a click away, which means that you reduce the time to make those resources available to your developers from weeks to just minutes. This results in a dramatic increase in agility for the organization, since the cost and time it takes to experiment and develop is significantly lower.

    Stop spending money running and maintaining data centers – Focus on projects that differentiate your business, not the infrastructure. Cloud computing lets you focus on your own customers, rather than on the heavy lifting of racking, stacking, and powering servers.

    Go global in minutes – Easily deploy your application in multiple regions around the world with just a few clicks. This means you can provide lower latency and a better experience for your customers at minimal cost.

Types of computing deployment:
    (Cloud computing is processing over the internet where the exact location of the servers is unknown).
    Public - AWS, Azure, GCP
    Hybrid
    Private (On premise) - You manage in personal data center
    https://docs.aws.amazon.com/whitepapers/latest/aws-overview/types-of-cloud-computing.html


Cloud Computing Model
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


(Geographic) Regions
    Availability Zones (two or more)
        Edge Locations (CloudFront CDN)

Geographic Regions
    Example: AWS GovCloud (US-West, Secret)
    Choose based on needs. Consider latency, costs, regulations, and services.
    Broken up into at least two Availability Zones
    Largest region is/ was US-East N. Virginia (seven AZs)

Availability Zones
    Example: TBD
    Physically isolated server locations
    Connected via high speed fiber optics
    If one location fails, AWS will connect to another (Fault tolerance)

Edge Locations
    100+ locations
    Caches content for high speed delivery to users
    Provides DDOS protection


SDKs, CLI Access, and AWS API
    SDKs (Python, Node, Java, .NET, PHP, Ruby, Go, C++, iOS, Andriod, React Native, Unity, Xamarin, etc)
        SDKs use http calls


Deployment Options
    All at once
    Rolling (a batch at a time), Rolling with additional batch.
    Immutable, two environments temporarily.
    Blue - Green