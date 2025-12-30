Level Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.


Explanation:

In Bandit Level 22, the password for the next level is generated automatically using a cron job. First, I used the cd /etc/cron.d command to move into the cron directory where scheduled tasks are stored. Then I used the ls command to list all files and identified the file related to bandit23. 
After that, I used the cat command to read cronjob_bandit23, which showed that a script named cronjob_bandit23.sh is executed every minute.

Next, I used the cat /usr/bin/cronjob_bandit23.sh command to read the cron script. From this script, I understood that the username is obtained using the whoami command and a string is created using echo.
This string is then converted into an MD5 hash using the md5sum command, and only the hash value is extracted using the cut command. This hash is used as the filename inside the /tmp directory where the password is stored.

After understanding the script logic, I manually recreated the same command using
  "echo I am user bandit23 | md5sum | cut -d ' ' -f 1"
to get the correct filename. Finally, I used the cat command with that filename inside /tmp to display the password for the Bandit23 level.

<img width="711" height="507" alt="image" src="https://github.com/user-attachments/assets/fe4ba64d-f038-47b3-9b94-ba2b6ee1ba81" />


<img width="677" height="422" alt="image" src="https://github.com/user-attachments/assets/f08d1657-cb05-4539-ad06-0264eb1b547f" />
