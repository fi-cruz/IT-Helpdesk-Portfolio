# Azure Lab – Installing Active Directory Domain Services

## Objective

Deploy Active Directory Domain Services (AD DS) on a Windows Server 2022 virtual machine in Microsoft Azure and promote the server to a Domain Controller.

---

## Environment

- Microsoft Azure Virtual Machine
- Windows Server 2022 Datacenter (Desktop Experience)
- Remote access using RDP
- Domain created: fidel.local

---

## Deployment Steps

### 1. Access Server via Remote Desktop

Connected to the Azure Windows Server VM using Remote Desktop Protocol (RDP) with administrator credentials.

---

### 2. Install Active Directory Role

Opened **Server Manager** and initiated the role installation wizard.

Steps:

1. Click **Add Roles and Features**
2. Select **Role-based or feature-based installation**
3. Choose the local server
4. Select **Active Directory Domain Services**
5. Accept additional features required
6. Complete installation

---

### 3. Promote Server to Domain Controller

After installation completed:

1. Click the notification flag in Server Manager
2. Select **Promote this server to a domain controller**
3. Choose **Add a new forest**
4. Enter root domain name: `fidel.local`
5. Set Directory Services Restore Mode password
6. Complete configuration

The server automatically rebooted to finalize the promotion process.

---

## Verification

After reboot:

- Logged into the server using domain credentials
- Opened **Active Directory Users and Computers**
- Verified the domain `fidel.local` was successfully created

---

## Skills Demonstrated

- Windows Server administration
- Active Directory deployment
- Domain controller configuration
- Azure virtual machine management
- Enterprise identity infrastructure setup
