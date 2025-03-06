# Active_Directory_Preparation

<p align="center">
<img src="https://i.imgur.com/dD3HdHo.jpeg" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Preparation in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create two (2) vitrual machines
- Set client to use Domain controller as DNS server
- Step 3
- Step 4

<h2>Deployment and Configuration Steps</h2>

<p>
In this first section, the preparation for setting up Active Directory will be shown following the steps listed above. Virtual machines would be set up, one of which would act as a *Domain Controller* running Windows server while the other would act as a *Client* running Windows 10.<br /> 

We'll start off by creating a Resource group.  Resource Group is a container that holds related resources for an Azure solution. It helps organize, manage, and monitor resources such as virtual machines, databases, storage accounts, and networking component
</p>
<br />
<p>
<img src="https://i.imgur.com/qwgqJOD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p> 
<p>
Next, we'll create a Virtual Network. Once it is created, we'll move on to creating the virtual machines. <br /> A Virtual Network is a foundational networking service that enables secure communication between Azure resources, the internet, and on-premises networks. It is similar to a traditional network in an on-premises data center but provides the scalability and flexibility of the cloud.
<br />

<p>
<img src="https://i.imgur.com/ia58fYB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will have two(2) virtual machines(VM) created for this project. The first VM will serve a the Domain Controller(DC) while the other will serve as the client. 
<br /><br /> A Domain Controller (DC) is a server in a Windows Server Active Directory (AD) environment that manages network security, authentication, and access control. It is responsible for authenticating and authorizing users and computers in a domain by handling login requests, enforcing security policies, and managing user accounts.
<br /> <br /> FIRST VIRUAL MACHINE<br />
Name: DC-1<br />
Operating System: Windows (Windows Server 2022 Datacenter Azure Edition)
<br />
SECOND VIRTUAL MACHINE(VM)<br />
Name: client 1<br />
Operating System: Windows (Windows 10 Pro) <br />

To create a virtual machine, navigate to "Virtual Machines", choose the Resource group,  name the VM, select the region, select the image (base operating system), select the size (to support the workload to be run). On the networking page, make sure the Virtual network created earlier is slected. Click "Review+Create" and then "Create". 
<br />
Repeat the same process to creat both Virtual machines
Now we have the virtual machines running, the Domain Controller's NIC(network Interface card) Private IP address would be set to static. 
</p>
<br />

<p>
<img src="https://i.imgur.com/2cdkZFq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
