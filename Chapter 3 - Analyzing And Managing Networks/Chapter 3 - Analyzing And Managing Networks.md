
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
![[Pasted image 20260324022333.png]]
### Key Observations
MAC address is updated to the new value.
### What I learned
MAC addresses uniquely identify network devices and can be modified for testing or privacy.

---
## Question 4
Check if any wireless network interfaces are available on the system.
### Approach
I used a command that lists wireless network interfaces.
### Commands
- `iwconfig` → shows wireless interfaces
### Output
##### STEP 1 : Check wireless interfaces
![[Pasted image 20260324023037.png]]
### Key Observations
Wireless interfaces typically appear as wlan0 or similar.
### What I learned
Wireless interfaces allow connection to WiFi networks.

---
## Question 5
Obtain a new IP address automatically from a DHCP server.
### Approach
I requested the system to obtain an IP address dynamically from the network.
### Commands
- `dhclient` → requests IP from DHCP server
### Output
##### STEP 1 : Request DHCP IP
![[Pasted image 20260324024631.png]]
##### STEP 2 : Verify new IP
![[Pasted image 20260324024650.png]]
### Key Observation
DHCP automatically assigns IP configuration.
### What I learned
DHCP simplifies network configuration by automatically assigning IP addresses.

---
## Question 6
Identify the DNS server and mail associated with a website.
### Approach
I queried DNS records to find nameserver and mail server details.
### Commands
- `nslookup` → queries DNS
- `dig` → advanced DNS lookup
### Output
##### STEP 1 : Find nameserver

##### STEP 2 : Find mail server

### Key Observations
DNS records include:

- NS → nameserver
- MX → mail server