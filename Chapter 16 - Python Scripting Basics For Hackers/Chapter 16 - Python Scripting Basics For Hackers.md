
---
## Question 1
Create the SSH banner grabbing script and modify it to capture the banner from FTP port 21.
### Approach
Adjust socket connection port number from SSH port 22 to FTP port 21.
### Commands
- `python3 script.py` → run python script
- `socket` → create network connection
- `port 21` → FTP service port
### Output
##### STEP 1 : edit script port value
##### STEP 2 : modify port inside script
##### STEP 3 : run script
### Key Observations
Different services run on different ports.
FTP commonly listens on port 21.
### What I learned
Port targeting changes reconnaissance results.

---
## Question 2
Modify the banner grabbing script so the user enters the target IP instead of hardcoding it.
### Approach
Use input() function to dynamically receive IP address.
### Commands
- `input()` → receive user input
- `python3` → execute script
### Output
##### STEP 1 : edit script
##### STEP 2 : add user prompt
##### STEP 3 : run script
### Key Observations
Dynamic input increases script flexibility.
Removes need to edit code repeatedly.
### What I learned
User input improves tool usability.

---
## Question 3
Modify tcp_server.py so the listening port is provided by the user.
### Approach
Prompt for port number and convert input to integer.
### Commands
- `input()` → accept user data
- `int()` → convert string to number
### Output
##### STEP 1 : edit tcp server script
##### STEP 2 : add port input
##### STEP 3 : run server
### Key Observations
Ports must be integers for socket binding.
Flexible port selection supports multiple services.
### What I learned
Dynamic configuration improves network tool adaptability.

---
## Question 4
Create the FTP password cracking script and modify it to read passwords from a wordlist variable.
### Approach
Load password 