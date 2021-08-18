# Additional security services

## AWS Key Management Service (AWS KMS)
- It enables you to perform encryption operations through the use of **cryptographic keys**
-  A cryptographic key **is a random string of digits** used for **locking (encrypting) and unlocking (decrypting)** data.
-  You can use AWS KMS to create, manage, and use cryptographic keys. You can also control the use of keys across a wide range of services and in your applications.
-  You can choose the specific levels of access control that you need for your keys.
-  You can specify which IAM users and roles are able to manage keys. Alternatively, you can temporarily disable keys so that they are no longer in use by anyone. Your keys never leave AWS KMS, and you are always in control of them.

## AWS WAF
- Is a web application firewall that lets you monitor network requests that come into your web applications.
- AWS WAF works together with Amazon CloudFront and an Application Load Balancer.
-  AWS WAF works in a similar way to block or allow traffic. However, it does this by using a [**web access control list (ACL)**](https://docs.aws.amazon.com/waf/latest/developerguide/web-acl.html) to protect your AWS resources.

#### Example 
- Your application has been receiving malicious network requests from several IP addresses
- You want to prevent these requests from continuing to access your application, but you also want to ensure that legitimate users can still access it. You configure the web ACL to allow all requests except those from the IP addresses that you have specified.
- When a request comes into AWS WAF, it checks against the list of rules that you have configured in the web ACL. If a request did not come from one of the blocked IP addresses, it allows access to the application.
-  However, if a request came from one of the blocked IP addresses that you have specified in the web ACL, it is denied access.

## Amazon Inspector
- Amazon Inspector helps to **improve the security and compliance of applications by running automated security assessments.** It checks applications for security vulnerabilities and deviations from security best practices, such as **open access to Amazon EC2 instances and installations of vulnerable software versions.**
- After Amazon Inspector has performed an assessment, it provides you with a list of security findings. The list prioritizes by severity level, including a detailed description of each security issue and a recommendation for how to fix it.

## Amazon GuardDuty
- [**Amazon GuardDuty**](https://aws.amazon.com/guardduty) is a service that provides intelligent threat detection for your AWS infrastructure and resources.
- It identifies threats by continuously monitoring the network activity and account behavior within your AWS environment.
- GuardDuty begins monitoring your network and account activity. You do not have to deploy or manage any additional security software. GuardDuty then continuously analyzes data from multiple AWS sources, including VPC Flow Logs and DNS logs.
- If GuardDuty detects any threats, you can review detailed findings about them from the AWS Management Console. Findings include recommended steps for remediation.
- You can also configure AWS Lambda functions to take remediation steps automatically in response to GuardDuty’s security findings.