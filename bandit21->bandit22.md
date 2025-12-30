Level Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed

Explanation:

In Bandit Level 21, first use the cd command to change the directory to /etc/cron.d. 
Then use the ls command to list the files in that directory. From the list, choose the file related to bandit22 and view its contents using the cat command. 
This file shows which script is executed by the cron job. Next, use the cat command again to read /usr/bin/cronjob_bandit22.sh. From the output of this script, you can understand where the password for the next level is stored. 
Finally, use the path shown in the script to locate and read the file containing the Bandit22 password using the cat command.

<img width="738" height="504" alt="image" src="https://github.com/user-attachments/assets/9132aace-4e70-4372-87b8-bc8f46a79156" />


<img width="761" height="241" alt="image" src="https://github.com/user-attachments/assets/87880dd0-f88b-4dc2-a4ea-623579f8b70a" />
