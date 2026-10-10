


| Ticket ID      | Category                  | Scenario/Task | Outcome | Tools & Skills |
| :--- | :--- | :--- | :--- | :--- |
| **TKT-001**     | Network Diagnostics  | Investigate network configuration and connectivity.  | Inspected IP configuration, renewed the DHCP lease, flushed the DNS cache and tested connectivity.   | Command Prompt, IP configuration, DNS, ping |
| **TKT-002**     | Active Directory Administration| Create a test domain user and assign appropriate group membership. | Created a test user and configured its security group membership. | Active Directory, user accounts, security groups |
| **TKT-003**     | File and Folder Permissions | Configure folder access for an Active Directory security group. | Configured NTFS permissions and tested folder access from a Windows client. |  Windows Server, NTFS permissions, security groups, file sharing |
| **TKT-004**     | Account Troubleshooting | Investigate a simulated domain account sign-in issue. | Identified a disabled test account and re-enabled it. | Active Directory, account troubleshooting |
| **TKT-005**     | Group Policy Management | Inspect domain password policy settings. | Reviewed password policy configuration and identified a potential security improvement | Group Policy, GPMC, Windows administration |
| **TKT-006**     | Windows Troubleshooting | Investigate Windows performance using built-in tools. | Monitored CPU and memory usage and inspected running processes under a simulated workload. | Task Manager, process monitoring, performance checks | 
| **TKT-007**     | Event Log Investigation | Investigate Windows events related to system errors. | Examined a critical system event and considered a possible cause in a VirtualBox lab. | Event Viewer, Windows Logs, error investigation |

<br><br>
## TKT-001: Network Diagnostics

Used Windows command-line tools to inspect network configuration, practise DHCP lease renewal, clear the DNS resolver cache and test connectivity.  
 
![IP Configuration](evidence/TKT-001-ip-config.png)

![IP Lease Renewal and DNS Cache](evidence/TKT-001-ipconfig-renew.png)

![Network Connectivity](evidence/TKT-001-connectivity-ping-test.png)

<br><br>

## TKT-002: Active Directory Administration

Created a test domain user and configured its security group membership in Active Directory.

![Test User Creation](evidence/TKT-002-user-creation.png)

![Security Group Membership](evidence/TKT-002-group-membership.png)

<br><br>

## TKT-003: File and Folder Permissions

Configured NTFS permissions to grant an Active Directory security group appropriate access to a folder.

![NTFS Permissions](evidence/TKT-003-ntfs-permissions.png)

![Folder Access Test](evidence/TKT-003-access-test.png)

<br><br>

## TKT-004: Account Troubleshooting

Investigated simulated domain sign-in issue by disabling and re-enabling a test user account in Active Directory.

![Troubleshoot](evidence/TKT-004-disabled-account.png)

![Account Restored](evidence/TKT-004-account-restored.png)

<br><br>

## TKT-005 Group Policy Management

Inspected domain Group Policy settings and reviewing password policy configuration in a Windows Server lab

![Password Policy Settings](evidence/TKT-005-password-policy.png)

<br><br>

## TKT-006: Windows Troubleshooting

Simulated a Windows performance investigation by opening multiple browser tabs and monitoring CPU and memory utilisation in Task Manager.

![Task Manager Processes](evidence/TKT-006-task-manager.png)

![System Performance](evidence/TKT-006-performance.png)

<br><br>

## TKT-007: Event Log Investigation

Investigated a critical Windows system event relating to an unexpected shutdown and considered the possible cause in a VirtualBox lab environment.

![Windows Event Investigation](evidence/TKT-007-event-investigation.png)
