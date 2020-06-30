# Users
A user profile within an AWS account / root account.

* Have no permissions when first created
* Are assined Secret Access Key and Access Key ID when first created.
* You can only view the Access Keys once, if lost new ones must be created.
* You can create password rotation policies.
* You can create password policies "A password policy is a set of rules that define the type of password an IAM user can set." (e.g. Minimum password length is 6 characters)
* *IAM integrates with existing active directory account allowing single sign-on.*

### Power Users
Access to all AWS services except the management of groups and users within IAM.

### Adminastrator access
= root

### Access Advisor
Access Advisor shows the services that this user can access and when those services were last accessed.

# Roles

A way to assign permissions to AWS Resources, AWS accounts, and other???

# Groups

A collection of users. Each user inherits the permissions of the group.

# Policies

A collection of policy documents.

# Policy Documents

JSON that assigns permissions to a policy.

# Account Alias