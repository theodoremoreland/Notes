Global services to remember
    IAM 
    Route 53
    SNS
    SES
    CloudFront

On premise services:
    Snowball
    Snowball edge
    Storage gateway
    Codedeploy
    opsworks 


Services
    Storage (Tentative)

        Elastic Block Storage (EBS) - ???
            A block of storage for AWS server
            SSD (general purpose SSD, provisioned iops SSD)
	        magnetic  (throughput optimized HDD, Cold HDD, magnetic)

        Elastic File System (EFS) - ???
                Network mounting file storage (EFS share and EFS mount targets)
        Storage Gateway - ???
        Snowball
            Physical device for uploading HUGE amounts of data (up to petabytes)

    Database
        RDS (MairaDB, Aurora, MySQL, PostgreSQL, Microsoft SQL Server, Oracle)
        DynamoDB
            Serveless
            NoSQL
            High speed, Low latency
        RedShift
            Petabyte scale data warehouse
            Based on PostgreSQL engine
        ElasticCache
            In memory access as opposed to on disk
            Can put a node in front of RDS instance to cache frequently accessed data
        Database Migration Services (DMS)
        Neptune
            Graph database
            Billions of relationships
            ms latency for graph queries

    Compute
        EC2
            Different price rates: 
                on demand
                reserved (contract terms) - upfront payments for predictable loads
                Standardized instances
                Convertible instances
                Scheduled reserved instances
                Spot (bid a price, price moves around) - for flexible starts and ends times, only feasible at very low compute prices
                Useful for users with urgent needs for large amounts of additional capacity
                Dedicated hosts (physical servers dedicated to your use (for legal reasons)) - great for licensing. Can be paid upfront for 70% of the on demand price.

        Lightsail
        Lambda
        Batch
        Elastic Beanstalk
        Serverless Application Repository
        AWS Outposts
        EC2 Image Builder

    Networking & Content Delivery 
        VPC
        CloudFront
        Route 53
        API Gateway - FAAS
        Direct Connect
        AWS App Mesh
        AWS Cloud Map
        Global Accelerator

    Management & Governance 
        AWS Organizations
        CloudWatch
            Billing Alerts
        AWS Auto Scaling
        CloudFormation
        CloudTrail
        Config
        OpsWorks
        Service Catalog
        Systems Manager
        AWS AppConfig
        Trusted Advisor
        Control Tower
        AWS License Manager
        AWS Well-Architected Tool
        Personal Health Dashboard
        AWS Chatbot
        Launch Wizard
        AWS Compute Optimizer

    Application Integration
        Step Functions
        Amazon AppFlow
        Amazon EventBridge
        Amazon MQ
        Simple Notification Service
        Simple Queue Service
        SWF

    Customer Engagement
        Amazon Connect
        Pinpoint
        Simple Email Service

    Analytics
        Athena
            AWS Athena is an interactive query service which enables you to analyze and query data located in S3 using standard SQL.
            Serverless, pay per query / per TB scanned
            No complex ETL
            Works directly with data in S3

        EMR
        CloudSearch
        Elasticsearch Service
        Kinesis
        QuickSight
        Data Pipeline
        AWS Data Exchange
        AWS Glue
        AWS Lake Formation
        MSK

    Security, Identity, & Compliance 
        IAM
        Resource Access Manager
        Cognito
        Secrets Manager
        GuardDuty
        Inspector
        Amazon Macie
            (for PII - personally identifiable information)
            Use machine learning and NLP to discover, classify, and protect sensitive data stored in S3
            Dashboards (report / analytics)

        AWS Single Sign-On
        Certificate Manager
        Key Management Service
        CloudHSM
        Directory Service
        WAF & Shield
        AWS Firewall Manager
        Artifact
        Security Hub
        Detective
    
    Developer Tools 
        CodeStar
        CodeCommit
        CodeBuild
        CodeDeploy
        CodePipeline
        Cloud9
            Web browser based IDE for Ec2.
            Update code in real time (like saving to local machine via local IDE)
            Drag and drop files
            Share IDE for pair programming
            AWS CLI and 40+ programming languages pre-installed.
        X-Ray

    End User Computing 
        WorkSpaces
        AppStream 2.0
        WorkDocs
        WorkLink

    Internet of Things 
        IoT Core
        FreeRTOS
        IoT 1-Click
        IoT Analytics
        IoT Device Defender
        IoT Device Management
        IoT Events
        IoT Greengrass
        IoT SiteWise
        IoT Things Graph

    Game Development
        Amazon GameLift


Always free (Free tier)
    Amazon DynamoDB
        25 GB
        of storage
    AWS Lambda
        1 Million
        free requests per month
    Amazon SNS
        1 Million
        publishes
    Amazon CloudWatch
        10
        custom metrics and alarms
    Amazon Chime
        Basic
        unlimited use
    Amazon Cognito
        50,000
        MAUs each month
        Mobile user identity and synchronization.
    Amazon Glacier (Glacier API only)
        10 GB
        of storage retrievals
    Amazon Macie
        1 GB
        processed by the content classification engine
    Amazon SES
        62,000
        outbound messages per month
    Amazon SQS
        1 Million
        requests
    Amazon SWF
        10,000
        activity tasks
    AWS CodeBuild
        100 build minutes
    AWS CodeCommit
        5
        active users per month
    AWS CodePipeline
        1
        active pipeline per month
    AWS Database Migration Service
        750 Hours
        of Amazon DMS Single-AZ dms.t2.micro instance usage
    AWS Glue
        1 Million objects stored in the AWS Glue Data Catalog
    AWS Key Management Service
        20,000 free requests per month
    AWS License Manager
        Unlimited
    Storage Gateway
        First 100 GB per account is free
    Step Functions
        4,000 state transitions per month
    X-Ray
        100,000 traces recorded per month
    AWS Well-Architected Tool
        Unlimited
    https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc


Figure out what determines the price for Lambda--
Figure out what determines the price for EBS--
	Volumes
	Snapshots
	Data transfer
Figure of what determines the price for S3--
	Storage class
	Storage
	Requests
	Data transfer
Figure out what determines the price for Glacier
	Storage
	Data retrieval time

What is Snowball?
	A PB scale data transfer system… figure it out

    What determines the price for Snowball?
        Service fee per job
        Daily charge
        Data transfer
        Price RDS
        Clock hours
        Characteristic
        Purchase types
        Number of instances
        Provisional storage
        Additional storage
        Requests
        Deployment type
        Data transfer

Dynamo
    Write
    Read
    Amount of data stored
    
Cloudfront
    Number of requests
    Traffic distribution
    Data transfer out