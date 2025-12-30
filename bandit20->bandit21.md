Level Goal


There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. 
It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).




Explanation:

In Bandit Level 20, the goal is to learn how to use a setuid (SUID) binary to get the password for the next level. When you log in to bandit20, you will find an executable file called suconnect. This program is special because it runs with bandit21’s permissions, not bandit20’s. The program expects you to provide a TCP port number as an argument.
When executed, it connects to the given port on localhost and waits to receive the current level’s password (bandit20 password). If the password you send is correct, the program responds by sending back the bandit21 password.

To solve this level, you must first create a listening service on your own machine using a tool like nc (netcat). In one terminal, you open a listening port and send the bandit20 password through that port. In another terminal, you run ./suconnect <port_number>. T
he suconnect program connects to your netcat listener, receives the password you sent, verifies it, and then returns the password for bandit21.
This level teaches how network sockets, local TCP connections, and SUID programs can be combined to securely pass information between processes.


<img width="746" height="620" alt="Screenshot 2025-12-30 145000" src="https://github.com/user-attachments/assets/a6d08acc-5dc6-405d-bda4-b36ca729eeb2" />


<img width="1821" height="885" alt="Screenshot 2025-12-30 145101" src="https://github.com/user-attachments/assets/8ea82d6b-f60c-4ffc-8d5b-473f85b6bba4" />




