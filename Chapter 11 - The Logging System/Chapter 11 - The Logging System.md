
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
Open rsyslog configuration file and change rotation policy to weekly