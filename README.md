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
<img src="https://github.com/user-attachments/assets/68f5519d-0a2b-4d6c-a271-5be49e4f4af9" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
Open the most recent ticket. Observe the properties of the ticket (Priotity, Department, SLA, etc.). Notice john is in "read only" mode and can't do much except make an internal note. Feel free to leave a note, but its not necessary for the rest of this scenerio.
</p>
<br />

<h2></h2>
