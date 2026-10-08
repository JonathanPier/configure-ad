<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
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

- Install Active Directory
- Create a Domain Admin user within the domain
- Join Client-1 to your domain (mydomain.com)
- Setup Remote Desktop for non-administrative users on Client-1
- Create a bunch of additional users and attempt to log into client-1 with one of the users


<h2>Install Active Directory</h2>

<p>
<img width="872" height="416" alt="image" src="https://github.com/user-attachments/assets/afcc31af-5a2c-47c9-b3c1-baba5a4f8995" />
<img width="874" height="446" alt="image" src="https://github.com/user-attachments/assets/c5eaab87-d97d-4268-b286-b8daf05c6ec3" />
<img width="1103" height="550" alt="image" src="https://github.com/user-attachments/assets/05aaf1e3-5f82-4255-98d7-113893731bf5" />
<img width="1076" height="472" alt="image" src="https://github.com/user-attachments/assets/a6c75d22-3747-4e85-bebe-7d864cac31e4" />
<img width="1092" height="546" alt="image" src="https://github.com/user-attachments/assets/970a73d6-45d6-4db1-a97e-a9eb1f9a5772" />


</p>
<p>
Active Directory is an important technology used in many organizations to manage computers, users, and network resources. Active Directory, commonly known as AD, is a directory service developed by Microsoft for Windows-based networks. It provides a centralized system for managing users, computers, security, and access to resources. Organizations install Active Directory because managing a large number of users and computers individually can be difficult, time-consuming, and less secure.

One of the main reasons for installing Active Directory is centralized user management. In a company, there may be hundreds or thousands of employees who need access to computers and network resources. Instead of creating separate accounts on every computer, an administrator can create user accounts in Active Directory. Each employee can then use a domain account to log in to authorized computers and access the resources they need. This makes account management much easier for the IT department</p>
<br />


<h2>Create a Domain Admin user within the domain</h2>

<p>
<img width="1052" height="606" alt="image" src="https://github.com/user-attachments/assets/b90f4b96-a9ca-465a-a7d1-5f545b57955d" />
<img width="857" height="576" alt="image" src="https://github.com/user-attachments/assets/8fbaa12c-f3c4-432b-ad8f-737ac4820c8d" />
<img width="1014" height="539" alt="image" src="https://github.com/user-attachments/assets/55c1af04-abb9-4a4d-abe7-26b169d6829a" />
<img width="1137" height="624" alt="image" src="https://github.com/user-attachments/assets/ff2384c6-cc38-44fa-8d0a-81ae33566bc3" />
<img width="1030" height="632" alt="image" src="https://github.com/user-attachments/assets/c2fd0e77-f611-4c3a-b50b-04d0aa4dd89b" />
<img width="777" height="502" alt="image" src="https://github.com/user-attachments/assets/61573020-f1fd-40ab-892a-fef1c604e2f4" />
<img width="989" height="361" alt="image" src="https://github.com/user-attachments/assets/dedec804-30ba-44c8-841b-bbc60e580520" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


<h2>Join Client-1 to your domain (mydomain.com)</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


<h2>Setup Remote Desktop for non-administrative users on Client-1</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


<h2>Create a bunch of additional users and attempt to log into client-1 with one of the users</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
