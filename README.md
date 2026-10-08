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
In a Windows Active Directory environment, creating a Domain Admin user is important for managing and maintaining the organization's network. A Domain Admin is a user account that has administrative privileges across the Active Directory domain. These privileges allow authorized IT administrators to manage users, computers, security settings, and other resources within the domain from a centralized location. However, because Domain Admin accounts have extensive permissions, they should be created and used carefully.

One of the main reasons for creating a Domain Admin user is to centrally manage the domain. In an organization, administrators may need to create, modify, or remove user accounts, manage computer accounts, reset passwords, and configure different network resources</p>
<br />


<h2>Join Client-1 to your domain (mydomain.com)</h2>

<p>
<img width="1012" height="605" alt="image" src="https://github.com/user-attachments/assets/14e8fc2c-ee1b-4713-9413-fe785fbc396e" />
<img width="1014" height="613" alt="image" src="https://github.com/user-attachments/assets/c95bc029-484f-45a8-9631-95c5b0ce8cf9" />
<img width="999" height="607" alt="image" src="https://github.com/user-attachments/assets/841bdf64-ce6e-4595-815a-42bd89f80dc5" />
<img width="978" height="589" alt="image" src="https://github.com/user-attachments/assets/80557496-a707-4d02-99f1-3bcab389d9c6" />
<img width="940" height="497" alt="image" src="https://github.com/user-attachments/assets/15186226-fc86-4962-a59a-7ef542c49e76" />
</p>
<p>
Joining Client-1 to the domain is an important step when setting up a Windows Active Directory network. A domain allows computers and users to be managed centrally by a Windows Server running Active Directory Domain Services (AD DS). By joining Client-1 to the domain, the computer becomes part of the organization's network and can communicate with the domain controller for authentication, security, and management purposes.

One of the main reasons for joining Client-1 to the domain is centralized user authentication. Before joining the domain, Client-1 normally uses local user accounts that are managed only on that individual computer. After joining the domain, users can sign in using their domain accounts, such as COMPANY\John. The domain controller verifies the user's credentials and determines whether the user is authorized to access the network</p>
<br />


<h2>Setup Remote Desktop for non-administrative users on Client-1</h2>

<p>
<img width="824" height="595" alt="image" src="https://github.com/user-attachments/assets/cd58fe13-defc-43a8-a517-40817c964af4" />
<img width="1180" height="664" alt="image" src="https://github.com/user-attachments/assets/7902a922-6d4c-4895-82bf-db9084b816ff" />
<img width="1097" height="716" alt="image" src="https://github.com/user-attachments/assets/27722c72-a202-442e-8fd8-0db20b3e36d2" />



</p>
<p>
Remote Desktop is an important Windows feature that allows a user to connect to and control a computer from another location through a network. In an Active Directory environment, setting up Remote Desktop for non-administrative users on Client-1 allows authorized employees to remotely access their assigned computer without giving them unnecessary administrative privileges. This provides flexibility while maintaining appropriate security and access control.

One of the main reasons for enabling Remote Desktop for non-administrative users is remote access. Employees or authorized users may need to access Client-1 without being physically present at the computer. For example, a user might need to access files, applications, or work-related settings from another computer within the organization. Remote Desktop allows the user to connect to Client-1 using their authorized domain credentials.

Another important reason is user productivity. In a workplace, employees may work from different locations or need to access their office computer remotely. By allowing approved non-administrative users to use Remote Desktop, they can continue working with the applications and resources available on Client-1. This can reduce the need for users to be physically present at their workstation.</p>
<br />


<h2>Create a bunch of additional users and attempt to log into client-1 with one of the users</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
