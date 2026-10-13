# Laboratory 09 – Cloud Automation Engineer

## Mission Overview

This mission focuses on using Bash scripting and cron scheduling to automate application data backups on a Linux system.

## Objectives

- Understand Bash scripts, variables, and cron jobs.
- Create and execute a backup script.
- Use `chmod` to make a script executable.
- Compress application data into a `.tar.gz` archive.
- Schedule a backup using crontab.
- Document automation tasks using Markdown.

## Commands Executed

```bash
mkdir -p /root/app-data
echo "This is critical client data." > /root/app-data/data.txt
nano /root/backup.sh
chmod +x /root/backup.sh
/root/backup.sh
ls -lh /root/backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

I learned how to write a Bash script, create a compressed backup, change file permissions, and schedule tasks using cron. I also learned how automation can reduce repetitive manual work and make cloud operations more consistent.
