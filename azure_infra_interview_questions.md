# Azure Infrastructure Engineer – Interview Questions and Answers (8–9 Years Experience)

## Section 1: Azure Infrastructure & Automation

### Q1. How do you manage and automate Azure infrastructure deployments?
**Answer:**
I primarily use **Terraform** or **ARM/Bicep templates** combined with **PowerShell** or **Azure CLI** scripts for infrastructure automation. I integrate these with **CI/CD pipelines in Jenkins** or **GitHub Actions**. I ensure state management with remote backends and use **modular design** for reusability. I also leverage **Azure DevOps Pipelines** when needed for enterprise projects.

### Q2. Explain how you use PowerShell and MS Graph API in managing Azure resources.
**Answer:**
I use **PowerShell with the MS Graph API** to manage **Entra ID (Azure AD)**, **Intune policies**, **users**, **groups**, and **device compliance policies**. For example, I automate user provisioning, policy assignment, and license management. I use `Invoke-RestMethod` to call Graph endpoints and wrap them in reusable functions/modules.

### Q3. How do you use Intune in device lifecycle management?
**Answer:**
I configure **compliance policies**, **configuration profiles**, **application deployments**, and **conditional access policies** through **Intune**. Using **PowerShell scripts** and **Graph API**, I automate bulk onboarding of devices, policy assignment, and health monitoring of enrolled endpoints.

---

## Section 2: CI/CD & DevOps

### Q4. Describe a CI/CD pipeline you built using Jenkins for a cloud-based application.
**Answer:**
In one project, I built a Jenkins pipeline to automate the deployment of a .NET Core application to Azure App Service. It included:
- Source code checkout from GitHub.
- Code quality checks using SonarQube.
- Artifact build and storage in Azure Artifacts.
- ARM/Bicep deployment for infrastructure.
- Application deployment using Azure CLI.
- Post-deployment health checks and Slack notifications.

### Q5. How do you integrate Ansible in your automation workflows?
**Answer:**
I use Ansible for provisioning and configuration of VMs (both Linux and Windows). For example, installing software on Azure VMs after deployment or managing on-prem hybrid environments. I run Ansible via Jenkins jobs, and sometimes wrap it in a PowerShell or Python interface.

### Q6. What branching strategy and Git practices do you follow?
**Answer:**
I follow **GitFlow** or **Trunk-based development** based on team size and project nature. I ensure:
- Clear naming conventions.
- Code reviews via pull requests.
- Branch protection rules on `main`/`release`.
- Tags/releases for versioning.
- GitHub Actions/Jenkins triggers on push/merge.

---

## Section 3: Power Platform & Automation

### Q7. How have you used PowerApps and Power Automate in process automation?
**Answer:**
I built a PowerApp for internal application access request automation, integrated with **Power Automate** to call **Graph API** and **ServiceNow APIs** to:
- Create approval tasks.
- Update access logs in SharePoint/Dataverse.
- Notify via Teams.
I also used **custom connectors** to integrate with external APIs like JIRA.

### Q8. Explain how you would integrate OpenAI in a business process workflow.
**Answer:**
I would use **Power Automate** to call the **OpenAI API** using an HTTP connector to:
- Summarize tickets or emails.
- Generate response templates.
- Translate or classify support requests.
In a real-world use case, I created a ChatGPT-based assistant inside a PowerApp to provide IT helpdesk suggestions by querying a knowledge base.

### Q9. Have you integrated Digital.ai Release or ServiceNow with your automation stack?
**Answer:**
Yes. I used PowerShell and Python to integrate **Digital.ai Release pipelines** with **ServiceNow Change Management**, ensuring:
- Change request creation before deployment.
- Status updates back to SNOW post-deployment.
- Audit compliance using event logs pushed to centralized dashboards (Power BI/Log Analytics).

---

## Section 4: Soft Skills, Agile, and Collaboration

### Q10. How do you manage sprint planning and requirement breakdown in Agile?
**Answer:**
I collaborate with product owners to break down requirements into **user stories** and **tasks**, estimating with **story points**. I use tools like **JIRA** and follow **Scrum ceremonies** (stand-ups, planning, reviews). I help the team identify dependencies, risks, and ensure regular feedback cycles.

### Q11. How do you mentor or cross-train team members on Azure and automation topics?
**Answer:**
I prepare documentation on **Confluence**, create internal **demo sessions**, and conduct **hands-on workshops** on:
- Azure concepts (RBAC, ARM, VNets).
- Jenkins pipelines.
- Intune/Graph API scripting.
I also build labs for team hands-on practice and track skill progress via assessments.

---

## Section 5: Scenario-Based / Leadership

### Q12. You’re asked to automate a manual approval-heavy deployment process across teams. How would you approach it?
**Answer:**
- **Step 1**: Understand existing manual steps and approvals.
- **Step 2**: Design workflow in Power Automate integrated with approval gates.
- **Step 3**: Integrate GitHub/Jenkins with ServiceNow for change control.
- **Step 4**: Add audit logging using Application Insights / Log Analytics.
- **Step 5**: Train users and roll out in phases.
Always ensuring rollback plans and compliance alignment.

### Q13. How do you ensure security and compliance in your automation scripts and pipelines?
**Answer:**
- Secure secrets using **Azure Key Vault** or **Jenkins Credentials plugin**.
- RBAC and least privilege access on Azure resources.
- Code scanning tools (Dependabot, SonarQube, Checkov).
- Pipeline audit logging.
- Periodic script reviews and compliance with coding standards.

---

## Section 6: Quick Technicals

| Area                  | Quick Check                                                  |
|-----------------------|--------------------------------------------------------------|
| **PowerShell Cmdlets**| `Get-AzVM`, `New-AzResourceGroupDeployment`, `Invoke-RestMethod` |
| **Graph API Endpoint**| `https://graph.microsoft.com/v1.0/users`                      |
| **Azure CLI Example** | `az group create --name dev-rg --location eastus`            |
| **Jenkinsfile**       | Declarative or scripted pipelines using `pipeline {}` syntax  |
| **Git Command**       | `git rebase`, `git cherry-pick`, `git tag -a v1.0`           |
| **Intune Automation** | Device enrollment, profile deployment via Graph API          |

---

*Prepared for the role of Azure Infrastructure Engineer at Allianz Group – Pune.*

