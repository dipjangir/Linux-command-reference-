# Cron Basics (Crontab)

**Cron** ek time-based job scheduler hai Linux me. Iska use automate karne ke liye hota hai tasks ko (jaise backup, script run, system updates etc.)

**Crontab (cron table)** ek file hoti hai jisme scheduled commands/scripts ko define kiya jata hai.

---

## 1. Crontab Syntax

```bash
*  *  *  *  *  command-to-execute
|  |  |  |  |
|  |  |  |  └───── Day of Week (0 - 7) (Sunday = 0 or 7)
|  |  |  └──────── Month (1 - 12)
|  |  └──────────── Day of Month (1 - 31)
|  └──────────────── Hour (0 - 23)
└──────────────────── Minute (0 - 59)


---

2. Common Examples

Schedule	Crontab Expression	Description

Every minute	* * * * *	Runs every minute
Every day at 5am	0 5 * * *	Daily at 5:00 AM
Every Monday at 3pm	0 15 * * 1	Every Monday at 3:00 PM
Every 10 minutes	*/10 * * * *	Runs every 10 minutes
First day of month	0 0 1 * *	At 12:00 AM on the 1st of every month



---

3. Crontab Commands

crontab -e   # Crontab file edit karo
crontab -l   # Scheduled jobs list karo
crontab -r   # Crontab delete karo


---

4. Run a Script with Cron

Example: Ek script /home/user/backup.sh ko daily 1AM pe run karna ho:

0 1 * * * /home/user/backup.sh

Note: Script executable honi chahiye (chmod +x backup.sh) and full path use karo.


---

5. Best Practices

Always use full paths (e.g., /usr/bin/python3, not python3)

Output ko log file me redirect karo (e.g., ... >> /var/log/myscript.log)

Environment variables set karne pad sakte hain


---

