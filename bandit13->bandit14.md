Level Goal
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14.
For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. 
Look at the commands that logged you into previous bandit levels, and find out how to use the key for this level.


Explanation:
Bandit Level 13 introduces the concept of SSH key-based authentication, which is commonly used in secure systems instead of password-based login.
After logging in as bandit13, the user is provided with a file named sshkey.private, which contains a private SSH key. By using the cat command, the user can view the contents of this private key file. 
The key can then be copied and saved into a new file named private.key. To log in to the next level, the -i option is used with the ssh command to specify the private key file while connecting as bandit14 on the local host. 
After successfully logging in to Bandit Level 14, the user reads the file /etc/bandit_pass/bandit14 to obtain the password for the next level. 
This level helps users understand how SSH private keys are used for authentication and highlights the importance of secure access methods in Linux systems.


<img width="706" height="517" alt="image" src="https://github.com/user-attachments/assets/9e4e8d3b-4511-430e-a2f9-06b7810e3c41" />


<img width="825" height="783" alt="image" src="https://github.com/user-attachments/assets/0ca5953a-b8e8-4dfe-8b05-e02da3b54291" />


<img width="793" height="495" alt="image" src="https://github.com/user-attachments/assets/6d8e75e2-6303-48b0-93c8-845dbfc96dac" />


<img width="666" height="205" alt="image" src="https://github.com/user-attachments/assets/4252b487-e1e2-40d8-b76a-f03dc65b4f1a" />



