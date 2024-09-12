# [Aws- (cloud computing)]()


Cloud Computing

## AWS Overview
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




# Public Cloud

- **Offered by third-party providers.**
- **Available over the public internet.**
- **Scales quickly and conveniently.**

# Private Cloud

- **Offered to select users over the internet or a private network.**
- **Greater security controls.**
- **Requires traditional datacenter staffing.**

## Key Differences

| Feature                     | Public Cloud                                     | Private Cloud                                       |
|-----------------------------|--------------------------------------------------|-----------------------------------------------------|
| **Accessibility**           | Open to anyone over the public internet.         | Restricted to select users over a private network.   |
| **Security Controls**       | Relies on the provider's security measures.      | Allows for greater control and customization.        |
| **Data Sensitivity**        | Suitable for information not very sensitive.     | Suitable for highly sensitive information.
| **Costs**                   | Generally cheaper than private clouds.           | Can be costlier due to dedicated infrastructure.     |
| **Infrastructure Sharing**  | Utilizes shared infrastructure.                  | Doesn't utilize shared infrastructure.               |
| **Customer Support**        | Supports multiple customers.                    | Supports only one dedicated customer.                |
| **Security Level**          | Requires a higher level of security.             | Requires a medium level of security.                 |
| **Logical Segregation**     | May use VLANs, access lists, VRF lite, MPLS, etc. | Doesn't have to be too sensitive on logical segregation.|
| **Server Hosting**          | Utilizes shared servers.                         | Uses dedicated servers.                              |
| **Proactive Monitoring**    | No dedicated proactive monitoring.               | Has dedicated proactive monitoring.  
| **Cost Structure**          | Generally a fixed cost.                          | Variable total cost of ownership (TCO).              |
| **Architecture**            | Multitenant architecture.                        | Dedicated customer architecture.                     |




## Hybrid Cloud
- Combination of public and private clouds.
- Shared security responsibility.

# AWS GovCloud (US) and China Regions

### 1. AWS GovCloud (US):
- Designed for U.S. government agencies and customers with strict regulatory and compliance requirements.
- Isolated cloud regions that comply with ITAR, FedRAMP, and other security and compliance standards.
- Located in two regions: **AWS GovCloud (US-West)** and **AWS GovCloud (US-East)**.
- Services offered are identical to the standard AWS regions but with additional compliance measures.
- Ensures data sovereignty; data stored in GovCloud remains within the United States.
- Requires account access authorization through special vetting and approval processes.

### 2. AWS China Regions:
- AWS services are provided by local partners: **Ningxia** (operated by NWCD) and **Beijing** (operated by Sinnet).
- These regions are isolated from other AWS global regions and require separate accounts.
- Follow Chinese regulatory and legal requirements, ensuring data localization within China.
- AWS Global infrastructure services like IAM, EC2, and S3 are available but subject to regional restrictions.
- Accessing services in China requires a dedicated China-region account, separate from global AWS accounts.
- Designed to meet the unique compliance needs of companies operating within China.




# Serverless

## Compute Service
- Fargate: Serverless compute engine for containers.
- Lambda: Serverless computing service.

## Database
- Aurora Serverless: On-demand, autoscaling configuration for Amazon Aurora.

## Storage
- EFS (Elastic File System): Shared file system without pre-defined size increase.
- DRBD: Distributed Replicated Block Device.

## Block Storage
- Object Storage
- RAID (Redundant Array of Independent Disks)
- SAN (Storage Area Network)

# Networking in AWS

**Amazon Virtual Private Cloud (VPC):**
- Create a virtual network with custom IP ranges, subnets, and route tables.
- Supports both public/private subnets and IPv4/IPv6.

**Elastic Load Balancing (ELB):**
- Distributes traffic across EC2 instances.
- Types: **ALB** (HTTP/HTTPS), **NLB** (TCP), **Gateway Load Balancer**.
- Routes traffic to healthy instances, improving fault tolerance.

**AWS Direct Connect:**
- Dedicated connection from on-premises to AWS, bypassing the internet.
- Provides secure, low-latency, and consistent performance.

**AWS Transit Gateway:**
- Central hub for connecting multiple VPCs and on-prem networks.
- Simplifies network management with scalable connections.

**Amazon Route 53:**
- Scalable DNS service for domain registration and routing.
- Supports simple, weighted, and latency-based routing for optimal performance.

**Security Groups and NACLs:**
- **Security Groups**: Stateful firewalls for instances to control traffic.
- **NACLs**: Stateless firewalls for subnets, with separate inbound/outbound rules.

**AWS Global Accelerator:**
- Improves app performance globally with static IPs.
- Routes traffic to optimal AWS regions and handles failover.

**VPC Peering:**
- Connects two VPCs for private communication using IP addresses.
- Supports inter-region and cross-account peering.

**AWS VPN:**
- **Site-to-Site VPN**: Connects on-prem networks to AWS VPCs.
- **Client VPN**: Provides secure remote access to AWS resources.



## AWS Services
- SQS (Simple Queue Service): Queue service.
- CodeBuild: Build tool, compiler.
- CloudTrail: Records AWS API calls.
- CodeDeploy: Automates code deployments.
- CodePipelines: Continuous delivery service.
- CodeCommit: Version control service.
- CodePipeline + CodeCommit: Service control system (SCS).
- Amazon Polly: Text-to-speech service.
- Amazon Lex: Conversational interfaces
 AWS Comprehend: Natural language processing.
- SNS (Simple Notification Service): Publish-subscribe messaging.
- Braket: Quantum computing service.
- RabbitMQ: Message broker with a pub-sub model.

## Auto Scalling

- AWS Auto Scaling adjusts resources in your Auto Scaling group to match desired capacity, ensuring:

## load balancer

**AWS Load Balancer
AWS Load Balancer is a service that provides:**

- **Horizontal Scaling:** Distributes incoming application traffic across multiple targets for better availability.
- **High Availability:** Ensures fault tolerance and availability of applications.
- **Types:**
  - **Classic Load Balancer:** Layer 4 & 7, the original load balancer.
  - **Application Load Balancer:** Layer 7, for routing based on content.
  - **Network Load Balancer:** Layer 4, handles TCP/UDP traffic.
- **Implementation of Horizontal Scaling:** Facilitates scaling applications horizontally for increased capacity.
- **Required for High Availability:** Essential for maintaining high availability of applications.


- **Availability:** Maintains application availability.
- **Dynamic Scaling:** Scales Amazon EC2 capacity based on demand.
- **Optimization:** Automatically adjusts resources for efficient performance.
- **Management:** Simplifies resource scaling and management.

## Eks service on Aws

AWS EKS (Elastic Kubernetes Service)

AWS EKS provides:

- **Managed Kubernetes:** Fully managed Kubernetes service.
- **Easy Deployment:** Simplifies the deployment, management, and scaling of containerized applications using Kubernetes.
- **Benefits:**
  - Automates Kubernetes cluster provisioning and maintenance.
  - Integrated with AWS services and features.
  - Supports popular Kubernetes tools and applications.
- **Worker Nodes:** Managed EC2 instances running in your account.
- **Control Plane:** Managed by AWS, reducing operational overhead.
  

# AWS ECS (Elastic Container Service)

AWS ECS is a service that provides:

- **Container Orchestration:** Manages the deployment and scaling of containerized applications.
- **Compatibility:** Works with Docker containers.
- **Key Features:**
  - **Task Definitions:** Defines containers to be launched together.
  - **Clusters:** Logical grouping of container instances.
  - **Services:** Defines how tasks are deployed and maintained.
- **Integration:** Integrates with other AWS services like ELB, ECR, IAM, etc.
- **Managed Service:** Removes the need for you to install, operate, and scale your own cluster management infrastructure.

# AWS Secret Management

AWS provides services to securely manage sensitive information like passwords, API keys, and database credentials:

- **AWS Systems Manager Parameter Store:** 
  - **Stores:** Configuration data and secrets (plaintext or encrypted).
  - **Access:** IAM integration for permissions.
  - **Features:** Versioning, hierarchical storage.

- **AWS Secrets Manager:** 
  - **Stores:** Sensitive data with KMS encryption.
  - **Rotation:** Automatic secret rotation for supported services.
  - **Access:** Fine-grained control via IAM.
  - **Audit:** CloudTrail for secret access tracking.

- **HashiCorp Vault:** 
  - **Dynamic Secrets:** Generates temporary credentials on demand.
  - **Revocation:** Lease-based secret management.
  - **Access:** Policy-driven access control.
  - **Support:** Works with multiple backends, not limited to AWS.

