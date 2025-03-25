<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Ticket Lifecycle: Intake Through Resolution</h1>

In this lab, you’ll experience the full lifecycle of tickets within osTicket: from ticket intake as a user, through agent triage, resolution, and escalation. You'll observe how different ticket properties affect visibility and access, and learn how to properly work tickets to completion like a help desk pro.

---

<h2>🎥 Video Demonstration</h2>

- ### [YouTube: osTicket Ticket Lifecycle Walkthrough](https://www.youtube.com) *(Coming Soon)*

---

<h2>🧰 Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- osTicket Admin & Agent Panels
- Web Browser

---

<h2>🖥️ Operating System Used</h2>

- Windows 10 Pro (21H2)

---

<h2>🔐 Accessing the Panels</h2>

- **Admin / Analyst Login Page:**  
  `http://localhost/osTicket/scp/login.php`

- **End Users osTicket URL:**  
  `http://localhost/osTicket`

---

<h2>🎯 Lab Objectives</h2>

- Create tickets from the user portal
- Observe ticket properties in the agent panel
- Assign proper SLAs and departments
- Work tickets to completion based on severity
- Understand role-based access to tickets
- Reinforce the value of consistent ticket creation

---

<h2>📋 Lifecycle Practice Steps</h2>

### 🧼 Cleanup and Prep

1. **In Admin Panel**, go to:  
   `Agents > Departments`
   - Change `SysAdmins` to a **Top-Level Department**
   - DELETE the `Maintenance` department (do not archive)

---

### 🎫 Ticket 1: Business-Critical Outage

> As an end-user, submit a ticket:  
**"Entire mobile/online banking system is down"**

2. Log in to the user portal  
   Submit a new ticket with the above issue description

3. Log in as **Help Desk Agent (john)**  
   Observe the ticket’s current properties:
   - Priority
   - Department
   - SLA
   - Assigned To

4. Set the ticket properties:
   - SLA: `Sev-A (1 hour, 24/7)`
   - Department: `Online Banking`

5. Attempt to re-view/edit the ticket as **john**  
   - Can you still access or edit the ticket?
   - Note what happens if the department access doesn't match

6. Switch to **Agent jane**  
   - Work the ticket to completion

---

### 🎫 Ticket 2: Software Request

> As an end-user, submit a ticket:  
**"Accounting department needs Adobe upgrade, broken"**

7. As **Agent john**, observe the ticket:
   - Priority
   - Department
   - SLA
   - Assigned To

8. Set ticket properties:
   - SLA: `Sev-B (4 hours, 24/7)`
   - Department: `Support`

9. Work the ticket to completion as **john**

---

### 🎫 Ticket 3: Hardware Failure

> As an end-user, submit a ticket:  
**"CFO’s laptop will no longer turn on"**

10. As **Agent john**, observe the ticket:
    - Priority
    - Department
    - SLA
    - Assigned To

11. Set ticket properties:
    - SLA: `Sev-B (4 hours, 24/7)`
    - Department: `Support`

12. Work the ticket to completion as **john**

---

### 🔒 Escalation Behavior and Access Testing

13. Go back and set all existing tickets' properties:
   - Assign **Sev-A** to the **SysAdmins** ticket (the banking system one)

14. As **john**, attempt to view the ticket  
    - You may lose access due to department permissions

15. Switch to **Admin Panel**, give **john** view access to `SysAdmins` department

16. Switch back to **Agent Panel**  
    - Observe that the ticket is visible but **no longer editable**

17. Complete the remaining ticket work as needed.

---

<h2>📧 Email Notification Behavior</h2>

osTicket supports email alerts.  
Every time a ticket is updated, the end user can receive a notification and respond by replying to that email. This keeps users informed and allows two-way communication without logging into the portal.

---

<h2>🧠 Real-World Intake Scenarios</h2>

Tickets can be created in real life via:
- Email
- Phone calls
- Web forms
- Chat platforms
- Casual hallway encounters

⚠️ Even if you fix something on the spot, **create a ticket**.  
This improves visibility, metrics, and documentation.

---

<h2>📌 Final Notes and Practice Tips</h2>

- There’s a lot more to explore in osTicket — this lab scratches the surface.
- Practice the lab again until you can implement it start-to-finish with just this checklist.
- Experiment with the **email feature** to simulate real support flows.

---

<h2>💡 Building Technical Skill</h2>

Doing this lab repeatedly strengthens:
- Ticketing intuition
- Systems administration workflows
- End-user support skills
- Professional habits for real-world IT support

---

<h2>📬 Questions or Issues?</h2>

Open an issue in this repo or drop a comment on the walkthrough video if you need help.

---
