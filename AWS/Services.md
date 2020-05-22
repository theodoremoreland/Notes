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
        Simple Storage Service (S3) - FAAS
            // S3 Is not a global service.
            // S3 standard
            // S3 - IA
            // S3 One Zone - IA
            // Intelligent Tiering
            // S3 Glacier and S3 Glacier Deep Archive
            Object-based storage / file based
            Objects consist of a key / name and value / data
            Can apply policies to buckets / folders and objects / files
            Can limit access via IAM policies and 
            Tiered storage
            Lifecycle management
            Versioning
            Encrypting
            Bucket policies
            Built for 99.99% but promises only 99% availability and (11X9s durability)
            Read after write consistency for puts of new objects, not applicable when trying to read changes to existing files (i.e. delete or update)
            Eventual consistency = 
            Version id
            Metadata
            Access control list
            Torrent
            Spread across multiple facilities
            File can be 0 bytes to 5tb
            Unlimited storage
            Universal namespace
            Url always starts with s3 and ends with amazonaws.com (sort of)
            HTTP 200 if successful upload



        Glacier - FAAS
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