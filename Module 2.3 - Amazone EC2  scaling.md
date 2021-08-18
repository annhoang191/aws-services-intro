# Amazon EC2
## Scaling
**Scalability** involves beginning with only the resource you need and designing your architecture to automatically respond to changing demand by scaling out or in.
=> You don't have to worry about a lack of computing capacity to meet your customers' needs.

If you'ved tried to access a website that wouldn't load and frequently timed out, the website might have received more requests than it was able to handle.

## EC2 Auto Scaling
- Amazon EC2 Auto Scaling enables you to automatically add or remove EC2 instances in response to changing application demand.
- By automatically scaling your instances in and out as needed, you are able to maintain a greater sense of application availability.
- You can use two approaches 
	- Dynamic scaling: respond to changing demand.
	- Predictive scaling: automatically schedules the right number of EC2 instances based on predicted demand.
#### Notes
You can use dynamic and predictive scaling together to scale faster.

#### Example
You are preparing to launch an app on EC2 instances. When configuring the size of your Auto Scaling group, you might set the minimum number of EC2 instances at one. This means that at all times, there must be at least one EC2 instance running.
- The **minimum capacity** is the number of EC2 instances that launch immediately after you have created the Auto Scaling group. 
- In this example, the Auto Scaling group has a minimum capacity of one EC2 instance.
- Next, you can set the **desired capacity** at two EC2 instances even though your app needs a minimum of a single EC2.
- You can set the **maximum capacity** to scale out in response to increased demand, but only to a maximum of four instances.
![](https://miro.medium.com/max/487/1*uS9J8btKCQaMOhnUXp62aA.jpeg)