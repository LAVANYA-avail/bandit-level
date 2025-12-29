Level Goal
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once


Explanation:
Bandit Level 8 focuses on finding unique lines in a file using Linux text-processing commands. After logging in as bandit8 with the password obtained from the previous level, the user navigates to the home directory and finds a file named data.txt.
The challenge is to locate the line that appears only once in the file, which contains the password for Bandit Level 9. To solve this, the user uses the combination of sort and uniq -u commands. 
First, sort organizes all lines in alphabetical order, and then uniq -u filters out lines that are repeated, displaying only the unique line. By reading this line with cat or directly from the output, the user retrieves the password for the next level. 
This level teaches how to process and filter text efficiently using Linux commands, which is particularly useful when analyzing logs, configuration files, or large datasets.

<img width="631" height="517" alt="image" src="https://github.com/user-attachments/assets/a5e45182-f3dc-46c2-ba7b-6808e4ff2aa9" />

<img width="899" height="112" alt="image" src="https://github.com/user-attachments/assets/f46b7e60-5db6-408e-9816-3ad81a9a59c6" />

