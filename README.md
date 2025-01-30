<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create tickets
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/sVa324O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, log in using the admin username and password created during the osTicket installation.
</p>
<br />

<p>
<img src="https://i.imgur.com/rrHeu3P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once logged in, follow these steps to configure roles:

Navigate to the Admin Panel.
Go to Agent > Roles.
Create a new role named Supreme Admin.
Assign all available permissions to this role.
Roles are used for grouping permissions to streamline access management.
</p>
<br />

<p>
<img src="https://i.imgur.com/NzzjhiA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure departments:

Go to Agents > Departments.
Add a new department named SysAdmins.
Note that Access is used to assign agents to the department, but this step will be done later since no agents have been created yet.
</p>
<br />

<p>
<img src="https://i.imgur.com/6jCB8Ko.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure teams:

Navigate to Agents > Teams.
Add a new team and name it Online Banking.
Remember, teams can include agents from different departments, allowing for cross-department collaboration.
</p>
<br />

<p>
<img src="https://i.imgur.com/lHP8wLT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To allow anyone to create tickets:

Navigate to Settings > Users.
Ensure the option "Unregistered users can create tickets" is checked.
</p>
<br />

<p>
<img src="https://i.imgur.com/K3PvNhw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure agents:

Navigate to Agents > Agents.
Add a new agent by filling out the required details.
In the Agents tab, you can:
Assign agents to Teams and Departments.
Assign Roles and manage Permissions.
For example, you've created:

Jane (Department: SysAdmin)
John (Department: Support)
</p>
<br />

<p>
<img src="https://i.imgur.com/1NkKpDb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To add users (customers who report issues):

Go to the Agent Panel.
Navigate to Users and select Add User.
Fill in the user's details and save.
For example, you've created a user named Karen.
</p>
<br />

<p>
<img src="https://i.imgur.com/kSEkf2L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure an SLA:

Navigate to the Admin Panel > Manage > SLA.
SLAs (Service Level Agreements), which are set expected response and resolution times for customer issues, ensuring consistent support.
For example, you created three SLA levels:

Sev-A: Grace Period: 1 hour, Schedule: 24/7
Sev-B: Grace Period: 4 hours, Schedule: 24/7
Sev-C: Grace Period: 8 hours, Schedule: Business Hours
</p>
<br />

<p>
<img src="https://i.imgur.com/0FO6zeQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To configure Help Topics:

Under Manage, select Help Topics.
Help topics allow users to choose an issue category when creating a ticket.
For example, you created 5 help topics:

Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other
</p>
<br />
