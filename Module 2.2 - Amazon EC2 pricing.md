# Amazon EC 2
## Pricing
- Only pay for the compute time that you use.
- EC2 offers these pricing options for different use cases.

### On-Demand
- Ideal for short-term, irregular workloads that cannot be interrupted.
- No upfront costs or minimum contracts apply.
- The instances run continuously until you stop.
- Only pay for the compute time you use.
- Are not recommended for workloads that last a year or longer because these workloads can experience greater cost savings using Reserved Instances.
- 
#### Example
- Developing and testing applications and running applications that have unpredictable usage patterns.

### Saving plans
- Enable you to reduce your compute costs by committing to a consistent amount of compute usage for a 1-year or 3-year term.
- This term commitment results in savings up to 72% over On-Demand costs.
- Any usage up to the commitment is charged at the discounted Savings Plan rate (example: $10 an hour).
- Any usage beyond the commitment is charged at regular On-Demand rates.

#### Notes
- AWS Cost Explorer can analyze your EC2 usage over the past 7, 30, or 60 days. It also provides customized recommendations for Savings Plans. These recommendations estimate how much you could save on your monthly Amazon EC2 costs, based on previous Amazon EC2 usage.

### Reserved Instances
- Are billing discount applied to the use of On-Demand Instances in your account.
- You can purchase Standard Reserved and Convertible Reserved Instances for a 1-year or 3-year term - Scheduled Reserved Instances for a 1-year term.
- At the end of a Reserved Instance term, you can continue using the EC2 instance without interruption. However, you are charged On-Demand rates until you do one of the following:
	- Terminate the instance
	- Purchase a new Reserved Instance that matches the instance attributes (instance type, region, tenancy, platform)

### Spot instances
- Ideal for workloads with flexible start and end times, or that can withstand interruptions.
- They use unused EC2 computing capacity and offer you cost savings at up to 90% off on On-Demand prices.
- After you have launched a Spot Instance, if capacity is no longer available or demand for Spot Instances increates, your instance may be interrupted.
- This might not pose any issues for your background processing job. However in the earlier example of developing and testing applications, you would most likely want to avoid unexpected interruptions.
#### Example
You have a background processing job that can start and stop as needed (such as the data processing job for a customer survey). You want to start and stop the processing job without affecting the overall operations of your business.
=> If you make a spot request and EC2 capacity is available, your spot instance launches. However if you make a spot request and EC2 capacity is unavailable, the request is not successful until capacity becomes available. The unavailable capacity might delay the launch of your background processing job.

### Dedicated Hosts
- Are physical servers with EC2 instance capacity that is fully dedicated to your use.
- You can use your existing per-socket, per-core, per-VM software licenses to help maintain license compliance.
- You can purchase On-Demand Dedicated Hosts and Dedicated Hosts Reservations.
- Dedicated Hosts are the most expensive.