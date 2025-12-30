Level Goal

Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

Explanation:

In Bandit level 25 to 26, the main objective is to log in to the next level using an SSH private key, but the login shell is intentionally restricted. 
After logging in as bandit25, the user is given a private SSH key (bandit26.sshkey) instead of a normal password. When attempting to log in as bandit26 using this key, the session immediately closes because the default shell for bandit26 is not a normal shell but a restricted program that exits quickly.
To solve this, the user forces the terminal into a small window size before connecting via SSH, which causes the system to open the session using the more pager. While inside more, the user uses escape commands to open a shell by typing !sh. This successfully spawns an interactive shell as bandit26. 
Once inside, the user reads the password for the next level by using the cat command on the password file.
This level teaches how terminal behavior, pagers, and restricted shells can be bypassed using Unix command features.

<img width="1521" height="546" alt="image" src="https://github.com/user-attachments/assets/25391d52-d012-49c7-8e7a-4ea0933b3ee6" />

<img width="1363" height="193" alt="image" src="https://github.com/user-attachments/assets/0bf6dcdc-86f7-4c54-9f31-d18997633702" />

<img width="1089" height="392" alt="image" src="https://github.com/user-attachments/assets/906a8032-212c-4bd6-98d2-36e050b6fb0f" />


