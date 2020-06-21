# Record and evaluate configurations of your AWS resources

"AWS Config is a service that enables you to assess, audit, and evaluate the configurations of your AWS resources. Config continuously monitors and records your AWS resource configurations and allows you to automate the evaluation of recorded configurations against desired configurations." - AWS

### Discovery

AWS Config will discover resources that exist in your account, record their current configuration, and capture any changes to these configurations. Config will also retain configuration details for resources that have been deleted.

### Change management

When your resources are created, updated, or deleted, AWS Config streams these configuration changes to Amazon Simple Notification Service (SNS), so that you are notified of all the configuration changes. AWS Config represents relationships between resources so that you can assess how a change to one resource may impact other resources.

### Continuous audit and compliance

AWS Config is designed to help you assess compliance with your internal policies and regulatory standards by providing you visibility into the configuration of your AWS resources as well as third-party resources, and evaluating resource configuration changes against your desired configurations on a continuous basis.

### Compliance-as-code framework

You can use AWS Config as your framework for creating and deploying governance and compliance rules across your AWS accounts and regions. You can codify your compliance requirements as AWS Config rules and author remediation actions using AWS Systems Manager Automation documents and package them together within a conformance pack that can be easily deployed across an organization.

### Troubleshooting

Using AWS Config, you can quickly troubleshoot operational issues by identifying the recent configuration changes to your resources.

### Security analysis

Data from AWS Config enables you to continuously monitor the configurations of your resources and evaluate these configurations for potential security weaknesses.

https://aws.amazon.com/config/#:~:text=AWS%20Config%20is%20a%20service,recorded%20configurations%20against%20desired%20configurations.