


| Ticket ID      | Category                  | Scenario/Task | Outcome | Tools & Skills |
| :--- | :--- | :--- | :--- | :--- |
| **TKT-001**     | Network Diagnostics  | Practise investigating network configuration and connectivity.  | Inspected IP configuration and practised network connectivity and DNS checks.   | Command Prompt basics - IP configuration, DNS, ping |
| **TKT-002**     | Active Directory Administration| Create a test domain user and assign appropriate group membership. | Created a test user, assigned group membership and verified account properties. | Active Directory, user accounts, security groups |
| **TKT-003**     | File and Folder Permissions | Configure access to a shared folder for an Active Directory security group. | Configured and checked NTFS permissions for the security group. |  Windows Server, NTFS permissions, shared folders |
| **TKT-004**     | Account Troubleshooting | Practise investigating a domain account sign-in problem. | Inspected account status and relevant account settings. | Active Directory, account troubleshooting |
| **TKT-005**     | Group Policy Management | Practise checking why a required desktop setting may not be applied. | Inspected Group Policy configuration and checked policy application. | Group Policy, GPMC, Windows administration |
| **TKT-006**     | Windows Troubleshooting | Investigate Windows system performance using built-in tools. | Inspected resource usage and running processes in Task Manager. | Task Manager, process monitoring, performance checks | 
| **TKT-007**     | Event Log Investigation | Practise investigating Windows events related to system errors. | Reviewed relevant Windows event logs and examined event details. | Event Viewer, Windows Logs, error investigation |

<br><br>
## TKT-001: Network Diagnostics

### Investigation and Troubleshooting

1. **Physical Link Check**
   Verify Ethernet cable is securely plugged in PC and the router. Confirm green/amber link lights illuminate on the network adapter.
<br><br>

2. **Initial Network Audit**
   Execute `ipconfig /all` to evaluate the current network configuration.
   
  ![IP Configuration](evidence/TKT-001-ip-config.png)

<br><br>

3. **Refresh IP lease & Clear Resolver Cache**
   Apply client-side remediation commands using `ipconfig /release`, `ipconfig /renew`, `ipconfig /flushdns` to force the network adapter to drop invalid configuration data, obtain a fresh DHCP lease, and wipe the local DNS cache.

![IP Lease Renewal and DNS Cache](evidence/TKT-001-ipconfig-renew.png)

<br><br>

4. **Network Reachability & Verification**
   Executed ping tests using ping <gateway IP> and ping 1.1.1.1 (external IP address) to verify connectivity to the local gateway and an external network destination

![IP Lease Renewal and DNS Cache](evidence/TKT-001-connectivity-ping-test.png)

<br><br>


