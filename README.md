# cronBitwardenUpdate

Script to backup and update bitwarden selfhosted.

Stop Bitwarden,
Rsync files to NAS,
Updateself and Update Bitwarden using bitwarden.sh


Run by adding cron job using 

sudo crontab -e

Run every Saturday at 2am

0 2 * * 6 sudo /home/twadmin/scripts/bitwardenUpdateJob.sh | | /usr/bin/mail -s "Bitwarden Update Output" it@transworks.co.nz -a "From: notifications@transworks.co.nz"
