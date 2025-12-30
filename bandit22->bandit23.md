Level Goal

A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.


Explanation:
In Bandit Level 22, the password for the next level is generated automatically by a cron job that runs as bandit23. The password is not stored in a fixed file. Instead, the cron script dynamically creates a filename using the username and an MD5 hash. To get the password, we must analyze the cron job script and reproduce its logic manually.

After understanding the script logic, manually recreated the same command using
  "echo I am user bandit23 | md5sum | cut -d ' ' -f 1"
to get the correct filename. Finally, used the cat command with that filename inside /tmp to display the password for the Bandit23 level.

<img width="711" height="507" alt="image" src="https://github.com/user-attachments/assets/fe4ba64d-f038-47b3-9b94-ba2b6ee1ba81" />


<img width="677" height="422" alt="image" src="https://github.com/user-attachments/assets/f08d1657-cb05-4539-ad06-0264eb1b547f" />
