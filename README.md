# Active Directory & ServiceNow Help Desk Simulation Lab

A hands-on IT support lab combining Windows Server 2019, Windows 10, Active Directory, and ServiceNow ITSM to simulate common Tier 1 help desk incidents.

The project demonstrates Windows domain administration, user account management, troubleshooting, incident documentation, and IT service management workflows.

## Technologies & Tools

- Windows Server 2019
- Windows 10 Pro
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers (ADUC)
- Group Policy Objects (GPO)
- ServiceNow ITSM (Incident Management)
- Oracle VirtualBox
- Remote Desktop Protocol (RDP)

## Lab Environment

Built a virtualized Windows environment using VirtualBox consisting of:

- Windows Server 2019 configured as a domain controller.
- Custom Active Directory domain: `alexlab.local`.
- Windows 10 Pro client machines joined to the domain.
- Domain user accounts managed through Active Directory Users and Computers.

## Project Objectives

- Simulate common Tier 1 IT support requests.
- Troubleshoot Windows authentication and account access issues.
- Manage user accounts and permissions through Active Directory.
- Document incidents, investigation findings, and resolutions in ServiceNow.
- Practice incident lifecycle management, including ticket creation, status updates, work notes, and resolution documentation.

## Help Desk Scenarios

### 1. Active Directory Account Lockout

**Incident:** A user reports being unable to log into their Windows 10 workstation after multiple unsuccessful authentication attempts.

**Troubleshooting workflow:**

1. Review the incident reported by the user in ServiceNow.
2. Investigate the user's account in Active Directory Users and Computers.
3. Identify the account lockout.
4. Unlock the account through ADUC.
5. Verify successful authentication on the Windows 10 client.
6. Update the ServiceNow incident with investigation findings and resolution notes.

**ServiceNow workflow:**
- Create and categorize the incident.
- Assign an appropriate priority.
- Update the incident status as troubleshooting progresses.
- Document investigation steps using Work notes.
- Record the resolution and close the incident.

### 2. Password Reset & Account Management

Practice common account administration tasks, including password resets, user account changes, and login troubleshooting through Active Directory Users and Computers.

### 3. Group Policy Administration

- Created and configured Group Policy Objects to restrict Control Panel access.
- Applied policies to domain users and computers.
- Verified policy updates using `gpupdate /force`.

### 4. Windows Remote Support

- Configured Remote Desktop for remote troubleshooting.
- Managed local Windows user accounts.
- Installed third-party software and investigated application errors.

## ServiceNow Incident Management

Used ServiceNow ITSM to simulate an enterprise help desk ticketing workflow.

Practiced:
- Incident creation and categorization.
- Caller and assignment management.
- Impact, urgency, and priority classification.
- Incident status tracking.
- Internal work notes and troubleshooting documentation.
- Resolution notes and incident closure.

## Screenshots & Demonstrations

Screenshots documenting the lab environment and troubleshooting workflows will be added here.

Planned evidence:
- [ ] VirtualBox Windows Server and Windows 10 environment.
- [ ] Active Directory domain and user management.
- [ ] Account lockout and subsequent unlock.
- [ ] ServiceNow incident record.
- [ ] ServiceNow work notes and resolution documentation.

## Key Takeaways

This project provided practical experience combining Windows domain administration with IT service management workflows. It demonstrates how a Tier 1 support technician can investigate user-reported issues, troubleshoot underlying technical problems, document findings, and track incidents through resolution.

**Note:** This is a personal learning and simulation environment. ServiceNow incidents and troubleshooting scenarios are simulated and are not associated with a production IT environment.
