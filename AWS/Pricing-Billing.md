--- Look into Capex vs Opex / Variable Expense ---

Support plans
    Basic
        Free
        Support forums

    Developer
        $29 /month
        Tech support during business hours (email only)
        One person can open UNLIMITED cases
        General Guidance = less than 24 business hours
        System impaired = less than 12 business hours


    Business
        $100 / month
        24/7 Tech support (via email, chat, and phone)
        Unlimited people can open unlimited cases
        General guidance = less than 24 [all] hours
        System impaired = less than 12 [all] hours
        Production system impaired = less than 4 [all] hours
        Production system down = less than 1 [all] hours
        Trusted Advisor

    Enterprise
        $15,000 /month
        Unlimited people can open unlimited cases
        General guidance = less than 24 [all] hours
        System impaired = less than 12 [all] hours
        Production system impaired = less than 4 [all] hours
        Production system down = less than 1 [all] hours
        Business critical system down = less than 15 [all] minutes
        Technical Account Manager (TAM)

Pricing policies:
	Pay as you go
	Pay less when you reserve
    Pay even less per unit by using more
    Pay even less as AWS grows
    Custom pricing

Drivers of cost
    Compute
    Storage
    Data outbound

Start early with optimization lest cost spiral out of control
Maximize the power of flexibility

CloudWatch
    Monitors performance (of mainly EC2 instances)
    Billing Alerts can disperse a notification (e.g. email) once your AWS cost reach a certain point, but as of
    (6/8/2020) Billing Alerts must be enabled via the Billing Dashboard's "Billing Preferences". Billing Alarms
    for spending on the entire account are not enabled by default, despite being able to "create" them on the
    CloudWatch console.

CloudTrail
    Montitors API calls to AWS (i.e. commands to AWS services)

Cost Explorer
    Used to analyze cost AFTER they have been incurred.

Budgets
    Used to budget or predict cost BEFORE they are incurred.

    you can further specify the percent accrual toward the cost or usage threshold. For example, specifying 100%    the actual costs of a $1,000 budget will alert you when the $1,000 threshold is exceeded.

    You can also supplement these alerts by setting one against forecasted cost or usage values (e.g., 105% of your budgeted value), which will alert you of possible anomalies or changes in behavior.

    Each budget can have up to 5 associated alerts. Each alert can have up to 10 email subscribers and can optionally be published to an SNS topic

Simple Monthly Calculator (Deprecated - ETA June 30, 2020)
    Being replaced by AWS Pricing Calculator @ https://calculator.aws/#/
    (Trivia) [Was] hosted on an S3 bucket @ https://calculator.s3.amazonaws.com/index.html

AWS Pricing Calculator
    Can be used to estimate the monthly / yearly cost of specific configuartions for 1+ AWS services
    Located @ https://calculator.aws/#/

AWS Total Cost of Ownership (TCO) Calculator 
    Allows you to compare your on premises or colocation solution to AWS's cloud solution
    Generate savings reports (for download)
    Breaks down cost into four dimensions: Storage, IT Labor, Servers, Networking
    Breaks down how totals were calculated
    Makes assumptions about the technology and personnel
    Assumptions can be customized to user's specifications.
    Located @ https://aws.amazon.com/tco-calculator/


AWS Organizations
    Used to be a cap of 20 linked accounts
    
What determines price?
	Clock hours
    Instance type
    Pricing model
    Numbers of instances
    Load balancing
    Detailed monitoring
    Auto scaling
    Elastic IP Addresses
    Operating Systems and Software …..
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