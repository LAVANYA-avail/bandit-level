Level Goal
The password for the next level is stored in a file called --spaces in this filename-- located in the home directory

Explanation:
Bandit Level 2 introduces the challenge of working with filenames that contain spaces, which can cause issues if not handled correctly in the Linux command line. 
After logging in as bandit2 using the password from the previous level, the user discovers a file named “spaces in this filename” in the home directory.
Because Linux treats spaces as separators between command arguments, the filename cannot be read directly without special handling.
To access the file, the user encloses the filename within quotation marks or escapes the spaces, allowing the cat command to correctly interpret the entire name as a single file.Reading this file reveals the password for Bandit Level 3.
This level teaches the importance of proper quoting and escaping techniques when dealing with filenames that include spaces, a common situation in real-world Linux environments.


<img width="660" height="479" alt="image" src="https://github.com/user-attachments/assets/02d1ba6e-3ab9-4d1e-b18b-69812eb67057" />

<img width="577" height="311" alt="image" src="https://github.com/user-attachments/assets/8bc46728-f2ea-4ad4-9bb6-733ec8ed292c" />

