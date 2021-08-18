# AWS Organizations
- Your company has multiple AWS accounts. You can use [**AWS Organizations**](https://aws.amazon.com/organizations) to consolidate and manage multiple AWS accounts within a central location.
- When you create an organization, AWS Organizations automatically creates a **root**, which is the parent container for all the accounts in your organization.
- In AWS Organizations, you can centrally control permissions for the accounts in your organization by using [**service control policies (SCPs)**](https://docs.aws.amazon.com/organizations/latest/userguide/orgs_manage_policies_scps.html).
-  SCPs enable you to place restrictions on the AWS services, resources, and individual API actions that users and roles in each account can access.
- In AWS Organizations, you can apply **service control policies (SCPs) to the organization root, an individual member account, or an OU**. An SCP affects all IAM users, groups, and roles within an account, including the AWS account root user.
## Organization Units
- In AWS Organizations, you can group accounts into organizational units (OUs) to make it easier to manage accounts with similar business or security requirements.
- When you apply a policy to an OU, all the accounts in the OU automatically inherit the permissions specified in the policy.
- By organizing separate accounts into OUs, you can more easily isolate workloads or applications that have specific security requirements.
- If your company has accounts that can access only the AWS services that meet certain regulatory requirements, you can put these accounts into one OU. Then, you can attach a policy to the OU that blocks access to all other AWS services that do not meet the regulatory requirements.