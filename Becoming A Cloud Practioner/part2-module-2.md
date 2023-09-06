# Module 2: Storage

- Topic A: Block storage with Amazon EBS (Linux OS)
- Topic B: File storage with Amazon EFS (Windows OS)

<br>

<hr>
<hr>

<br>

## Topic A: Block storage with Amazon EBS (Elastic Block Storage) (Linux OS)

- Used for EC2
- Equal sized blocks inside a hardrive
- Amazon Instance Store:
  - EC2 -> Instance Store
  - When you kill/terminate the EC2, the Instance Store will be deleted
- Amazon Elastic Block Storage
  - EC2 -> Instance Store
  - Easy to use, scalable
  - Designed for EC2
  - When you kill/terminate the EC2, the EBS will NOT be deleted
- Amazon EBS snapshots - Snapshots (backups) - Only updates the files that were changed and adds new files but keeps the orginal

## Topic B: File storage with Amazon EFS (Elastic File Storage) (Windows OS)

- Used when you run out of disk space, you can move the files from EBS to EFS
- Is scalable (elastic)

## Comparison Table: S3 vs EBS vs EFS

This table provides a comparison of features between Amazon S3, Amazon EBS, and Amazon EFS.

| Feature          | Amazon S3                             | Amazon EBS                          | Amazon EFS                                |
| ---------------- | ------------------------------------- | ----------------------------------- | ----------------------------------------- |
| Scalability      | Automatically Scalable                | Manually Scalable                   | Auto Scalable                             |
| Data Location    | Same Region                           | Same AZ                             | Same Region                               |
| Data Replication | Auto Replicated to multiple AZs       | Replicas are added to same AZ       | Replicas are added to same region         |
| Attatchment      | Cannot be attached to an EC2 instance | Only available to a single instance | Can be accessed by 1000s of EC2 instances |
