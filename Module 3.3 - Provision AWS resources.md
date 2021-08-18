# Ways to interact with AWS Services

## AWS management console
- A web-based interface for accessing and managing AWS services. You can quickly access recently used services and search for other services by name, keyword, or acronym.
- The console includes wizards and automated workflows that can simplify the process of completing tasks.
- Can also use AWS Console mobile app to perform tasks such as monitoring resources, viewing alarms, and accessing billing information.
- Multiple identites can stay logged into the AWS Console mobile app at the same time

## AWS Command line interface
- To save time when making API requests, you can use the AWS CLI.
- It enables you to control multiple AWS services directly from the command line within one tool.
- AWS CLI available for Windows, macOS, and Linux.
- You can automate the actions that your services and apps perform through scripts. 
- Example: You can use command line to launch an EC2 instances, connect an EC2 instance to a specific Auto Scaling group, and more.

## Software Development Kits (SDK)
- Make it easier for you to use AWS services through an API designed for your programming language or platform.
- SKDs enables you to use AWS services with your existing apps or create entirely new apps that will run on AWS.
- AWS provides sample code for each supported programming languages. 

# AWS Elastic Beanstalk
- You provide code and configuration settings, and Elastic Beanstalk deploys the resources neccessary to perform the following tasks:
	- Adjust capacity.
	- Load balancing.
	- Automatic Scaling.
	- Application health monitoring.

# AWS CloudFormation
- You can treat your infrastructure as code: this means you can build an environment by writing lines of code instead of using the AWS management console to individually provision resources.
- It provisions your resources in a safe, repeatable manner, enabling you to frequently build your infrastructure and applications without having to perform manual actions. 
- It determines the right actions to perform when managing your stack and rolls back changes automatically if it detects errors.