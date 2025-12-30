Level Goal


A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
You do not need to create new connections each time

Explanation:


In Bandit level 24 to 25, the objective is to find the next password by interacting with a network service running on localhost.
After logging in as bandit24 using the password obtained from the previous level, the challenge description indicates that a service is listening on a specific port and requires input in a particular format.
The user connects to this service using the nc (netcat) command along with the given port number. Once connected, the service repeatedly asks for a 4-digit PIN along with the current level password. 
Since the correct PIN is unknown, the user performs a brute-force attack by looping through all possible 4-digit combinations (0000 to 9999) and sending each attempt to the service using a script with echo and nc.
When the correct PIN is sent along with the Bandit 24 password, the service responds with the password for Bandit 25.
This level mainly teaches how to use netcat, shell scripting, and brute-force techniques to interact with network services and extract hidden information.


<img width="646" height="483" alt="image" src="https://github.com/user-attachments/assets/0e47269d-06ba-491c-aeff-1f87f09f52ee" />


<img width="952" height="715" alt="image" src="https://github.com/user-attachments/assets/e3ff9ee6-7bcf-4233-a120-40bdf5f17885" />


<img width="714" height="751" alt="image" src="https://github.com/user-attachments/assets/bc06e754-7cb3-464d-8a91-b6115bd4c652" />


