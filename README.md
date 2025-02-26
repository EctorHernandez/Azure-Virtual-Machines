<p> 
<h1>Azure Virtual Machines</h1>
</p>
<p align="center">
<img src="https://i.imgur.com/LBQRQjX.png" alt="Traffic Examination"/>
</p>

<h1>Virtual Machine (VM) Creation in Azure</h1>
In this guide, we will learn how to create, deploy, and manage Virtual Machines using Microsoft Azure as well as go over some cost saving tips to help individuals and organizations.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure
- Virtual Machines
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>

- Step 1: Sign in or Create Microsoft Azure subscription
- Step 2: Begin VM Creation
- Step 3: Basic Tab overview
- Step 4: Disk Tab overview
- Step 5: Networking Tab Overview
- Step 6: Management Tab Overview
- Step 7: Review and Create

<h2>Sign in or Create Microsoft Azure subscription</h2>

<p>
<img src="https://i.imgur.com/jqjVkFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using your Computer search for Microsoft Azure and select the the offical Microsoft link. From here it will take you the page seen above. On the Azure page you can sign in or create an account. You need to do this to move forward.
</p>
<br />

<h2>Use Azure VM section to create machine</h2>

<p>
<img src="https://i.imgur.com/hPgd5az.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After signing in or up for Azure use either the search bar or the VN tab (seen above) select the VN feature in Azure to create a new virual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/zw2WpGM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select the create -> Azure Virtual machine
</p>
<p>
<img src="https://i.imgur.com/rQevqkk.png" height="45%" width="45%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Basics Tab</h2>

<h3> On the Basics tab we will select the primary setting for the VN. Below find steps that guide on what each section of this tab do.</h3>

<p>
<img src="https://i.imgur.com/dOX25pZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

 

</p>


- Step 1: Subscription:
    >Choose the subscription you'd like to use for the VM. This is where the the VN will be billed to.
    > <p>
<img src="https://i.imgur.com/DsbAq4T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 2: Resource Group:
    >Either create a new resource group or select an existing one. Resource groups help you organize your Azure resources.
     > <p>
<img src="https://i.imgur.com/0oeMxur.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 3: Virtual Machine Name:
    >  Provide a unique name for your VM.
    > <p>
<img src="https://i.imgur.com/wk8AOfj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 4: Region:
    >Select the Azure region where you want the VM to be located. Choose a region near you or your customers for better performance.
    > <p>
<img src="https://i.imgur.com/R7SDhxS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 5: Availability Options:
    >Choose between Availability Zones, Availability Sets, or No infrastructure redundancy required.
If high availability is important, consider selecting Availability Sets or Zones.
    > <p>
<img src="https://i.imgur.com/Uy3TCOS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 6: Image:
    >Choose the operating system image for the VM. Options include Windows Server, Ubuntu, RedHat, and others. You can also use custom images if required.
    > <p>
<img src="https://i.imgur.com/TgYamez.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 7: Size:
    >Select the size of the VM. You can choose based on the number of CPUs, memory, and storage you need. Azure provides recommended VM sizes based on the image selected.
    > <p>
<img src="https://i.imgur.com/Fa3woZK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 8:Authentication Type:
    >Choose between Password or SSH public key for authentication.
If you choose Password, enter a username and a secure password.
If you choose SSH public key, you'll need to provide an SSH public key for authentication.
    > <p>
<img src="https://i.imgur.com/8mqwcr1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Step 9: Inbound Port Rules:
    >Choose whether to allow inbound traffic to your VM. Common options are:
Allow selected ports (e.g., SSH, RDP).
Deny all inbound traffic (if you want to configure access later).
Disks Tab
    > <p>
<img src="https://i.imgur.com/Ry4A053.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

<p>
This finishes the Basics tab, next we'll select "Next: Disk" found at the bottom to set up Disk information.
</p>
<img src="https://i.imgur.com/JAl7Z8G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</b>

<br />

<h2>Disk Setup Tab</h2>
<p> In this section we'll go over the basic disk settings</p>
<p>
<img src="https://i.imgur.com/EZe8Gmo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- OS Disk Size:
  > The size of the disk used to store the operating system for a virtual machine (VM)
- OS Disk Type:
  > Select the type of disk: Standard HDD, Standard SSD, or Premium SSD
- Data Disks:
  > If you need additional storage, you can add data disks later. Data disks are separate from the OS disk and can be attached to the VM.

</b>

<h2>Networing Tab Overview</h2>
<p>Here, you’ll configure the networking settings for your VM.</p>
<p>
<img src="https://i.imgur.com/HTKHdOH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Virtual Network (VNet):
  > Select an existing Virtual Network or create a new one.
- Subnet:
  > Select a subnet within the VNet, or create a new one.
- Public IP:
  > If you haven't set a public IP previously, you can configure one here. This is essential for remote access.
- Network Security Group (NSG):
  > This is like a firewall. Choose an existing one or create a new one. The NSG defines which inbound and outbound traffic is allowed to and from the VM.
- Load Balancer:
  > If you are setting up a scalable VM environment, you can configure a load balancer here. Otherwise, leave it as None.


</b>
<h2>Management Tab</h2>
<p>This tab helps with monitoring and management configurations.</p>
<p>
<img src="https://i.imgur.com/VbEsyJ5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 

- Monitoring:
  > Choose whether you want to enable monitoring tools like Boot Diagnostics, Guest OS Diagnostics, or Azure Security Center.
- Auto-shutdown:
  >Optionally, you can set up an auto-shutdown time to save costs by automatically stopping the VM at a set time each day.
- Identity and Auto-scaling:
  > If applicable, configure VM identity and scaling options here.

</b>
<h2>Review + Create</h2>
<p>Once you’ve configured all your options, click Review + Create. Azure will display a summary of your VM configuration.</p> 
<p>
<img src="https://i.imgur.com/KC39vds.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p> 

- Review the settings to ensure everything is correct.
- If everything looks good, click the Create button.
<p>Azure will begin the deployment of your virtual machine. This can take a few minutes to complete.</p>
</b>
<h2>Connect to Your Virtual Machine</h2>
<p>Once the VM is created, you’ll need to connect to it:
</p>
- For a Windows VM:
In your Windows computer go to your search bar and search for Remote Desk Top
<img src="https://i.imgur.com/OGD4jw0.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>Select Remote Desktop Connection to open up the connection window.</p>
<p>Once opened take the public IP Address from the VN you made and type it into the field. 
After that use the user name and password you created back in the basics tab to sign into your new virual machine.</p>
<p>Select connect</p>
<P></P>
<img src="https://i.imgur.com/CU5rOq1.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
 
