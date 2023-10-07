![image](https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/33f4fb48-67f2-4a00-a130-4d8f5ce13c86)$${\color{red}Welcome \space \color{red}To \space \color{red}GIT}$$

## Backup
- **Step:1** Create a file and add some data.
  ```bash
  vim backup-tutorial.sh 
  ```
- **Step:2** Take backup of file with timestamp.
  ```bash
  cp backup-tutorial.sh backup-tutorial.sh_29092023_0410.backup
  ```
- **Step:3** If you want to back all data 
  ```bash
  cp backup-tutorial.sh_29092023_0410.backup backup-tutorial.sh
  ```

<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/fcb5aa30-dbe7-4648-9d62-72faa4d2e641" width="600" background-size="cover"/>


## Archive files
```bash
tar czvf backup-tutorial.Backup *.backup
```

<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/6e008ded-1e81-43f9-878a-9b87d944c6a8" width="600" background-size="cover"/>


**Ques: _How do you pass "msg" when you commit your git code?_**
The answer is the "-m" argument when passing commit. 
  ```bash
  git commit -m "My MSG"
  ```


**Ques: _If you were to make a change for a commit done 30 days ago with respect to a machine type used? How would you go about doing this change? Would you directly change it?_**
- git clone -> create new branch -> Then goto githubUI -> git blame (history) -> apply your changes

- Start by cloning the repository and creating a new branch. Then, goto the GitHub UI and utilize the "Blame" feature, which displays the detailed history of changes made to a specific file.

- You can find out when a change was made, what the commit message was, and  what is the motivation for using this particular machine type. All of this information is conveniently presented there.

- By using this data, I initially gain insight into the existing commits and attempt to understand the reasons behind previous changes. With this understanding, I proceed to make my own commit, fully conscious of both my own contribution and the context provided by the previous commits.

**Ques: _What is branch protection in GitHub?_**
- Branch protection in GitHub is a set of security and workflow controls that you can apply to specific branches within a GitHub repository.
- It's designed to help maintain code quality, ensure that certain processes are followed, and protect important branches from accidental or unauthorized changes.


**Ques: _What is the command to initialize a git repository?_**
```bash
git init
```

**Ques: _Initialize a git repository at /home/sarah/story-blog?_**

- **Step 1:** cd /home/sarah/story-blog
- **Step 2:** Run below cmd
  ```bash
  git init
  ```
  ```bash
  ls -a
  ```
  ```bash
  ls -al
  ```

**Ques: _Which hidden folder gets created after initializing a git repository?_**
- .git
- To find hidden folder Run below cmd
  ```bash
  ls -a
  ```

**Ques: _Once a git repository has been initialized, which stage contains the active changes in your local git repository?_**

**Option 1:-** _Committed Files_
**Option 2:-** _Pushed Files_
**Option 3:-** _Staging area_
**Option 4:-** _Working area_

- **The answer is:** Working area. This is where you make edits to your files and create new files. 

**<ins>Ques:-</ins> _Let’s add a file to our project inside /home/sarah/story-blog_**

**File name:-** lion-and-mouse.txt
**File content:-** A Lion lay asleep in the forest

- **Answer is**
  ```bash
  echo "A Lion lay asleep in the forest" >> lion-and-mouse.txt
  ```
  ```bash
  ls
  ```

**<ins>Ques:-</ins> _Which stage contains new changes that will soon be committed to local git repo ?_**<br/>
**Option 1:** _Committed Files_<br/>
**Option 2:** _Pushed Files_<br/>
**Option 3:** _Staging area_<br/>
**Option 4:** _Working area_<br/>
- **The answer is:** Staging area.

<a href="#" style="color: red, pointer-events: none, cursor: default, text-decoration: none">Look, ma! Red!</a>

**<ins>Ques:-</ins> _Stage the file <lion-and-mouse.txt> to make it available for commit._**
- git add lion-and-mouse.txt

**<ins>Ques:-</ins> _It is good that the file is untracked. But it is still under GIT's radar. If you run the "git add ." command accidentally git will start to track this file. Let's configure git to ignore this file permanently._**
- echo note.txt >> .gitignore

**<ins>Ques:-</ins> _What files are configured to be ignored by this repository?_**
- cat .gitignore

**<ins>Ques:-</ins> _The repository has many commits. Can you try to list the last 3 commits alone?_**
- git log -n 3

#  What this command do ```git log```?
- Display the commit history.
 <img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/a1ba8bd1-bb28-4265-9261-e0264eac63f3" width="600" background-size="cover"/>

#  What this command do ```git log --name-only```?
- The ```git log --name-only``` command is used to display the commit history but with an additional list of file names that were modified in each commit. 
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/5e2d5ac3-9af6-4267-9029-ebed2ca44598" width="600" background-size="cover"/>

#  What this command do ```git log --oneline```?
- It provides a single-line summary for each commit.
 <img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/754bce93-fd4d-4b72-9a2e-fabc4b68bd00" width="600" background-size="cover"/>

#  What this command do ```git show 26e4fcf```?
- Display detailed information about the commit identified by the hash 26e4fcf.
 <img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/4cc0d806-21c4-4963-a6f9-e34b44e89831" width="600" background-size="cover"/>

# What command is used to count the number of files currently tracked by Git in a Git repository?
```bash 
git ls-files | wc -l
```

# Rollback
- First I create a file and add some data and commit.
- After commit I edit data or add data.
- Before going to staging area [ means don't run ```git add <filename>``` ], I run this command to rollback the file ```git checkout <filename>``` 
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/e7a7d413-0b99-43b1-836a-5796c16f4571" width="600" background-size="cover"/>

# What this command do ```git diff```?
- The ```git diff``` used to see changes that haven't been committed yet [ means don't run ```git add <filename>``` ], showing added, modified, and deleted lines in files.
 <img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/93ed9a1e-8e69-4c08-bf24-60ebff23cc25" width="600" background-size="cover"/>



# What this command do ```git diff --cached```?
- The ```git diff --cached``` It provides a way to see what changes have been staged for the next commit but have not yet been committed. [ means run ```git add <filename>``` but don't run this command ```git commit``` ]
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/bf30eb47-b3cd-4e74-9f66-0a82e1abef56" width="600" background-size="cover"/>

# What this command do ```git restore --staged <filename>```?
- Removes the file from the staging area.
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/ea0a9d5d-7f30-4f5b-85a3-46a8604eaeb3" width="600" background-size="cover"/>


# Previous commit and current commit?
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/715ede7b-9b9c-46c6-a9cc-79f18d26b5e9" width="600" background-size="cover"/>


# revert back to commit and reset?
<img src="https://github.com/Krishna-Gopal-Pathak/DevOps/assets/142927819/75a321b9-4334-467c-9d38-1b652c76fc92" width="600" background-size="cover"/>

