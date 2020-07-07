"AWS CloudFormation allows you to use programming languages or a simple text file to model and provision, in an automated and secure manner, all the resources needed for your applications across all regions and accounts. This gives you a single source of truth for your AWS and third party resources."

## Links
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-anatomy.html

https://aws.amazon.com/serverless/sam/


# Template
* Define resources
* Code your infastructure in either JSON or YAML

## Template format

### Format Version (optional)
The AWS CloudFormation template version that the template conforms to. The template format version is not the same as the API or WSDL version. The template format version can change independently of the API and WSDL versions.

### Description (optional)
A text string that describes the template. This section must always follow the template format version section.

### Metadata (optional)
Objects that provide additional information about the template.

### Parameters (optional)
Values to pass to your template at runtime (when you create or update a stack). You can refer to parameters from the Resources and Outputs sections of the template.

### Mappings (optional)
A mapping of keys and associated values that you can use to specify conditional parameter values, similar to a lookup table. You can match a key to a corresponding value by using the Fn::FindInMap intrinsic function in the Resources and Outputs sections.

### Conditions (optional)
Conditions that control whether certain resources are created or whether certain resource properties are assigned a value during stack creation or update. For example, you could conditionally create a resource that depends on whether the stack is for a production or test environment.

### Transform (optional)
For serverless applications (also referred to as Lambda-based applications), specifies the version of the AWS Serverless Application Model (AWS SAM) to use. When you specify a transform, you can use AWS SAM syntax to declare resources in your template. The model defines the syntax that you can use and how it is processed.

You can also use AWS::Include transforms to work with template snippets that are stored separately from the main AWS CloudFormation template. You can store your snippet files in an Amazon S3 bucket and then reuse the functions across multiple templates.

### Resources (required)
Specifies the stack resources and their properties, such as an Amazon Elastic Compute Cloud instance or an Amazon Simple Storage Service bucket. You can refer to resources in the Resources and Outputs sections of the template.

### Outputs (optional)
Describes the values that are returned whenever you view your stack's properties. For example, you can declare an output for an S3 bucket name and then call the aws cloudformation describe-stacks AWS CLI command to view the name.

### Others
* Instrinsic functions
* Pseudo parameters
* Custom resources
* Conditional expressions

# Stack
* Created from template
* Create multiple stacks across multiple regions from the same template
* Monitor stack updates: in progress, complete, failed (entire stack will roll back)