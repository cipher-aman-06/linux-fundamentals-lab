
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
##### STEP 2 : find rsyslog files
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
##### STEP 2 : set weekly rotation
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
Stopping rsyslog 