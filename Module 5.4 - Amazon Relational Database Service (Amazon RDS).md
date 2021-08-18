# Amazon Relational Database Service (Amazon RDS)

## Relational database
- Data is stored in a way that relates it to other pieces of data.
- Use **structured query language (SQL)** to store and query data.

=> Data to be stored in an easily understandable, consistent, and scalable way.

## Amazon Relational Database Service
-  Is a service that enables you to run relational databases in the AWS Cloud.
-  It automates tasks such as hardware provisioning, database setup, patching, and backups.
- Can integrate Amazon RDS with other services to fulfill your business and operational needs, such as using AWS Lambda to query your database from a serverless application.
- Provides a number of different security options. Many Amazon RDS database engines offer **encryption at rest (protecting data while it is stored)** and **encryption in transit (protecting data while it is being sent and received).**

=> you can spend less time completing administrative tasks and more time using data to innovate your applications

### Amazon RDS Engines
- Amazon RDS is available on six database engines, which optimize for memory, performance, or input/output (I/O).
	- Amazon Aurora
	- Amazon PostgreSQL
	- MySQL
	- MariaDB
	- Oracle Database
	- Microsoft SQL Server
	
#### Amazon Aurora
- Is an enterprise-class relational database.
- It is compatible with MySQL and PostgreSQL relational databases.
- It is **up to five times faster than standard MySQL** databases and **up to three times faster than standard PostgreSQL** databases.
- It helps to reduce your database costs by **reducing unnecessary input/output (I/O) operations**, while ensuring that your database resources remain reliable and available.

=> Ideal for workloads require high availability. It **replicates six copies of your data across three Availability Zones** and **continuously backs up your data to Amazon S3.**