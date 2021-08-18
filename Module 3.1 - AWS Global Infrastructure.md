# Region
- Region: a large group of data centers.
- AWS build Regions to be closest to where the business traffic demands.
- Inside each Region we have multiple data centers that have all the compute, storage, and other services you need to run your applications.
- Each Region can be connected to each other Region through a high speed fiber network, controlled by AWS.

## Selecting a Region
Consider the following four business factors:
- **Proximity to your customers**: selecting a Region that close to your customers will help you to get content to them faster. For example: your company is based in Washington DC and many of your customers live in Singapore. You might consider running your infrastructure in the Northern Virginia Region to be close to your company headquarters, and run your applications from the Singapore Region.
- **Compliance with data government and legal requirement**: You might need to run your data out of specific area. For example if your company requires all of its data to reside within the boundaries of the UK, you would choose the London Region.
- **Availability services within Region**: 
	- sometimes the closest region might not have all the features that you want to offer customers. 
	- AWS frequently innovating by creating new services and expanding features within existing services. However, making new services available around the world sometimes requires AWS to build out physical hardware one Region at a time.
	- Suppose that developers want to build an application that uses Amazon Braket (quantum computing platform). Braket is not yet available in every Region around the world.
- **Pricing**: Several facotrs determine pricing. The cost of services can vary from Region to Region

# Availability Zone
- A single data center or a group of data centers within a Region.
- AZ are located tens of miles apart from each other.
- This is close enough to have low latency (the time between when content requestes and received) between AZ.
- If a disaster occurs in one part of the Region, they are distant enough to reduce the chance that multiple AZs are affected