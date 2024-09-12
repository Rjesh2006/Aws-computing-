# [AWS - Cloud Computing](#)

## Cloud Computing

### AWS Overview
#### Essential AWS Services Breakdown

**Compute:**
- **EC2**: Scalable virtual servers for running applications.
- **Lambda**: Serverless compute that runs code in response to events.
- **ECS**: Docker container orchestration service.
- **Elastic Beanstalk**: Easy deployment and scaling for web apps.

**Storage:**
- **S3**: Scalable object storage for data, files, and backups.
- **EBS**: Block storage for use with EC2 instances.
- **Glacier**: Low-cost archival storage for long-term data retention.
- **FSx**: Managed file systems for Windows and Linux workloads.

**Database:**
- **RDS**: Managed relational databases like MySQL, PostgreSQL, and Oracle.
- **DynamoDB**: Fully managed NoSQL database for fast performance.
- **Aurora**: High-performance managed database compatible with MySQL/PostgreSQL.
- **Redshift**: Data warehouse solution for big data analytics.

**Networking:**
- **VPC**: Custom virtual cloud networks within AWS.
- **Route 53**: Scalable DNS and domain registration service.
- **Direct Connect**: Dedicated network connection between on-prem and AWS.
- **CloudFront**: Content delivery network (CDN) for fast distribution of content.

**Security and Identity:**
- **IAM**: Identity and Access Management for secure access control.
- **Shield**: Managed DDoS protection for AWS applications.
- **Cognito**: User authentication and identity service for web and mobile apps.
- **KMS**: Key management service for creating and controlling encryption keys.

## Cloud Computing Benefits
- Faster time to market
- Cost savings
- Better collaboration
- Advanced security
- Data loss prevention
- Scalability and flexibility

## Cloud Computing Disadvantages
- Risk of vendor lock-in
- Less control over infrastructure
- Security concerns
- Integration complexity
- Unforeseen costs

# AWS Services

## Amazon S3 (Simple Storage Service)
- Object storage with 99.999999999% durability.
- Infinitely scalable storage.
- Global service with region-specific buckets.
- Security features: IAM policies, bucket policies, ACLs.
- Storage classes: Standard, IA, One Zone-IA, Glacier, Intelligent-Tiering.

## EC2 (Elastic Compute Cloud)
- Popular AWS offering for virtual machines.
- Infrastructure as code.
- Uses EBS and instance store for data.
- Types: General, CPU, RAM, Compute, Memory, Accelerated, Storage.

## ELB (Elastic Load Balancer)
- Horizontal scaling implementation.
- Types: Classic, Application (Layer 7), Network (Layer 4).

## IAM (Identity and Access Management)
- Manages access to AWS services.

## Other AWS Services
- Lambda, CloudWatch, RDS, Route 53, etc.

# Cloud Models

## Public Cloud
- Offered by third-party providers.
- Available over the public internet.
- Scales quickly and conveniently.

## Private Cloud
- Offered to select users over the internet or a private network.
- Greater security controls.
- Requires traditional datacenter staffing.

## Key Differences

| Feature                     | Public Cloud                                     | Private Cloud                                       |
|-----------------------------|--------------------------------------------------|-----------------------------------------------------|
| **Accessibility**            | Open to anyone over the public internet.         | Restricted to select users over a private network.   |
| **Security Controls**        | Relies on the provider's security measures.      | Allows for greater control and customization.        |
| **Data Sensitivity**         | Suitable for information not very sensitive.     | Suitable for highly sensitive information.           |
| **Costs**                    | Generally cheaper than private clouds.           | Can be costlier due to dedicated infrastructure.     |
| **Infrastructure Sharing**   | Utilizes shared infrastructure.                  | Doesn't utilize shared infrastructure.               |
| **Customer Support**         | Supports multiple customers.                    | Supports only one dedicated customer.                |
| **Security Level**           | Requires a higher level of security.             | Requires a medium level of security.                 |
| **Logical Segregation**      | May use VLANs, access lists, VRF lite, MPLS, etc.| Doesn't have to be too sensitive on logical segregation.|
| **Server Hosting**           | Utilizes shared servers.                         | Uses dedicated servers.                              |
| **Proactive Monitoring**     | No dedicated proactive monitoring.               | Has dedicated proactive monitoring.                  |
| **Cost Structure**           | Generally a fixed cost.                          | Variable total cost of ownership (TCO).              |
| **Architecture**             | Multitenant architecture.                        | Dedicated customer architecture.                     |

## Hybrid Cloud
- Combination of public and private clouds.
- Shared security responsibility.

# AWS GovCloud (US) and China Regions

### 1. AWS GovCloud (US):
- Designed for U.S. government agencies and customers with strict regulatory and compliance requirements.
- Isolated cloud regions that comply with ITAR, FedRAMP, and other security and compliance standards.
- Located in two regions: **AWS GovCloud (US-West)** and **AWS GovCloud (US-East)**.
- Ensures data sovereignty; data stored in GovCloud remains within the United States.

### 2. AWS China Regions:
- AWS services provided by local partners: **Ningxia** and **Beijing**.
- Isolated from other AWS global regions.
- Requires separate accounts and follows Chinese regulatory requirements.

# Serverless

## Compute Service
- **Fargate**: Serverless compute engine for containers.
- **Lambda**: Serverless computing service.

## Database
- **Aurora Serverless**: On-demand, autoscaling configuration for Amazon Aurora.

## Storage
- **EFS** (Elastic File System): Shared file system without pre-defined size increase.

## Block Storage
- **Object Storage**
- **RAID** (Redundant Array of Independent Disks)
- **SAN** (Storage Area Network)

# Networking in AWS

### Amazon Virtual Private Cloud (VPC)
- Create a virtual network with custom IP ranges, subnets, and route tables.

### Elastic Load Balancing (ELB)
- Distributes traffic across EC2 instances.

### AWS Direct Connect
- Dedicated connection from on-premises to AWS, bypassing the internet.

### AWS Transit Gateway
- Central hub for connecting multiple VPCs and on-prem networks.

### Amazon Route 53
- Scalable DNS service for domain registration and routing.

### Security Groups and NACLs
- **Security Groups**: Stateful firewalls for instances.
- **NACLs**: Stateless firewalls for subnets.

### AWS Global Accelerator
- Improves app performance globally with static IPs.

### VPC Peering
- Connects two VPCs for private communication.

### AWS VPN
- **Site-to-Site VPN**: Connects on-prem networks to AWS VPCs.
- **Client VPN**: Provides secure remote access to AWS resources.

## Other AWS Services
- **SQS**: Queue service.
- **CodeBuild**: Build tool.
- **CloudTrail**: Records AWS API calls.
- **CodeDeploy**: Automates code deployments.
- **CodePipelines**: Continuous delivery service.
- **CodeCommit**: Version control service.

## AWS Auto Scaling
- Adjusts resources in Auto Scaling groups to match demand.

## AWS Load Balancer
- **Horizontal Scaling**: Distributes incoming traffic across multiple targets.
- **High Availability**: Ensures fault tolerance.

### Load Balancer Types:
- **Classic Load Balancer**: Layer 4 & 7.
- **Application Load Balancer**: Layer 7, for routing based on content.
- **Network Load Balancer**: Layer 4, for handling TCP/UDP traffic.

## AWS EKS (Elastic Kubernetes Service)
- Managed Kubernetes service.
- Automates cluster provisioning and maintenance.
- Integrated with other AWS services.

## AWS ECS (Elastic Container Service)
- Container orchestration for managing Docker containers.
- Integrates with services like ELB, ECR, and IAM.

# AWS Secret Management

### AWS Systems Manager Parameter Store
- Stores configuration data and secrets.

### AWS Secrets Manager
- Manages sensitive data with KMS encryption.
- Offers automatic secret rotation.

### HashiCorp Vault
- Manages secrets dynamically with lease-based access control.
