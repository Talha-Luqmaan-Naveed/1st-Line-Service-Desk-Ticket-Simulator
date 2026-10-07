


| Tickets       | Issues                     | Resolution |
| ------------- | -------------              | ----------
| Ticket #1     | No Internet Connectivity   | **1. Physical Check:** Verify Ethernet cable is securely plugged in PC and the router. If it is plugged in correctly a green/amber light would show. <br><br>**2. Software Check:**<br>> `ipconfig /all` check for valid ipv4 address & gateway<br>> `ipconfig /release` & `ipconfig /renew` request fresh DHCP lease<br>> `ipconfig /flushdns` flushes the DNS cache   |
| Ticket #2     |  |


### Technical Verification
1. **Check IP Configuration (`ipconfig /all`)**
<p align="center">
   <img src="https://snipboard.io/8WvAJM.jpg" height="70%" width="70%" />

</p>
