# Module 2: Storage

## Topic A: Block Storage with Amazon EBS (Elastic Block Storage) (Linux OS)

In this section, we'll delve into the concept of block storage using Amazon Elastic Block Storage (EBS) in the context of a Linux operating system.

- **Usage with EC2 Instances**: Amazon EBS is primarily used to provide block-level storage for Elastic Compute Cloud (EC2) instances. It offers the flexibility to attach, detach, and reattach storage volumes to EC2 instances as needed.

- **Equal-Sized Blocks**: EBS volumes consist of equal-sized blocks, which can be thought of as individual storage units within a hard drive. This uniformity allows for efficient data management and allocation.

- **Amazon Instance Store**: It's essential to differentiate between Amazon EBS and Amazon Instance Store. When you terminate an EC2 instance that uses an Instance Store for storage, the data on that store is deleted along with the instance.

- **Amazon Elastic Block Storage**: On the other hand, EBS volumes persist even if you terminate the associated EC2 instance. This characteristic makes EBS a more suitable choice when you require data durability beyond the life of an EC2 instance.

- **Snapshots for Data Backup**: Amazon EBS provides a valuable feature known as snapshots. These snapshots act as backups and capture the state of your EBS volume at a particular moment. Importantly, snapshots are incremental, meaning they only update the files that have changed or new files, reducing storage costs and improving efficiency.

## Topic B: File Storage with Amazon EFS (Elastic File Storage) (Windows OS)

Moving on to Topic B, we explore file storage using Amazon Elastic File Storage (EFS) within a Windows operating system environment.

- **Scaling File Storage**: Amazon EFS becomes particularly useful when you've exhausted the available disk space on your Amazon EBS volumes. In such cases, you can seamlessly move files from EBS to EFS to address growing storage needs.

- **Scalability**: One of EFS's standout features is its scalability. It's designed to grow with your requirements, making it an ideal choice for workloads that demand dynamic and elastic file storage.

## Comparison Table: S3 vs. EBS vs. EFS

Let's summarize the key differences between Amazon S3, Amazon EBS, and Amazon EFS:

| Feature          | Amazon S3                                      | Amazon EBS                        | Amazon EFS                                    |
| ---------------- | ---------------------------------------------- | --------------------------------- | --------------------------------------------- |
| Scalability      | Automatically Scalable                         | Manually Scalable                 | Auto Scalable                                 |
| Data Location    | Same Region                                    | Same Availability Zone (AZ)       | Same Region                                   |
| Data Replication | Auto Replicated to multiple Availability Zones | Replicas are added to the same AZ | Replicas are added to the same region         |
| Attachment       | Cannot be attached to an EC2 instance          | Attached to a single EC2 instance | Can be accessed by thousands of EC2 instances |

This table provides a clear comparison of these AWS storage services, highlighting their unique features and use cases.
