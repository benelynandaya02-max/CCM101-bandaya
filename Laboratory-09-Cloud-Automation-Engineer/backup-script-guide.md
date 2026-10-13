# Backup Script Guide

## 1. Full Bash Script

The script creates a compressed backup of the application data directory.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="/root/app-data"
BACKUP_DIR="/root/backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p "$BACKUP_DIR"

# Compress the source directory into a tarball (.tar.gz)
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

The command `chmod +x /root/backup.sh` adds execute permission to the script. This allows it to be run as a program, provided the user has the necessary permissions.

## 3. Cron Job Configuration

The cron expression used is:

```cron
0 2 * * * /root/backup.sh
```

## 4. Meaning of the Five Time Fields

### Minute

The first field is `0`, which means the task runs at minute zero.

### Hour

The second field is `2`, which means the task runs at 2 AM.

### Day of Month

The third field is `*`, which means every day of the month.

### Month

The fourth field is `*`, which means every month.

### Day of Week

The fifth field is `*`, which means every day of the week.

## 5. Summary

The Bash script compresses the application data into a `.tar.gz` archive. The cron job schedules the script to run every night at 2 AM without requiring someone to execute it manually.
