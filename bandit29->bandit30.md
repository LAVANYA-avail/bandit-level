Level Goal

There is a git repository at ssh://bandit29-git@bandit.labs.overthewire.org/home/bandit29-git/repo via the port 2220. The password for the user bandit29-git is the same as for the user bandit29.

Clone the repository and find the password for the next level.

Explanation:

In Bandit level 29–30, first create a new directory using the mkdir command and move into that directory using the cd command. Then use the git clone command with the given SSH link to clone the repository.
After the repository is cloned, use the ls command to list the files and change into the cloned directory using the cd command. Inside the directory, use the ls command to see the files and read them using the cat command. 
In this level, the password is not present in the current branch, so Git branches must be checked. By listing the available branches and switching to the correct branch, the hidden file containing the password for the next level can be accessed.
This level helps in understanding how to work with Git branches and how sensitive data can exist in different branches of a repository.

<img width="847" height="779" alt="image" src="https://github.com/user-attachments/assets/6aeae619-3839-4b8b-a4a7-398c32750379" />


<img width="891" height="781" alt="image" src="https://github.com/user-attachments/assets/bd71e42b-02b0-4364-ac96-d2a516e97979" />


<img width="827" height="606" alt="image" src="https://github.com/user-attachments/assets/edbd1f2e-ec89-4563-808a-e2e80111c491" />

<img width="811" height="654" alt="image" src="https://github.com/user-attachments/assets/6af3ec09-c127-4c8c-b9dd-cbc4280f0fec" />

