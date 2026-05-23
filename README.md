# Cloud-Honeypot-Global-Threat-Monitoring-Azure-Sentinel-
A live cloud honeypot deployed in Microsoft Azure, utilizing a custom PowerShell script and Microsoft Sentinel (SIEM) to map global RDP brute-force attacks in real-time.
## Objective
[Write 2-3 sentences explaining the core purpose of this project. Why did you build it? What were you trying to observe regarding default cloud security configurations and real-world attack vectors?]

## Architecture & Technology Stack
- **Cloud Platform:** Microsoft Azure
- **Security Information and Event Management (SIEM):** Microsoft Sentinel
- **Log Management:** Log Analytics Workspace
- **Compute:** Windows 10 Virtual Machine (Vulnerable Configuration)
- **Scripting & Automation:** PowerShell
- **Query Language:** Kusto Query Language (KQL)
- **External API:** [Insert the name of the Geolocation API you used]

## Methodology

### 1. Intentional Vulnerability Deployment
[Explain how you configured the Virtual Machine. Mention the specific Network Security Group (NSG) rules you created to expose the machine to the internet. Why did you disable the local Windows Firewall?]

### 2. Log Ingestion & Geolocation
[Describe the purpose of the PowerShell script. Explain how it extracted the IP addresses from Windows Event ID 4625 (Failed Logons) and routed them through a third-party API to get the longitude and latitude of the attackers.]

### 3. SIEM Configuration & Visualization
[Explain how you connected the Log Analytics Workspace to Microsoft Sentinel. Describe the process of writing KQL queries to parse the custom log data and plot the geographical points on the Sentinel workbook map.]

## Findings & Results
[Write a paragraph analyzing your observations. How long did it take for the first attacks to start? Which regions were the most active? What does this prove about the necessity of strict identity management and network defenses?]

### Attack Map Dashboard
![Attack Map Dashboard](Insert-Link-To-Your-Screenshot-Here.png)

*The map above visualizes the global distribution of RDP brute-force attacks directed at the honeypot over a 24-hour period.*
