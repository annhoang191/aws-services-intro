# Client-Server model
- Client: web browser, desktop app that persion interacts to make request
- Server: services such as Amazon Elastic Compute Cloud (EC2 - a virtual server) 

# Cloud computing
To select a cloud strategy, a company must consider factors such as required cloud application components, preferred resource management tools, legacy IT infra requirements.

## Cloud-based deployment
- Run all parts of the app in the cloud
- Migrate existing apps to the cloud
- Design and build new app in the cloud

You can build those apps on low-level infra that requires your IT staff to manage them. Alternatively, you can build them using higher level services that reduce the management, architecting, and scaling requirements of the core infra
### Example
- A company might create an app consisting of virtual servers, databases, networking components that are fully based in the cloud

## On-premises deployment
- Deploy resource by using virtualization and resource management tools
- Increase resource utilization by using application management and virtualization technologies
On-premises is also known as **private cloud** deployment. In this model, resources are deployed on premises by using virtualization and resource management tools.
### Example
- You might have apps that run on technology that is fully kept in your on-premises data center. Through this model is much like legacy IT infra, its corporation of application management and virtualization technologies helps to increase resource utilization

## Hybrid deployment
- Connect cloud-based resources to on-premises infra
- Integrate cloud-based resources with legacy IT apps

In a hybrid deployment, cloud-based resources are connected to on-premises infra. You might want to use this approach in a number of situation.
### Example
- You have legacy apps that are better maintained on premises, or goverment regulations require your business to keep certain records on premises.
- A company wants to use cloud services that can automate batch data processing and analytics. However the company has several legacy apps that are more suitable on premises and will not be migrated to the cloud. With a hybrid deployment, the company would be able to keep the legacy apps on premises while benefiting from the data and analytics services that run in the cloud

# Benefits of cloud computing
- Trade upfront expense for variable exepense
	- Upfront expense: data centers, physical servers, and other resources that you would need to invest in before using them.
	- Variable expense: only pay for computing resources you consume instead of investing heavily in data centers and servers before you know how you're going to use them.
=> Companies can implement innovation solutions while saving on costs
- Stop spending money to run and maintain data centers
	- Computing in data centers often requires you to spend more money and time managing infra and servers
=> Cloud computing can help you focus less on these tasks and more on your apps and customers
- Stop guessing capacity 
	- No need to predict how much infra capacity you will need before deploying an app
=> You can launch an EC2 instance when needed and pay only for the the compute time you use. Instead of paying unused resources or having to deal with limited capacity. You can also scale in or scale out in response to demand
- Benefit from massive economies of scale
	- You can achieve lower variable cost than you can get on your own
	- The economy of scale translates into lower pay-as-you-go prices
- Increase speed and agility
	- This flexibility gives you more time to experiment and innovate.
	- When computing in data centers, it may take weeks to obtain new resources that you need. By comparision, cloud computing enables you to access new resources within minutes
- Go global in minutes
	- The global footprint of aws enables you to deploy apps to customers around the world quickly, while providing them with low latency.
=> If you are located in a different part of the world than your customers, customers are able to access your applications with minimal delays