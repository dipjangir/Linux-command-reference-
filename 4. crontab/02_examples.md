# Crontab Practical Examples

Yeh file kuch real-world cron jobs ke examples deti hai jo automation me help karte hain. Inko samajhne se tumhe scheduling me clarity milegi.

---

## 1. Script Daily Run at Midnight

```bash
0 0 * * * /home/user/myscript.sh

> Har raat 12 baje myscript.sh run hoga.




---

2. Every 15 Minutes

*/15 * * * * /home/user/check-status.sh

> Har 15 minute me check-status.sh run karega.




---

3. Every Sunday at 6:30 PM

30 18 * * 0 /home/user/cleanup.sh

> Har Sunday shaam 6:30 pe cleanup.sh chalega.




---

4. On 1st and 15th of Every Month

0 9 1,15 * * /home/user/report.sh

> Har mahine ke 1st aur 15th din subah 9 baje report.sh execute hoga.




---

5. Every Day Every Hour (for logging or sync)

0 * * * * /home/user/sync.sh >> /home/user/sync.log

> Har ghante sync.sh chalega aur output sync.log me store hoga.




---

6. Crontab with Environment Variables

MAILTO="your_email@example.com"
0 8 * * * /home/user/health-check.sh

> Subah 8 baje script run karega aur result email bhejega.




---

7. Run Python Script Weekly on Friday Night

0 22 * * 5 /usr/bin/python3 /home/user/db_backup.py

> Har Friday raat 10 baje Python script chalegi.




---

8. Run Every 2 Hours

0 */2 * * * /home/user/auto.sh

> Har 2 ghante me run karega.




---

Tips:

Log files ka use karo for debugging (e.g. >> /path/to/log.txt 2>&1)

Scripts ko test karo manually pehle

Crontab me absolute paths hi use karo


---
