# Home SIEM Server and Agents
<a href="https://github.com/MRC18014">Back to main page</a>
## Objective

The home SIEM server project was aimed to establish a working SIEM in a sandbox environment for vulnerability detection and remediation. This was achieved by using Oracle VirtualBox to create several virtual machines to run both the Wazuh SIEM Dashboard server in an Ubuntu Linux environment with several Wazuh agents including: Kali Linux, Linux Mint, and Microsoft Server 2022 edition. This hands-on experience was designed to deepen understanding of detecting known vulnerabilities, their origins and attack patterns, and methods of system hardening.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Deeper understanding of patching vulnerabilities and hardening systems.
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
<i><b>*Ref 1: Dashboard overview showing connected agents*</i></b></br>
This Image shows the Wazuh SEIM server running and monitoring several agents. For this lab environment, I decided to demonstrate versatility with the SIEM and manage several different types of operating systems ranging from Microsoft Windows Server 2022, to a few Linux operating systems in Linux Minx and Kali Linux.</br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2002%20-%20Microsoft%20Agent%20(Unpatched).png" width="75%" height="75%"></br>
<i><b>*Ref 2: Overview of Microsoft Windows Server 2022 vulnerabilities*</i></b></br>
The above image is an over of the Microsoft Windows Sever 2022 agent. I chose this operating system due to its usefulness in managing user accounts, account access policies, and user groups - traits that apply in a live environment. Since this a fresh install, there are many unpatched vulnerabilities listed.</br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2003%20-%20Microsoft%20Agent%20(Vulnerability).png" width="75%" height="75%"></br>
<i><b>*Ref 3: Microsoft Windows Server 2022 vulnerabilities in list form including their CVE ID and severity*</i></b></br>
This image lays out the more severe vulnerabilities, as well as the CVE ID, which give a description of the vulnerabilities, as well as the method to remediate said vulnerabilities. Most of these vulnerabilites were resolved by Microsoft over the years, so I applied the necessary patches.</br>
<img src="https://github.com/MRC18014/Projects/blob/main/CVE-01.png" width="75%" height="75%"></br>
<i><b>*Ref 4: Overview of CVE-2026-58640, the CVE listed on the top of the vulnerabilities list</i></b></br>
This image provides a brief description of the vulnerability. The information listed includes when the record was last updated, a CVSS score and severity level, which provides a qualitative and quantitative assessment of the vulnerability, as well as the vector string which lays out the vulnerability characteristics (example: AV:L - Actor Vector: Local - The attacker must have local access to the target system (such as being logged on via a console or SSH)). This information is important for determining how quickly the patches should be applied. Since this vulnerability was high, I made it a top priority. If this was at a low severity level, and if this was a live environment, I might have scheduled a maintenance period during a slow time to patch this.</br>
<img src="https://github.com/MRC18014/Projects/blob/main/CVE-02.png" width="75%" height="75%"></br>
<i><b>*Ref 5: List of Microsoft updates that patch the vulnerability</i></b></br>
This is an image of the bottom portion of the CVE-2026-58640 vulnerability page. This section covers the listed patches that remediates the known vulnerability, thus, helping to secure the vulnerable system</br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2004%20-%20Microsoft%20Agent%20(Patched).png" width="75%" height="75%"></br>
<i><b>*Ref 6: Microsoft Windows Server 2022 after applying patches to remediate vulnerabilities</i></b></br>
As shown in ref 6, after I applied the necessary patches, there are no more known serious vulnerabilities. There are, however, some areas that can checked on by examining the configuration assessment. It is worth noting that there may be instances where some configurations are acceptable, but should be addressed on a case-by-case basis. I will continue to monitor this system for vulnerabilities as this is not a one-and-done process, but a constant event.</br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005%20-%20Linux%20Agent.png" width="75%" height="75%"></br>
<i><b>*Ref 7: Overview of Kali Linux Agent dashboard*</i></b></br>
This image shows an overview of the Wazuh SIEM monitoring a recently deployed Kali Linux system. Since this system of a fresh and the most recent copy of Kali Linux, there are no known vulnerabilities at the time that I initiated this scan. There are, however, some opportunities for system hardening by reviewing the Security Configuration Assessment section.</br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005b%20-%20Linux%20Agent%20(Configuration%20-%20Before).png" width="75%" height="75%"></br>
<i><b>*Ref 8: Overview of Kali Linux configuration assessment*</i></b></br>
This section displays the results of the configuration scan. With these results, I'm able to go into the Linux system and disable any options that I currently do not need on my system. Doing this will help harden my system by reducing the attack surface for potential bad actors.
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005c%20-%20Linux%20Agent%20(Configuration%20-%20Before%20-%20Detailed).png" width="75%" height="75%"></br>
<i><b>*Ref 9: Detailed information of a potential misconfiguration and the method of remediation*</i></b></br>
I decided to look into the first flagged configuration ID, 30001. By clicking the ID, I'm given a description, a cause for disabling, how to disable the configuration, and various compliance factors (ex: PCI-DSS v3.2.1, NIST SP 800-53) that this ID would apply to, as well as how an attacker would apply this configuration in their attacks (MITRE Techniques), giving me a full scope in my decision to keep the configuration enabled or to disable it.</br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005d%20-%20Linux%20Agent%20(Configuration%20-%20After).png" width="75%" height="75%"></br>
<img src="https://github.com/MRC18014/Projects/blob/main/SIEM%20-%2005e%20-%20Linux%20Agent%20(Configuration%20-%20After%20-%20Detailed).png" width="75%" height="75%"></br>
<i><b>*Ref 10 & 11: Overview with the misconfiguration remediated*</i></b></br>

