
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
Use network manager CLI tool to scan networks and compare output readability.
### Commands
- `nmcli` → network manager command tool
### Output
##### STEP 1 : scan wifi networks
### Key Observations
nmcli output is structured and easier to read.
Shows signal strength and security type clearly.
### What I learned
nmcli provides user-friendly network scanning results.

---
## Question 5
Connect to a wireless network using nmcli command.
### Approach
Use nmcli to connect to WiFi using SSID and password.
### Commands
- `nmcli` → manage network connections
### Output
##### STEP 1 : connect to wifi
### Key Observations
Requires correct SSID and password.
Connection stored for future use.
### What I learned
WiFi connections can be managed fully via terminal.

---
## Question 6
Enable Bluetooth interface and search for nearby Bluetooth devices.
### Approach
Activate bluetooth adapter then scan for devices using Bluetooth tools.
### Commands
- `hciconfig` → manage bluetooth device
- `hcitool` → scan bluetooth devices
### Output
##### STEP 1 : enable bluetooth adapter
##### STEP 2 : scan bluetooth devices
### Key Observations
Bluetooth devices identified by MAC address.
Devices must be discoverable.
### What I learned
Bluetooth scanning can detect nearby smart devices.

---
## Question 7
Verify if detected Bluetooth devices are reachable using 12ping.
### Approach
Use Bluetooth ping tool to check connectivity with device MAC address.
### Commands
- `12ping` → test bluetooth connectivity
### Output
##### STEP 1 : test bluetooth connection
### Key Observations
Response confirms device is within range.
Uses MAC address for communication.
### What I learned
Bluetooth reachability testing helps confirm device presence.
