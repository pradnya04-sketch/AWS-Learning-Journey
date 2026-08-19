# Cloud Concepts ☁️

This section documents the cloud concepts I learned while preparing for the **AWS Certified Cloud Practitioner (CLF-C02)** certification.

My approach is to understand the concepts first and then apply them through AWS hands-on practice.

---

## 1. How Does a Website Work?

A basic website communication can be understood as:

**Client → Network → Server**

- **Client:** The device used by the user, such as a computer or mobile phone. It has an IP address.
- **Network:** Connects the client to the server and allows data to travel between them.
- **Server:** Receives requests from the client and provides the required response.

For example, when sending an email or accessing a website, the client sends a request through the network to a server.

### What is inside a Server?

A server can be understood through its major components:

- **Compute:** CPU used for processing
- **Memory:** RAM used for temporary data and processing
- **Storage:** Used to store data
- **Database:** Used to store data in a structured way
- **Networking:** Routers, switches, DNS servers and other networking components

### Basic Network Components

**Network:**  
A collection of connected devices that can communicate and share data.

**Router:**  
A networking device that forwards data packets between networks and determines where the packets should be sent.

**Switch:**  
A networking device that forwards data to the appropriate device within a network.

---

## 2. What is Cloud Computing?

Cloud computing is the **on-demand delivery of computing resources** such as:

- Computing power
- Database storage
- Applications
- Other IT resources

through cloud services.

Instead of owning and maintaining all the required hardware ourselves, we can use resources provided by a cloud service provider.

Examples of cloud providers include:

- AWS
- Google Cloud
- Microsoft Azure

The cloud provider owns and maintains the underlying infrastructure while customers provision and use the resources they need.

---

## 3. Five Characteristics of Cloud Computing

### 1. On-Demand Self-Service

Users can provision computing resources when they need them without requiring human interaction from the service provider.

### 2. Broad Network Access

Cloud resources and services can be accessed over networks using different types of devices and platforms.

### 3. Resource Pooling

The provider pools computing resources and serves multiple customers using shared infrastructure.

### 4. Rapid Elasticity

Resources can be quickly increased or decreased based on demand.

### 5. Measured Service

Cloud usage is measured, allowing customers to pay based on the resources they consume.

---

## 4. Advantages of Cloud Computing

The major advantages I learned are:

### 1. Trade Capital Expense (CAPEX) for Operational Expense (OPEX)

Instead of making large upfront investments in physical infrastructure, cloud users can pay for resources as they use them.

### 2. Benefit from Massive Economies of Scale

Cloud providers operate infrastructure at a very large scale, allowing them to achieve cost efficiencies.

### 3. Stop Guessing Capacity

Resources can be provisioned based on actual requirements instead of estimating future capacity.

### 4. Increase Speed and Agility

Cloud resources can be provisioned quickly, allowing organizations to experiment and deploy faster.

### 5. Stop Spending Money Running and Maintaining Data Centers

Organizations can reduce the need to maintain their own physical data center infrastructure.

### 6. Go Global in Minutes

Cloud infrastructure allows applications and resources to be deployed in different geographical locations more easily.

---

## 5. Problems Solved by Cloud Computing

Cloud computing helps address problems such as:

- Flexibility
- Cost-effectiveness
- Scalability
- Elasticity
- High availability and fault tolerance
- Agility

---

# 6. Cloud Service Models

Cloud services can be broadly categorized into:

## IaaS — Infrastructure as a Service

IaaS provides the basic building blocks of cloud IT infrastructure.

It can provide resources such as:

- Computing
- Data storage
- Networking

The customer has more control over the infrastructure and is responsible for managing more components.

**Examples:**

- Amazon EC2
- Microsoft Azure Virtual Machines
- Google Compute Engine

---

## PaaS — Platform as a Service

PaaS removes the need for customers to manage the underlying infrastructure.

The customer can focus more on developing and managing applications.

**Examples:**

- AWS Elastic Beanstalk
- Heroku
- Google App Engine
- Microsoft Azure services

---

## SaaS — Software as a Service

SaaS provides a completed software product that is managed and operated by the service provider.

The customer mainly uses the application instead of managing the underlying infrastructure.

**Examples:**

- Dropbox
- Zoom
- Google Apps

---

## IaaS vs PaaS vs SaaS

The main difference is **how much of the technology stack is managed by the customer versus the cloud provider.**

| Component | On-Premises | IaaS | PaaS | SaaS |
|---|---|---|---|---|
| Application | Customer | Customer | Customer | Provider |
| Data | Customer | Customer | Customer | Provider |
| Runtime | Customer | Customer | Provider | Provider |
| Middleware | Customer | Customer | Provider | Provider |
| OS | Customer | Customer | Provider | Provider |
| Virtualization | Customer | Provider | Provider | Provider |
| Servers | Customer | Provider | Provider | Provider |
| Storage | Customer | Provider | Provider | Provider |
| Networking | Customer | Provider | Provider | Provider |

The main idea is:

**On-premises → maximum responsibility for the customer**

**SaaS → maximum management by the provider**

---

# 7. Cloud Deployment Models

## Private Cloud

A private cloud is used by a single organization.

### Advantages

- Greater control over the cloud environment
- Can be suitable for sensitive applications
- Can meet specific business requirements

### Disadvantages

- Can be expensive to maintain
- Requires management of the infrastructure

---

## Public Cloud

Cloud resources are owned and operated by a third-party cloud service provider.

Examples include:

- AWS
- Microsoft Azure
- Google Cloud

Multiple customers use resources provided by the cloud provider.

### Main idea

Customers share the provider's underlying infrastructure while their resources and data remain logically separated.

---

## Hybrid Cloud

Hybrid cloud combines private infrastructure with public cloud resources.

For example, an organization can keep sensitive systems on its private infrastructure while using public cloud services for additional capacity.

### Main benefits

- Control over sensitive assets
- Flexibility
- Ability to use public cloud scalability and cost benefits

---

# 8. AWS Pricing Fundamentals

AWS follows a **pay-as-you-go** approach for many services.

Instead of paying a large upfront amount for physical infrastructure, customers generally pay for the resources they use.

Examples from my notes include:

- Compute → pay for computing time
- Storage → pay for stored data
- Data transfer → charges can apply when data is transferred out of the cloud

The key idea is:

**Use resources → measure usage → pay according to usage**

---

# 9. AWS Cloud History

Some important milestones in AWS history that I learned:

- **2002:** AWS launched internally
- **2003:** Amazon identified infrastructure as one of its core strengths
- **2004:** AWS launched publicly with SQS
- **2006:** AWS launched publicly with S3, S3 and EC2 services
- **2007:** AWS launched in Europe

---

# 10. AWS Cloud Use Cases

AWS can be used to build sophisticated and scalable applications.

Examples include:

- Enterprise applications
- Backup and storage
- Big data analytics
- Websites
- Mobile and social applications
- Gaming

---

# 11. AWS Global Infrastructure

AWS has a global infrastructure designed to provide reliable and scalable cloud services.

The main components covered in my learning are:

1. AWS Regions
2. Availability Zones
3. Edge Locations / Points of Presence

---

## AWS Region

An AWS Region is a geographical area containing multiple data centers.

Regions are located around the world.

### Factors for choosing a Region

When choosing an AWS Region, factors include:

1. **Compliance**
2. **Proximity to customers**
3. **Available services**
4. **Pricing**

A region can also help with requirements such as lower latency and disaster recovery.

---

## Availability Zone (AZ)

An Availability Zone is one or more physically separate data centers within an AWS Region.

Availability Zones are designed to be isolated from failures in other Availability Zones while being connected through AWS networking.

Using multiple Availability Zones can improve:

- Availability
- Fault tolerance
- Resilience

---

## Edge Locations / Points of Presence

Edge locations are distributed locations used to deliver content closer to users.

They help reduce latency by bringing content closer to the users requesting it.

AWS has a large number of Points of Presence distributed across many geographical locations.

---

# 12. Global Services vs Regional Services

## Global Services

Global services are not restricted to a single AWS Region.

Examples from my notes include:

- IAM
- Route 53
- CloudFront
- WAF

These services can provide functionality across AWS Regions.

---

## Regional Services

Regional services are associated with a specific AWS Region.

Examples include:

- EC2
- Elastic Beanstalk
- Lambda
- Rekognition

For example, when launching an EC2 instance, a specific AWS Region is selected.

---

# 13. Shared Responsibility Model

AWS follows a **Shared Responsibility Model**.

The responsibilities are divided between:

**AWS and the Customer**

### AWS Responsibility

AWS is responsible for the **security of the cloud**.

This includes the underlying infrastructure such as:

- Physical data centers
- Physical servers
- Networking infrastructure
- Physical security

### Customer Responsibility

The customer is responsible for **security in the cloud**.

Depending on the service being used, this can include:

- Customer data
- Applications
- Identity and access management
- Operating systems
- Network and firewall configuration
- Encryption
- Data protection

The exact responsibility of the customer depends on the AWS service being used.

### Simple way to remember

**AWS → Security OF the cloud**

**Customer → Security IN the cloud**

---

# 14. AWS Acceptable Use Policy

AWS has an Acceptable Use Policy that defines prohibited uses of AWS services.

Important points from my notes include:

- No illegal, harmful or offensive use or content
- No security violations
- No network abuse
- No email or other messaging abuse

---

# 📌 Key CLF-C02 Takeaways

The most important concepts I want to remember from this topic are:

- Cloud computing provides IT resources on demand.
- Cloud uses a pay-as-you-go model.
- Cloud helps reduce the need for large upfront infrastructure investments.
- Scalability means increasing or decreasing resources according to requirements.
- Elasticity focuses on automatically adapting resources to changing demand.
- IaaS provides infrastructure.
- PaaS provides a platform for application development.
- SaaS provides a complete software product.
- Public, private and hybrid are different cloud deployment models.
- An AWS Region is a geographical area containing multiple Availability Zones.
- Availability Zones provide isolated infrastructure within a Region.
- Edge locations help deliver content closer to users.
- Some AWS services are global while others are regional.
- AWS and the customer share security responsibilities.
- AWS is responsible for security **of** the cloud.
- The customer is responsible for security **in** the cloud.
