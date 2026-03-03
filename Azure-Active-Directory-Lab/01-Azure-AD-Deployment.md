# Azure Lab – Domain User Management

## Environment
- Microsoft Azure Virtual Machine
- Windows Server 2022 Datacenter (x64)
- Active Directory Domain Services Installed
- Domain: helpdesk.local

---

## Objective
Simulate enterprise user management tasks performed by Help Desk technicians.

---

## Tasks Performed

### 1. Created Organizational Units
- CorporateUsers
- SecurityGroups

### 2. Created Domain Users
- fcruz
- mlopez
- tadmin

### 3. Created Security Groups
- IT-Support (Domain Security)
- Accounting (Domain Security)

### 4. Assigned Group Membership
- fcruz → IT-Support
- tadmin, mlopez → Accounting

### 5. Simulated Help Desk Ticket
- Reset password for fcruz
- Disabled account
- Re-enabled account

---

## Skills Demonstrated
- Active Directory administration
- Organizational unit structuring
- Role-based access control
- Password reset procedures
- Account lifecycle management
