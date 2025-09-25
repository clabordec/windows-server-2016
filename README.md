<p align="center">
<img src="https://github.com/user-attachments/assets/ba0dfda5-4426-4e1d-b8fc-b91f973aedb4" width="650" alt="Microsoft Active Directory Logo"/>
</p>



<h1>Installing and setting up Windows Server 2016 in VMware Workstation Pro</h1>
This project outlines the installation and set up of Windows Server 2016 along with the installation and management of Active Directory and Group Policy Management within VMware Workstation Pro 17.<br />


<h2>Environments and Technologies Used</h2>

- VMware Workstation Pro (Virtual Machines/Compute)
- Active Directory Domain Services

<h2>Operating Systems Used </h2>

- Windows Server 2016

<h2>High-Level Deployment and Configuration Steps</h2>

- Install and set up Windows Server 2016 onto the VM
- Add Active Directory Domain Services to the Server
- Promote the server as the Domain Controller

<br>


<h1>Deployment and Configuration Steps</h1>

## Installing and setting up Windows Server 2016
### Go to a search browser and type in the following `windows server 2016 iso download` choose the highlighed link
<p>
<img src="https://github.com/user-attachments/assets/9df76665-fd60-4efd-900d-9f5e17768a74" width="550" alt="Disk Sanitization Steps"/>
</p>

### Click on the `64-bit edition` download, based on your network speed, this may take between 5-30 minutes based on your computer specs
<p>
<img src="https://github.com/user-attachments/assets/dde6fcdf-6a2c-4e53-ae5e-57a6ce98da2d" width="550" alt="Disk Sanitization Steps"/>
</p>

### Save the ISO in any location, in this case I have saved the ISO to the following location, I've also renamed the ISO image:
<p>
<img src="https://github.com/user-attachments/assets/4e7c94c5-7322-4b84-b913-4bab2cfe4471" width="550" alt="Disk Sanitization Steps"/>
</p> 

### Open VMware Workstation Pro and create a new VM
<p>
<img src="https://github.com/user-attachments/assets/cc525cd1-4138-4a4b-84db-7d0f720788ba" width="550" alt="Disk Sanitization Steps"/>
</p>

### Click Next
<p>
<img src="https://github.com/user-attachments/assets/b99d9086-cb9f-47e6-b9d6-6677b41b1386" width="550" alt="Disk Sanitization Steps"/>
</p>

### To aviod any issue with the VM starting up successfully, choose `I will install the operating system later.` radio option, then click next
<p>
<img src="https://github.com/user-attachments/assets/600e745f-0ce4-4dbc-abf7-bf99e481a92d" width="550" alt="Disk Sanitization Steps"/>
</p>

### Select `Microsoft Windows` as the OS, and `Windows Server 2016` as the version
<p>
<img src="https://github.com/user-attachments/assets/7df34f80-20ad-4228-84f6-65b1dda50bff" width="550" alt="Disk Sanitization Steps"/>
</p>

### Give the VM a name, and choose a file path
<p>
<img src="https://github.com/user-attachments/assets/6aa43cac-1226-414a-a4bf-3ec0d2b37a89" width="550" alt="Disk Sanitization Steps"/>
</p> 

### Depending on your computer specs, assign the necessary amount of storage to the VM
<p>
<img src="https://github.com/user-attachments/assets/31ed9d1c-7047-41a9-b67e-fc86c6bb2616" width="550" alt="Disk Sanitization Steps"/>
</p>

### Click finish
<p>
<img src="https://github.com/user-attachments/assets/8a4c2b72-44db-42c4-9969-c1458343df83" width="550" alt="Disk Sanitization Steps"/>
</p>

### Go to the newly created VM, right-click on the VM and choose settings
<p>
<img src="https://github.com/user-attachments/assets/920cdfde-3eeb-4bec-bac4-1f648cc69abf" width="550" height="550" alt="Disk Sanitization Steps"/>
</p> 

### Based on the specs of your device, change the memory to a decent amount so that the VM will run smoothly
<p>
<img src="https://github.com/user-attachments/assets/37492e45-dcd8-4cf8-ac40-4ef5ba5804a9" width="550" alt="Disk Sanitization Steps"/>
</p> 

### Add the ISO file onto the VM, then click `OK`
<p>
<img src="https://github.com/user-attachments/assets/36d0e895-5e2c-4759-b54f-bb69aa7fe178" width="550" alt="Disk Sanitization Steps"/>
</p> 

### Power up the VM
<p>
<img src="https://github.com/user-attachments/assets/c33ca256-748f-4f2d-862c-23a028e7adfc" width="550" alt="Disk Sanitization Steps"/>
</p> 

### Once the VM is powered on, click within the VM and rapidly press space bar or any key of your choosing until you see the following, then hit enter
<p>
<img src="https://github.com/user-attachments/assets/673de096-0f20-48aa-9ece-1defee174ec9" width="550" alt="Disk Sanitization Steps"/>
</p>

### Click Next
<p>
<img src="https://github.com/user-attachments/assets/5a2f044b-79d7-4c62-a745-a7ad0d71afce" width="550" alt="Disk Sanitization Steps"/>
</p>

### Click Install now
<p>
<img src="https://github.com/user-attachments/assets/e437c752-91c3-4064-8cc8-2583498a19c8" width="550" alt="Disk Sanitization Steps"/>
</p>

### Choose the `Windows Server 2016 Standard Evaluation(Desktop Experience)` to have a Graphical User Interface(GUI) for the VM, then click `Next`
<p>
<img src="https://github.com/user-attachments/assets/c356ab87-b55d-4d3d-adae-20747bdfe77a" width="550" alt="Disk Sanitization Steps"/>
</p> 

### Go through the Mircosoft Software License Terms, click the checkbox to agree then click Next
<p>
<img src="https://github.com/user-attachments/assets/29749b67-470e-4e6b-a355-8703bf4f7a69" width="550" alt="Disk Sanitization Steps"/>
</p>

### Since this is a brand new VM with a brand new OS, choose the custom option to create a new OS
<p>
<img src="https://github.com/user-attachments/assets/150f1f9f-6ed7-467b-adf2-4589a65d9e66" width="550" alt="Disk Sanitization Steps"/>
</p>

### Ensure that the storage is correct, then click Next
<p>
<img src="https://github.com/user-attachments/assets/018feeaa-4429-440f-a465-bf199e8ce8cc" width="550" alt="Disk Sanitization Steps"/>
</p>

### Depending on your network speed, the process of installing the OS can take between 5-30 minutes
<p>
<img src="https://github.com/user-attachments/assets/6ff01d6e-89c6-46b6-9d01-6a1e63f24900" width="550" alt="Disk Sanitization Steps"/>
</p>

### Once the OS has been installed, input a password, be sure to remember the password, or you will need to re-install the OS if you forget it, then click Finish
<p>
<img src="https://github.com/user-attachments/assets/1c4d5835-9756-47b6-b92a-e715181386a6" width="550" alt="Disk Sanitization Steps"/>
</p>

### After inputting the new password, press Ctrl+Alt+Insert to unlock the Windows Start Screen within the VM
<p>
<img src="https://github.com/user-attachments/assets/f8a8e5ad-710b-47b6-978f-fe4a9e39d4bb" width="550" alt="Disk Sanitization Steps"/>
</p>

### Enter the new password
<p>
<img src="https://github.com/user-attachments/assets/ed45f5f3-75f0-45de-b840-9ece2dfd4d4a" width="550" alt="Disk Sanitization Steps"/>
</p>

### Once logged in, Server Manager will be the first application that will open
<p>
<img src="https://github.com/user-attachments/assets/8c57e57d-62a4-419d-a2b7-97162208121a" width="550" alt="Disk Sanitization Steps"/>
</p>

<br>

## Installing and setting up Active Directory
### Within Server Manager, go to Manage >> Add Roles and Features
<p>
<img src="https://github.com/user-attachments/assets/28842a3d-154e-43de-8485-3e4d7836935b" width="550" alt="Disk Sanitization Steps"/>
</p>

### Click Next
<p>
<img src="https://github.com/user-attachments/assets/ca78a244-d6c0-4d50-af1c-e5c1b2eb529c" width="550" alt="Disk Sanitization Steps"/>
</p> 

### Choose `Role-based or featured-based installation` then click Next
<p>
<img src="https://github.com/user-attachments/assets/472df778-2402-41ec-9328-9032fdff3cf4" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Choose `Select a Server from the server pool` then click Next
<p>
<img src="https://github.com/user-attachments/assets/e3de74af-56b1-4d33-92dd-ec5a65f5dccb" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Add the following `Active Directory Domain Services` Role then click Next
<p>
<img src="https://github.com/user-attachments/assets/208d19d9-3a48-4169-b262-f2b72b1543b5" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Make sure that Group Policy Management is checked then click Next
<p>
<img src="https://github.com/user-attachments/assets/baa0e613-1501-4f75-8919-36975906403e" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Click Next
<p>
<img src="https://github.com/user-attachments/assets/46e4e047-1843-4f30-9d00-70060a26e6cd" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Click Install after review all of the Roles and Features
<p>
<img src="https://github.com/user-attachments/assets/6836fed2-58b6-4a7f-ad3d-d40a61a1ff59" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />


## Promoting the server as a Domain Controller
### Once the installation for AD DS has been completed click on `Promote this server to a domain controller`
<p>
<img src="https://github.com/user-attachments/assets/0460ced4-e359-4f1c-98fb-0c87307ff1ce" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Under `Select the deployment operation` choose `Add a forest`, then provide a domain name, in this case I will use `chaanyah.com` as the domain name, then click Next
<p>
<img src="https://github.com/user-attachments/assets/36f6c3b3-0903-4462-92b6-0748abc561fa" width="550" alt="Disk Sanitization Steps" />
</p>
<br />

### Be sure to keep the `Forest Function Level` and `Domain Function Level` set to Windows Server 2016, and enter a secure password for the domain, then click Next
<p>
<img src="https://github.com/user-attachments/assets/fe61dff2-8390-445e-8714-fdfb8c981039" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Click Next
<p>
<img src="https://github.com/user-attachments/assets/67fc3d2c-4f59-4171-81a3-b8cfe23e274a" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### The NetBIOS domain name will appear as the domain name without the `.com`, click Next
<p>
<img src="https://github.com/user-attachments/assets/9d478166-6bfc-4c9e-8f02-1e3473c1f4b0" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Click Next
<p>
<img src="https://github.com/user-attachments/assets/fea0e96f-c539-4d0d-9431-cd757565f824" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Click Next
<p>
<img src="https://github.com/user-attachments/assets/318d9442-21fb-4364-a000-7ebf7cb8104e" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Make sure all prerequisites pass, ignore the warning signs, Click Install
<p>
<img src="https://github.com/user-attachments/assets/19f9aca7-c007-4fa1-9c63-4538671ddbf4" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Once the installation is complete, you will be prompted with the following message, the VM will automatically sign out in 5-10 seconds depending in Internet speed
<p>
<img src="https://github.com/user-attachments/assets/439dc6be-88ce-4525-91a6-aad4628deeb1" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Enter in the password that was created for the domain
<p>
<img src="https://github.com/user-attachments/assets/c98f1966-a837-4bf3-8ba5-23271779600e" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Go to Server Manager, then click on Tools, you will see all of the features for Active Directory, along with others that was installed
<p>
<img src="https://github.com/user-attachments/assets/53391199-f405-4d90-a789-9dd5f0e1b78d" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />


# End of Project
