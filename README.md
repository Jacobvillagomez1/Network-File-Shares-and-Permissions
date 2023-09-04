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
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/230ee7bf-0922-47ed-889d-e45f64f9c75f"/>
</p>
<p>
Next click Active Directory Users and Computers
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/f1100013-48b1-4881-b7d8-2d60ae3891fa"/>
</p>
<p>
Now go to the Employees section and you will see all 2000 Employees created
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/a6eeb55c-53e2-4bfd-ace5-5d0ca3170be1"/>
</p>
<p>
Next click a random user and copy the display name on a notepad to not forget the name
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/4df9e089-bc9a-4d98-8686-58e2ed54c95f"/>
</p>
<p>
Now type File Explorer in the search bar and open the app
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/61ee3cc5-3546-49cb-b5b4-fdd503dde7fa"/>
</p>
<p>
Now click on Windows (C)
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/dd83be67-ef2e-4a5e-8d79-250221a84f9e"/>
</p>
<p>
From here create the following file read access, write access, no access, and accounting. To do this right click anywhere and click create new folder
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/dd8cc1a4-1d35-4666-ab06-ec675f456856"/>
</p>
<p>
Next right click read access and go to properties
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/620acc5d-b8f1-4416-a8c2-0e7b2c19648d"/>
</p>
<p>
Go to the Sharing section and click share
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/0c89a6d6-9db0-4eb3-9799-8d0577e96762"/>
</p>
<p>
Next type domain users and click add
</p>
<br />


<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/4cf9f4b0-503d-43dc-a2db-f2e577d9ac61"/>
</p>
<p>
Now click the permissions level and click the read permission. Then click shar on the bottom right 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/fc619215-34ad-483a-bf01-4366cc3d34c5"/>
</p>
<p>
To finish click Done 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/1e029fb3-57fd-4f64-8964-6b2ef357a456"/>
</p>
<p>
Right click write access and go to the properties section 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/e38ece3b-4b6a-4c14-87a8-8a04ac1e95cd"/>
</p>
<p>
Next click the Sharing tab, and click share 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/42414c37-d074-4487-bfeb-0efa09b237d8"/>
</p>
<p>
Under permission level click read/write and then click share
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/32258a97-cc4a-4bea-ad3b-240c496013e5"/>
</p>
<p>
To finish click done 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/23084462-438d-4269-81a4-502835dc8b59"/>
</p>
<p>
Then click close 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/d9c7e980-c5a3-4608-b34f-e2f546e30dc9"/>
</p>
<p>
Right click no access and click properties
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/82ae32c0-cc32-4924-a1b0-2e36e1fda214"/>
</p>
<p>
Then click the sharing tab and then click share 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/f7a912a9-b9a1-47df-830e-80c3e78c58b3"/>
</p>
<p>
Next in the permission level click read/write then click share 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/fb926a23-51f1-49a0-850d-1c2470ce876f"/>
</p>
<p>
To finish click Done 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/0ddb12bd-cc55-46e2-a404-a733fd7f6e82"/>
</p>
<p>
Then close the file 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/c968dc0d-81aa-4176-a03c-e515ac9d3385"/>
</p>
<p>
Next go to DC-1 VM and go to Network > dc-1 in file explorer and click read access 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/1a8001fc-a8eb-4338-8002-f77e938b839a"/>
</p>
<p>
Now right click go to new and click text document 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Network-File-Shares-and-Permissions/assets/143027686/56ca95a4-be4f-4037-8bb8-5a39b88bfa47"/>
</p>
<p>
Next you will see that we dont have permission to create the file 
</p>
<br />
