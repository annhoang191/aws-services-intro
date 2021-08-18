# Amazon CloudTrail
- [**AWS CloudTrail**](https://aws.amazon.com/cloudtrail/) records API calls for your account. 
- The recorded information includes the identity of the API caller, the time of the API call, the source IP address of the API caller, and more.
- With CloudTrail, you can view a complete history of user activity and API calls for your applications and resources.
- Events are typically updated in CloudTrail within 15 minutes after an API call. You can filter events by specifying the time and date that an API call occurred, the user who requested the action, the type of resource that was involved in the API call, and more.

#### Example
The coffee shop owner is browsing through the AWS Identity and Access Management (IAM) section of the AWS Management Console. They discover that a new IAM user named Mary was created, but they do not who, when, or which method created the user.
=> In the CloudTrail Event History section, the owner applies a filter to display only the events for the “CreateUser” API action in IAM. The owner locates the event for the API call that created an IAM user for Mary. This event record provides complete details about what occurred:  _On January 1, 2020 at 9:00 AM, IAM user John created a new IAM user (Mary) through the AWS Management Console._

## CloudTrail Insight
- Within CloudTrail, you can also enable [**CloudTrail Insights**](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/logging-insights-events-with-cloudtrail.html). This optional feature allows CloudTrail to automatically detect unusual API activities in your AWS account.
- CloudTrail Insights might detect that a higher number of Amazon EC2 instances than usual have recently launched in your account. You can then review the full event details to determine which actions you need to take next.
