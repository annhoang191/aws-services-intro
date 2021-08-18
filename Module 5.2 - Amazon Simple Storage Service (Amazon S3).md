# Amazon S3

## Object Storage
![](https://cloud.vn/images/basic/object-storage-1.png)
- Each object **consists of data, metadata, and a key**. The data might be an image, video, text document, or any other type of file.
- Metadata contains information about what the data is, how it is used, the object size, and so on.
- An object’s key is its unique identifier.
#### Notes
When you **modify a file in block storage, only the pieces that are changed are updated**. When a **file in object storage is modified, the entire object is updated.**

## Amazon Simple Storage Service (Amazon S3)
- Is a service that provides object-level storage. Amazon S3 stores data as objects in buckets.
- You can upload any type of file to Amazon S3, such as images, videos, text files, and so on.
- Amazon S3 offers unlimited storage space.
- The maximum file size for an object in Amazon S3 is **5 TB**.
- When you upload a file to Amazon S3, you can set permissions to control visibility and access to it.
- You can also use the Amazon S3 versioning feature to track changes to your objects over time.
#### Example
Use Amazon S3 to store backup files, media files for a website, or archived documents.

### Amazon S3 Storage Classes
- You pay only for what you use =>  can choose from [a range of storage classes](https://aws.amazon.com/s3/storage-classes) to select a fit for your business and cost needs.
- Consider these two factors:
	- How often you plan to retrieve your data
	- How available you need your data to be
#### S3 Standard
- Designed for frequently accessed data.
- Stores data in a minimum of three Availability Zones.
- Provides high availability for objects.
- Has a higher cost than other storage classes intended for infrequently accessed data and archival storage.

=> This makes it a good choice for a wide range of use cases, such as **websites, content distribution, and data analytics.**

#### S3 Standard-Infrequent Access (S3 Standard-IA)
- Ideal for infrequently accessed data.
- Similar to S3 Standard but has a lower storage price and higher retrieval price.
- Store data in a minimum of three Availability Zones.
- Provides the same level of availability as S3 Standard but with a lower storage price and a higher retrieval price.

=> Is ideal for **data infrequently accessed but requires high availability** when needed

#### S3 One Zone-Infrequent Access (S3 One Zone-IA)
- Stores data in a single Availability Zone.
- Has a lower storage price than S3 Standard-IA.

=> This makes it a good storage class to consider if the following conditions apply:
		- You want to **save costs** on storage.
		- You can **easily reproduce your data** in the event of an Availability Zone failure.
		
#### S3 Intelligent-Tiering
- Requires a small monthly monitoring and automation fee per object.
- Amazon S3 monitors objects’ access patterns.
- If you haven’t accessed an object for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, S3 Standard-IA.
- If you access an object in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, S3 Standard.

=> Ideal for **data with unknown or changing access patterns**.

#### S3 Glacier
- Low-cost storage designed for data archiving.
- Able to retrieve objects within a few minutes to hours.

=> Is ideal for **data archiving**. For example, you might use this storage class to store archived customer records or older photos and video files.

#### S3 Glacier Deep Archive
- Lowest-cost object storage class ideal for archiving.
- Able to retrieve objects within 12 hours.

=> When deciding between Amazon S3 Glacier and Amazon S3 Glacier Deep Archive, consider **how quickly you need to retrieve archived objects.**