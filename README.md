<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Prerequisites</h2>

- If you haven't installed and setup osTicket yet on your machine, please follow the guide <a href="https://github.com/christianDCdev/osTicket-prereqs">here</a> and come back
- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>
<h3>&#9312; Configure Roles (used for grouping permissions)</h3>

<p>

- Once logged into osTicket, navigate to "Admin Panel" -> Agents -> Roles
- Click "Add New Role"
<img src="https://i.imgur.com/egyX7q9.png" height="80%" width="80%" alt="New Role window"/>

- Name the role for someone that has full access (in my case I named the role "Supreme Admin")
- Under "Permissions" tab, enable all check boxes
- Click "Add Role" once your finished, and if done correctly, your new role will be under the "Roles" list
<img src="https://i.imgur.com/52Hqo4p.png" height="80%" width="80%" alt="Role list"/>

</p>
<br />
<h3>&#9313; Configure Departments (used for ticket visibility)</h3>

<p>

- Within osTicket, navigate to "Admin Panel" -> Agents -> Departments
- Click "Add New Department" then fill out the following fields:
  - Parent: Top Level Department
  - Name: SysAdmins
<img src="https://i.imgur.com/aP0Rvsl.png" height="80%" width="80%" alt="New department page"/>

- Click "Create Dept"
  
</p>
<br />
<h3>&#9314; Configure Teams  </h3>

<p>

- Within osTicket, navigate to "Admin Panel" -> Agents -> Teams
- Click "Add New Team"
- Name the team "Online Banking" and click "Create Team"
<img src="https://i.imgur.com/IphnRA8.png" height="80%" width="80%" alt="New team page"/>
  
</p>
<br />
<h3>&#9315; Allow anyone to create a ticket</h3>

<p>

- Within osTicket, navigate to "Admin Panel" -> Settings -> Users
- Disable "Registration Required" box (should be unchecked)
- Click "Save Changes"
<img src="https://i.imgur.com/o5fMnC2.png" height="80%" width="80%" alt="User Settings"/>
</p>
<br />
<h3>&#9316; Configure Agents (employees / workers)</h3>

<p>

- Within osTicket, navigate to "Admin Panel" -> Agents -> Add New Agent
- Fill out necessary fields
<img src="https://i.imgur.com/sjJU9tz.png" height="80%" width="80%" alt="Agent creation"/>

- Within "Access" tab, assign department and role
<img src="https://i.imgur.com/k0GP3v9.png" height="80%" width="80%" alt="Agent dept and roleassignment"/>

- Within "Teams" tab, assign team, then click "Create" to finish
<img src="https://i.imgur.com/ndfpvuA.png" height="80%" width="80%" alt="Agent team assignment"/>

- In my case, I created 2 agents with the following assignments:
  - Agent 1:
    - Name: Jane Doe
    - Email Address: Jane@lognpacific.com
    - Username: jane
    - Password: Password1
    - Department: Support / SysAdmins
    - Role: Supreme Admin
    - Team: Online Banking
  - Agent 2:
    - Name: John Doe
    - Email Address: john@lognpacific.com
    - Username: john
    - Password: Password1
    - Department: Support
    - Role: View Only
    - Team: (Unassigned)
  
</p>
<br />
<h3>&#9317; Configure Users (customers)</h3>

<p>

- Within "Agent Panel", navigate to Users -> Add User
- Fill out necessary fields and click "Add User" to finish
<img src="https://i.imgur.com/ndfpvuA.png" height="80%" width="80%" alt="Add user page"/>
  
</p>
<br />
<h3>&#9318; Configure SLA</h3>

<p>

- 
  
</p>
