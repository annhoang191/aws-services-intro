# Amazon Database Migration Service
- It enables you to migrate relational databases, nonrelational databases, and other types of data stores.
- You move data between a source database and a target database.
- [The source and target databases](https://aws.amazon.com/dms/resources) can be of the same type or different types.
- During the migration, your source database remains operational, reducing downtime for any applications that rely on the database.
#### Example
you have a MySQL database that is stored on premises in an Amazon EC2 instance or in Amazon RDS. Consider the MySQL database to be your source database. Using AWS DMS, you could migrate your data to a target database, such as an Amazon Aurora database.

## Use cases
- **Development and test database migrations**: enabling developers to test applications against production data without affecting production users.
- **Database consolidation**: combining several databases into a single database.
- **Continuous replication**: sending ongoing copies of your data to other target sources instead of doing a one-time migration.
- 