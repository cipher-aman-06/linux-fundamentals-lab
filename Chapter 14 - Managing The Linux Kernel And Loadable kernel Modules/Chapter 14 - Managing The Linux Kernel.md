
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