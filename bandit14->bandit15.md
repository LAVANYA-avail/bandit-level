Level Goal


The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

Explanation:

Bandit Level 14 focuses on reading data from a network service using a secure connection. After logging in as bandit14, the password for the next level is not stored in a normal file in the home directory. 
Instead, it is provided by a service running locally on port 30000. The user must connect to this service and send the current level’s password to receive the password for bandit15. This is done using a networking tool that can communicate with TCP services.
By securely connecting to the local service and supplying the correct password, the service responds with the password for the next level.
This level teaches how services can expose information over network ports and how command-line tools can be used to interact with such services securely.


<img width="704" height="497" alt="image" src="https://github.com/user-attachments/assets/b12be06a-10b2-47b1-acd3-40851a0e47e1" />


<img width="595" height="281" alt="image" src="https://github.com/user-attachments/assets/93921839-1ae6-4744-8c92-9c4dcb6e1c95" />




