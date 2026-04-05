
---
## Question 1
Configure the MySQLscanner script to execute automatically every Wednesday at 3PM.
### Approach
Use cron scheduler to run script weekly at specified day and time.
### Commands
- `crontab -e` → edit cron jobs
- `0 15 * * 3` → schedule format (3 PM Wednesday )
### Output
##### STEP 1 : open cron editor
![[Pasted image 20260405160622.png]]
##### STEP 2 : add scheduled task
![[Pasted image 20260405160342.png]]
![[Pasted image 20260405160642.png]]
### Key Observations
Cron uses 24-hour time format.
Day value 3 represents Wednesday.
### What I learned
Cron enables precise automation of security scripts.

---
## Question 2
Schedule the MySQLscanner script to execute on the 10th day of April, June, and August.
### Approach
Define cron job specifying day of month and selected months.
### Commands
- `crontab -e` → edit cron jobs
- `10 4,6,8` → specific months
### Output
##### STEP 1 : open cron editor
![[Pasted image 20260405161626.png]]
##### Schedule monthly execution
![[Pasted image 20260405161858.png]]
![[Pasted image 20260405162002.png]]
### Key Observations
Multiple months separated by comma.
Runs once per selected month.
### What I learned
Cron allows selective month scheduling.

---
## Question 3
Configure the script to run at 10 AM every Tuesday, Wednesday, and Thursday.
### Approach
Specify weekday range in cron expression.
### Commands
- `crontab -e` → edit cron jobs
- `2-4` → Tuesday to Thursday
### Output
##### STEP 1 : open cron editor
##### STEP 2 : add weekday schedule
### Key Observations
Weekday numbering starts from Sunday=0.
Range simplifies multi-day scheduling.
### What I learned
Cron ranges reduce repetitive entries.

---
## Question 4
Configure the script to execute every day at 12 PM using cron shortcut syntax.
### Approach
Use cron predefined expression for daily execution at noon.
### Commands
- `@daily` → cron shortcut
- `crontab -e` → edit cron jobs
### Output
##### STEP 1 : open cron editor
##### STEP 2 : add daily schedule
### Key Observations
Shortcut expressions simplify cron syntax.
Noon equals hour value 12.
### What I learned
Cron shortcuts speed up configuration.

---
## Question 5
Configure PostgreSQL service to automatically start when system boots.
### Approach
Use update-rc.d to enable service startup during boot process.
### Commands
- `update-rc.d` → manage startup services
- `systemctl enable` → alternative method
### Output
##### STEP 1 : enable PostgreSQL at boot
### Key Observations
Service persistence ensures availability after reboot.
Startup services may expose network ports.
### What I learned
Boot persistence is crit