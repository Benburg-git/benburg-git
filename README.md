<h1 align="center">Hi 👋, I'm Sunday Abiodun</h1>

<h3 align="center">Cloud Security & DevSecOps Engineer</h3>

<p align="center">
Microsoft Sentinel SIEM/SOAR • Azure & AWS Security • Terraform • Kubernetes • Secure CI/CD
</p>

<p align="center">
Building secure cloud infrastructure, automating security controls, and engineering faster incident response.
</p>

---

## 👨‍💻 About Me

I'm a **Cloud Security & DevSecOps Engineer** based in the United Kingdom, focused on securing cloud environments, automating infrastructure, and embedding security throughout the software development lifecycle.

My work spans **AWS & Azure Security, Microsoft Sentinel SIEM/SOAR, Infrastructure as Code, Kubernetes Security, DevSecOps, Application Security, and Incident Response**.

I enjoy solving security problems through automation — from building secure cloud infrastructure with Terraform to integrating security controls directly into CI/CD pipelines.

- 🛡️ Building and securing cloud environments across **AWS & Azure**
- 🔎 Working with **Microsoft Sentinel SIEM/SOAR** for detection and response
- 🏗️ Building Infrastructure as Code with **Terraform**
- ☸️ Securing containerized workloads with **Docker & Kubernetes**
- 🔐 Implementing **IAM, encryption, secrets management & least privilege**
- 🔄 Integrating security into **CI/CD pipelines**
- 🚨 Focused on **Detection Engineering & Incident Response**
- 🔍 Applying **Application Security & DevSecOps** practices

---

## 🛠️ Technical Stack

### ☁️ Cloud & Infrastructure

<p>
<img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
<img src="https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white" />
</p>

### 🛡️ Security & SIEM

<p>
<img src="https://img.shields.io/badge/Microsoft_Sentinel-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white" />
<img src="https://img.shields.io/badge/AWS_GuardDuty-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/AWS_Security_Hub-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
<img src="https://img.shields.io/badge/CloudTrail-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
</p>

**Security Engineering:** SIEM • SOAR • Incident Response • Detection Engineering • IAM • KMS • Secrets Management • Vulnerability Management • Application Security

### ☸️ Containers & Kubernetes

<p>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
<img src="https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white" />
<img src="https://img.shields.io/badge/HashiCorp_Vault-FFEC6E?style=for-the-badge&logo=vault&logoColor=black" />
</p>

### 🔄 DevSecOps & CI/CD

<p>
<img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
<img src="https://img.shields.io/badge/Gitleaks-Security-red?style=for-the-badge" />
<img src="https://img.shields.io/badge/Checkov-IaC_Security-blue?style=for-the-badge" />
<img src="https://img.shields.io/badge/tfsec-Terraform_Security-purple?style=for-the-badge" />
<img src="https://img.shields.io/badge/Trivy-Vulnerability_Scanning-1904DA?style=for-the-badge" />
<img src="https://img.shields.io/badge/OPA-Policy_as_Code-7D9199?style=for-the-badge&logo=openpolicyagent&logoColor=white" />
</p>

---

# 🚀 Featured Security Engineering Projects

## 🔐 SentinelPay — Secure AWS Payment Platform

**Cloud Security • AWS • Terraform • DevSecOps • Detection Engineering**

SentinelPay is a security-focused AWS infrastructure project designed to demonstrate how cloud security controls can be embedded directly into infrastructure and CI/CD workflows.

### 🏗️ Architecture

                         Internet
                            │
                            ▼
                    ┌───────────────┐
                    │      ALB      │
                    └───────┬───────┘
                            │
                 ┌──────────┴──────────┐
                 │                     │
                 ▼                     ▼
          Payments API              KYC API
           ECS Fargate             ECS Fargate
                 │                     │
                 └──────────┬──────────┘
                            │
                 ┌──────────┴──────────┐
                 │                     │
                 ▼                     ▼
          PostgreSQL RDS        ElastiCache Redis
                 │                     │
                 └──────────┬──────────┘
                            │
                     Private Subnets

### 🔒 Security Controls

- Multi-AZ AWS VPC architecture
- Public Application Load Balancer with private workloads
- ECS Fargate containerized services
- PostgreSQL RDS isolated in private subnets
- ElastiCache Redis isolated in private subnets
- Customer-managed AWS KMS encryption
- AWS Secrets Manager
- IAM least-privilege controls
- GitHub Actions → AWS OIDC federation
- AWS GuardDuty threat detection
- AWS Security Hub
- Multi-region AWS CloudTrail
- VPC Flow Logs
- Infrastructure security scanning

### 🔄 DevSecOps Pipeline

    Developer
        │
        ▼
    Feature Branch
        │
        ▼
    Pull Request
        │
        ├──── Gitleaks
        ├──── Terraform fmt
        ├──── Terraform validate
        ├──── Checkov / tfsec
        ├──── OPA / Conftest
        └──── Vulnerability Scanning
                     │
                     ▼
               Terraform Plan
                     │
                     ▼
                  Review
                     │
                     ▼
                   Merge
                     │
                     ▼
            GitHub Actions OIDC
                     │
                     ▼
                    AWS

**Technology:** `AWS` `Terraform` `ECS Fargate` `RDS` `Redis` `KMS` `Secrets Manager` `GuardDuty` `Security Hub` `CloudTrail` `GitHub Actions` `OIDC` `Checkov` `tfsec` `OPA` `Conftest`

---

## 🛡️ SecureFlow — Kubernetes & Vault Security

**Kubernetes Security • HashiCorp Vault • DevSecOps • Secrets Management**

SecureFlow is a security-focused Kubernetes project demonstrating secure workload identity and secrets management using **HashiCorp Vault**.

### 🏗️ Architecture

                 Kubernetes Cluster
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ▼              ▼              ▼
      Frontend      Auth Service   Transaction Service
          │              │              │
          └──────────────┼──────────────┘
                         │
                         ▼
                  HashiCorp Vault
                         │
                         ▼
                 Kubernetes Auth
                         │
                         ▼
                  Vault Policies
                         │
                         ▼
                  Secret Injection

### 🔐 Security Implementation

- Kubernetes Service Accounts
- HashiCorp Vault Kubernetes authentication
- Vault Agent Injector
- Application-specific Vault policies
- Secure application secret injection
- RBAC
- Least-privilege access
- Workload identity
- Kubernetes secrets management

**Technology:** `Kubernetes` `Docker` `HashiCorp Vault` `Helm` `RBAC` `Service Accounts` `DevSecOps`

---

# 🚨 Detection Engineering & Incident Response

I work with **Microsoft Sentinel SIEM/SOAR** to explore security monitoring, threat detection, investigation, and automated response.

              Security Telemetry
                      │
                      ▼
             Microsoft Sentinel
                      │
        ┌─────────────┼─────────────┐
        │             │             │
        ▼             ▼             ▼
    Analytics      Incidents    Investigation
      Rules
        │             │             │
        └─────────────┼─────────────┘
                      │
                      ▼
                SOAR Playbooks
                      │
                      ▼
             Automated Response
                      │
                      ▼
                Remediation

### Areas of Focus

`Microsoft Sentinel` • `SIEM` • `SOAR` • `KQL` • `Detection Engineering` • `Security Automation` • `Threat Detection` • `Incident Investigation` • `Incident Response`

---

# 🔐 Security-First Engineering

My approach combines preventative, detective, and responsive security controls.

                        SECURITY
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
       PREVENT           DETECT          RESPOND
          │                │                │
       IAM / RBAC       Sentinel       SOAR Playbooks
       KMS              GuardDuty      Automation
       Secrets          CloudTrail     Remediation
       IaC Security     Security Hub   Incident Response
          │                │                │
          └────────────────┼────────────────┘
                           │
                           ▼
                  Secure Engineering

### My Engineering Principle

> **Build Securely → Detect Quickly → Respond Efficiently → Automate Repetitive Work**

---

# 📚 Currently Developing

- 🔎 Microsoft Sentinel & KQL
- 🤖 SOAR & Security Automation
- ☁️ Azure Security Architecture
- ☁️ AWS Cloud Security
- 🏗️ Terraform & Infrastructure as Code
- ☸️ Kubernetes Security
- 🔐 Identity & Access Management
- 🚨 Detection Engineering
- 🔍 Application Security
- 🧪 DevSecOps
- 🎯 Threat Modelling

---

# 🤝 Let's Connect

I'm interested in **Cloud Security, DevSecOps, Security Engineering, Application Security, Detection Engineering, and Cloud Infrastructure**.

📍 **United Kingdom**

💼 **LinkedIn:** sunday-abiodun-b9a766275

📧 **Email:** sundayyabiodunn@gmail.com

---

<p align="center">
<b>☁️ Secure the Cloud • 🔐 Embed Security • 🚨 Detect Threats • 🤖 Automate Response</b>
</p>
