# SecurityOperations

**Incident Handling Process**
1. Recon - Gather information  

2. Weaponize -  the malware to be used for initial access is developed and embedded into some type of exploit or deliverable payload. Extremely light ans undetectable.

3. Deliver - the exploit or payload is delivered to the victim(s). Traditional approaches are phishing emails that either contain a malicious attachment or a link to a web page.

4. Exploit -  when an exploit or a delivered payload is triggered. During the exploitation stage of the cyber kill chain, the attacker attempts to execute code on the target system in order to gain access or control.

5. Install - the initial stager is executed and is running on the compromised machine. Some common techniques used in the installation stage include:
  
**Droppers**: Attackers may use droppers to deliver malware onto the target system. A dropper is a small piece of code that is designed to install malware on the system and execute it. The dropper may be delivered through various means, such as email attachments, malicious websites, or social engineering tactics. 

**Backdoors**: A backdoor is a type of malware that is designed to provide the attacker with ongoing access to the compromised system. The backdoor may be installed by the attacker during the exploitation stage or delivered through a dropper. Once installed, the backdoor can be used to execute further attacks or steal data from the compromised system. 

**Rootkits**: A rootkit is a type of malware that is designed to hide its presence on a compromised system. Rootkits are often used in the installation stage to evade detection by antivirus software and other security tools. The rootkit may be installed by the attacker during the exploitation stage or delivered through a dropper.


6. C&C (Command and Control) - the attacker establishes a remote access capability to the compromised machine.

7. Action - objective of the attack. The objective of each attack can vary. Some adversaries may go after exfiltrating confidential data, while others may want to obtain the highest level of access possible within a network to deploy ransomware.

