Level Goal

To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it.
The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

Explanation:

In Bandit Level 19, the password for the next level cannot be read directly because the file is owned by another user. Instead, a special program called bandit20-do is provided, which has permission to run commands as the user bandit20.
By executing this program with a command such as cat /etc/bandit_pass/bandit20, you can read the password file that normally cannot be accessed. 
This works because bandit20-do uses elevated privileges (setuid) to run the command as bandit20. Once the password is displayed, it is used to log in to Bandit Level 20 using the normal SSH command.

<img width="769" height="513" alt="image" src="https://github.com/user-attachments/assets/e45f4c31-470f-4b55-9bcd-22dcb6c53a6f" />


<img width="719" height="309" alt="image" src="https://github.com/user-attachments/assets/1e069275-4f7f-4ee1-a887-af88ce0207dc" />
