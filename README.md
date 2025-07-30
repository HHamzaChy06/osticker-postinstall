<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket Logo" width="400"/>
</p>

# osTicket - Post-Installation Setup & Configuration

This walkthrough explains how to configure osTicket after the initial installation to prepare it for production use. These steps include creating roles, departments, SLAs, and adjusting user permissions to ensure your help desk operates efficiently.

- **Admin / Analyst Login:** [Admin Portal](http://localhost/osTicket/scp/login.php)  
- **End-User Portal:** [Submit Tickets](http://localhost/osTicket)

---

## Tools and Environment

- Microsoft Azure (Virtual Machine hosting)
- Remote Desktop (RDP) for VM access
- Internet Information Services (IIS) to host osTicket

### Operating System
- Windows 10 Pro(21H2)

---

## Configuration Objectives

- Define roles and permissions for help desk agents.
- Organize ticket visibility using departments and teams.
- Set up Service Level Agreements (SLAs) for response times.
- Create help topics to streamline ticket creation.
- Adjust user access and security settings.

---

## Step-by-Step Configuration

### Step 1: Create Roles
1. Open **Admin Panel → Agents → Roles**.
2. Create a new role with full permissions (example: Supreme Admin).

![Create Role](https://github.com/user-attachments/assets/dd1f2373-7147-4a4d-9b20-565ea0f363ff)  
![Role Permissions](https://github.com/user-attachments/assets/9e2b8b13-ffb1-479f-aed5-64f45d590379)

---

### Step 2: Create Departments
1. Go to **Admin Panel → Agents → Departments**.
2. Add a department to manage ticket visibility (example: SysAdmins).

![Create Department](https://github.com/user-attachments/assets/1e219835-21a6-4987-a193-937a87d7f9b1)

---

### Step 3: Set Up Teams
1. Open **Admin Panel → Agents → Teams**.
2. Create a team that combines agents from different departments (example: Online Banking).

![Create Team](https://github.com/user-attachments/assets/7b0e4f93-e614-400c-b7a0-67e3f7f7e308)

---

### Step 4: Adjust User Settings
1. Navigate to **Admin Panel → Settings → User Settings**.
2. Recommended changes:
   - Disable ticket creation for unregistered users.
   - Require registration and login to submit tickets.

![User Settings](https://github.com/user-attachments/assets/bf61aa9b-d246-40fb-ab72-19a0e4fe4d7e)

---

### Step 5: Add Agents
1. Go to **Admin Panel → Agents → Add New**.
2. Add new agents and assign departments.  
   - Example: Jane (SysAdmins)  
   - Example: John (Support)

![Add Agent 1](https://github.com/user-attachments/assets/3bd02a07-516c-487c-a125-8b9a63159fca)  
![Add Agent 2](https://github.com/user-attachments/assets/39bfc106-1a9a-4085-a932-47dc1b35a8d2)  
![Agent Permissions](https://github.com/user-attachments/assets/ecde1247-be9a-443e-a808-c0897ccfe4cc)  
![Agent Assigned](https://github.com/user-attachments/assets/ea57ba21-029f-4ed5-9540-9316843e3849)

---

### Step 6: Add Users
1. Open **Agent Panel → Users → Add New**.
2. Add example users:
   - Karen
   - Ken

![Add Users](https://github.com/user-attachments/assets/206151c8-f6ce-4b02-8867-5b4d5f942857)  
![User List](https://github.com/user-attachments/assets/b5f4d93b-8314-44a9-9734-0b552e120a3c)

---

### Step 7: Configure SLAs
1. Go to **Admin Panel → Manage → SLA**.
2. Create Service Level Agreements:
   - Sev-A: 1 hour response (24/7)
   - Sev-B: 4 hours response (24/7)
   - Sev-C: 8 hours response (Business Hours)

![SLA Config 1](https://github.com/user-attachments/assets/b3e82dc9-8f86-4376-af93-d00097f34cf6)  
![SLA Config 2](https://github.com/user-attachments/assets/5e57a1cf-44ed-406d-aa0b-1f7cadac2343)  
![SLA Config 3](https://github.com/user-attachments/assets/65d45620-f0e4-4d95-a572-2b114a2920c4)

---

### Step 8: Create Help Topics
1. Navigate to **Admin Panel → Manage → Help Topics**.
2. Add topics to organize tickets:
   - Business Critical Outage
   - Personal Computer Issues
   - Equipment Request
   - Password Reset
   - Other

![Help Topics 1](https://github.com/user-attachments/assets/1c6ceb7d-2df0-4f65-9190-456ce9a422a9)  
![Help Topics 2](https://github.com/user-attachments/assets/20cf716b-9eb3-49f2-95ad-7a9db573dca1)

---

By completing these post-installation steps, osTicket is fully configured for real-world help desk operations. Roles, SLAs, and user settings ensure tickets are managed efficiently and securely.

