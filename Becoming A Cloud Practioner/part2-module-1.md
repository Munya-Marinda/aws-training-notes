# Module 1: Security

- Topic A: Shared responsibility model
- Topic B: AWS IAM

  - Interactive Demo 1: Working with IAM
  - Interactive Demo 2: IAM Policies and roles

- Topic C: AWS Organizations
- Topic D: Application Security

<br>

<hr>
<hr>

<br>
 
### Terminology

- MFA (Multi factor authentication)
  - Extra layer of security, example: being notified of an attempted login
  - YUBI Key : A YubiKey is a hardware authentication device developed by Yubico, a company specializing in authentication and encryption solutions. YubiKeys are designed to enhance security by providing two-factor authentication (2FA) and multi-factor authentication (MFA) capabilities for various online services, applications, and systems.
- Encryption (server side, client side)
- Edge Location : a site that CloudFront uses for caching content of your site
- Authentication
- Authorization

## Topic A: Shared responsibility model

- On premises VS Cloud
- Security In the cloud
  - Security provided by AWS (off prem)
- Security Of the cloud
  - Security created by the AWS customer (off prem)
  - for example, creating rules for access for the different users for your account, 'who and who cannot access what'

## Topic B: AWS IAM (Identity and Access Management)

- Interactive Demo 1: Working with IAM - Authntication VS Authorization - Do you have a ticket VS do you have a passport - Username and Password, Key VS Permissions policies
  - IAM allows you to manage access to AWS services and resources
  - Users:
    - Root users : all access, access to cloudtrail (logs of all users)
    - IAM users
      - Given permissions by Root user, acts as a sub Root user.
      - Best practice, create individual IAM users for each person who needs access to AWS.
    - IAM groups is a group of IAM users

<br>

- Interactive Demo 2: IAM Policies and roles
  - A document (.json) that grants or denies access to to AWS services or resources.
  - Best Practice:
    - Apply policies to users groups and try as little as possible to apply policies to users.
  - IAM Roles
  - Give you temporary access to policies applied to your roles. example: switching from Developer to DeOps

## Topic C: AWS Organizations

- Help control and manage your organization accounts
- - Root
  - AWS Account 1
  - AWS Account 2
  - OU (Organizational Unit)
    - AWS Account 3
    - AWS Account 1
- Consolidated Billing Overview
  - Feature that allows you to recieve a single billing for all AWS accounts in your organization.
  - Can see how much account spent in the organization
  - Can share savings across the accounts in your organization
  - Cannot set a maximum amount to be spent per group, but you can set thresholds that will notify you when the amount is increased above the thresholds amount. (you are charged for what you use)
  - Can also devide resoures amongst accounts
  - - Root (S3 = 14GB)
      - AWS Account 1 (2GB)
      - AWS Account 2 (5GB)
      - OU (Organizational Unit) (7GB)
        - AWS Account 3 (2GB)
        - AWS Account 4 (5GB)

## Topic D: Application Security

- AWS Security Firewall (1 line of defence)
  - AWS WAF (Web Application Firewalls)
    - Protects webs apps or APIs against unwanted traffic
- AWS Shield
  - Protects against DDos attacks
- AWS Protector
  - Allows you to perform automated security assessments on your applications
  - Records all activities and allows you to 'inspect'
  - Notifies us of the issues and vulnerabilities and gives recommendations
- Encryption
  - At-rest : encryption of data where its stored
  - In-transit : encryption of data while its being transferred
- AWS KMS (Key Management System)
  - Allows encryption operations through the use of cryptographic keys.
- AWS GuardDuty (Intelligent Threat Detection)
  - Provides Intelligent Threat Detection threat detection for AWS products and services.
  - Continuously analyzes network and account activities
  - Gives detailed review of findings
