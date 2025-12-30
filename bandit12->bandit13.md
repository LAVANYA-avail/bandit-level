Level Goal


The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name.
Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)


Explanation:



Bandit Level 12 is designed to teach how to work with files that have been compressed multiple times using different formats. After logging in as bandit12 with the password from the previous level, the user is given a file that appears as a hex dump rather than a normal readable file. 
The first step is to convert this hex dump back into a binary file using the xxd -r command. Once converted, the file must be examined and decompressed repeatedly using the correct tools such as gzip, bzip2, and tar, depending on the file type at each stage. 
This process continues until the final plain text file is extracted, which contains the password for Bandit Level 13.
This level emphasizes the importance of identifying file types correctly and understanding how different compression methods work. It also demonstrates how real-world forensic and penetration-testing tasks often require multiple decoding and extraction steps to access hidden information.



<img width="895" height="645" alt="Screenshot 2025-12-30 065216" src="https://github.com/user-attachments/assets/85661238-4432-4e4d-afcd-feb2048725fe" />


<img width="601" height="198" alt="Screenshot 2025-12-30 065230" src="https://github.com/user-attachments/assets/74bba77d-d5cf-4bf4-92c6-09bb5170ada4" />


<img width="940" height="836" alt="Screenshot 2025-12-30 065200" src="https://github.com/user-attachments/assets/089f6dfb-f218-48d5-b991-7b30e78c1495" />


<img width="923" height="684" alt="Screenshot 2025-12-30 065148" src="https://github.com/user-attachments/assets/9447886c-56e9-4655-b8ea-c1a024c54484" />





