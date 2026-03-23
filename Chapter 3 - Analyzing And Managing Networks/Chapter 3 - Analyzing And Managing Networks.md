
---
## Question 1
Identify the network interfaces currently active on the system.
### Approach
I used a networking command to display details of all available network interfaces and their configurations.
### Commands
- `ip a` → displays all network interfaces  
    OR
- `ifconfig` → shows network interface configuration
### Output
##### STEP 1 : Show network interfaces
![[Pasted image 20260323212000.png]]
### Key Observations
Interfaces such as :
- eth0 → wired interface
- lo → loopback interface
### What I learned
Linux systems use network interfaces to communicate with other systems and networks.

---
## Question 2
Assign a new IP address to the eth0 network interface.
### Approach
I manually configured the IP address for the eth0 interface.
### Commands
