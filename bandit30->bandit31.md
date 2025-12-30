Level Goal

There is a git repository at ssh://bandit30-git@bandit.labs.overthewire.org/home/bandit30-git/repo via the port 2220. The password for the user bandit30-git is the same as for the user bandit30.

Clone the repository and find the password for the next level.

Explanation:

In Bandit level 30–31, first create a new directory using the mkdir command and move into that directory using the cd command. Then use the git clone command followed by the given SSH link to clone the repository.
After cloning, use the ls command to list the files and change into the cloned directory using the cd command. Inside the directory, use the ls command to view the files and read them using the cat command. In this level, the password is not stored in a normal file, but it is saved as a Git tag.
By listing the available Git tags and viewing the correct tag, the password for the next level can be found. This level teaches how Git tags can store important information and how to retrieve data from them.

<img width="940" height="647" alt="image" src="https://github.com/user-attachments/assets/797208f1-a669-4afe-8038-e0eb8bce6030" />

<img width="633" height="339" alt="image" src="https://github.com/user-attachments/assets/f1577ede-3e61-4fc9-a3a2-4b3b30e561ca" />

