


| Ticket ID      | Category                  | Issue/Request Description  |Resolution Summary | Key Technologies |
| :--- | :--- | :--- | :--- | :--- |
| **Ticket #1**     | Network Diagnostics  | User reports no internet or local network access  | Checks physical connection, refreshes the DHCP lease, flushes the local DNS cache, and verifies full internet and gateway connection      | `ipconfig`, `ping`, `nslookup`, `DHCP`, `DNS`                          |
| Ticket #2     |  |


### Technical Verification: Ticket #1
1. **Physical Link Check**
   Verify Ethernet cable is securely plugged in PC and the router. Confirm green/amber link lights illuminate on the network adapter.
<br><br>

2. **Initial Network Audit**
   Execute `ipconfig /all` to evaluate the current network configuration.
<p align="center">
   <img src="https://snipboard.io/8WvAJM.jpg" height="70%" width="70%" /><br>
</p>  

<br><br>

3. **Refresh IP lease & Clear Resolver Cache**
   Apply client-side remediation commands using `ipconfig /release`, `ipconfig /renew`, `ipconfig /flushdns` to force the network adapter to drop invalid configuration data, obtain a fresh DHCP lease, and wipe the local DNS cache.
<p align="center">
   <img src="https://snipboard.io/K7lpEG.jpg" height="70%" width="70%" /><br>
</p>  

<br><br>

4. **Network Reachability & Verification**
   Execute ping tests using `ping (Gateway IP)` and `ping (Internet)` to confirm active configuration to both the local gateway and external public internal resources.
<p align="center">
   <img src="https://snipboard.io/07TrnC.jpg" height="70%" width="70%" /><br>
</p>

<br><br>
