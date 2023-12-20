## Backups 

- Create a tar archive of /var/log with a snapshot to perform incremental backup
- Wait a few minutes and perform the same operation with a new archive
- Compare content of both tar files
- Secure export this archive out of the system using rsync
- Make a script to perform a backup and schedule it with cron

