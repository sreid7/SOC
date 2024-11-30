# SecurityOperations


**Incident Handling Process**
1. Recon - Gather information  

2. Weaponize -  the malware to be used for initial access is developed and embedded into some type of exploit or deliverable payload. Extremely light and undetectable.

3. Deliver - the exploit or payload is delivered to the victim(s). Traditional approaches are phishing emails that either contain a malicious attachment or a link to a web page.

4. Exploit -  when an exploit or a delivered payload is triggered. During the exploitation stage of the cyber kill chain, the attacker attempts to execute code on the target system in order to gain access or control.

5. Install - the initial stager is executed and is running on the compromised machine. Some common techniques used in the installation stage include:
  
**Droppers**: Attackers may use droppers to deliver malware onto the target system. A dropper is a small piece of code that is designed to install malware on the system and execute it. The dropper may be delivered through various means, such as email attachments, malicious websites, or social engineering tactics. 

**Backdoors**: A backdoor is a type of malware that is designed to provide the attacker with ongoing access to the compromised system. The backdoor may be installed by the attacker during the exploitation stage or delivered through a dropper. Once installed, the backdoor can be used to execute further attacks or steal data from the compromised system. 

**Rootkits**: A rootkit is a type of malware that is designed to hide its presence on a compromised system. Rootkits are often used in the installation stage to evade detection by antivirus software and other security tools. The rootkit may be installed by the attacker during the exploitation stage or delivered through a dropper.


6. C&C (Command and Control) - the attacker establishes a remote access capability to the compromised machine.

7. Action - objective of the attack. The objective of each attack can vary. Some adversaries may go after exfiltrating confidential data, while others may want to obtain the highest level of access possible within a network to deploy ransomware.

--------------------

**NIST Incident Handling (Defensive Security Model)**

1. Preparation: Creating policies, procedures, and tools for defense.

2. Detection and Analysis: Identifying and analyzing the signs of an incident (this is when the Exploit and Deliver stages of the Kill Chain are detected).

3. Containment, Eradication, and Recovery:

  Containment: Preventing the attacker from further compromising systems (corresponds with Install and C&C).
  Eradication: Removing the threat from the system.
  Recovery: Restoring normal operations, ensuring no further threats remain.

4. Post-Incident Activities: Analyzing the attack to improve defenses (post-exploitation phase).

--------------------


**Preparation Prerequisites**
During the preparation, we need to ensure that we have:

Skilled incident handling team members (incident handling team members can be outsourced, but a basic capability and understanding of incident handling are necessary in-house regardless)
Trained workforce (as much as possible, through security awareness activities or other means of training)
Clear policies and documentation
Tools (software and hardware)


**Clear Policies & Documentation**
Some of the written policies and documentation should contain an up-to-date version of the following information:

Contact information and roles of the incident handling team members
Contact information for the legal and compliance department, management team, IT support, communications and media relations department, law enforcement, internet service providers, facility management, and external incident response team
Incident response policy, plan, and procedures
Incident information sharing policy and procedures
Baselines of systems and networks, out of a golden image and a clean state environment
Network diagrams
Organization-wide asset management database
User accounts with excessive privileges that can be used on-demand by the team when necessary (also to business-critical systems, which are handled with the skills needed to administer that specific system). These user accounts are normally enabled when an incident is confirmed during the initial investigation and then disabled once it is over. A mandatory password reset is also performed when disabling the users.
Ability to acquire hardware, software, or an external resource without a complete procurement process (urgent purchase of up to a certain amount). The last thing you need during an incident is to wait for weeks for the approval of a $500 tool.
Forensic/Investigative cheat sheets


**Tools (Software & Hardware)**
Moving forward, we also need to ensure that we have the right tools to perform the job. These include, but are not limited to:

Additional laptop or a forensic workstation for each incident handling team member to preserve disk images and log files, perform data analysis, and investigate without any restrictions (we know malware will be tested here, so tools such as antivirus should be disabled). These devices should be handled appropriately and not in a way that introduces risks to the organization.
Digital forensic image acquisition and analysis tools
Memory capture and analysis tools
Live response capture and analysis
Log analysis tools
Network capture and analysis tools
Network cables and switches
Write blockers
Hard drives for forensic imaging
Power cables
Screwdrivers, tweezers, and other relevant tools to repair or disassemble hardware devices if needed
Indicator of Compromise (IOC) creator and the ability to search for IOCs across the organization
Chain of custody forms
Encryption software
Ticket tracking system
Secure facility for storage and investigation
Incident handling system independent of your organization's infrastructure


-----------------------


**Initial Investigation** 

Collect as much information as possible at this stage about the following:

1. Date/Time when the incident was reported. Additionally, who detected the incident and/or who reported it?
2. How was the incident detected?
3. What was the incident? Phishing? System unavailability? etc.
4. Assemble a list of impacted systems (if relevant)
5. Document who has accessed the impacted systems and what actions have been taken. Make a note of whether this is an ongoing incident or the suspicious activity has been stopped
6. Physical location, operating systems, IP addresses and hostnames, system owner, system's purpose, current state of the system
7. (If malware is involved) List of IP addresses, time and date of detection, type of malware, systems impacted, export of malicious files with forensic information on them (such as hashes, copies of the files, etc.)
With that information at hand, we can make decisions based on the knowledge we have gathered.





