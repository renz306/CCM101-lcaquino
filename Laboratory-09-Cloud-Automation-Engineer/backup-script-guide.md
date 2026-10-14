# Backup Script Guide

## 1. Creating the Backup Script

A Bash backup script automates the process of saving important files into a compressed archive. In this activity, the script copies the contents of the `app-data` directory into a `.tar.gz` file. A timestamp is added to the filename so that each backup can be identified separately.

### Script Code

```bash
#!/bin/bash

# Set the source and destination directories
SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Starting backup process..."

# Create the backup folder when needed
mkdir -p "$BACKUP_DIR"

# Compress the application data
tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup process finished at $TIMESTAMP!"
```

## 2. Making the Script Executable

Before running the script, execute the following command:

```bash
chmod +x backup.sh
```

This command grants execute permission to `backup.sh`. Once the permission is set, the script can be launched using:

```bash
./backup.sh
```

## 3. Scheduling Backups with Cron

Cron can run the backup script automatically at a specified time. For example, the following entry schedules a backup every day at 2:00 AM.

```bash
0 2 * * * /root/backup.sh
```

Make sure `/root/backup.sh` matches the actual location of your script.

### Cron Schedule Explanation

| Field | Value | Description |
|---|---|---|
| Minute | `0` | Runs at minute zero |
| Hour | `2` | Runs at 2:00 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

## 4. Verifying the Backup

After running the script, use this command to check the generated archives:

```bash
ls -l backups/
```

To view the contents of a backup archive without extracting it, use:

```bash
tar -tzf backups/backup_FILENAME.tar.gz
```

Replace `backup_FILENAME.tar.gz` with the actual name of your backup file.

## Conclusion

Using Bash and Cron makes routine backups easier to manage. The script compresses application data, while the timestamp helps organize multiple backup versions. Scheduling the script with Cron reduces the need for manual execution and supports regular data protection.

