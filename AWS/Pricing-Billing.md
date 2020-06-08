--- Look into Capex vs Opex ---

Support plans
    Basic - Free
    Developer $29 /month
    Business $100 /month
    Enterprise $15,000 /month (TAM)

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

Budgets

    you can further specify the percent accrual toward the cost or usage threshold. For example, specifying 100%    the actual costs of a $1,000 budget will alert you when the $1,000 threshold is exceeded.

    You can also supplement these alerts by setting one against forecasted cost or usage values (e.g., 105% of your budgeted value), which will alert you of possible anomalies or changes in behavior.

    Each budget can have up to 5 associated alerts. Each alert can have up to 10 email subscribers and can optionally be published to an SNS topic

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