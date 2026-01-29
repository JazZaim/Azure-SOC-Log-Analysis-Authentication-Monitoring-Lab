<h1>Azure-Soc-Log-Monitoring-Lab</h1>

<h2>Description</h2>
This project simulates entry-level SOC analyst responsibilities by deploying a Windows virtual machine in Microsoft Azure, generating authentication activity, and ingesting Windows Security logs into Azure Log Analytics for monitoring and investigation.
<br /> 
<br />
<h2>The objective was to practice: </h2>
- Log ingestion and validation, authentication failure analysis, security event triage, cloud-based SOC workflows.

Windows VM → Windows Security Events → Azure Log Analytics → SOC Investigation

<h2>Tools & Technologies </h2>
- Microsfot Azure, Windows 11 Virutal Machine, Windows Event Viewer.

<h2>Program walk-through:</h2>

<p align="center">
  <b> Step 1 </b>
<br>Azure Enironment Setup: <br/>
  - Created an Azure subscription and resrouce group (SOC-Lab1), Deployed a Windows 11 VM in West US 2, Configured networking components (VNet,NSG, Public IP)
<img src="https://imgur.com/a4e00gL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/7hpl6Aq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/CEGQyC0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b> Step 2 </b>
<br> Endoint Access & Validation <br/>
  Connected to the VM using remote access,
  Verified OS and user context by using command prompt.
<img src="https://imgur.com/iHOpLhi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b> Step 3 </b>
<br> Local Firewall & Logging Configuration </br>
<p>Reviewed Windows Defender Firewall Profiles. </p>
<p>Ensured security logging was enabled for authentication events. </p>
<img src="https://imgur.com/4Art1l5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b> Step 4 </b>
  <br> Genereated failed authetian attempts. </br> 
  <br> Identified Event 4625 (Failed log-in) in Widnows Even Viewer. </br>
<img src="https://imgur.com/8UAQFjn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<b> Step 5 (Last Step) </b>
<br> Investigation Using KQL </br> 
<p>Exectured the follwoing query to validate log ingestion. </p>
<img src="https://imgur.com/lnAY6hB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p> SOC Analysis: </p>
<br> - Confirmed failed log-in activity </br>
<br> - Identified system and account context </br>
<br> Validated timestamps for investigative correlation </br> 
<br />
<br />
<b> Skills Demonstrated </b>
<br> -SIEM log ingestion & Validation </br>
<br> -Windows Authentication event analysis </br> 
<br> -Cloud Security Fundamentals </br> 
<br> -SOC investigative thinking </br>
<br />
<br /> 
<b> Conclusion</b>
-This lab demonstrates hands on SOC experience using Azure and Windows security closely mirroring tasks performed by SOC Analysts and Insider Threat teams.
