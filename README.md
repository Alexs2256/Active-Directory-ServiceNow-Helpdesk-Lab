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

## Troubleshooting Scenarios

### 1. Active Directory Account Lockout

<img width="674" alt="Active Directory account lockout simulation" src="https://github.com/user-attachments/assets/aae88e87-0786-4d43-bbda-c2d6bfbe5e15" />

[Video Demonstration](https://www.youtube.com/watch?v=n91-uzhOnew)

**Incident:** A user reports being unable to log into their Windows 10 workstation after multiple unsuccessful authentication attempts.

**Troubleshooting workflow:**

1. Reviewed the user's reported issue in ServiceNow.
2. Investigated the user's account in Active Directory Users and Computers.
3. Identified the account lockout.
4. Unlocked the account through ADUC.
5. Verified successful authentication on the Windows 10 client.
6. Updated the ServiceNow incident with investigation findings and resolution notes.

### 2. Password Reset & Account Management

**Incident:** A user reports being unable to access their Windows 10 workstation because they forgot their domain password.

**Troubleshooting workflow:**

<img width="682" height="465" alt="image" src="https://github.com/user-attachments/assets/31199274-bda8-4b25-8353-71b176b47469" />

1. Reviewed the password reset request in ServiceNow.
2. Located the user's account in Active Directory Users and Computers.
3. Verified the account status and identified the need for a password reset.
4. Reset the domain password through ADUC.
5. Verified successful authentication on the Windows 10 domain-joined client.
6. Documented the troubleshooting steps and resolution in ServiceNow.

### 3. Group Policy Administration

<img width="694" height="458" alt="image" src="https://github.com/user-attachments/assets/5126f8b7-2c53-47d2-9b13-04b4d7ff38f4" />

- Created and configured a Group Policy Object (GPO) in Group Policy Management on Windows Server 2019.
- Enabled the policy “Prohibit access to Control Panel and PC settings.”
- Linked the GPO to the appropriate domain or organizational unit.
- Ran gpupdate /force on the Windows 10 domain-joined client to apply the policy.
- Verified that the domain user could no longer access Control Panel or PC settings.

### 4. Windows Remote Support

- Configured Remote Desktop for remote troubleshooting.
- Managed local Windows user accounts.
- Installed third-party software and investigated application errors.
- Used administrative tools and diagnostic utilities to isolate and resolve common user-reported problems.

## ServiceNow Incident Management

Used ServiceNow ITSM to simulate an enterprise help desk ticketing workflow, documenting Active Directory troubleshooting scenarios through incident records.

**Practiced:**
- Incident creation and categorization.
- Caller and assignment management.
- Impact, urgency, and priority classification.
- Incident status tracking.
- Internal work notes and troubleshooting documentation.
- Resolution notes and incident closure.

**ServiceNow Incident Demonstration:**

<img width="1533" alt="ServiceNow incident management workflow" src="https://github.com/user-attachments/assets/d83c6c73-cc9e-4e61-8544-29240dc46ae6" />

<img width="1532" height="486" alt="image" src="https://github.com/user-attachments/assets/3a562e29-d009-462b-a3f2-160dccbf770c" />

[Video Demonstration](https://www.youtube.com/watch?v=gTaHLg82k9Y)

## Key Takeaways

This project provided practical experience combining Windows domain administration with IT service management workflows. It demonstrates how a Tier 1 support technician can investigate user-reported issues, troubleshoot underlying technical problems, document findings, and track incidents through resolution.

**Note:** This is a personal learning and simulation environment. ServiceNow incidents and troubleshooting scenarios are simulated and are not associated with a production IT environment.
