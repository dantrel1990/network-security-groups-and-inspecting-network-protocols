# network-security-groups-and-inspecting-network-protocols
<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1 (create sample file shares with various permissions)
- Step 2 (attempt to access file shares as a normal user)
- Step 3 (create an "ACCOUNTANTS' security group, assign permissions, and test access)

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/5YpTaoj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of simple file shares with various permissions i have created in server manager
</p>
<br />

<p>
[<img src="https://i.imgur.com/lLrfhdA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  Above is an example of me trying to access a shared account that has denied me access because 
  normal users do not have access only members of the accounting security group have access because any member of the accountant's security group has written access.
</p>

<p>
<img src="https://i.imgur.com/f3nZywp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
Above is an image detailing how I added an. doe to the ACCOUNTANTS security group so that the shared folders can now be accessed.
</p>


