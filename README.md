# GitHub Tutorial

_by Karla Osorno_

---
### Git vs. GitHub
_Git and Github are both similar but they have small differences_  
**Git:**
* Git _doesn't_ need Github in order to function correctly
* It's a version control that keeps "snapshots" of you code. What does this mean? This means that it will keep your exact code saved.
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
_Here you will learn how to create a repository on GitHub_
1. Go to GitHub.com and click on the plus sign in the top right corner. Click on new repository.
2. Pick a title for your repository. Remember that instead of spaces, you should use a dash (-). The name that you put on GitHub
 has be also be the _exact_ same name as the repository name on Cloud9.
3. Pick from public or private. Check "**Initialize this repository with a README**". Finally click create repository.
4. Now it's time to add a remote. A remote is what creates the connection between your "local machine" and the "cloud".
5. You can add your remote by typing `git remote add origin <URL>`


---
### Workflow & Commands
_After you learn to initialize your repository or directory, you're going to want to learn commands to create content in your repositories/directories._
1. mkdir and cd are useeful commands. You can make a directory in Cloud9 by typing `mkdir github-learning`.
2. Then you can navigate to this directory by typing `cd github-learning`
3. You can then create a README.md file by typing `touch README.md`. You can open this file by typing `c9 README.md`
4. Type something into the README.md file (example: "this is the first line of code")
    * If you see a grey circle it means your changes have not been saved, click command + S to save.
5. Type `ls` and you should be be able to see your README.md file listed

**In a git repository you will type git before every command**
* Whenever you're in Cloud9 `git init` is what creates a new git repository. You need to type this before typing any git commands.
* Use `git status` often so you can keep track of your work and what is added. Changes that haven't been added will appear in red and changes that have
 been added will appear in green.
* Type `git add.` to add your changes to the staging area (so it can be ready to get commited)
* After you add, you will commit your changes using `git commit -m "your message goes here"`. You will write a concise description of what you have changed.
Also do _not_ write your message in past tense. (Example: if you edited your readme file, you should write "edit readme file")
* Since you already created a remote, you will type `git push origin -u master`. This wil "push" your repository to GitHub.


---
### Rolling Back Changes