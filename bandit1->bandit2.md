Level Goal
The password for the next level is stored in a file called - located in the home directory


Explanation:
Bandit Level 1 focuses on understanding how Linux handles files with special characters in their names.
After logging in as bandit1 using the password obtained from the previous level, the user finds a file named - in the home directory. Since filenames beginning with a hyphen are interpreted as command-line options, the file cannot be read using the usual cat - command. 
To solve this problem, the user specifies the file’s relative path by using cat ./-, which clearly indicates that the hyphen is a filename and not an option. 
Executing this command displays the contents of the file, which contains the password for Bandit Level 2.
This level teaches how Linux parses command-line arguments and highlights the importance of using relative or absolute paths when dealing with special filenames.

<img width="644" height="484" alt="image" src="https://github.com/user-attachments/assets/755398e9-2ae1-497e-97fb-cbc7b2c620e5" />


<img width="565" height="253" alt="image" src="https://github.com/user-attachments/assets/7ce3ba9d-557f-458f-8425-897cb2ae77fd" />

