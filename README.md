<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle </h1>
Ticket lifecycle for the open-source help desk ticketing system osTicket.<br />
<br />
Part 1: Ticket Creation (2 steps) <br />
Part 2: Answering tickets and troubleshooting Permissions (8 steps)<br />
Part 3: Assigning, escalating, and closing tickets (8 steps)<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure Active Subscription (Creation of Reasearch Group, VMs, Virtual Networks, Subnets)
- Enable Internet Information Services(IIS)
- PHP Manager
- Rewrite Manager
- C++ Redistributbal
- MySQL Server
- Install osTicket
- Assigning Permissions
  
- osTicket
- Chief User: james
- Agents: jane.doe and jon.doe
- 






<h2>Part 1 (Ticket Creation) Steps: 1 - 2 </h2>


![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/cb391b3e-9a4f-4df8-8d76-858ba9917545)
<p>
Step 1: Click open a New Ticket
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/1e7f050e-ce88-4fad-8086-edae2b12c883)
![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/3c3d2ce2-aa8d-49b8-97fd-c5c836122e5b)
![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/41cb0f73-c580-4e35-bedb-b949738ef997)
<p>
Step 2: Fill out the form with client and ticket information. Click Create Ticket. (ex: Thomas Engine, Bob Builder, Mac Donald)
</p>
<br />
<br />
<br />

<h2>Part 2: (Answering Tickets and troubleshooting Permissions) Steps: 1 - 8</h2>

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/c5d490ff-3ae9-49f7-8e01-4e15dd02f33f)
<p>
Step 1: Help desk will navigate to http://localhost/osTicket/scp/login.php to answer tickets. Enter credentials
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/5ec41bae-8f1b-4009-8a31-822c99ecd064)
<p>
Step 2: We know from Step 1, that 3 tickets have been created. We cannot see them currently becausee jane.doe does not have permissions. 
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/b57a4bc4-1d1a-439c-a762-c4f0f35cce74)
<p>
Step 3: Log Out as jane.doe and log in as Admin: james
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/18acc8b1-718b-4c50-9330-236f1fc43cd9)
<p>
Step 4: This is agent panel where we can view tickets. Click on ticket to see department (ex: When is the printing cominDg)
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/680b93bc-c296-4ddb-a9bb-f10b53d89cec)
<p>
Step 5: When need to give jane.doe permissions to the Department: Support, so she can answer support tickets.
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/35793aad-fd11-45d4-945f-b03c74bdf601)
<p>
Step 6:  Click Admin Panel -> Agents . This is a list of all Agents. Notice how jane.doe is in NOT in the Support department. Click Jane Doe -> Access
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/8f131eed-9325-41ec-b778-414b017593f3)
<p>
Step 7: We can change her primary department, or add extended access permissions to the Support. Add as Chief Admin, to the Support -> Save
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/7b6f6f91-000a-4c73-8892-59ca9bdd8901)
<p>
Step 8: Log out as admin. Log back in as jane.doe. Jane Doe with Chief Admin for Support can now see/answer the tickets. Note: Chief Admin was used as the example, but it is not best practice to give Admin to Agents that don't absolutely need it. It would be better to give them access only to what they need to perform their duties.
</p>
<br />
<br />
<br />


<h2>Part 3: (Assigning, escalating tickets, and closing) Steps: 1 - 8</h2>

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/f7a74d25-372f-4f2c-9e0d-5010c3bc5205)
<p>
Step 1: Click the ticket (Entire system not working)
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/c0495ddb-0ffa-4f65-87b0-8905570e926a)
![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/63a361dc-afeb-47d5-b490-3e1bc9853dfa)
<p>
Step 2: This is a huge business impacting incident, therefore we change Priority to Emergency. Changed Assigned To: jane.doe(whoever the escalation engineer is or queue manager, etc). Also we change the SLA to the most urgent: SEV-A
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/0dd0acdd-5d2f-494c-bdee-1a7f9fab8816)
<p>
Step 3: If Support is not equipped to handle the ticket, it may also be a good idea to escalate the department as well (ex: System Administrators)
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/28078867-8386-431a-8634-1e5c74fe527d)
<p>
Step 4: View of ticket history.
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/cd49acad-632e-4f63-bbb8-12dfb142e1f7)
<p>
Step 5: In this example, we leave the Ticket Status: Open, until it is resolved.
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/c30eb2f9-ef59-4e1a-b6f1-1aad7618a67f)
<p>
Step 5: Ticket has now been properly assigned to Jane Doe, and Priority has been escalated
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/c30eb2f9-ef59-4e1a-b6f1-1aad7618a67f)
<p>
Step 6: Ticket has now been properly assigned to Jane Doe, and Priority has been escalated
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/ff543722-c5ba-4c57-8797-68d8736253a9)
![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/16d19540-ae04-4785-9ad6-e65629e5640a)
<p>
Step 7: A response is posted to declare the ticket solved. Change ticket status to Resolved.
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/87e18877-2f31-4cd7-af33-6ae2fcd302e8)
<p>
Step 7: After resolving the ticket, it is removed from the ticket tab. If we want to see the ticket, click Closed,
</p>
<br />

![image](https://github.com/jameswsm/ticket-lifecycle/assets/170709350/749e14f2-585e-4144-bf04-05079e7a1ca3)
<p>
Step 8: This tab tells us important information like when a ticket is closed, and by whom.
</p>
<br />






