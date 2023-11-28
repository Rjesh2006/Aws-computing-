# Aws-computing-

Cloud Computing

## AWS Overview
- Cloud computing delivers various services over the internet.
- AWS (Amazon Web Services) is a comprehensive cloud platform.

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

# AWS Gov Cloud and China Regions

Certainly! Here's the information converted into GitHub-flavored markdown code:

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

## Network
- VPC (Virtual Private Cloud)
- Direct Connect: Connect your on-premises database with AWS databases directly.

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

AWS Auto Scaling

AWS Auto Scaling adjusts resources in your Auto Scaling group to match desired capacity, ensuring:

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

