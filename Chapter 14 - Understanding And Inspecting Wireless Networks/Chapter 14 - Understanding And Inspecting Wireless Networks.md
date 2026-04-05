
---
## Question 1
Display all network interfaces and identify any wireless related information.
### Approach
Use network configuration tool to list interfaces and check wireless capability.
### Commands
- `ifconfig` → shows network interfaces
- `ifconfig -a` → shows all interfaces
### Output
##### STEP 1 : list network interfaces
### Key Observations
Wireless interfaces often named wlan0.
Shows IP, MAC address, and status.
### What I learned
Network interface details reveal connectivity options.

---
## Question 2
Identify wireless network adapter details using wireless configuration command.
### Approach
Use iwconfig to check wireless interface properties.
### Commands
- `iwconfig` → shows wireless interface details
### Output
##### STEP 1 : check wireless adapters
### Key Observations
Displays ESSID, frequency, signal strength.
Non-wireless interfaces show "no wireless extensions".
### What I learned
Wireless adapter information is accessible via terminal tools.

---
## Question 3
Scan nearby WiFi networks and list available access points.
### Approach
Use wireless scanning command to discover nearby networks.
### Commands
- `iwlist` → scans WiFi networks
- `grep` → filter output
### Output
##### STEP 1 : scan available wifi networks
### Key Observations
Shows SSID, encryption type, signal level.
Requires sudo privileges.
### What I learned
WiFi reconnaissance reveals nearby targets.

---
## Question 4
List available WiFi networks using nmcli and compare usability with iwlist.
### Approach
Use network manager 