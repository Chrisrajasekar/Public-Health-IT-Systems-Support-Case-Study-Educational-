# Public Health IT Systems Support – Case Study (Educational)
![Public Sector](https://img.shields.io/badge/Public%20Sector-IT-blue)
![Healthcare IT](https://img.shields.io/badge/Domain-Healthcare%20IT-green)
![IT Support](https://img.shields.io/badge/Role-IT%20System%20Support%20Specialist-orange)
![ITIL Aligned](https://img.shields.io/badge/Framework-ITIL%20Aligned-purple)
![Security Aware](https://img.shields.io/badge/Focus-Security%20%26%20Reliability-red)
![Documentation](https://img.shields.io/badge/Strength-Documentation%20%26%20Runbooks-yellow)


This repository demonstrates my technical approach to **IT Systems Support** within a public health context. Using the **Windsor-Essex County Health Unit (WECHU)** as a reference point, this case study showcases how I manage high-availability infrastructure, secure sensitive health data, and provide tiered support for critical community services.

⚠️ Disclaimer
* This is an **educational, hypothetical case study** created for a professional portfolio.
* **No scanning, testing, or probing** of WECHU systems was performed.
* All observations are based on publicly available information and industry-standard IT best practices for health organizations.
* The infrastructure diagrams and risk assessments are conceptual models designed to demonstrate my technical mindset.

🎯 **Focus Areas**
* **System Support Mindset**: Ensuring 24/7 availability for community-critical health data.
* **Infrastructure Reliability**: Managing the "Backbone" (Servers, SQL Databases, Networking).
* **Security Awareness**: Aligning with PHIPA and ISO 27001 standards.
* **Incident Response**: Structured triage for outages and security events.
* **Documentation**: Clear SOPs for end-users and technical teams.

_______________________________


🌐 **Highlights of the WECHU Website**

The wechu.org platform is more than a website; it is a **Public Health Service Portal**.

* **Criticality**: Serves as the primary source for the Food Safety Inspection Dashboard, Respiratory Illness Tracking, and Immunization Reporting.
* **Availability**: Downtime directly impacts the community's ability to access health mandates and mandatory reporting tools for healthcare providers.
* **IT Support Relevance**: Requires seamless integration between web-frontends and backend SQL databases to ensure real-time data accuracy for the public.
_______________________________

🧩 **Infrastructure (Logical & Hypothetical)**

This diagram illustrates the flow of data from public interactions to secure backend storage, emphasizing the support layers managed.Focuses on logical infrastructure, not real or inferred architecture.

<img width="1408" height="768" alt="WECHU Infra" src="https://github.com/user-attachments/assets/82c73f63-e223-40e5-9fed-88d63cdc27a9" />

**Key Layers Included**

* Access Layer
* Presentation Layer
* Core Infrastructure (Data & Applications)
   * Identity & Access Management (AD / Entra ID)
   * Relational Databases
* Support & Security Services
  * System monitoring
  * Backup & recovery
_______________________________

🛡️ **Vulnerability & Risk Awareness**

This section outlines common risks faced by public health IT environments, not vulnerabilities specific to WECHU.

* **Endpoint Patching Delays**: Mitigated via automated patch management tools to prevent exploits on staff laptops.
* **Vendor Update Failures**: Strict testing of Ministry-based application updates in a sandbox environment before production rollout.
* **Credential Compromise**: Implementing MFA and monitoring for "impossible travel" alerts in Azure AD.
* **Data Integrity Risks**: Ensuring SQL database migrations are validated with checksums to prevent loss of sensitive health data.
_______________________________

🚨 **Incident Response**

My approach to system failures follows a **Detect → Triage → Communicate → Resolve → Document workflow**.

<img width="873" height="160" alt="Screenshot 2026-02-02 at 6 15 33 PM" src="https://github.com/user-attachments/assets/c02fe3fd-cd88-4b81-9e13-aad7d1d0fc15" />

**Scenarios**
* Website outage
* Email outage
* Endpoint security failure
* Database performance issue
_______________________________

💾 **Backup & Disaster Recovery (DR) Strategy**
* **3-2-1 Rule**: 3 copies of data, 2 different media, 1 offsite.Backup types (full, incremental)
* **RPO / RTO**: Setting Recovery Point Objectives (RPO) for health databases to ensure minimal data loss during a restore.
* **Verification**: Monthly "Restoration Drills" to ensure backups are not just successful, but functional.Ministry-based application backup awareness
_______________________________

🧑‍💻 **End-User Support Model**

I utilize an ITIL-aligned support framework to ensure staff can focus on public health, not tech issues.
Ticketing: Expertise in ServiceNow and Remedy for lifecycle management.

**Tiered Support**:

***Tier 1***: Password resets, hardware peripherals, basic connectivity.

***Tier 2***: Database integration, server configuration, application errors.

***Tier 3***: Vendor liaison (Ministry of Health) for complex system bugs.
_______________________________

📘 **Documentation Samples**

* Password reset SOP
* New laptop setup checklist
* Checklist New-Staff Provisioning
* Printer troubleshooting guide

