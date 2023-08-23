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


<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/Jacobvillagomez1/Creating-Resources-Groups-Storage-Accounts-and-Containers/assets/143027686/7d4b9bf6-474d-41e8-b189-c3e6d017f5f2"/>
</p>
<p>
First we need to type Resource Groups in the Azure search bar then click the create resource group tab.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Creating-Resources-Groups-Storage-Accounts-and-Containers/assets/143027686/45b556ff-eb52-43aa-a484-b3dc796f29a8"/>
</p>
<p>
Once we are in the Resource Group make sure its under your subscription, the Resource Group name can be named RG-01, and your region US West US 3.
</p>
<br />

<p>
