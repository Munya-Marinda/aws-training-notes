# Module 3: Networking

- Topic A: Amazon Virtual Private Cloud (Amazon VPC)

  - Interactive Demo 1: Building a VPC

- Topic B: Network access control lists and security groups
  - Interactive Demo 2: Viewing Internet Gateways and route tables
  - Interactive Demo 3: Viewing ACLs and SGs

---

### Terminology

- OS
  - Operating System
- DNS
  - Domain Name System
- CIDR
  - Classess Inter-domain Routing
- HTTP
- IP
- ACL
  - Access Control Lists: contains a list of traffic rules to protect access to public and private subnets.
  - Allows control for IN and OUT traffic
- Security Groups
  - Come after the ACL that protects the public sub. They add further security to EC2 or S3
  - Allows control for IN and OUT traffic
- Data Packets
- Protocols
  - HTTP, FTP, SSH
- Port/ Port Number
- IP Addresses
- Routing
- Subnet/Subnetting/Subnet Mask
  - Dividing networks
  - Public and Private Subnets
- Switch
- Router
- Gateway
- NAT (Network Address Translation) gateway (acts as a proxy server)
  - Allows communication between the private subnet and the internet

<br>
<br>

# Amazon VPC (Virtual Private Cloud) Server

    Used to subnet networks between private and public

- Allows you to assolate your instances and buckets
- Only allowed VPCs in the same region

<br>
<br>

# Virtual Private Gateway

- You can access private subnet using a Virtual Private Gateway

<br>
<br>

# AWS Direct Connect

- Dedicated private connection between your network and AWS Cloud
- Coporate Data Center >>> AWS Direct Connect endpoint >>> Virtual Private Gateway
