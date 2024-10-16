<h1>Description</h1>
Project consists of using the cloud platform Azure to create Windows and Linux virtual machines to monitor different types of network traffic. The environments allow you to install and configure Wireshark, Firewalls, and perform packet inspection via Remote Desktop Protocol.
<br />


<h2>Utilities Used</h2>

- <b>Microsoft Azure</b> 
- <b>Wireshark</b>
- <b>Powershell</b>
- <b>Network Security Groups (Firewalls)</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (22H2)
- <b>Linux</b> (Ubuntu)

<h2>Program walk-through:</h2>

<p align="center">
Create our virtual machine environment: <br/>
<img src="https://i.imgur.com/JgIHKGS.png" height="80%" width="80%" alt="My Azure Resource Group"/>
<br />
<br />
Connect to Windows VM via RDP and observe ICMP traffic:  <br/>
<img src="https://i.imgur.com/O2CVji6.png" height="80%" width="80%" alt="Observe ping requests and replies within WireShark"/>
<br />
<br />
Configuring a Firewall (Network Security Group): <br/>
<img src="https://i.imgur.com/NiutjfA.png" height="80%" width="80%" alt="Blocking ICMP traffic for our Windows VM"/>
<br />
  Now we see the inbound ICMP request but no response from the Windows VM: <br/>
<img src="https://i.imgur.com/gRwEmxZ.png" height="80%" width="80%" alt="Now we see the request but no response from our Windows VM"/>
<br />
<br />
Observe SSH traffic:  <br/>
<img src="https://i.imgur.com/FJevm9e.png" height="80%" width="80%" alt="Open PowerShell, and type: ssh labuser@<private IP address"/>
<br />
<br />
Observe DHCP traffic:  <br/>
<img src="https://i.imgur.com/tPkyAF0.png" height="80%" width="80%" alt="Open PowerShell as admin and run: ipconfig forwardslashrenew"/>
<br />
<br />
Observe DNS traffic:  <br/>
<img src="https://i.imgur.com/1QsyrlF.png" height="80%" width="80%" alt="Observe the DNS traffic being shown in WireShark"/>
<br />
<br />
Observe RDP traffic:  <br/>
<img src="https://i.imgur.com/pCn3jRh.png" height="80%" width="80%" alt="Back in Wireshark, filter for RDP traffic only"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
