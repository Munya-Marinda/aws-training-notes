# Module 3: Compute in The Cloud

## Topic A: Amazon EC2 (Elastic Compute Cloud)

In this section, we'll explore Amazon Elastic Compute Cloud (EC2) and its key components.

- **Amazon Machine Image (AMI)**: An Amazon Machine Image provides all the information needed to launch an instance of Amazon EC2. It includes the operating system, applications, and user-defined parameters. AMIs serve as the blueprint for your EC2 instances.

- **Instance Types**: EC2 offers various instance types tailored to specific use cases.
  - **General Purpose**: Suited for a wide range of tasks.
  - **Compute Optimized**: Ensures that the same computation is not performed multiple times, optimizing processing speed.
  - **Memory Optimized**: Ideal for memory-intensive tasks, where data storage is crucial.
  - **Accelerated Compute**: Used for tasks like gaming and streaming, where accelerated processing is required.
  - **Storage Optimized**: Designed for low-latency, high-I/O tasks, ensuring efficient data storage and retrieval.

## Topic B: Amazon EC2 Auto Scaling

This topic introduces Amazon EC2 Auto Scaling, a service that automates the scaling of EC2 instances based on predefined conditions.

- **Automation**: EC2 Auto Scaling allows you to automate the process of adjusting the number of EC2 instances in a group, ensuring that you have the right number of instances to handle varying workloads.

- **Linear Scaling**: Instances can be added or removed in a linear manner to meet the demands of your application. A load balancer is often employed to evenly distribute incoming traffic among the instances.

## Topic C: Elastic Load Balancing

Elastic Load Balancing plays a vital role in distributing incoming traffic across multiple EC2 instances. Let's explore its different modes.

- **Application Balancing**: This mode directs traffic to specific application URLs, making it suitable for web applications and services with distinct endpoints.

- **Gateway Balancing**: It routes traffic to different Virtual Private Clouds (VPCs), allowing for a distributed network architecture.

- **Network Balancing**: In this mode, the load balancer manages protocol-level traffic such as FTP, SSH, and HTTPS. It ensures efficient and secure communication between clients and backend services.

These topics provide an overview of key aspects related to Amazon EC2 and the tools available for managing and optimizing compute resources in the cloud.