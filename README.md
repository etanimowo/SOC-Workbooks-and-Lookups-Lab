# SOC-Workbooks-and-Lookups-Lab
> **Disclaimer:**  
> All usernames, hostnames, IP addresses, and scenarios in this repository are **fictional and part of a TryHackMe training lab**.  
> They do not represent real individuals, organizations, or production systems.

---
## Overview
This lab focuses on **Security Operations Center (SOC) workbooks** and **lookup methods** to streamline alert triage. SOC analysts often need contextual information about employees, servers, and network activities to determine whether alerts are legitimate or malicious. This lab provided hands-on experience with **asset inventory, identity inventory, network diagrams, and workbook creation** to efficiently triage security alerts.

---
## Learning Objectives
- Familiarize with SOC investigation workbooks and their purpose  
- Learn to access and use **identity inventory** to gather context on employees and roles  
- Understand and utilize **asset inventory** for servers and workstations  
- Explore **corporate network diagrams** to analyze alert events  
- Practice building **SOC workflows and playbooks** for consistent alert triage  

---
## Workshops
### Workshop 1: Email Analysis
**Objective:** Investigate atypical email alerts using SOC workbooks  

**Key Skills:**
- Email header analysis  
- Identifying suspicious attachments or links  
- Using identity and asset inventory for context  

**Example Workflow (Text-Based Visual):**
[Email Alert Received] 
        |
        v
[Enrichment: Lookup Sender/User]
        |
        v
[Investigation: Check Header & Attachments]
        |
        v
[Verdict: Safe / Escalate]

### Workshop 2: PowerShell Analysis
Objective: Investigate PowerShell script execution alerts on endpoints

**Key Skills:**
- Using endpoint logs and SIEM to track PowerShell commands
- Enriching user and host data using asset and identity inventories
- Following SOC workbook steps to make verdicts

**Example Workflow (Text-Based Visual):**
[PowerShell Alert Received] 
        |
        v
[Enrichment: Identify User & Host]
        |
        v
[Investigation: Analyze PowerShell Commands]
        |
        v
[Verdict: Safe / Escalate]

### Workshop 3: Network Analysis
Objective: Analyze unusual network activity and connections

**Key Skills:**
- Mapping external IPs to internal IPs
- Using subnets and network diagrams to understand traffic patterns
- Determining if network scans or port connections are malicious

**Example Workflow (Text-Based Visual):**
[Network Alert Received]
        |
        v
[Map External IP to Internal IP]
        |
        v
[Analyze Subnets & Ports]
        |
        v
[Investigation: Lookup Asset/Identity]
        |
        v
[Verdict: Safe / Escalate]

### Tools and Resources Used
- SIEM Platforms: Splunk, ELK, or other SOC interfaces
- Threat Intelligence Sources for alert enrichment
- Identity Inventory: Employee and service account details
- Asset Inventory: Server and workstation catalog
- Network Diagrams: Visual maps of subnets, services, and connections
- SOC Workbooks/Playbooks: Step-by-step investigation guides

### Skills Developed
- Conducting alert triage using structured workbooks
- Performing user and asset lookups for context in SOC investigations
- Analyzing email, PowerShell, and network alerts
- Building workflow playbooks for consistent investigations
- Differentiating legitimate vs suspicious activity

### Key Lessons Learned
- SOC workbooks reduce triage errors and streamline investigations
- Proper identity and asset inventories provide critical context
- Network diagrams enhance understanding of complex network events
- Following structured steps ensures high-quality alert triage
- L1-L2 collaboration is essential for escalation and remediation

### Lab Flags / Proof of Completion
- Workshop 1 (Email Analysis): FLAG- THM{the_most_common_soc_workbook}
- Workshop 2 (PowerShell Analysis): FLAG- THM{be_vigilant_with_powershell}
- Workshop 3 (Network Analysis): FLAG- THM{asset_inventory_is_essential}

### Tables for User and Asset Lookups
| User     | Role     | Department | Working Hours |
|----------|---------|-----------|---------------|
| G.Baker  | Analyst | Finance   | 09:00-17:00   |
| R.Lund   | Manager | Finance   | 08:00-16:00   |

| Server       | Purpose          | Access Level    |
|-------------|-----------------|-------------------|
| HQ-FINFS-02 | Financial Files | Finance Team Only |

## Conclusion
This lab strengthened SOC triage skills across email, PowerShell, and network alerts, emphasizing the importance of workbooks, lookups, and structured workflows. Analysts can efficiently investigate alerts, reduce errors, and escalate incidents properly, ensuring a more secure corporate environment.
