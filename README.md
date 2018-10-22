# GitHub Tutorial

_by Karla Osorno_

---
### Git vs. GitHub
_Git and Github are both similar but they have small differences_  
**Git:**
* Git _doesn't_ need Github in order to function correctly
* It's a version control that keeps "snapshots" of you code. What does this mean? This means that 
it will keep your exact code saved.
* Git runs in the command line
* Basic Git workflow:
    * There are folders that contain files
        * Once git is initialized, it is called a repository
    * You can edit files and save them while you work
    * You can add files to the stage then commit them  

**GitHub:**
* GitHub.com is the "cloud" where your work is saved on
    * You work on a "local machine", cloud9
* It keeps track of your snapshots or "commits"
* GitHub is a website where you can publish your repositories and collaborate with other people
* Github _requires_ Git

---
### Initial Setup
_Before you can start using Git in your workspace you will need to do the inital setup_
1. Create a Github account (with an HSTAT email if you have)
2. Log into Cloud9 with GitHub
3. Create a new workspace in Cloud9 called "Github-Learning"
4. Log into GitHub and click on your profile icon and click on settings
5. On the left sidebar click on SSH and GPG and click on new SSH key
6. Then in title, put "cloud9"
7. switch back to Cloud9, in the top right, click on the gear icon
8. In SSH keys tab, copy and paste the _second_ SSH key into GitHub (it starts with **ssh-rsa**)
9. Add the SSH key
10. In Cloud9 open the github-learning IDE
11. test the connection by typing `ssh -T git@github.com`
12. You should see `Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access.`


---
### Repository Setup



---
### Workflow & Commands



---
### Rolling Back Changes