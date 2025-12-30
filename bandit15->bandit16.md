Level Goal

The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

Explanation:

Bandit Level 15 introduces secure communication using SSL/TLS. In this level, the password for the next level is not stored in a file but is provided by a service running on localhost at port 30001, which requires an encrypted connection.
Unlike the previous level that used plain text communication, this level expects the user to connect using SSL so that the data is transmitted securely. To interact with this service, a tool capable of establishing SSL/TLS connections is required.
After connecting securely and sending the current level’s password, the service verifies it and responds with the password for bandit16. 
This level teaches the difference between unencrypted and encrypted network communication and demonstrates how SSL/TLS is used to protect sensitive information such as passwords when transmitted over a network.


<img width="685" height="510" alt="image" src="https://github.com/user-attachments/assets/82208a78-cab0-44c3-9b77-719f17eee3d8" />


<img width="712" height="710" alt="image" src="https://github.com/user-attachments/assets/490b1422-0d26-45fb-a9d0-a819366fed34" />



<img width="999" height="673" alt="image" src="https://github.com/user-attachments/assets/f282a167-b640-4c6f-a7dd-bfda2e2c06f1" />


