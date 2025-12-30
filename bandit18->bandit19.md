Level Goal
The password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.


Explanation:

In Bandit Level 18, you first start by logging in as usual with the SSH command using the password from Bandit 17. 
Once logged in, instead of being able to use a normal interactive shell, the system is set up to immediately log you out. 
To access the password for the next level, you need to read the readme file directly using the cat command during login. Essentially, you combine logging in and reading the file in one step, like this:

    "ssh bandit18@bandit.labs.overthewire.org -p 2220 cat readme"


This command uses your Bandit 17 password to log in and immediately outputs the contents of the readme file, which contains a Base64 encoded password for Bandit 19. 
You then decode this using base64 -d to get the actual password and log in to the next level.



<img width="607" height="256" alt="image" src="https://github.com/user-attachments/assets/b57b299f-a941-4ab9-95cd-87b49d7fc88c" />
