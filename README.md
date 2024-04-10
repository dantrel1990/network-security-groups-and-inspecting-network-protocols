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
<img src="https://i.imgur.com/FD99KCh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Above is an example of logging into DC-1 domain admin accountant(mydomain.com\jane_admin)
</p>
<br />

<p>
<img src="https://i.imgur.com/x0OHUYE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of logging into Client-1 as a normal user(mydomain\abcuser)
</p>
<br />

<p>
<img src="https://i.imgur.com/AQ37KMD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of 4 folders read-access, write-access, no-access, accounts 
</p>
<br />

<p>
<img src="https://i.imgur.com/4dY1dq8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of a read-access group with the domain permissions to read
</p>
<br />

<p>
<img src="https://i.imgur.com/iqEL1BR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of a write-access group with the domain permissions to read\write
</p>
<br />


<p>
<img src="https://i.imgur.com/cLjPaVX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of a no-access group domain admins permissions read\write
</p>
<br />

<p>
<img src="https://i.imgur.com/gTTGlZa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of a read-access folder only with the permissions to read and nothing follows
</p>
<br />

<p>
<img src="https://i.imgur.com/IFSns1k.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of a write-access folder with only the permissions to read\write
</p>
<br />

<p>
<img src="https://i.imgur.com/2LnLhlo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of a no-access folder with no permissions granted to domain users only domain controllers
</p>
<br />

<p>
<img src="https://i.imgur.com/aVddc5h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Above is an example of an accounting group with the permission to read\write
</p>
<br />
