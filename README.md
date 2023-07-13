<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket: Post-Installation Configuration</h1>

In this tutorial I will outline the difference between Admin panel and Agent panel in osTicket. I will also do some post-Installation Configuration.

<h2>Objectives</h2>

-  Hands on Experience with osTicketing system
-  Experience as both the administrator AND the user of a ticketing system
-  Gain a better understanding of all parts of ticketing system such as <b>Tickets properties, SLAs, Departments, Permissions</b> and <b>Users</b>.

<h2>Environment and Technologies Used</h2>

-  Microsoft Azure (Virtual Machines/Compute)
-  Remote Desktop
-  osTicket
  
<h2>Operating System Used</h2>

-  Windows 10 pro

<h2>List of Prerequisites</h2>

-  All you need for this lab is to do <a href="https://github.com/danielbangm/osticket-prereqs/blob/main/README.md">the first part.</a>

<h2>Projects Steps</h2>

-  Step 1: Admin panel vs Agent panel

As soon as I log in osTicket using my credential provided in the previous section, I notice that I am using the Agent Panel because the is a possibility to click on the Admin panel. Basically to know which oanel you are using you have to check which one is showing and clickable. For example if the Admin panel is showing therefore you're using the Agent panel and vice verca. The 2 work environments are totally different.
![image](https://github.com/danielbangm/post-install-config/assets/22795502/7c63f20c-ec00-4528-9dfe-f823b11551b0)
![image](https://github.com/danielbangm/post-install-config/assets/22795502/719a38c0-1dc1-4bda-a337-7e99eff93963)

-  Step 2: Configure Roles

To configue Roles I just go to Admin Panel -> Agents -> Roles . To learn more about Roles and have a better understanding I went to <a href="https://docs.osticket.com/en/latest/Admin/Agents/Roles.html">osTicket definition of Roles.</a> Then I created a first Roles named Supreme Admin. 
![image](https://github.com/danielbangm/post-install-config/assets/22795502/a241a669-f6db-442e-a4f0-ac2bf3c70c0c)

-  Step 3: Configure Departments

To configure Departments I just go to Admin Panel -> Agents -> Departments. For a better understanding, read on <a href="https://docs.osticket.com/en/latest/Admin/Agents/Departments.html">osTicket definition of Departments.</a> Then I created my first Department named System Administrators.
![image](https://github.com/danielbangm/post-install-config/assets/22795502/322ca1fb-84e3-48e1-96bc-80c5733ee49f)

-  Step 4: Configure Teams

To configure Teams I go to Admin Panel -> Agents -> Teams. I learned about teams visiting <a href="https://docs.osticket.com/en/latest/Admin/Agents/Teams.html>osTickets definition of Teams.</a> Then I created 2 Teams: Level I Support and Level II Support
![image](https://github.com/danielbangm/post-install-config/assets/22795502/06345d06-37aa-4bad-a5be-e426e826b882)

-  Step 5: Allow Everyone to Create Tickets

In order to allow anyone to create tickets I am going to Admin Panel -> Settings -> User Settings and I just want to make sure that Registration Required: Require registration and login to create tickets 
![image](https://github.com/danielbangm/post-install-config/assets/22795502/f3fa94b6-f03d-481e-a1bd-0841fe5fd750)

-  Step 6: Configure Agents (workers)

Agent are the workers, the actual helpdesk technicians who going to use osTicket on a daily basis to attempt to resolve tickets. O I created 2 Agents Jane Doe and John Doe by going to Admin Panel -> Agents -> Add New
![image](https://github.com/danielbangm/post-install-config/assets/22795502/9ee0b99f-a6ef-4839-aa2b-15a2bec85c9d)

-  Step 7: Configure Users (customers)

Now I am going to configure 2 Users or Customers named Karen and Ken by going to Agent Panel -> Users -> Add New. These Users can create tickets in my system for my Agents to look at them.
![image](https://github.com/danielbangm/post-install-config/assets/22795502/cb561329-45a3-48fa-90cc-7dc5351bb2c8)

-  Step 8: Configure SLA

To create SLA I go to Admin Panel -> Manage -> SLA. And to better understand this I read <a href="https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html>osTicket definition of SLA.</a> I create 3 SLA with these level of severity Sev-A (1 hour, 24/7), Sev-B (4 hours, 24/7), Sev-C (8 hours, business hours)
![image](https://github.com/danielbangm/post-install-config/assets/22795502/4387b04e-3044-49ca-8c23-4976797b9566)

-  Step 9: Configure Help Topics

To configure Help Topic I go to Admin Panel -> Manage -> Help Topics. I create 4 Help Topics named Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset.
![image](https://github.com/danielbangm/post-install-config/assets/22795502/1c66a215-c59d-4f27-8630-ca3a284817a4)
