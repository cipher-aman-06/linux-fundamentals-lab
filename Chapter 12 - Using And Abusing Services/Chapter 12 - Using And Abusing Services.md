
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
![[Pasted image 20260403054721.png]]
##### STEP 2 : verify service status
![[Pasted image 20260403054735.png]]
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
![[Pasted image 20260403055407.png]]
##### STEP 2 : add webpage content
![[Pasted image 20260403055938.png]]
##### STEP 3 : view webpage
![[Pasted image 20260403060011.png]]
![[Pasted image 20260403060035.png]]
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
### What I learned
SSH allows secure remote command execution.

---
## Question 4
Run MySQL server, update root password, and access internal database.
### Approach
Start MySQL service, login as root, change password, then switch database.
### Commands
- `systemctl` → start database service
- `mysql` → database client
- `ALTER USER` → change password
### Output
##### STEP 1 : start mysql service
##### STEP 2 : login mysql
##### STEP 3 : change password
##### STEP 4 : switch database
### Key Observations
MySQL root account controls database permissions.
Weak passwords create security risk.
### What I learned
Database credentials must be properly secured.

---
## Question 5
Activate PostgreSQL service and configure it for Metasploit usage.
### Approach
Start PostgreSQL database and initialize it for penetration testing tools.
### Commands
- `systemctl` → manage services
- `service postgresql start` → start database
- `msfdb init` →initialize metasploit database
### Output
##### STEP 1 : start postgresql service
##### STEP 2 : initialize metasploit database
##### STEP 3 : verify database connection
### Key Observations
Metasploit stores can results in PostgreSQL database.
Database improves penetration testing workflow.
### What I learned
Security tools often rely on databases to store findings.

---
### Security Insights
1. Running web servers increases exposed attack surface.
2. Web page content can reveal attacker presence if misconfigured.
3. SSH allows remote control, making brute-force attacks possible.
4. Weak database credentials can lead to privilege escalation.
5. Metasploit databases store sensitive penetration testing data.

---
