
---
## Question 1
Display running processes and identify the first and last process in the list
### Approach
I used the `ps` command with the `aux` option to display all active processes running on the system and observed which process appears first and which appears last.
### Commands
- `ps` → shows active processes
- `aux` → displays all processes for all users with detailed information
### Output
##### STEP 1 : Display all running processes
ps aux
##### STEP 2 : Identify first and last process
systemd (first process usually : )
ps aux (last process : )
### Key Observations
Processes are displayed with :
- PID → process ID
- CPU usage
- memory usage
- command name
### What I learned
Linux allows monitoring of all running processes including system and user processes.

---
## Question 2
Identify the two processes consuming the most system resources
### Approach
I used the `top` command to monitor real-time system resource usage and identified the two processes using the highest CPU or memory.
