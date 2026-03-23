
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

##### STEP 2 : Install a software package

##### STEP 3 : Verify installation

### Key Observations
-  Kali Linux uses repositories to manage software packages
- `apt` automatically installs dependencies required for the software.
- Root privileges are required to install system packages.
### What I learned
Kali Linux uses the APT package manager to install, update, and manage software efficiently from trusted repositories.

---
