


| Tickets       | Issues                     | Resolution |
| ------------- | -------------              | ----------
| Ticket #1     | No Internet Connectivity   | **1. Physical Check:** Verify Ethernet cable is securely plugged in PC and the router. Confirm green/amber link lights illuminate on the network adapter. <br><br>**2. Software Check:**<br>> `ipconfig /all` Check for valid ipv4 address & gateway<br>> `ipconfig /release` & `ipconfig /renew` Request fresh DHCP lease<br>> `ipconfig /flushdns` Flushes the DNS cache<br>> `ping (Default Gateway)` & `ping 8.8.8.8` Verify local gateway and internet availability   |
| Ticket #2     |  |


### Technical Verification
1. **Check IP Configuration (`ipconfig /all`)**
<p align="center">
   <img src="https://snipboard.io/8WvAJM.jpg" height="70%" width="70%" />

</p>
