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

- Configure approproate users (roles, departments, etc.)
- Configure SLA Plan
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/OO1oam2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access to. To configure role settings: 
  <ul>
    <li>Admin Panel -> Agents -> Roles</li>
    <li> Create Supreme Admin -> Set permissions</li>
  </ul>
</p>
<br />

<p>
<img src="https://i.imgur.com/6sp7ggG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Departmen. To configure department settings: 
  <ul>
    <li>Admin Panel -> Agents -> Departments</li>
    <li>Create System Administrators -> Set permissions or add members (if applicable)</li>
  </ul>
</p>
<br />

<p>
<img src="https://i.imgur.com/9J1eC7w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Teams allow you to pull agents from different departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter. Teams permissions will supersede the parameters of the agents’ department rules. To configure team settings:
  <ul>
    <li>Admin Panel -> Agents -> Teams</li>
    <li>Create Level II Support -> Set permissions (if applicable)</li>
  </ul>
</p>
<br />

<p>
<img src="https://i.imgur.com/iUdRGfP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To allow anyone to create tickets:
  <ul>
    <li>Admin Panel -> Settings -> User</li>
    <li>Make sure "Registration Required: Require registration and login to create tickets" is unchecked</li>
    <li>Save changes</li>
  </ul>
</p>
<br />

<p>
<img src="https://i.imgur.com/2qfGYAt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Agents are given access to the help desk with the intent to respond and resolve the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. To configure agent settings:
  <ul>
    <li>Admin Panel -> Agents -> Add New</li>
    <li>Add agent 1 -> Set permissions</li>
    <li>Add agent 2 -> Set permissions</li>
  </ul>
In this case, Jane Doe and John Cena was created.
</p>
<br />

<p>
<img src="https://i.imgur.com/rDiEYQT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Users can now create an account and log-in to create a ticket or check a ticket’s status. As always with osTicket, users or ticket creators are associated with their email address as the unique identifier of each user. To configure user (customers) settings:
  <ul>
    <li>Agent Panel -> Agents -> Add New</li>
      <li>Add user 1 -> Set permissions</li>
      <li>Add user 2 -> Set permissions</li>
  </ul>
In this case, Karen Martinez and Ted Bezos were created as users
</p>
<br />
