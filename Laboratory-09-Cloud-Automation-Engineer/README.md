
# Laboratory 09 – The Cloud Automation Engineer

## Mission Overview

This laboratory explores how Bash scripts and Cron can automate repetitive tasks in a Linux environment. I created a sample data folder, developed a backup script, and learned how to generate compressed backup files automatically.

## Objectives

- Practice writing Bash scripts.
- Create files and directories using Linux commands.
- Set script permissions using `chmod`.
- Generate compressed backups using `tar`.
- Learn how Cron schedules recurring tasks.
- Record the laboratory activities using Markdown.

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir app-data` | Creates a directory for sample data. |
| `echo "This is critical client data." > app-data/data.txt` | Creates a text file containing sample data. |
| `cat app-data/data.txt` | Displays the contents of the file. |
| `nano backup.sh` | Creates or edits the backup script. |
| `chmod +x backup.sh` | Allows the script to execute. |
| `./backup.sh` | Runs the backup process. |
| `ls -l backups/` | Checks the generated backup files. |
| `crontab -l` | Displays the current Cron schedule. |
| `env EDITOR=nano crontab -e` | Opens the Cron configuration for editing. |

## Skills Learned

- Writing and running Bash scripts.
- Organizing application data into directories.
- Creating `.tar.gz` backup archives.
- Managing Linux file permissions.
- Understanding scheduled tasks through Cron.
- Improving technical documentation using GitHub Markdown.

## Mission Reflection

This activity helped me understand how automation makes system administration easier. By creating a Bash script, I learned how to back up important files without manually repeating every command. I also discovered that Cron can schedule scripts to run at specific times, making routine maintenance more efficient.

Overall, this laboratory improved my Linux command-line skills and introduced me to practical cloud automation techniques.
