<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/y6QoC74.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I start by creating two virtual machines in Azure one as the domain controller the other as client one. Client one will be used to connect to my domain controller. Similiar to being in college and how all their computers use the same domain controller so no matter what computer your using your login connects you to their network. My virtual machine for my domain controller has a dynamic IP address so by clicking on my virtual machine DC1, then in settings click networking, network interface, IP configurations im then prompted to change my IP from dynamic to static so my IP adress does not change. From here as prompted in the picture ill check both vortual machines to be sure their on the same network and subnet.
</p>
<br />

<p>
<img src="https://i.imgur.com/pTMuxY9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next I open client 1 virtual machine by copying the public IP address and opening it through remote desktop connection. From there I open the command line and start a perpectual ping to my other virtual machine called DC1 using DC1 public IP address. That reply kept coming back "timed out" because I had to open my virtual machine DC1 in remote desktop and enable two rules inside DC1 firewall wall. Remeber ICMPV4 protocol is the protocl ping uses. This is all to ensure connectivity between the client and domain controller. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
