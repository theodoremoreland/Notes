## Sections
- [Pricing Principles](#Pricing-Principles)
- [Pricing Tools](#Pricing-Tools)
- [Cost Management](#Cost-Management)
- [Support Plans](#Support-Plans)
- [Definitions](#Definitions)


## Links

https://aws.amazon.com/pricing/

https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/billing-what-is.html

https://aws.amazon.com/organizations/

https://aws.amazon.com/premiumsupport/plans/

https://aws.amazon.com/premiumsupport/plans/enterprise/



# Pricing Principles

### Pay-as-you-go

"Pay-as-you-go allows you to easily adapt to changing business needs without overcommitting budgets and improving your responsiveness to changes." - AWS

### Save when you reserve

"For certain services like Amazon EC2 and Amazon RDS, you can invest in reserved capacity.  With Reserved Instances, you can save up to 75% over equivalent on-demand capacity.  When you buy Reserved Instances, the larger the upfront payment, the greater the discount." - AWS

### Pay less by using more

"With AWS, you can get volume based discounts and realize important savings as your usage increases.  For services such as S3, pricing is tiered, meaning the more you use, the less you pay per GB." - AWS

# Pricing Tools

### Simple Monthly Calculator (Deprecated - ETD June 30, 2020)

Being replaced by AWS Pricing Calculator @ https://calculator.aws/#/
(Trivia) [Was] hosted on an S3 bucket @ https://calculator.s3.amazonaws.com/index.html

### AWS Pricing Calculator

Can be used to estimate the monthly / yearly cost of specific configuartions for 1+ AWS services
Located @ https://calculator.aws/#/

### AWS Total Cost of Ownership (TCO) Calculator

Allows you to compare your on premises or colocation solution to AWS's cloud solution
Generate savings reports (for download)

Breaks down cost into four dimensions:
1. Storage
2. IT Labor
3. Servers
4. Networking

Breaks down how totals were calculated
Makes assumptions about the technology and personnel
Assumptions can be customized to user's specifications.
Located @ https://aws.amazon.com/tco-calculator/


# Cost Management


## Tagging

"Amazon Web Services allows customers to assign metadata to their AWS resources in the form
of tags. Each tag is a simple label consisting of a customer-defined key and an optional value
that can make it easier to manage, search for, and filter resources. Although there are no
inherent types of tags, they enable customers to categorize resources by purpose, owner,
environment, or other criteria." - AWS

**Going to Resource Groups > Tag Editor in the AWS Console (in the upper left of screen) allows you to view all resources attached to the AWS account. This can be used to find potentially hidden resources that incurr cost or used to find resources of a certain type and/or tag.**

## Billing

    Cost Explorer

        Analyze cost AFTER they have been incurred.

        Analyze your cost and usage data.

        Monthly Costs by AWS Service.

        Hourly and Resource Level Granularity.

        Savings Plans

    Budgets

        Budget or predict service cost BEFORE they are incurred.

        Can notify users when cost reach/are predicted to reach a budget.

        Can specify the percentage of usage or cost for a given budget to recieve alerts. 

        Each budget can have up to 5 associated alerts.
        
        Each alert can have up to 10 subscribers & be publish to SNS.

### CloudWatch

Monitors performance (of mainly EC2 instances)
Billing Alerts can disperse a notification (e.g. email) once your AWS cost reach a certain point, but as of
(6/8/2020) Billing Alerts must be enabled via the Billing Dashboard's "Billing Preferences". Billing Alarms
for spending on the entire account are not enabled by default, despite being able to "create" them on the
CloudWatch console.

## AWS Organizations

"Enables you to centrally apply policy-based controls across multiple accounts in the AWS Cloud.
You can consolidate all your AWS accounts into an organization, and arrange all AWS accounts into distinct organizational units." - AWS

Root account / AWS Organization's host can control resources across entire organization UNLESS the created "with only consolidated billing features"

Tentative cap of 20 linked accounts


# Support Plans

All support plans include:
* 24x7 access to customer service, documentation, whitepapers, and support forums.
* AWS Trusted Advisor
* AWS Personal Health Dashboard

### Basic

* Free


### Developer

* **$29 / month** *(or 3% of monthly AWS usage)*

* <ins>Enhanced Technical Support:</ins>

    Cloud Support Associate

    Business hours (E-MAIL ONLY)

    ONE person can open UNLIMITED cases

    Case Severity / Response Times:

        General Guidance:
         < 24 business hrs

        System impaired:
         < 12 business hrs


### Business


* **$100 / month** *(or 10%-3% of monthly AWS usage based on bill)*

* Full set of Trusted Advisor checks

* AWS Support API

* <ins>Enhanced Technical Support:</ins>

    Cloud Support Engineer

    24/7 (via e-mail, chat, and phone)

    UNLIMITED people can open UNLIMITED cases (IAM supported)

    Case Severity / Response Times:

        General guidance:
         < 24 hrs

        System impaired:
         < 12 hrs

        Production system impaired:
        < 4 hours

        Production system down:
        < 1 hr


### Enterprise


* **$15,000 / month** *(or 10%-3% of monthly AWS usage based on bill)*

* Full set of Trusted Advisor checks

* AWS Support API

* Access to online self-paced labs

* **Technical Account Manager (TAM)** 

* **Concierge Support Team**

* <ins>Enhanced Technical Support:</ins>

    Cloud Support Engineer

    24/7 (via e-mail, chat, and phone)

    UNLIMITED people can open UNLIMITED cases (IAM supported)

    Case Severity / Response Times:

        General guidance:
         < 24 hrs

        System impaired:
         < 12 hrs

        Production system impaired:
        < 4 hours

        Production system down:
        < 1 hr

        Business critical system down:
        < 15 minutes



https://aws.amazon.com/premiumsupport/plans/
https://aws.amazon.com/premiumsupport/plans/enterprise/



## Definitions

### Technical Account Manager (TAM)

"Your designated technical point of contact who provides advocacy and guidance to help plan and build solutions using best practices, coordinate access to subject matter experts and product teams, and proactively keep your AWS environment operationally healthy." - AWS

### Concierge Support Team

"AWS billing and account experts that specialize in working with enterprise accounts. They will quickly and efficiently assist you with your billing and account inquiries, and work with you to implement billing and account best practices so that you can focus on what matters: running your business." - AWS