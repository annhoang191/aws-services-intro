# Serverless computing
When you use EC2 instances, you have to do the following:
- Provision instances (virtual servers).
- Upload your code.
- Continue to manage the instances while your app is running.

**Serverless** means your code runs on servers but you do not need to provision or manage these servers. It can gives you these benefits:
- You can focus more on innovating new products and features instead of maintaining servers.
- The flexibility to scale serverless applications automatically.
- Serverless computing can adjust the application's capacity by modifying the units of consumptions, such as throughput and memory.

## AWS Lambda
- A service that lets you run code without needing to provision or manage servers.
- You pay only for the compute time that you consume. Charges apply only when your code is running.
- You can also run code for virtually any type of application or backend service, all with zero administration.
### How Lambda works
![](https://d1.awsstatic.com/product-marketing/Lambda/Diagrams/product-page-diagram_Lambda-HowItWorks.68a0bcacfcf46fccf04b97f16b686ea44494303f.png)
1. You upload code to Lambda.
2. You set your code to trigger from an event source, such as AWS services, mobile apps, HTTP endpoints.
3. Lambda run your code only when triggered.
4. Pay only for the compute time that you use.

### Example
A simple lambda function might involve automatically resizing uploaded images to the AWS Cloud. The function triggers when uploading a new image.

# Containers
- It provides you with a standard way to package your application's code and dependencies into a single object. 
- Can use containers for processes and workflows in which there are  essential requirements for security, reliability, and scalability.

## Amazon Elastic Container Services (Amazon ECS)
- A highly scalable, high-performance container management system that enables you to run and scale containerized application on AWS.
- It supports Docker containers: supports the use of open-source Docker Community Edition and subscription-based Docker Enterprise Edition.
- You can use API calls to launch and stop Docker-enabled applications.

## Amazon Elastic Kubernetes Service (Amazon EKS)
- A fully managed services that you can use to run Kubernetes on AWS.
- Kubernetes is an open source software that enables you to deploy and manage containerized applications at scale. 
- AWS actively works together with the Kubernetes community. 
- As new features release for Kubernetes applications, you can easily apply these updates to your applications managed by Amazon EKS

## AWS Fargate
- A serverless compute engine for containers.
- It works with both ECS and EKS.
- You do not need to provision or manage servers.
- Fargate manages your server infra for you.
- Pay only for the resources that are required to run your containers.