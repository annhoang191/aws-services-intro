# Amazon Elastic Block Store (Amazon EBS)
## Instance stores
- Block-level storage volumes behave like physical hard drives.
- Provides temporary block-level storage for an Amazon EC2 instance.
- Is disk storage that is physically attached to the host computer for an EC2 instance, and therefore has the same lifespan as the instance.
- When the instance is terminated, you lose any data in the instance store.
### Notes
Amazon **EC2 instances are virtual servers**. If you start an instance from a stopped state, **the instance might start on another host**, where the previously used instance store volume does not exist 
=>Therefore, AWS **recommends instance stores for use cases that involve temporary data that you do not need in the long term.**

## Amazon Elastic Block Stores (Amazon EBS)
- Is a service that provides block-level storage volumes that you can use with Amazon EC2 instances.
- If you stop or terminate an Amazon EC2 instance, all the data on the attached EBS volume remains available.
- To create an EBS volume, you define the configuration (such as volume size and type) and provision it.
- After you create an EBS volume, it can attach to an Amazon EC2 instance.
- Because **EBS volumes are for data that needs to persist, it’s important to back up the data.**

### Amazon EBS Snapshot
- Is an incremental backup.
- The first backup taken of a volume copies all the data. For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved.
![](https://docs.amazonaws.cn/en_us/AWSEC2/latest/UserGuide/images/snapshot_1a.png)