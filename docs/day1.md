# Cloud Computing Fundamentals

## Table of Contents

- Cloud Computing
- Five Essential Characteristics
- Cloud Deployment Models
- Cloud Service Models
- Shared Responsibility Model
- Four Pillars of Customer Responsibility
- Best Practices
- Interview Question

---

# Cloud Computing

Cloud computing provides on-demand access to computing resources over the internet. According to NIST, cloud computing consists of:

- **5 Essential Characteristics**
- **4 Deployment Models**
- **3 Primary Service Models** (plus Serverless/FaaS)

---

# 1. Five Essential Characteristics

## 1. On-Demand Self-Service

Users can provision and deprovision computing resources without human interaction from the cloud provider.

### Example
Creating a Virtual Machine or Database instantly through the cloud console.

### Analogy
Instead of calling an electrician every time you need a new light fixture, you simply flip a switch.

### Benefits

- Fast provisioning
- Automation
- Reduced operational delays

---

## 2. Broad Network Access

Cloud services are available over the internet and can be accessed from:

- Laptop
- Mobile
- Tablet
- Desktop

### Analogy

Accessing your bank account from anywhere using your phone.

### Benefits

- Accessibility
- Work from anywhere
- Device independence

---

## 3. Resource Pooling

Cloud providers pool physical resources to serve multiple customers (multi-tenancy).

Customers don't know the exact physical location of their resources.

### Analogy

Living in an apartment building where utilities are shared efficiently.

### Benefits

- Better utilization
- Cost efficiency
- Economies of scale

---

## 4. Rapid Elasticity

Resources automatically scale up or down based on demand.

### Example

An e-commerce website automatically adding servers during Black Friday sales.

### Analogy

An airport escalator handling crowds during rush hour.

### Benefits

- Scalability
- Flexibility
- Pay only for resources used

---

## 5. Measured Service

Customers pay only for consumed resources.

Examples include:

- Compute hours
- Storage used
- Network bandwidth

### Analogy

Electricity bill based on actual usage.

### Benefits

- Cost optimization
- Usage monitoring
- Predictable billing

---

# 2. Cloud Deployment Models

## Public Cloud

Infrastructure is owned and managed by a third-party provider.

Examples

- AWS
- Microsoft Azure
- Google Cloud Platform

### Characteristics

- Multi-tenant
- Internet accessible
- Highly scalable
- Cost effective

### Best For

- Websites
- Startups
- Development environments

---

## Private Cloud

Infrastructure dedicated to a single organization.

### Characteristics

- Maximum security
- Full control
- Higher cost

### Best For

- Banking
- Healthcare
- Government

---

## Hybrid Cloud

Combination of Public Cloud and Private Cloud.

### Characteristics

- Sensitive workloads remain private
- Burst workloads move to public cloud

### Best For

Large enterprises requiring both security and scalability.

---

## Community Cloud

Shared cloud infrastructure among organizations with similar requirements.

### Examples

- Universities
- Government agencies
- Healthcare organizations

### Benefits

- Shared governance
- Lower cost than private cloud
- Industry-specific compliance

---

# 3. Cloud Service Models

## Infrastructure as a Service (IaaS)

The provider manages infrastructure while the customer manages everything above the operating system.

### Provider Manages

- Physical servers
- Storage
- Networking
- Virtualization

### Customer Manages

- Operating System
- Middleware
- Applications
- Data
- Security

### Examples

- Amazon EC2
- Azure Virtual Machines
- Google Compute Engine

### Analogy

Renting an empty workshop.

---

## Platform as a Service (PaaS)

The provider manages the platform while the customer focuses on application development.

### Provider Manages

- Infrastructure
- Operating System
- Runtime
- Middleware

### Customer Manages

- Application
- Data

### Examples

- AWS Elastic Beanstalk
- Azure App Service
- Google App Engine

### Analogy

Renting a fully equipped commercial kitchen.

---

## Software as a Service (SaaS)

Complete software managed by the provider.

### Customer Only Manages

- User accounts
- Configuration
- Data usage

### Examples

- Gmail
- Microsoft 365
- Salesforce

### Analogy

Staying in a hotel.

---

## Function as a Service (FaaS)

A serverless model where code executes only when triggered by an event.

### Event Examples

- HTTP request
- File upload
- Queue message
- Database event

### Advantages

- No server management
- Automatic scaling
- Pay per execution
- Lower operational overhead

### Examples

- AWS Lambda
- Azure Functions
- Google Cloud Functions

---

# Service Responsibility Comparison

| Responsibility | IaaS | PaaS | SaaS |
|---------------|------|------|------|
| Physical Security | Provider | Provider | Provider |
| Networking | Provider | Provider | Provider |
| Virtualization | Provider | Provider | Provider |
| Operating System | Customer | Provider | Provider |
| Middleware | Customer | Provider | Provider |
| Runtime | Customer | Provider | Provider |
| Applications | Customer | Customer | Provider |
| Data | Customer | Customer | Provider |
| IAM | Customer | Customer | Customer |

---

# 4. Shared Responsibility Model

## Definition

The Shared Responsibility Model defines which security responsibilities belong to the cloud provider and which belong to the customer.

**Provider = Security OF the Cloud**

**Customer = Security IN the Cloud**

---

## Cloud Provider Responsibilities

The provider manages:

- Physical data centers
- Hardware
- Storage infrastructure
- Networking
- Hypervisor
- Global availability
- Managed cloud services

---

## Customer Responsibilities

The customer manages:

- IAM
- Data
- Encryption
- Firewalls
- Network configuration
- Monitoring
- Logging
- Compliance
- Application security

---

# Four Pillars of Customer Responsibility

## 1. Data Protection

Responsible for:

- Encrypting sensitive data
- Managing encryption keys
- Data classification
- Data backup

### Best Practice

Encrypt sensitive data before storing it in cloud services.

---

## 2. Identity & Access Management (IAM)

Responsible for:

- Users
- Groups
- Roles
- Policies
- MFA
- Least Privilege

### Principle of Least Privilege

Users should receive only the permissions they actually need.

---

## 3. Network Security

Responsible for configuring:

- VPC
- Security Groups
- Network ACLs
- Routing
- Firewalls

### Example

Security Groups control access to EC2 instances.

---

## 4. Monitoring & Auditing

Use cloud-native tools such as:

- AWS CloudTrail
- Amazon CloudWatch

Responsibilities include:

- Enable logging
- Monitor events
- Create alerts
- Investigate suspicious activities

---

# Best Practices

## Assume Breach

Design systems assuming attackers may gain access.

Implement:

- Defense in Depth
- Zero Trust
- Strong IAM
- Encryption

---

## Infrastructure as Code (IaC)

Provision infrastructure using code instead of manually creating resources.

Examples

- Terraform
- AWS CloudFormation

Benefits

- Repeatability
- Version control
- Auditing
- Reduced human error

---

## Golden Rule

Whenever something fails, ask:

- Did I configure IAM correctly?
- Is encryption enabled?
- Are network rules correct?
- Are logs enabled?
- Did I follow least privilege?

---

# Interview Question

## Which controls remain your responsibility when using managed cloud services?

Even when using managed services, customers remain responsible for:

- Identity and Access Management (IAM)
- User authentication
- Encryption and key management
- Data protection
- Network configuration
- Security Groups
- Firewalls
- Monitoring and logging
- Compliance
- Application security
- Backup and recovery (where applicable)

**Memory Tip**

> **Provider secures the Cloud. Customer secures everything IN the Cloud.**

---

# Key Takeaways

- Cloud computing has **5 Essential Characteristics**.
- Cloud deployment includes **Public, Private, Hybrid, and Community** models.
- Service models include **IaaS, PaaS, SaaS, and FaaS**.
- Security follows the **Shared Responsibility Model**.
- Customers are always responsible for **IAM, data, encryption, monitoring, and configuration**.
