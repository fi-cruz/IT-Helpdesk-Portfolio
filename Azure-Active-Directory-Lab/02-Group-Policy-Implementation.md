# Azure Lab – Group Policy Implementation

## Objective
Demonstrate administrative control using Group Policy in an Active Directory environment.

## Environment
- Azure VM
- Windows Server 2022
- Domain: fidel.local

## Task
Restricted user access to Control Panel using Group Policy.

## Steps Performed
- Created new GPO: Disable-Control-Panel-Policy
- Configured Administrative Template
- Enabled “Prohibit access to Control Panel”
- Linked GPO to CorporateUsers OU

## Security Concept Demonstrated
- Centralized policy management
- Least privilege enforcement
- Enterprise-level compliance control
