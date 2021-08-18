# Subnets
- A section of a VPC in which you can group resources based on security or operational needs.
- They can be public or private.
	- **Public subnet**: contain resources that need to be accessible by the public, such as an online store's website.
	- **Private subnet**: contain resources that should be accessible only through your private network, such as a database that contains customers' personal information and order histories.
- In VPC subnets can communicate with each other.
# Network traffic in VPC
- When a customer requests data from an app hosted in the AWS Cloud, this request is sent as a packet.
- A packet: a unit of data sent over the internet or a network. It enters into a VPC through an internet gateway. Before a packet can enter into a subnet or exit from a subnet, it checks for permissions.
- These permissions indicate who sent the packet and how the packet is trying to communicate with the resources in a subnet.
- VPC component that checks packet permissions for the subnets is a **Network Access Control List (ACL)**

## Network Access Control List (ACL)
- A virtual firewall that controls inbound and outbound traffic at the subnet level.
- Each AWS account includes a default network ACL. When configuring your VPC, you can use your account's default network ACL or create custom network ACL.
- **By default ACL allows all inbound and outbound traffic**, but you can modify it by adding your own rules.
- For custom network all inbound and outbound traffic is denied until you add rules to specify which traffic to allow.
- All network ACL have an explicit deny rule: it ensures that if a packet doesn't match any of the other rules on the list, the packet is denied.

## Stateless packet filtering
- ACLs perform stateless packet filtering: they remember nothing and check packets that cross the subnet border each way: inbound and outbound.
- When a packet response for that request comes back toe the subnet, the ACL does not remember your previous request. The ACL checks the packet response against its list of rules to determine whether to allow or deny.
- After a packet has entered a subnet, it must have its permissions evaluated for resources within the subnet, such as EC2 instances.
- The component that checks packet permissions for an EC2 is a security group

# Security groups
- A virtual firewall that controls inbound and outbound traffic for an EC2 instance.
- **By default a security group denies all inbound traffic and allow all outbound traffic**. You can add custom rules to configure.
- If you have multiple EC2 within a subnet, you can associate them with the same security group or use different security groups for each instance.

## Stateful packet filtering
- Security groups perform stateful packet filtering: They remember previous decision made for incoming packet.
- When a packet response for that request returns to the instance, the security group remembers your previous request. The security group allows the response to proceed, regardless of inbound security group rules.

=> Both network ACLS and security groups enable you to configure custom rules for the traffic in your VPC. 
![](https://jayendrapatil.com/wp-content/uploads/2016/03/security-diagram.png)