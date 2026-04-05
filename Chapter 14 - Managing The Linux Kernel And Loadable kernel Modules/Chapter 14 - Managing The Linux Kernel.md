
---
## Question 1
Find which Linux kernel version is currently running.
### Approach
Use uname command to display kernel release information.
### Commands
- `uname -r` → shows kernel version
- `uname -a` → shows full system kernel details
### Output
##### STEP 1 : display kernel version
![[Pasted image 20260405142529.png]]
### Key Observations
Kernel version identifies system capabilities.
Important for exploit compatibility checks.
### What I learned
Kernel version helps determine vulnerability targets.

---
## Question 2
Show all currently loaded kernel modules.
### Approach
Use lsmod to list active kernel modules in memory.
### Commands
- `lsmod` → lists loaded kernel modules
- `less` → scroll output
### Output
##### STEP 1 : list kernel modules
![[Pasted image 20260405142900.png]]
### Key Observations
Shows module name, size, dependencies.
Loaded modules increase attack surface.
### What I learned
Kernel modules extend OS functionality dynamically.

---
## Question 3
Turn on packet forwarding using sysctl command.
### Approach
Modify kernel runtime parameter to allow system to forward network packets.
### Commands
- `sysctl` → modify kernel parameters
- `net.ipv4.ip_forward` → controls packet forwarding
### Output
##### STEP 1 : enable IP forwarding
![[Pasted image 20260405143355.png]]
### Key Observations
Change applies immediately in memory.
Used for routing and MITM setups.
### What I learned
Kernel parameters can be changed without reboot.

---
## Question 4
Modify sysctl configuration file to control packet forwarding permanently, then disable it.
### Approach
Edit persistent configuration file and reload settings.
### Commands
- `nano` → edit configuration file
- `sysctl -p` → apply config changes
- `net.ipv4.ip_forward=0` → disable forwarding
### Output
##### STEP 1 : edit sysctl configuration
![[Pasted image 20260405143921.png]]
##### STEP 2 : disable IP forwarding
![[Pasted image 20260405144122.png]]
##### STEP 3 : apply configuration
![[Pasted image 20260405144132.png]]
### Key Observations
Persistent settings survive reboot.
Misconfiguration may expose routing capability.
### What I learned
System-wide kernel behaviour can be permanently configured.

---
## Question 5
Inspect detailed information about a specific kernel module.
### Approach
Use modinfo to retrieve metadata about module such as author and dependencies.
### Commands
