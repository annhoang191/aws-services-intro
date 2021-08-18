# Domain Name System (DNS)
- DNS resolutioin involves a customer DNS resolver communicating with a company DNS server.
- You can think of DNS as a phone book of the internet. DNS resolution is the process of translating a domain name to an IP address.
1. When you enter the domain name into your browser, this request is sent to a customer DNS resolver.
2. The customer DNS resolver ask the company DNS server for the IP address that corresponds to the website.
3. The company DNS server responds by providing the IP address for the website, such as 192.0.2.0

## Amazon Route 53
- A DNS web service
- It gives developers and businesses a reliable way to route end users to internet applications hosted in AWS
- It connects user requests to infrastructure running in AWS (EC2, load balancer,...)
- It can route users to infrastructure outside AWS.
- It has the ability to manage the DNS records for domain names. You can register new domain names directly in Route 53.
- You can also transfer DNS records for existing domain names managed by other domain registers. This enable you to manage all of your domain names within a single location.

### Example of how Amazon Route 53 and Amazon Cloud front deliver content
![](https://blog.shikisoft.com/assets/images/post_imgs/cloudfront/cloudfront-dynamic-web-architecture.png)

1. Customer requests data from the application by going to AnyCompany's website.
2. Route 53 uses DNS resolution to identify AnyCompany.com's corrresponding IP address, 192.3.3.2. This information is sent back to the customer.
3. The customer's request is sent to the nearest edge location through Amazon Cloudfront.
4. Amazon Cloudfront connects to the Application Load Balancer, which sends the incoming packet to an Amazon EC2 instance.