# Network-Scanning-and-Firewall-Defense
Acted as both attacker and defender in a segmented lab network. Used Nmap to scan and profile a subnet from External Kali, then configured pfSense firewall rules to progressively restrict ICMP and traffic to protect the LAN, verifying results with before and after scans.

<b>Task A — Step 1:</b> Ran Wireshark in the Internal Kali VM while External Kali scanned the network. <br/>
<img src="Task%20A1.png" height="80%" width="80%" alt="Sword vs Shield Task A Step 1"/>
<br />
<br />

<b>Task A — Step 2:</b> Used Nmap in External Kali to profile the subnet topology, including open ports, service versions, and operating systems. <br/>
<img src="Task%20A%202.png" height="80%" width="80%" alt="Sword vs Shield Task A Step 2"/>
<br />
<br />

<b>Task B — Step 1a:</b> Configured a pfSense firewall rule to block ICMP traffic from External Kali to the Ubuntu VM. <br/>
<img src="TASK%20B1.png" height="80%" width="80%" alt="Sword vs Shield Task B Step 1a"/>
<br />
<br />

<b>Task B — Step 1b:</b> Tested the firewall rule in the terminal to confirm ICMP was blocked from External Kali to Ubuntu. <br/>
<img src="TASK%20B2.png" height="80%" width="80%" alt="Sword vs Shield Task B Step 1b"/>
<br />
<br />

<b>Task B — Step 2a:</b> Configured pfSense to block all ICMP traffic from External Kali to the LAN side. <br/>
<img src="PART%20B3.png" height="80%" width="80%" alt="Sword vs Shield Task B Step 2a"/>
<br />
<br />

<b>Task B — Step 2b:</b> Tested the terminal to confirm all ICMP traffic from External Kali to the LAN was blocked. <br/>
<img src="PART%20B4.png" height="80%" width="80%" alt="Sword vs Shield Task B Step 2b"/>
<br />
<br />

<b>Task B — Step 3a:</b> Cleared the previous rule and configured pfSense to block all traffic from External Kali to the LAN, except FTP traffic directed to Ubuntu. <br/>
<img src="TASK%20B5.png" height="80%" width="80%" alt="Sword vs Shield Task B Step 3a"/>
<br />
<br />

<b>Task B — Step 3b:</b> Tested the terminal to confirm only FTP traffic to Ubuntu was allowed through the firewall. <br/>
<img src="TASK%20B6.png" height="80%" width="80%" alt="Sword vs Shield Task B Step 3b"/>
<br />
<br />

<b>Task B — Step 4:</b> Kept the Task B.3 firewall rules in place and rescanned the subnet with Nmap in External Kali to compare results before and after the firewall changes. <br/>
<img src="TASK%20B7.png" height="80%" width="80%" alt="Sword vs Shield Task B Step 4"/>
<br />
<br />
