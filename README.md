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

- Windows 11 Pro</b> (25H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles (Grouping Permissions)
- Configure Departments (Ticket Visibility, Help Desk, SysAdmins, Networking)
- Configure Teams (Pull agents from different departments)
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA (Service Level Agreement)
- Configure Help Topics (when users create a ticket)

<h2>Configuration Steps</h2>

<p>
<img width="3199" height="1799" alt="image" src="https://github.com/user-attachments/assets/b4504637-394b-4237-93b4-1eb535bcbdc3" />
</p>
<p>
After signing in with your admin credentials for osTicket, you'll be greeted with this page. You'll want to click "Admin panel" located towards the top right of the page.
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/760b8d41-d018-4197-b2a3-2623a5f08333" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/dc30e63e-7ba5-4b2f-be8e-9ef8cab5ec56" />
</p>
<p>
Once you're in the admin panel, click on the agents tab, followed by the roles sub category. From there we'll create a new role titled "Supreme Admin".   
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1ca3add7-dd8a-4731-95a6-464adda2eb36" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/7ecf343d-b24f-45a3-8f80-fec30fc72c2c" />
</p>
<p>
Click on the tab labeled permissions and check every box. Including the ones under "Tasks" & "Knowledgebase". Go ahead and add the role when finished. 
</p>
<br />

<p>
<img width="1917" height="1079" alt="image" src="https://github.com/user-attachments/assets/8eb104e7-562e-4556-aa6d-2552e384d2e1" />
From there you'll click on Departments.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/198c2622-180e-40e4-b4ba-8a31ae62c781" />
Create a new department.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3af5a42a-5387-42cd-af46-3e3e054539e5" />
Leave the parent as "Top Level Department" and title the department "SysAdmins". We will assign agents access later on.
</p>
<br />

<p>
<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/586b5db5-39d2-424b-a0de-5041681971c4" />
From there you'll click on Teams.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/06a1b7af-dd3a-4c00-8516-f0f42c8e1e71" />
Create a new team titled "Online Banking".
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ef673c1e-3cbe-469b-9ece-6bbfa3963a4f" />
You can hover over the settings tab and select the users sub category. 
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1e81d599-93c8-4c16-b627-9daceef74906" />
All this information should be the same but the key box you want unchecked is "Registration Required".
</p>
<br />

<p>
<img width="1919" height="1077" alt="image" src="https://github.com/user-attachments/assets/9717d19b-23b7-4f4c-beb8-1bc6a83ebf29" />
After saving those changes, hover over the agents tab and click on the agents sub category. 
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/65b26348-df1c-4076-9deb-1532adf0bba8" />
Click "Add New Agent".
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ce89dc7e-cc63-4df2-82b0-77a9e30ffd15" />
After filling in the name, email, and username for the agent. Click on Set Password next to the username box, this will bring up another box.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/53d47289-974c-4efa-8ed1-3a6ec973d5b2" />
Uncheck the two boxes, and type the password in both text boxes. Click set to finish assigning the password for that agent.
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/37012c71-21f3-4f82-a428-0df983b7d831" />
Click on the tab labeled "Access", set the users Department to "SysAdmins" and Role to "Supreme Admin".
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/484acf13-7941-4c6f-bdb2-8d939c8e70e1" />
Click on the tab labeled "Teams" and add the user to the Online Banking team created earlier. Click Create to finsih the changes made to the Agent.
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/49023dd0-6dd1-4d3a-be49-3ab0f7639558" />
Click on the agents tab again, then click "Add New Agent" again. This agent will go to the support Department.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/82e1cea4-78a5-4995-9922-af75eb5e4626" />
Fill in the Name, Email, and username for the new agent. Then click on Set Password.
Same thing as the previous Agent, Uncheck the two boxes, and type the password in both text boxes. Click set to finish assigning the password for that agent.
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/32349292-99ef-431a-aa87-67b700959c85" />
Click on the tab labeled "Access", set the users Department to "Support" and Role to View Only. You can create it after that, no permissions need to be changed.
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/62fb7f67-2a02-4318-aa0e-3c6b088cfeba" />
After your two Agents have been created, Click on agent panel located on the top right of the page. You will notice the text switches from "Agent Panel to "Admin Panel" after clicking. 
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ce1cc4dd-83c5-4a19-915c-892fdc942fed" />
Click on the "Users" tab, then click "Add user". 
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b5f27ce3-3491-4690-b701-7a3ddb13d085" />
Fill in the Users Email and Name then click "Add User" to add them to the Directory.
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/876c48ad-3c2b-4f34-bc25-5bb967b15c24" />
Go back to the admin panel by clicking "Admin Panel" located at the top right of the page. 
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/1e129cfe-203e-48ef-a03a-06067d87b2a2" />
Hover over the Manage tab, then click on "SLA". We'll be adding three different SLA's each with different Grace Periods.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/65465c4c-2667-4b54-b544-1f20790e10a8" />
Click "Add New SLA Plan".
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f9de65e6-921f-43bd-9f3e-d8fa6ed5a0a2" />
Title the SLA "Sev-A", set the Grace Period to 1 hour, and the Schedule should be set to 24/7. After all that is set, click Add Plan.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2ca0c1a9-7845-4417-a806-e97699a389f2" />
Create a new SLA titled "Sev-B", set the Grace Period to 4 hours, and the Schedule to 24/7. Add the plan once complete.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b128fe5c-94ab-44ce-b571-640e45e59a6b" />
For the last SLA titled "Sev-C", set the Grace Period to 8 hours, and the schedule will be set to business hours unlike the other 2 SLA's that were just created. Add the plan once complete.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/450a3954-519a-49f1-83aa-a58141e06613" />
You should see all 3 SLA's that we're just created on the main SLA page.
</p>
<br />

<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/ac31ccd9-5abe-4e82-9435-8e6be90a9e54" />
Click on the "Help Topics" sub category and click "Add New Help Topic".
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c2f22195-5fae-42a7-80c1-67c13c7c7b07" />
Title the Topic "Business Critical Outage" and set the Parent Topic to "Report a Problem". After those are set, Add the Topic.
</p>
<p>
<img width="1919" height="1072" alt="image" src="https://github.com/user-attachments/assets/f545d277-752d-4e0e-a5bf-8a3ed279489b" />
Click on the "Help Topics" sub category and click "Add New Help Topic". Title this one "Personal Computer Issues" and set the Parent Topic to "Report a Problem". Add the Topic once set.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c666daf0-13c3-49af-b208-f6dd5f1bc8e7" />
Click on the "Help Topics" sub category and click "Add New Help Topic". Title this one "Equipment Request" and set the Parent Topic to "General Inquiry". Add the Topic once set.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0f384656-5fb4-4ebb-b5b2-c5dd3e51776c" />
Click on the "Help Topics" sub category and click "Add New Help Topic". Title this one "Password Reset" and set the Parent Topic to "Report a Problem". Add the Topic once set.
</p>
<p>
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c12c8d6a-b2e5-4510-8674-bf39213c4d88" />
Click on the "Help Topics" sub category and click "Add New Help Topic". Title this one "Other" and set the Parent Topic to "General Inquiry". Add the Topic once set.
</p>
<br />

This concludes the Post-install setup of osTicket.
