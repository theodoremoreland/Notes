Support Plans (all get billing support)
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
        Trusted Advisor?

    Enterprise
        $15,000 /month
        Unlimited people can open unlimited cases
        General guidance = less than 24 [all] hours
        System impaired = less than 12 [all] hours
        Production system impaired = less than 4 [all] hours
        Production system down = less than 1 [all] hours
        Business critical system down = less than 15 [all] minutes
        Technical Account Manager (TAM)
        Concierge?


Pricing Tools
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


Cost Management
    AWS Organizations
        Used to be a cap of 20 linked accounts

    CloudWatch
        Monitors performance (of mainly EC2 instances)
        Billing Alerts can disperse a notification (e.g. email) once your AWS cost reach a certain point, but as of
        (6/8/2020) Billing Alerts must be enabled via the Billing Dashboard's "Billing Preferences". Billing Alarms
        for spending on the entire account are not enabled by default, despite being able to "create" them on the
        CloudWatch console.

    CloudTrail
        Montitors API calls to AWS (i.e. commands to AWS services)

    Billing
        Cost Explorer
            Used to analyze cost AFTER they have been incurred.

        Budgets
            Used to budget or predict cost BEFORE they are incurred.

            you can further specify the percent accrual toward the cost or usage threshold. For example, specifying 100%    the actual costs of a $1,000 budget will alert you when the $1,000 threshold is exceeded.

            You can also supplement these alerts by setting one against forecasted cost or usage values (e.g., 105% of your budgeted value), which will alert you of possible anomalies or changes in behavior.

            Each budget can have up to 5 associated alerts. Each alert can have up to 10 email subscribers and can optionally be published to an SNS topic


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

What determines price?
	Clock hours
    Instance type
    Pricing model
    Numbers of instances
    Load balancing
    Detailed monitoring
    Auto scaling
    Elastic IP Addresses
    Operating Systems and Software