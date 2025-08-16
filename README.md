# CST8919_Assignment2
## 📌 Objective
This report outlines the Microsoft Azure services that will be investigated during this course and contrasting terms of service comparisons between them, against Amazon Web Services (AWS), and Google Cloud Platform (GCP).
---

## 🔑 Providers Compared
- Microsoft Entra ID (formerly Azure Active Directory – Single Sign On/Identity and Access Management)  
- Azure Monitors & Log Analytics  
- Azure Policy  
- Microsoft Defender for cloud  
- Microsoft Sentinel (SIEM “SOAR” )  

---
## 🗂 Quick Comparison Table

| Azure Service                  | AWS Equivalent                            | GCP Equivalent                  | Notes |
|--------------------------------|-------------------------------------------|---------------------------------|-------|
| **Microsoft Entra ID** (SSO/IAM) | AWS IAM Identity Center (SSO)             | Google Cloud Identity            | Azure in hybrid AD; AWS mult-account; GCP close with Workspace |
| **Azure Monitor & Log Analytics** | Amazon CloudWatch + CloudTrail            | Google Cloud Operations Suite    | All the three offer observability, logs, and metrics |
| **Azure Policy**               | AWS Config + Service Control Policies (SCP) | Google Organization Policy       | Azure is of simple GUI; AWS is deeply integrated with Org accounts; GCP policy linked to resource hierarchy |
| **Defender for Cloud**         | AWS Security Hub + Inspector + GuardDuty   | Google Security Command Center   | Azure – Unified cloud & hybrid posture; AWS – Modular; GCP – Identity & Workload security. |
| **Microsoft Sentinel** (SIEM/SOAR) | AWS Security Hub + OpenSearch SIEM stack  | Chronicle Security Operations    | Sentinel is their cloud native SIEM/SOAR, then you have AWS needs multiple tools, and GCP has this thing called cloud chronicler that's specifically big data security. |

---
## 1. Microsoft Entra ID (Azure Active Directory)  
### AWS: IAM Identity Center (formerly AWS SSO)  
### GCP: Google Cloud Identity  

**Overview**  
- **Entra ID**: Cloud + Hybrid Identity & Access Mgmt, SSO, MFA, CA.  
- **AWS IAM Identity Center**: Administers workforce identity, and assists AWS Organizations.  
- **Google Cloud Identity**: The Google Workspace closely connected IAM in the Cloud.

**Core Features**  
- SSO among SaaS, on-prem and cloud applications  
- MFA, policies of conditional access  
- Federation with third party identity providers  

**Security & Compliance**  
- They all support **ISO 27001, SOC 2, HIPAA, GDPR, etc.**  
- for hybrid enterprise AD integration, Azure is strongest.  

**Pricing Model**  
- **Azure**: Free, P1, P2 levels of access (per-user license).  
- **AWS**: By IAM; expenditure is related to services consumed.  
- **GCP**: Free & Premium plans; charged per-user-per-month.  

**DevSecOps Integration**  
- Entra ID can be combined with **Azure DevOps/GitHub**.  
- CodePipeline/CloudFormation has an interface with AWS IAM SSO.  
- GCP can be connected to **Cloud Build/IAM roles**.

---

## 2. Azure Monitor & Log Analytics  
### AWS: Amazon CloudWatch + CloudTrail  
### GCP: Google Cloud Operations Suite (Stackdriver)  

**Overview**  
- **Azure Monitor**: Single pane visibility for apps, VMs, containers, logs & metrics.  
- **CloudWatch/CloudTrail**: Observebility + auditing log.  
- **GCP Operations Suite**: Logging, monitoring, tracing, error monitoring.

**Core Features**  
- The collection of metrics, the aggregation of logs  
- Dashboard, alerts, distributed tracing  
- Telemetry Custom support via API/SDK
- 
**Security & Compliance**  
- All provide **audit logging and encryption at rest/in transit**.  
- Comply to standards: **SOC, HIPAA, ISO 27001**.

**Pricing Model**  
- Ingest + retention pay-as-you-go.  
- **Azure**: Log Analytics Priced per GB.  
- **AWS**: CloudWatch Logs Gr/GB, CloudTrail request.  
- **GCP**: Free with quotas (then pay per Gig); pay per storage.

**DevSecOps Integration**  
- CI/CD observability dashboard , incident response alert hook.  
- They all are incorporated with **Prometheus, Grafana, third-party SIEM tools**.
---

## 3. Azure Policy  
### AWS: AWS Config + Service Control Policies (SCP)  
### GCP: Organization Policy  

**Overview**  
- **Azure Policy**: Implement rule based governance over resources.  
- **AWS Config/SCP**: Tracks resources compliance, applies org-wide restrictions.  
- **GCP Organization Policy**: Organizes constraints on the org/folder/project levels.

**Core Features**  
- compliance auditing, drift detection etc
- Use Enforce to restrain VM size, region or resource type  
- In-built templates for regular security scenarios
- 
**Security & Compliance**  
- Ensures policy-as-code Compliance framework governance.  
- CIS benchmarks, PCI DSS, GDPR capability.
- 
**Pricing Model**  
- **Azure**: Per resource eval/hour.  
- **AWS**: Billed on a per rule basis of Config evaluation.  
- **GCP**: No extra for Org Policies.  

**DevSecOps Integration**  
- Terraform, Bicep, ARM, CloudFormation Infrastructure as code checks.  
- Automates guardrails in CI-CD
  
---

## 4. Microsoft Defender for Cloud  
### AWS: Security Hub + Inspector + GuardDuty  
### GCP: Security Command Center  

**Overview**  
- **Defender for Cloud**: Single-vendor, cloud workload protection platform, (CWPP + CSPM).  
- **AWS**: Requires some tooling Security Hub (CSPM) Inspector (vuln scanning) GuardDuty (threat detection).  
- **GCP**: Risk Posture, Threat Intelligence is part of Security Command Center.  

**Core Features**  
- Workload protection Generate vulnerability scanning  
- CloudSecurityPostureManagement(CSPM)  
- Threat detection & compliance dashboards.
- 
**Security & Compliance**  
- The three are compliant standards (PCI DSS, ISO 27001, HIPAA).  
- Azure is also good at paired/on-prem + cloud integration.  

**Pricing Model**  
- **Azure**: It is free (CSPM) paid per workload/resource for CWPP.  
- **AWS**: Pricing per service individually.  
- **GCP**: Free (Basic) and Premium tier (per resource).  

**DevSecOps Integration**  
- Pipelines containing policy advice.  
- CI/CD gates incorporated by the results of vulnerability scan.  

---
## 5. Microsoft Sentinel (SIEM/SOAR)  
### AWS: Security Hub + OpenSearch SIEM stack  
### GCP: Chronicle Security Operations  

**Overview**  
- **Sentinel**: Cloud-Native SIEM. SOAR for Threat Detection in Real-Time.  
- **AWS**: Security Hub(compliance) + OpenSearch (acapetencias SIEM)  
- **GCP Chronicle**: Context-Aware, big data native SIEM with Google Threat Intel.  

**Core Features**  
- Threat detection via AI/ML  
- Autonomous playbooks (SOAR)  
- Log, threat feed and 3rd party SOC tool integrations  

**Security & Compliance**  
- International standard: **ISO, FedRAMP, SOC, HIPAA**.  
- It is enterprise SOC-designed.  

**Pricing Model**  
- **Azure Sentinel**: USBased metering for CONS per Ingested GB/day.  
- **AWS**: Pay for Security Hub + log ingestion on top.  
- **GCP Chronicle**: Data Ingestion + Analytics Query Based Pricing.  

**DevSecOps Integration**  
- Integrates with **DevOps pipelines, monitoring alerts, SIEM automation**.  
- Defender for Cloud is deeply integrated with Sentinel.  
- Chronicle utilizes Google threat intelligence.  

---

## 📖 Conclusion
- Azure offers **one, integrated security & compliance solutions**, particularly powerful in **hybrid + Microsoft ecosystem**.  
- The AWS provides fragmented yet modular services, which is powerful in multi-account governance.  
- GCP reiterates **simplicity, the use of AI to identify threats and Workspace integration**.  

All of them support the integration of DevSecOps, yet, **Azure is the best fit in the case of hybrid environment in enterprises, AWS for multi-cloud and modular adopters and GCP in the case of AI/analytics-intensive organizations**.  

---

   



