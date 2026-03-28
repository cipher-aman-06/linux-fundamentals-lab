
---
## Question 1
Install a new software package using Kali Linux repositories
### Approach
I used Kali Linux package management tools to install software from the official repository. First, I updated the package list and then installed a package using the apt package manager.
### Commands
- `sudo apt update` → updates package list from repositories
- `sudo apt install <package-name>` → installs the selected software package
- `apt list --installed` → shows installed packages
### Output
##### STEP 1 : Update repository package list
![[Pasted image 20260324033601.png]]
##### STEP 2 : Install a software package
![[Pasted image 20260324033629.png]]
##### STEP 3 : Verify installation
![[Pasted image 20260324033656.png]]
### Key Observations
-  Kali Linux uses repositories to manage software packages
- `apt` automatically installs dependencies required for the software.
- Root privileges are required to install system packages.
### What I learned
Kali Linux uses the APT package manager to install, update, and manage software efficiently from trusted repositories.

---
## Question 2
Remove an installed software package from the system
### Approach
After installing a package, I removed it using the APT remove command to understand how software uninstallation works in Linux.
### Commands
- `sudo apt remove <package-name>` → removes installed package
- `sudo apt purge <package-name>` → removes package with configuration files
- `sudo apt autoremove` → removes unnecessary dependencies
### Output
##### STEP 1 : Remove installed package
![[Pasted image 20260328191402.png]]
##### STEP 2 : Remove unused dependencies
![[Pasted image 20260328195301.png]]
### Key Observations
- Removing packages helps maintain system performance.
- `autoremove` cleans unnecessary dependencies.
- `purge` removes configuration files completely.
### What I learned
Linux allows full control over installed software and unused dependencies can be cleaned to optimize the system.

---
## Question 3
Update the system repository information
### Approach
I refreshed the system's package database to ensure I have the latest information about available software versions.
### Commands
- `sudo apt update` → refreshes repository package index
- 