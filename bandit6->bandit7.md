Level Goal
The password for the next level is stored somewhere on the server and has all of the following properties:

->owned by user bandit7
->owned by group bandit6
->33 bytes in size

Explanation:
Bandit Level 6 focuses on searching for files based on ownership and permissions across the entire filesystem. 
After logging in as bandit6 using the password obtained from the previous level, the user is tasked with finding a file that is owned by the user bandit7, belongs to the group bandit6, and has an exact size of 33 bytes. 
Since this file is not located in the home directory, the search must be performed from the root directory. To accomplish this, the user uses the find command with options to filter files by user, group, and size. Because searching the whole filesystem generates many permission‑denied errors, these error messages are redirected to /dev/null to keep the output clean.
Once the correct file is found, the user reads its contents using the cat command, which reveals the password for Bandit Level 7.
This level teaches effective file searching across large systems and demonstrates how to manage permission errors in Linux.

<img width="710" height="500" alt="image" src="https://github.com/user-attachments/assets/d224dc80-37f7-4ebd-aba7-775bfab29a52" />

<img width="669" height="261" alt="image" src="https://github.com/user-attachments/assets/40a7b835-80d8-467f-81a1-c616351b9037" />

