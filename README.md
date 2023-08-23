# Network File Shares and Permissions
<p align="center">
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>Network File Shares and Permissions</h1>
In this tutorial, going off On-premises Active Directory Deployed in the Cloud (Azure) [https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs] we will create Network files and share permissions between them. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Active Directory Domain Services
- Server Manager
- Windows Administrative Tools
- Active Directory Users and Computers


<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>

- Log into Cilent-1 and DC-1 VM from [https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs]
- Open DC-1 VM go to Windows Administrative Tools
- Load Active Directory Users and Computers
- Select a random user and log into with Remote Desktop Connection
- Go back to DC-1 VM open File Explorer got to Windows (C) and create the following files (read access, write access, no access, and accounting)
- Go into all the files propeties and allow certain permissions
- Go back to Cilent-1 VM and create a write file txt. file
- Go back to DC-1 VM and create a txt.file to read access for other users to see
- Create a new organzational unit called SECURITY GROUPS
- Create a new group in SECURITY GROUPS called ACCOUNTIANS
- Allow the accounting file to shar persmission with the ACCOUNTIANS
- Add the user in Cilent-1 to ACCOUNTIANS role
- Log into the user with ACCOUNTIANS role


<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/be899399-e38a-4eb4-8e91-7fb71e688195"/>
</p>
<p>
First we need to log back into Cilent-1 and DC-1 from [https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs] using Remote Desktop Connection. Copy the Public IP and log into the VM indivudally.  
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/969fd9a4-964a-40b3-bb7d-6540aa3c2aa5"/>
</p>
<p>
Open DC-1 VM and click the window icon on the bottom left, then click Windows Administrative Tools
</p>
<br />

<p>
