
---
## Question 1
Search the system to identify every file related to rsyslog.
### Approach
Use file indexing search tool to quickly locate rsyslog-related files.
### Commands
- locate → fast file search using database
- updatedb → update locate database
### Output
##### STEP 1 : update file database
![[Pasted image 20260402230419.png]]
##### STEP 2 : find rsyslog files
![[Pasted image 20260402230453.png]]
### Key Observations
locate searches from indexed database, not live scan.
rsyslog files usually exist in /etc and /var/log directories.
### What I learned
Fast file searching helps identify log storage locations quickly.

---
## Question 2
Modify log configuration so logs are rotated every 7 days.
### Approach
Open rsyslog configuration file and change rotation policy to weekly.
### Commands
- `nano` → terminal text editor
- `vim` → advanced editor
- `cat` → view file contents
### Output
##### STEP 1 : open configuration file
![[Pasted image 20260402230632.png]]
##### STEP 2 : set weekly rotation
![[Pasted image 20260402230723.png]]
### Key Observations
Log rotation prevents log files from growing too large.
Rotation frequency affects forensic data availability.
### What I learned
Log retention policies control how long system evidence exists.

---
## Question 3
Turn off logging service and observe entries generated in syslog file.
### Approach
Stop logging daemon and monitor syslog behavior.
### Commands
- `systemctl` → manage system services
- `cat` → read file contents
- `tail` → monitor log updates
### Output
##### STEP 1 : stop logging service
##### STEP 2 : check syslog activity
##### STEP 3 : monitor log changes
### Key Observations
Stopping rsyslog reduces logging events.
System may record service stop event before logging halts.
### What I learned
Disabling logs can reduce traces of system activity.

---
## Question 4
Securely overwrite and remove kernel log files permanently.
### Approach
Use secure deletion tool that overwrites data before removing files.
### Commands
- `shred` → overwrite file data
- `rm` → remove files
- `Is` → verify deletion
### Output
##### STEP 1 : locate kern log files
##### STEP 2 : securely delete logs
### Key Observations
shred overwrites file multiple times.
Recovery becomes extremely difficult after shredding.
### What I learned
Secure deletion prevents forensic recovery of sensitive logs.

---
### Security Insights
1. Location log files helps attackers identify evidence storage paths.
2. Log rotation settings influence how long activity traces remain.
3. Disabling logging reduces detection visibility of malicious actions.
4. Secure deletion techniques prevent recovery of incriminating logs.

---
