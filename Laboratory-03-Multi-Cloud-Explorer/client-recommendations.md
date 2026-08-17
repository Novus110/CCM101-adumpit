# Client Recommendations

## Client A – Startup Company

**Recommended Platform:** Amazon Web Services (AWS)

**Explanation:** AWS is the best fit for a budget-conscious startup expecting rapid growth, since it offers a generous free tier and pay-as-you-go pricing that scales smoothly as usage increases. Its huge service catalog means the startup won't need to migrate providers later as their needs grow more complex, whether that's adding databases, analytics, or machine learning. AWS also has the largest developer community and documentation base, which reduces the learning curve and troubleshooting time for a small technical team. Elastic, serverless options let the startup avoid paying for idle infrastructure during its early, unpredictable growth phase.

**Services to use:**
- **AWS Lambda** – serverless compute so they only pay for what they use, ideal for an app with unpredictable traffic
- **Amazon S3** – low-cost, scalable storage for app assets and user data
- **Amazon RDS** – managed database that removes the overhead of self-managing infrastructure

## Client B – University

**Recommended Platform:** Microsoft Azure

**Explanation:** Since the university already runs Windows Server, Microsoft 365, and Active Directory, Azure offers the most seamless migration path with minimal retraining or reconfiguration. Azure Hybrid Benefit lets the university apply its existing Windows Server and SQL Server licenses directly to cloud resources, lowering migration costs. Azure Arc and Azure Stack also support a gradual, hybrid rollout, so the university can move services to the cloud incrementally rather than all at once. This reduces risk for an institution that likely needs to keep some systems on-premises during the transition.

**Services to use:**
- **Microsoft Entra ID** – extends their existing Active Directory identity management into the cloud
- **Azure Virtual Machines** – lets them lift-and-shift existing Windows Server workloads
- **Azure SQL Database** – managed version of the SQL Server databases they already use

## Client C – AI Research Company

**Recommended Platform:** Google Cloud Platform (GCP)

**Explanation:** GCP is the strongest choice for a company building AI and machine learning applications, since it offers purpose-built infrastructure like custom Tensor Processing Units (TPUs) alongside GPUs for high-performance model training. Vertex AI provides an end-to-end ML platform for building, training, and deploying models, backed by Google's own research in AI. BigQuery also gives the company a fast, serverless way to analyze the large datasets typically needed to train ML models. Google's high-performance private global network further reduces latency for large-scale distributed training jobs.

**Services to use:**
- **Vertex AI** – unified platform for training and deploying machine learning models
- **Google Compute Engine (with GPU/TPU support)** – high-performance computing for training workloads
- **BigQuery** – fast, large-scale data analytics to prepare and explore training datasets

## Client D – Global E-Commerce Company

**Recommended Platform:** Amazon Web Services (AWS)

**Explanation:** AWS is well-suited for a global e-commerce company because of its extensive worldwide infrastructure of regions and Availability Zones, which supports low-latency access for customers everywhere. Services like Elastic Load Balancing and Auto Scaling automatically adjust capacity to handle traffic spikes, such as seasonal sales events, without manual intervention. AWS's maturity in high-availability architecture also means the company can design multi-region failover systems to keep the storefront online during outages. Its proven track record hosting large-scale retail workloads (including Amazon's own retail platform) makes it a reliable choice for mission-critical, always-on infrastructure.

**Services to use:**
- **Amazon EC2 with Auto Scaling** – automatically scales compute capacity with demand
- **Elastic Load Balancing (ELB)** – distributes traffic across servers/regions for high availability
- **Amazon CloudFront** – content delivery network for fast, low-latency access worldwide

## Multi-Cloud Decision Matrix

| Business Requirement | Recommended Platform | Justification |
|---|---|---|
| Startup Company | AWS | Generous free tier, pay-as-you-go pricing, and room to scale without switching providers |
| Enterprise Organization | AWS | Broadest service catalog and mature enterprise support/compliance certifications |
| Microsoft Environment | Azure | Native integration with Active Directory, Windows Server, and Microsoft 365 |
| AI / Machine Learning | GCP | Purpose-built AI infrastructure (TPUs, Vertex AI) and strength in data analytics |
| Kubernetes Deployment | GCP | Originator of Kubernetes; GKE is the most mature managed Kubernetes service |
| Global Web Application | AWS | Largest global infrastructure footprint with strong auto-scaling and CDN tools |
