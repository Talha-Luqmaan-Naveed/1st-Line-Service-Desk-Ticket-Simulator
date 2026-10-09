


| Ticket ID      | Category                  | Issue/Request Description  |Resolution Summary | Key Technologies |
| :--- | :--- | :--- | :--- | :--- |
| **TKT-001**     | Network Diagnostics  | User reports no internet or local network access  | Checks physical connection, check IP configuration, connectivity and DNS resolution     | Windows Command Prompt, IP configuration, Ping, DNS, DHCP   |
| **TKT-002**     | Active Directory | New client requires a domain account  | Create a test user, assigns appropriate group membership and verify account properties | Active Directory, ADUC |
| **TKT-003**     | File and Folder Permission Management | User cannot access a shared folder | Configure and check NTFS permissions for an AD security group | Windows Server, Active Directory, NTFS |
| **TKT-004**     | Account Troubleshooting | User reports they cannot sign in to their domain account | Investigate account status and possible sign-in issues | Active Directory, Windows |
| **TKT-005**     | Group Policy Management | User reports a required desktop setting is not being applied | Checked Group Policy configuration and application | GPMC, GPO, Active Directory |
| **TKT-006**     | Windows Troubleshooting | User reports their computer is running slowly | Check system resource usage and running processes | Windows, Task Manager | 
| **TKT-007**     | Event Log Investigation | User reports a recurring Windows error | Review Event Viewer for relevant errors | Event Viewer, Windows Logs, Windows Troubleshooting |


### Technical Verification: Ticket #1
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


