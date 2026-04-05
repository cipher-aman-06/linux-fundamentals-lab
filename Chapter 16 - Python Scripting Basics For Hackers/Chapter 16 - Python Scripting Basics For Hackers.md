
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
