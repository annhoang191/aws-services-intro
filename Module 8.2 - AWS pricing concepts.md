# AWS pricing concept
## How AWS pricing works
- AWS offers a range of cloud computing services with pay-as-you-go pricing.
- **Pay for what you use**: For each service, you **pay for exactly the amount of resources that you actually use**, without requiring long-term contracts or complex licensing.
- **Pay less when you reserve**: Some services offer reservation options that provide a significant discount compared to On-Demand Instance pricing.
	- Ex: your company is using Amazon EC2 instances for a workload that needs to run continuously. You might choose to run this workload on Amazon EC2 Instance Savings Plans, because the plan allows you to save up to 72% over the equivalent On-Demand Instance capacity.
- **Pay less with volume-based discounts when you use more**: Some services offer tiered pricing, so the per-unit cost is incrementally lower with increased usage.
	- Ex: the more Amazon S3 storage space you use, the less you pay for it per GB.
## AWS Pricing Calculator
- It lets you explore AWS services and create an estimate for the cost of your use cases on AWS.
- You can organize your AWS estimates by groups that you define. A group can reflect how your company is organized, such as providing estimates by cost center.
- When you have created an estimate, you can save it and generate a link to share it with others.

#### Example
your company is interested in using Amazon EC2. However, **you are not yet sure which AWS Region or instance type would be the most cost-efficient for your use case**. In the AWS Pricing Calculator, **you can enter details such as the kind of operating system you need, memory requirements, and input/output (I/O) requirements. By using the AWS Pricing Calculator, you can review an estimated comparison of different EC2 instance types across AWS Regions.**

## AWS Pricing example
### AWS Lambda
- You are charged based on the number of requests for your functions and the time that it takes for them to run.
- AWS Lambda allows 1 million free requests and up to 3.2 million seconds of compute time per month.
- can save on AWS Lambda costs by signing up for a Compute Savings Plan: it offers lower compute costs in exchange for committing to a consistent amount of usage over a 1-year or 3-year term. This is an example of **paying less when you reserve**.

#### Example
all the AWS Lambda usage occurred in the Northern Virginia Region. The bill lists separate charges for the number of requests for functions and their duration.

Both the number of requests and the total duration of requests in this example are under the thresholds in the AWS Free Tier, so the account owner would not have to pay for any AWS Lambda usage in this month.

### AWS EC2
- You pay for only the compute time that you use while your instances are running.
- You can significantly reduce Amazon EC2 costs by using Spot Instances.
- Using a Spot Instance would provide you with up to 90% cost savings while still meeting the availability requirements of your workload if your workload is a batch processing job.

### Amazon S3
- **Storage -** You pay for only the storage that you use. You are charged the rate to store objects in your Amazon S3 buckets based on your objects’ sizes, storage classes, and how long you have stored each object during the month.
-  **Requests and data retrievals -** You pay for requests made to your Amazon S3 objects and buckets. For example, suppose that you are storing photo files in Amazon S3 buckets and hosting them on a website. Every time a visitor requests the website that includes these photo files, this counts towards requests you must pay for.
-  **Data transfer -** There is no cost to transfer data between different Amazon S3 buckets or from Amazon S3 to other services within the same AWS Region. However, you pay for data that you transfer into and out of Amazon S3, with a few exceptions. There is no cost for data transferred into Amazon S3 from the internet or out to Amazon CloudFront. There is also no cost for data transferred out to an Amazon EC2 instance in the same AWS Region as the Amazon S3 bucket.
-  **Management and replication -** You pay for the storage management features that you have enabled on your account’s Amazon S3 buckets. These features include Amazon S3 inventory, analytics, and object tagging.