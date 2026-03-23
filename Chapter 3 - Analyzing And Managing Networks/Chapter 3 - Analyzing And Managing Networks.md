
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
- `ifconfig` → configure interface  
    OR modern command:
- `ip addr add` → assigns IP address
### Output
##### STEP 1 : Assign IP address
![[Pasted image 20260323212645.png]]
##### STEP 2 : Verify IP change
![[Pasted image 20260323212703.png]]
### Key Observations
The IP address for eth0 changes to the assigned value.
### What I learned
IP addresses identify devices in a network and can be manually configured.

---
## Question 3
Modify the MAC address of the eth0 network interface.
### Approach
I changed the hardware address (MAC address) associated with the network interface.
### Commands
- `ifconfig` → changes MAC address  
    OR
- `ip link` → modern command
### Output
##### STEP 1 : Disable interface
![[Pasted image 20260324022216.png]]
##### STEP 2 : Change MAC address
![[Pasted image 20260324022234.png]]
##### STEP 3 : Enable interface
![[Pasted image 20260324022249.png]]
##### STEP 4 : Verify change

### Key Observations
MAC address is updated to the new value.
### What I learned
MAC addresses uniquely identify network devices and can be modified for testing or privacy.

---
## Question 4
