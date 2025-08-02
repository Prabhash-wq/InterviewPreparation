# Azure Interview Questions and Answers for 8+ Years Experienced Candidates

[...previous content retained...]

## Azure Networking - Part 2

### Q55. What is Azure DNS?
**Answer:** Azure DNS allows you to host your DNS domain in Azure and manage DNS records using the same credentials, APIs, and tools as your other Azure services. 
**Use case:** You can manage custom domain names for your web apps, VMs, and other Azure services from within Azure.

### Q56. What is a Network Security Group (NSG)?
**Answer:** NSG acts as a virtual firewall. It controls inbound and outbound traffic to network interfaces, VMs, and subnets.
**Example:** Allow port 80 inbound for web servers, deny everything else.

### Q57. What are UDRs in Azure?
**Answer:** User Defined Routes (UDRs) allow you to override Azure's default system routes to control traffic flow. 
**Use case:** Force traffic to pass through a firewall or NVA (network virtual appliance).

### Q58. What is ExpressRoute?
**Answer:** It creates a private connection between your on-premises network and Azure datacenter, bypassing the public internet. 
**Use case:** Enterprises needing low-latency, secure connectivity to Azure for production apps.

### Q59. What is a Virtual Network Gateway?
**Answer:** A VPN Gateway connects Azure VNets to on-prem networks via IPsec/IKE VPN tunnels. 
**Use case:** Extend on-premises data center to Azure over a secure tunnel.

## Identity, Security & Access

### Q60. What is Azure Active Directory (AAD)?
**Answer:** A cloud-based identity and access management service that helps employees sign in and access resources. 
**Use case:** Single sign-on (SSO) for Office 365, SaaS, and custom apps.

### Q61. Difference between AAD and on-prem AD?
**Answer:**
- **AAD:** Cloud-native, supports SSO, OAuth, SAML, OpenID Connect.
- **On-prem AD:** Kerberos-based, domain-joined computers.
**Integration:** Azure AD Connect syncs identities between on-prem and cloud.

### Q62. What is Azure RBAC?
**Answer:** Role-Based Access Control allows you to assign permissions to users, groups, and apps based on roles. 
**Example:** Assign Reader role to a user for read-only access to resources.

### Q63. What are Azure Policies?
**Answer:** Azure Policies enforce rules on resource creation and configurations to ensure compliance. 
**Example:** Prevent users from creating resources in disallowed regions.

### Q64. What is Key Vault?
**Answer:** A service to store secrets, keys, and certificates securely. Supports integration with apps and services.
**Use case:** Store database connection strings or API keys securely.

## Real-Time Analytics

### Q65. What is Azure Stream Analytics?
**Answer:** Real-time event processing engine for analyzing streaming data from devices, sensors, websites.
**Use case:** Monitor IoT telemetry data from smart devices.

### Q66. What is Azure Synapse Analytics?
**Answer:** Integrated analytics service that combines big data and data warehousing. 
**Use case:** Analyze large volumes of structured and unstructured data from a data lake.

### Q67. Azure Data Explorer vs Synapse?
**Answer:**
- **Data Explorer:** Optimized for telemetry/log analytics.
- **Synapse:** Broader capabilities, integrates with Power BI, ML.

## DevOps, CI/CD & Infrastructure as Code

### Q68. What is Azure DevOps?
**Answer:** End-to-end DevOps platform with tools for CI/CD, Boards, Repos, Pipelines, Artifacts.
**Use case:** Automate build and deployment pipeline for .NET web app.

### Q69. Difference between Azure DevOps Pipelines vs GitHub Actions?
**Answer:**
- **Azure Pipelines:** Mature integration with Azure, YAML/CD support.
- **GitHub Actions:** GitHub-native, suitable for open source and CI.

### Q70. What is Infrastructure as Code (IaC)?
**Answer:** Managing infrastructure using code instead of manual setup. Tools: Terraform, Bicep, ARM templates.
**Example:** Define and deploy a complete Azure environment via Terraform.

### Q71. Terraform vs ARM vs Bicep?
**Answer:**
- **Terraform:** Open-source, multi-cloud.
- **ARM:** Native Azure JSON templates.
- **Bicep:** Simplified syntax over ARM.

## Monitoring & Logs

### Q72. What is Azure Monitor?
**Answer:** A unified monitoring service that collects metrics, logs, and telemetry from Azure resources.
**Use case:** Monitor CPU usage of VMs, configure alerts.

### Q73. What is Log Analytics?
**Answer:** Feature of Azure Monitor to query and analyze log data using KQL (Kusto Query Language).
**Example:** Find VMs with failed login attempts.

### Q74. What is Application Insights?
**Answer:** APM (Application Performance Monitoring) for apps. Tracks performance, exceptions, requests.
**Use case:** Monitor a web app’s response time and error rate.

### Q75. How to enable alerts in Azure?
**Answer:** Via Azure Monitor using alert rules based on metrics or logs.
**Example:** Send an email if VM CPU > 80% for 5 minutes.

## Event-Driven Messaging

### Q76. What is Azure Event Grid?
**Answer:** A fully managed event routing service using publish-subscribe model.
**Use case:** Notify a function app when blob is uploaded.

### Q77. What is Azure Event Hub?
**Answer:** A big data streaming platform for ingesting large volumes of events.
**Use case:** Collect telemetry data from thousands of IoT devices.

### Q78. What is Azure Service Bus?
**Answer:** Enterprise-grade messaging service with features like queues, topics, sessions.
**Use case:** Order processing system with retry logic and dead-lettering.

### Q79. Difference between Event Hub, Event Grid, and Service Bus?
**Answer:**
- **Event Grid:** Lightweight eventing (e.g., blob created).
- **Event Hub:** High-throughput telemetry ingestion.
- **Service Bus:** Enterprise messaging with reliability, ordering.

## Azure Cognitive Services & ML

### Q80. What is Azure Cognitive Services?
**Answer:** Pre-built AI services for vision, speech, language, and decision-making.
**Use case:** OCR extraction from scanned documents.

### Q81. What is Azure ML?
**Answer:** Platform for training, deploying, and managing machine learning models.
**Use case:** Predict churn rate using customer data.

## Performance Optimization Techniques

### Q82. How to scale Azure Web App?
**Answer:** 
- **Vertical scaling:** Change pricing tier.
- **Horizontal scaling:** Add instances with auto-scaling rules.

### Q83. How to optimize Azure VM cost?
**Answer:**
- Use reserved instances.
- Right-size VM sizes.
- Use spot VMs for non-critical workloads.

### Q84. What is Azure Advisor?
**Answer:** Provides best practices recommendations to optimize cost, performance, security, and reliability.
**Use case:** Get alerts for underutilized resources.

### Q85. What is Autoscaling in Azure?
**Answer:** Automatic adjustment of resources (e.g., VMSS, App Services) based on load.
**Use case:** Add more VM instances during high traffic hours.

[...continued if needed for more questions...]

