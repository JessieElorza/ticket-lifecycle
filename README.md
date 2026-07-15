# ticket-lifecycle
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 11(Desktop)
- Windows 11</b> (25H2)

<h2>Ticket Lifecycle Stages</h2>

- New Ticket
- Assignment and Communication
- Transferring
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<p>
<img src="https://github.com/user-attachments/assets/a189fca3-89ca-452b-bf02-f825cb5a9132" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/f97d8ade-47cc-4189-9fbb-8a3a0166d079" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p> 
<p>
Begin by navigating to Admin Panel -> Agents -> Departments. Check Departments and Delete the Maintenance Department. This will ensure ticket flow and visibility and that tickets won't be routed to an unused department.
</p>
<br />

<h2></h2>

### Ticket #1

<br />
<p>
<img src="https://github.com/user-attachments/assets/8e1c8371-53ed-4c4e-aa69-a422f765d05b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket support ticket URL: http://localhost/osTicket/
</p>
<p>
Open a new page for the end users. Once link is copied and pasted into the URL in the virtual machine it will direct you to the end users ticket creation page for clients. Click Open a New Ticket.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/670560fc-6a18-4f1f-a81a-f06ab51a8b27" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the creation of the new ticket I will use a fake end user called "karen". In the ticket as karen select the help topic as "General Inquiry / Other" (It should be business critical outage, but it will be adjusted when observing the ticket as a support agent). Enter the clients scenario in the summary. Submit the ticket. Note: The email being used is fake and only for this tutorial.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/68f5519d-0a2b-4d6c-a271-5be49e4f4af9" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin login (http://localhost/osTicket/scp/login.php) we are going to login as john as a help desk agent. If you can't login as john look at the previous tutorial.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/ff154504-cf17-4269-a7e6-0c82bead9fab" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/87524f2c-e08e-434d-a28e-c693a2377c91" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/8cc7a793-b995-4902-9ac5-19ba057a7b70" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open the most recent ticket. Observe the properties of the ticket (Priority, Department, SLA, etc.). Notice john is in "read only" mode and can't do much except make an internal note. Feel free to leave a note, but its not necessary for the rest of this scenario. We now want to give John permissions to do more with the ticket so log out for now and we'll log back in as adminuser to upgrade John's access.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/ed64ca16-2289-4b49-a5d0-9ac7bc307dd6" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/06578b10-455a-40f9-ab76-ca9094055a5d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We now want to give John permissions to do more with the ticket. In the Admin Login page log back in as "adminuser". Navigate to Agent Panel -> Agents -> Agents -> John Doe -> Access. Give John "All access" and save changes.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/944c8794-f7bc-4eff-a912-5e79764619f3" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login back as john and view the ticket again. Notice you can change and modify the ticket. Update the Priority from "Normal" to "Emergency" as the entire banking system being down is a big issue and needs to be dealt with right away. Update SLA to "Sev-A" (Sev-A is 1 hour, 24/7) because it's urgent and needs to be completed ASAP. Update help topic from "General Inquiry / Other" to "Business Critical Outage" to catergorize the situation more aptly and communicate to the team precisely the severity of the situation and to cause less confusion about the issue.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/a161859c-1a34-4143-a298-0ef8ee4de3a6" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This issue needs someone else to work on it to ensure the issue is handled correctly. Change the "Assigned to" to "Jane Doe" and Transfer the ticket to the Department of "SysAdmins". With the way Johns permissions are setup he will no longer have access to the ticket but all his contributions will still be visible.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/5db5177c-0109-41a6-a652-2c1fc4014214" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Logout as john and login as Jane, the account we created in the prior tutorial. Open the ticket that was worked on and transferred to you by john. You can observe everything that john did in the ticket thread before the ticket was transferred.
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/9934626c-89ec-459a-b159-8c70e9be6d41" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/dee2d6c8-ca66-47a8-a56a-fad58782960a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
As jane we need to investigate and troubleshoot the issue, provide updates to the client user, and team, resolve and close the ticket. I left 2 replies as "Jane" as she worked with the team and client through the ticket. Once the ticket is completed changed the status from "Open" to "Resolved".
</p>
<br />

<h2></h2>

<p>
<img src="https://github.com/user-attachments/assets/d330f9d7-915d-4d28-8a0e-cf2f21c731c4" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After a quick follow up with the client, confirmation of the issue being resolved is confirmed by Karen and all systems are running smoothly. The ticket is completed and wechanged the status of the ticket from "Resolved" to "Closed".
</p>
<br />

<h2></h2>

<p>
height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<h2></h2>

### Ticket #2

<br />
<p>
<img src="https://github.com/user-attachments/assets/d330f9d7-915d-4d28-8a0e-cf2f21c731c4" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After a quick follow up with the client, confirmation of the issue being resolved is confirmed by Karen and all systems are running smoothly. The ticket is completed and wechanged the status of the ticket from "Resolved" to "Closed".
</p>
<br />
