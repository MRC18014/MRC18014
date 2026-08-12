# Home SIEM Server and Agents
<a href="https://github.com/MRC18014">Back to main page</a>
## Objective

The home SIEM server project was aimed to establish a working SIEM in a sandbox environment for vulnerability detection and remediation. This was achieved by using Oracle VirtualBox to create several virtual machines to run both the Wazuh SIEM Dashboard server in an Ubuntu Linux environment with several Wazuh agents including: Kali Linux, Linux Mint, and Microsoft Server 2022 edition. This hands-on experience was designed to deepen understanding of detecting known vulnerabilities, their origins and attack patterns, and methods of system hardening.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Oracle VirtualBox to create and manage the various virtual machines
- Ubuntu Linux to deploy and manage the SIEM dashboard
- Wazuh Security Information and Event Management (SIEM) platform as the SIEM that managed the compliance and threat detection of the various virtual machines
- Kali Linux to install a Wazuh SIEM agent onto and provide information regarding vulnerabilities in a Linux environment.
- Linux Mint to install a Wazuh SIEM agent onto and provide information regarding vulnerabilities in another Linux environment.
- Microsoft Server 2022 Edition to install a Wazuh SIEM agent onto and provide information regarding vulnerabilities in a Windows environment.

## Reference Images
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2001%20-%20Dashboard.png" width="75%" height="75%"></br>
<i>*Ref 1: Dashboard overview showing connected agents*</i>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2002%20-%20Microsoft%20Agent%20(Unpatched).png" width="75%" height="75%"></br>
<i>*Ref 2: Overview of Microsoft Windows Server 2022 vulnerabilities*</i>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2003%20-%20Microsoft%20Agent%20(Vulnerability).png" width="75%" height="75%"></br>
<i>*Ref 3: Microsoft Windows Server 2022 vulnerabilities in list form including their CVE ID and severity*</i>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005%20-%20Linux%20Agent.png" width="75%" height="75%"></br>
<i>*Ref 4: Overview of Kali Linux Agent dashboard*</i>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005b%20-%20Linux%20Agent%20(Configuration%20-%20Before).png" width="75%" height="75%"></br>
<i>*Ref 5: Overview of Kali Linux configuration assessment*</i>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005c%20-%20Linux%20Agent%20(Configuration%20-%20Before%20-%20Detailed).png" width="75%" height="75%"></br>
<i>*Ref 6: Detailed information of a potential misconfiguration and the method of remediation*</i>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005d%20-%20Linux%20Agent%20(Configuration%20-%20After).png" width="75%" height="75%"></br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005e%20-%20Linux%20Agent%20(Configuration%20-%20After%20-%20Detailed).png" width="75%" height="75%"></br>
<i>*Ref 6 & 7: Overview with the misconfiguration remediated*</i>
