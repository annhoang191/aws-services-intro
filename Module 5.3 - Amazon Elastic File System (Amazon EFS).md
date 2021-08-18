# Amazon Elastic File System - Amazon EFS

## File Storage
- Multiple clients (such as users, applications, servers, and so on) can access data that is stored in shared file folders.
- A storage server uses block storage with a local file system to organize files. Clients access data through file paths.

=> File storage is ideal for use cases in which **a large number of services and resources need to access the same data at the same time.**

## Amazon Elastic File System
- Is a scalable file system used with AWS Cloud services and on-premises resources.
- As you add and remove files, Amazon EFS grows and shrinks automatically.
- It can scale on demand to petabytes without disrupting applications.
- Amazon EFS is a regional service.
- It stores data in and across **multiple** Availability Zones.
- The duplicate storage enables you to access data concurrently from all the Availability Zones in the Region where a file system is located.
- On-premises servers can access Amazon EFS using AWS Direct Connect.