
---
## Question 1
Launch the Apache web server service using terminal commands.
### Approach
Use service manager to start Apache and verify it is running.
### Commands
- `systemctl` → manage linux services
- `service` → start/stop services
- `status` → verify service state
### Output
##### STEP 1 : start apache service
##### STEP 2 : verify service status
### Key Observations
Apache runs on port 80 by default.
Service must be active to host webpages.
### What I learned
Web servers are controlled using system services.

---
## Question 2
Modify the default webpage file to display a message about entering hacking field.
### Approach
Edit index.html file in Apache root directory and add custom text.
### Commands
- `nano` → edit file
- `echo` → insert text
- `cat` → display file
### Output
##### STEP 1 : open index file
##### STEP 2 : add webpage content
##### STEP 3 : view webpage
### Key Observations
Apache serves files from /var/www/html directory.
index.html is default homepage file.
### What I learned
Website content can be controlled by editing HTML files.

---
## Question 3
Enable SSH service and remotely connect to kali machine from another device in same network.
### Approach
Start SSH server then connect using IP address from another system.
### Commands
- `systemctl` → manage services
- `ssh` → remote login
- `ip a` → find IP address
### Output
##### STEP 1 : start ssh service
##### STEP 2 : find system IP
##### STEP 3 : connect remotely
### Key Observations
SSH uses port 22 by default.
Remote login requires correct username and IP.