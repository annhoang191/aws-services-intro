# Elastic Load Balancing
- The AWS service that automatically distributes incoming application traffic across multiple resources, such as EC2 instances.
- A load balancer acts as a single point of contact for all incoming web traffic to your Auto Scaling group. This means that as you add or remove EC2 instances in response to the amount of incoming traffic, these requests route to the load balancer first.
- If you have multiple EC2 instances, Elastic Load Balancing distributes the workload across the multiple instances so that no single instance has to carry the bulk of it.
- Elastic Load Balancing and EC2 are separate services, they work together to help ensure that apps running in EC2 can provide high performance and availability.
## Example
 Suppose that a few customers have come to the coffee shop and are ready to place their orders.
- **Low-Demand period**: If only a few registers are open, this matches the demands of customers who need service. The coffee shop is less likely to have open registers with no customers. In this example you can think of the registers as EC2 instances.
- **High-Demand period**: as number of customers increases, the coffee shops opens more registers to accommodate them. In the diagram, the Auto Scaling group represent this. Additionally, a coffee shop employee directs customers to the most appropriate register so that the number of request can evenly distribute across the open registers. You can think of this coffee shop employee as a load balancer.
![](https://miro.medium.com/max/1740/1*JKv06SJiCDJqExr7dUBCyA.jpeg)