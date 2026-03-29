
---
## Question 1
Create a simple greeting script similar to HelloHackersArise
### Approach
I created a basic bash script that prints a greeting message when executed.
### Commands
- `nano` → create script file
- `echo` → display message
- `chmod +x` → make script executable
### Output
##### STEP 1 : create script file
![[Pasted image 20260330010435.png]]
##### STEP 2 : add script code
![[Pasted image 20260330010844.png]]
##### STEP 3 : make executable
![[Pasted image 20260330010936.png]]
##### STEP 4 : run script
![[Pasted image 20260330011041.png]]
### Key Observations
Script executes commands automatically when run.
### What I learned
Bash scripts automate repeated tasks.

---
## Question 2
Create script to scan systems for MSSQL service on port 1433
### Approach
I created a script that scans IP addresses to check if port 1433 ( Microsoft SQL Server is open. )
### Commands
- `for` → loop through IP addresses
- `nc` → check open port
- port 1433 → MSSQL default port
### Output
##### STEP 1 : create script
![[Pasted image 20260330011600.png]]
##### STEP 2 : script code
![[Pasted image 20260330011824.png]]
##### STEP 3 : make executable
![[Pasted image 20260330012122.png]]
##### STEP 4 : run script
![[Pasted image 20260330012751.png]]
### Key Observations
Script checks multiple systems automatically.
### What I learned
Port scanning can be automated using bash loops.

---
## Question 3
Modify scanner to accept IP range and port from user input
### Approach
I modifies the script so user enters starting IP, ending IP, and port number. Script displays only open ports.
### Commands
- `read` → take user input
- `seq` → generate number range
- `nc` → test port connectivity
### Output
##### STEP 1 : edit script
![[Pasted image 20260330013110.png]]
##### STEP 2 : updated script
![[Pasted image 20260330013716.png]]
##### STEP 3 : run script
![[Pasted image 20260330013810.png]]
### Key Observations
Script dynamically scans based on user input.
### What I learned
Scripts can interact with users and adapt behaviour dynamically.

---
