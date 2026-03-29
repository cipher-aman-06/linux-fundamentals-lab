
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
### Commands
- `top` → shows live system process activity
### Output
##### STEP 1 : open process monitor
top
##### STEP 2 : identify highest resource processes

### Key Observations
Processes are dynamically sorted based on CPU usage.
### What I learned
Some processes consume more resource and may affect system performance.

---
## Question 3
Terminate the process consuming the most resources
### Approach
I identified the process ID (PID) of the resource-heavy process and terminated it using the kill command.
### Commands
- `kill` → stops a process
- `-9` → force stop process
### Output
##### STEP 1 : find PID using top
##### STEP 2 : terminate process
##### STEP 3 : confirm process stopped
### Key Observations
Process disappears from the process list after termination.
### What I learned
Processes can be manually stopped to free system resources.

---
## Question 4
Reduce the priority of a running process
### Approach
I used the renice command to change the priority level of a running process to 19 (lowest priority).
### Commands
- `renice` → modifies process priority
- nice values range :
	- -20 → highest priority
	- 19 → lowest priority
### Output
##### STEP 1 : find PID
##### STEP 2 : change process priority
##### STEP 3 : Verify change
### Key Observation
Lower priority processes receive fewer CPU resources.
### What I learned
Process priority can be controlled to optimize system performance.

---
## Question 5
Create a script and schedule it to run automatically at a specific time
### Approach
I created a simple bash script and scheduled it using the at command to execute at a specific time.
### Commands
- `nano` → create scrip
- `chmod` → make script executable
- `at` → schedule task
- `atq` → view scheduled jobs
### Output
##### STEP 1 : create script file
