
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
![[Pasted image 20260405203123.png]]
##### STEP 2 : modify port inside script
![[Pasted image 20260405203236.png]]
##### STEP 3 : run script
![[Pasted image 20260405203151.png]]
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
![[Pasted image 20260405203352.png]]
##### STEP 2 : add user prompt
![[Pasted image 20260405203330.png]]
##### STEP 3 : run script
![[Pasted image 20260405203416.png]]
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
![[Pasted image 20260405203444.png]]
##### STEP 2 : add port input
![[Pasted image 20260405203528.png]]
##### STEP 3 : run server
![[Pasted image 20260405203604.png]]
### Key Observations
Ports must be integers for socket binding.
Flexible port selection supports multiple services.
### What I learned
Dynamic configuration improves network tool adaptability.

---
## Question 4
Create the FTP password cracking script and modify it to read passwords from a wordlist variable.
### Approach
Load password list from file and iterate through entries.
### Commands
- `open()` → read file
- `for loop` → iterate passwords
- `python3` → run script
### Output
##### STEP 1 : edit script
##### STEP 2 : load wordlist
##### STEP 3 : run script
### Key Observations
Wordlists automate brute force attempts.
Common passwords increase success probability.
### What I learned
Automation significantly speeds password testing.

---
## Question 5
Modify banner grabbing script to handle closed ports by printing a message.
### Approach
Use try-except block to catch connection errors.
### Commands
- `try/except` → error handling
- `socket.error` → detect failure
### Output
##### STEP 1 : edit script
##### STEP 2 : add exception handling
##### STEP 3 : run script
### Key Observations
Closed ports trigger connection errors.  
Error handling prevents script crashes.
### What I learned
Exception handling improves tool reliability.

---
### Security Insights
1. Changing ports enables enumeration of different services.
2. User-supplied IPs allow flexible target selection.
3. Custom port listeners help simulate vulnerable services.
4. Wordlists enable scalable brute force attacks.
5. Error handling avoids detection through crashes.

---
