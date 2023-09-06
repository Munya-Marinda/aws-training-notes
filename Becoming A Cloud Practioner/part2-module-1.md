# Module 1: Security

## Topic A: Shared Responsibility Model

- Topic B: AWS IAM
  - Interactive Demo 1: Working with IAM
  - Interactive Demo 2: IAM Policies and Roles
- Topic C: AWS Organizations
- Topic D: Application Security

---

### Terminology

- MFA (Multi-factor authentication): An extra layer of security, for example, being notified of an attempted login.
- YubiKey: A hardware authentication device developed by Yubico, specializing in authentication and encryption solutions, providing two-factor authentication (2FA) and multi-factor authentication (MFA) capabilities for various online services.
- Encryption (server-side, client-side)
- Edge Location: A site used by CloudFront for caching your site's content.
- Authentication
- Authorization

## Topic A: Shared Responsibility Model

- On-Premises vs. Cloud
- Security in the Cloud
  - Security provided by AWS (off-premises)
- Security of the Cloud
  - Security created by AWS customers (off-premises)
  - For example, creating access rules for different users in your account, determining 'who can access what.'

## Topic B: AWS IAM (Identity and Access Management)

### Interactive Demo 1: Working with IAM

- Authentication vs. Authorization
  - "Do you have a ticket?" vs. "Do you have a passport?"
  - Username and Password vs. Key and Permissions policies
- IAM allows you to manage access to AWS services and resources.
- Users:
  - Root users: Full access, access to CloudTrail logs for all users.
  - IAM users:
    - Permissions granted by Root user, acting as sub Root users.
    - Best practice: Create individual IAM users for each person needing AWS access.
  - IAM groups: A collection of IAM users.

### Interactive Demo 2: IAM Policies and Roles

- A document (.json) that grants or denies access to AWS services or resources.
- Best Practice:
  - Apply policies to user groups and use as few policies as possible on individual users.
- IAM Roles
  - Provide temporary access with policies assigned to roles. For example, switching from Developer to DevOps.

## Topic C: AWS Organizations

- Helps control and manage organization accounts
- Root
  - AWS Account 1
  - AWS Account 2
  - OU (Organizational Unit)
    - AWS Account 3
    - AWS Account 1
- Consolidated Billing Overview
  - Feature allowing a single billing for all AWS accounts in your organization.
  - Monitor account spending within the organization.
  - Share savings across organization accounts.
  - Cannot set a maximum spending limit per group, but can set thresholds for notifications when spending exceeds a certain amount (you are charged for what you use).
  - Resource allocation among accounts.
  - Root (S3 = 14GB)
    - AWS Account 1 (2GB)
    - AWS Account 2 (5GB)
    - OU (Organizational Unit) (7GB)
      - AWS Account 3 (2GB)
      - AWS Account 4 (5GB)

## Topic D: Application Security

- AWS Security Firewall (1st line of defense)
  - AWS WAF (Web Application Firewall)
    - Protects web apps or APIs against unwanted traffic.
- AWS Shield
  - Protects against DDoS attacks.
- AWS Protector
  - Allows automated security assessments on your applications.
  - Records all activities and allows inspection.
  - Notifies of issues, vulnerabilities, and provides recommendations.
- Encryption
  - At-rest: Encryption of data where it's stored.
  - In-transit: Encryption of data while it's being transferred.
- AWS KMS (Key Management System)
  - Allows encryption operations using cryptographic keys.
- AWS GuardDuty (Intelligent Threat Detection)
  - Provides intelligent threat detection for AWS products and services.
  - Continuously analyzes network and account activities.
  - Offers a detailed review of findings.
