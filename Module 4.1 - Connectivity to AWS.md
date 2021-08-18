# Amazon Virtual Private Cloud (VPC)
- Amazon VPC is a networking service that you can use to establish boundaries around your AWS resources.
- It enables you to provision an isolated section of the AWS Cloud. 
- In this isolated section, you can launch resources in a virtual network that you define.
- Within a virtual private cloud, you can organize your resources into subnets. 
- **Subnet**: a section of a VPC that can contain resources such as EC2 instances.

## Internet Gateway
- To allow public traffic from the internet to access your VPC, you attach an internet gateway to the VPC.
- Internet gateway: a connection between VPC and the internet.
![](https://docs.aws.amazon.com/vpc/latest/userguide/images/internet-gateway-overview-diagram.png)

## Virtual private gateway
- To access private resources in a VPC, you can use a virtual private gateway.
- It is the component that allow protected internet traffic to enter into the VPC. 
- It enables you to establish a virtual private network connection between your VPC and a private network, such as on-premises data center or internal corporate network.
- It allows traffic into the VPC only if it is coming from an approved network.
![](https://d2908q01vomqb2.cloudfront.net/5b384ce32d8cdef02bc3a139d4cac0a22bb029e8/2020/08/25/site-to-site-vpn-scenarios-vgw-1.png)

## AWS Direct connect
- A service that enables you to establish a dedicated private connection between your data center and a VPC.
- The private connection that AWS Direct Connect provides helps you to reduce network costs and increase the amount of bandwidth that can travel through your network.
![](https://d2908q01vomqb2.cloudfront.net/5b384ce32d8cdef02bc3a139d4cac0a22bb029e8/2019/11/20/dxg_overviewE.png)
