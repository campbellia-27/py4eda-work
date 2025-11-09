# HW3A Solution - Git and Version Control
## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to
`~/insy6500/class_repo`.
6
### Key Commands Used
- `git clone <url>` - Create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections
## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files# HW3A Solution - Git and Version Control
## Part 1: Repository Cloning
I successfully cloned the class repository from `https://github.com/olearydj/INSY6500` to
`~/insy6500/class_repo`.
6
### Key Commands Used
- `git clone <url>` - Create local copy of remote repository
- `git log` - View commit history
- `git remote -v` - Check remote repository connections
## Part 2: Portfolio Repository Creation
I created my personal course repository with:
- Professional README.md describing the project
- Proper .gitignore to exclude unnecessary files
- Organized directory structure for homework, projects, and notes
### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`
## Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub
### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)
### Details
Complete this section with details from your setup:
- Repository URL: https://github.com/campbellia-27/py4eda-work
- Output of `git remote -v`: origin  https://github.com/campbellia-27/py4eda-work.git (fetch)
origin  https://github.com/campbellia-27/py4eda-work.git (push)
- The output of `git log --oneline`: 1b51362 (HEAD -> master, origin/master) Add empty folders with .gitkeep
b4c2109 Updated hw3a-solution with final edits
c68b59e Complete Part 3 documentation
d52b607 Add hw3a solution document
70bb0ba Initial commit: Add README and .gitignore

## Questions
### Reflections
#### **Question 1:**
Git Workflow Benefits You’ve now experienced the basic Git workflow: edit
files, stage changes, commit with messages, and push to GitHub.

a) Before this assignment, how did you typically manage different versions of your work (e.g.,
assignments, code, documents)? Compare that approach to using Git. What are 2-3 specific
advantages Git provides?
- Before this assignment, I was manually saving every time I made a change to code. This led to having many versions of the same code saved in one project folder. Although this is a way to save code over time, it becomes disorganized very quickly, and if you forget to save an od version, you could be in big trouble if you change your code and it fails to run. With git, there are many advantages that outweigh what I was doing before:
1. With Git, all changes made to your code can quickly be found because git has a history of all the commits you have made during your project.
2. Git also allows you to work on the same project as someone else without overwriting changes. This makes it very good for collaboration, and I know that many of my friends in computer science utilize git and git hub for group projects.
3. This advantage is similar to the first one listed but it allows for more clarity on how changes have been made over time. This makes it easy to address questions about research and how you might have learned something over time.

b) Describe a situation from your academic or professional work where Git’s commit history
would have been valuable. What problem would it have solved?
- Over the summer, I created a data analysis tool for the tutoring center. I was completely new to coding, and I had no idea about git. As a result, I was having to save new versions of my code every time I made updates. Often, I would be lazy and not save my changes. There were multiple times, where I changed my code, but the changes were invalid, and I could not go back and find my old working code. Going forward, I will absolutely use git.
#### **Question 2: Repository Organization**
You now work with two repositories that serve different purposes:
- class_repo - cloned from the instructor, read-only reference
- my_repo - your own work, pushed to GitHub  

a) Explain why it’s important to keep these separate. What would happen if you tried to put everything in one repository

- It's important to keep these repos seperate, because the class repo is read-only and has a different use than my_repo, which allows me to push to my own git hub. I imagine if you tried to put everything into one repository it could cause conflicts between the two and files from one could be overwritten.

b) Think about your future coursework or projects. Describe how you might organize multiple
repositories. For example, how would you handle a group project versus individual assign-
ments versus reference material?

- For reference materials, I would probably create one repo, like the class_repo we create for this assignemnt, with all of my read only files. If there is a lot of information on the subject or specific project, I may include it within my project repo.
- For individual assignments, I would create a new repo for each assignment, so I could easily track changes and keep the assignments seperated.
- Finally, for group projects, I would have a group repository that everyone could push and pull from to make sharing files easy. Also, branches could be added for more specific work.

#### **Question 3: Commit Messages and History**
Look at the commit messages you wrote during
this assignment (use git log --oneline if needed).

a) Compare these two commit messages:  
• “update”  
• “Add hw3a solution documenting Git workflow and repository structure”  
Which is more useful? Why? When might you need to find this commit again in the future?  
- The second message is much more useful, because it describes exactly what change was made, but the other one just says update with zero context around what the update actually was. In the future, if I want to know when I added homework 3a and why, I have access to it.  

If you would like to learn more about best practices for these important messages, you might be
interested in:  
• The Conventional Commits specification - a popular convention where commits start with
prefixes like feat:, fix:, docs: to enable automation  
• How to Write a Git Commit Message - a comprehensive guide to writing effective commit
messages

b) Imagine you’re working on a data analysis project over several weeks. Describe how you would
decide when to make a commit. What makes a good “unit of work” for a single commit?  
- That's a tough question to answer, but I would commit changes anytime I make changes to the code that work. If the change causes bugs, you probably wouldn't want to commit that, but if your change advances the project and works correctly I see no reason why it shouldn't be committed. This could be something as simplye as creating a new 20 line function of code.

### **Graduate Questions**
#### **Question 1: The Three-Stage Model Git uses three stages:**
Working Directory → Staging Area → Repository. Many version control systems skip the staging area and commit all changes directly.
Without a staging area, you’d have to commit everything at once with a message like “various
updates” - making it hard to understand your history later. The staging area lets you review and
organize your changes before committing, creating a clean, understandable history where each
commit represents one logical change.  

a) Think about the work you did in this assignment. You created README.md, .gitignore, and
hw3a-solution.md. Why was it valuable to commit the README and .gitignore together
first, then commit hw3a-solution.md separately later? What would have been lost if you’d
committed everything  

- It was valuable to commit README and .gitignore together because they are both part of setting up the project. If I included hw3a-solution, it would make it more difficult to find where the assignment setup ended and where the actual assignment work started. Now, this is easy because the commits are seperated.

b) Imagine you’re working on a homework assignment over several days. You:  

• Write code to load data  

• Start working on a new analysis function (half-finished)  

• Fix a typo in a comment  

• Update your README  

Which of these changes should you commit now, and which should you wait on? Why? How
does staging help you make this decision  

- I would start by committing the code to load data, the fixed typo, and the updated README. I would start with these, because they are all complete and finished. I would most likely avoid committing the half finished analysis function, since committing something incomplete might add confusion later. Staging helps with this decision because it allows me to specify which files go into each commit instead of all of them at once.

c) Explain how git status helps you make decisions about what to stage and commit. When
in your workflow should you use it?  

- git status lets the user see everything that is currently in their repository including what has been modified and staged. In doing so, it allows you to get an idea of what might need to be updated in you repository if something hasn't been updated or clearly shown prior to your commit. This will allow you to make sure you haven't left anyhing important out of your repository.

#### **Question 2: Local vs. Remote Repositories**
You experienced both local repositories (on your computer) and remote repositories (on GitHub).  

a) Git is described as a “distributed” version control system. Based on your experience with
class_repo and my_repo, explain what this means. How is it different from just storing files
in Google Drive or Dropbox?  

- I think it is different because if you update a file in dropbox or google drive, because it overwrites the file for everybody. However, with git, you have the ability to control what you choose to commit or update. Also, this is all done locally with Git, whereas google drive and dropbox use the cloud. This allows me to make changes on my computer and push them to github when I am ready. To do this on drive or dropbox, you would have to download a local copy, change it, then reupload the updated version as a new file.

b) You can work on your local repository (my_repo) even without an internet connection - making
commits, viewing history, etc. Then later you can git push to sync with GitHub. Explain
why this architecture is valuable for developers. What workflows does it enable?  

- This architecture is valuable to the developer because it allows them to work anywhere as long as they have access to their computer. As a result, they don't need an internet connection and could make updates in a variety of unique situations. If there is a group development project, the team can split up the work among the different branches of the repository and work locally, and once they have created their code, they can push it to github and pull other developers' work.

c) Describe the relationship between git clone, git pull, and git push. Why can you pull
from class_repo but not push to it, while your my_repo allows both  

- git clone creates a full copy of the remote repository from github on my local device. This lets me update it and pull changes from guthub or push my changes to the repository on github. This does not work for the class_repo, because it is a read only repo that we are not authorized to push to.

#### **Question 3: Professional Portfolio**
You’ve created a public repository on GitHub that will 
be visible to potential employers or collaborators.  

a) Throughout the remainder of this course, you’ll add more work to this repository. What
should you consider when deciding what to commit? How do you balance showing your work
process (including mistakes and iterations) versus presenting polished final product?  

- This is an interesting question and something that I have already been thinking about. When deciding what to commit, I will consider the amount of work it took me as well as the difficulty level. If a code change is small and somewhat trivial, I will most likely avoid committing it. When I am trying to show a balanced work process, I think it is okay to show mistakes, but the mistake as well as why it is important should be clearly explained in the repository. Overall, I would want it to accurately depict my learning process, without showing any disorganization or lack of effort in my work.  

b) Your README.md is the first thing people see when they visit your repository. What makes
a README effective for a portfolio repository versus a README for an open-source project
someone might want to use?  

- I think for a portfolio repository it is important to answer the higher level questions of why you made the code, what problem it solves, and what you learned during the process. This is because your github repository should show personal growth to outside observers. For an open-source project readme, you will be communicating information to other developers. As a result, it should probably be more technical and focused on how the code actually operates as well as how it can be improved.

c) Reflect on the value of building this public portfolio during your coursework rather than
waiting until you’re job searching. What habits should you develop now to make this portfolio
valuable later?  

- The value of building the repository now is that I can more accurately depict what I have done and what I am working on currently. It would be much more difficult to do this at some later date, because I may not have a handle on what I did. By working on it now, I can continuously improve and refine it to make it look good for future employers. In regard to good habits, I should create clear commits, update readme files, and create clear comments throughout my code.
- Organized directory structure for homework, projects, and notes
### Understanding Git Workflow
The three-stage workflow:
1. Working Directory: Where I edit files
2. Staging Area: Where I prepare commits with `git add`
3. Repository: Where commits are permanently stored with `git commit`
## Part 3: GitHub Publishing
Successfully published repository to GitHub:
- Used `git remote add origin` to connect local repo to GitHub
- Used `git push -u origin main` to upload commits
- Verified all files and commits are visible on GitHub
### The Remote Connection
My local repository is now connected to GitHub:
- `git remote -v` shows the remote URL
- `git push` will send my commits to GitHub
- `git pull` will get updates from GitHub (if changes are made on GitHub)
### Details
Complete this section with details from your setup:
- Repository URL: ...
- Output of `git remote -v`:
- The output of `git log --oneline`:
## Questions
### Reflections
#### **Question 1:**
Git Workflow Benefits You’ve now experienced the basic Git workflow: edit
files, stage changes, commit with messages, and push to GitHub.

a) Before this assignment, how did you typically manage different versions of your work (e.g.,
assignments, code, documents)? Compare that approach to using Git. What are 2-3 specific
advantages Git provides?
- Before this assignment, I was manually saving every time I made a change to code. This led to having many versions of the same code saved in one project folder. Although this is a way to save code over time, it becomes disorganized very quickly, and if you forget to save an od version, you could be in big trouble if you change your code and it fails to run. With git, there are many advantages that outweigh what I was doing before:
1. With Git, all changes made to your code can quickly be found because git has a history of all the commits you have made during your project.
2. Git also allows you to work on the same project as someone else without overwriting changes. This makes it very good for collaboration, and I know that many of my friends in computer science utilize git and git hub for group projects.
3. This advantage is similar to the first one listed but it allows for more clarity on how changes have been made over time. This makes it easy to address questions about research and how you might have learned something over time.

b) Describe a situation from your academic or professional work where Git’s commit history
would have been valuable. What problem would it have solved?
- Over the summer, I created a data analysis tool for the tutoring center. I was completely new to coding, and I had no idea about git. As a result, I was having to save new versions of my code every time I made updates. Often, I would be lazy and not save my changes. There were multiple times, where I changed my code, but the changes were invalid, and I could not go back and find my old working code. Going forward, I will absolutely use git.
#### **Question 2: Repository Organization**
You now work with two repositories that serve different purposes:
- class_repo - cloned from the instructor, read-only reference
- my_repo - your own work, pushed to GitHub  

a) Explain why it’s important to keep these separate. What would happen if you tried to put everything in one repository

- It's important to keep these repos seperate, because the class repo is read-only and has a different use than my_repo, which allows me to push to my own git hub. I imagine if you tried to put everything into one repository it could cause conflicts between the two and files from one could be overwritten.

b) Think about your future coursework or projects. Describe how you might organize multiple
repositories. For example, how would you handle a group project versus individual assign-
ments versus reference material?

- For reference materials, I would probably create one repo, like the class_repo we create for this assignemnt, with all of my read only files. If there is a lot of information on the subject or specific project, I may include it within my project repo.
- For individual assignments, I would create a new repo for each assignment, so I could easily track changes and keep the assignments seperated.
- Finally, for group projects, I would have a group repository that everyone could push and pull from to make sharing files easy. Also, branches could be added for more specific work.

#### **Question 3: Commit Messages and History**
Look at the commit messages you wrote during
this assignment (use git log --oneline if needed).

a) Compare these two commit messages:  
• “update”  
• “Add hw3a solution documenting Git workflow and repository structure”  
Which is more useful? Why? When might you need to find this commit again in the future?  
- The second message is much more useful, because it describes exactly what change was made, but the other one just says update with zero context around what the update actually was. In the future, if I want to know when I added homework 3a and why, I have access to it.  

If you would like to learn more about best practices for these important messages, you might be
interested in:  
• The Conventional Commits specification - a popular convention where commits start with
prefixes like feat:, fix:, docs: to enable automation  
• How to Write a Git Commit Message - a comprehensive guide to writing effective commit
messages

b) Imagine you’re working on a data analysis project over several weeks. Describe how you would
decide when to make a commit. What makes a good “unit of work” for a single commit?  
- That's a tough question to answer, but I would commit changes anytime I make changes to the code that work. If the change causes bugs, you probably wouldn't want to commit that, but if your change advances the project and works correctly I see no reason why it shouldn't be committed. This could be something as simplye as creating a new 20 line function of code.

### **Graduate Questions**
#### **Question 1: The Three-Stage Model Git uses three stages:**
Working Directory → Staging Area → Repository. Many version control systems skip the staging area and commit all changes directly.
Without a staging area, you’d have to commit everything at once with a message like “various
updates” - making it hard to understand your history later. The staging area lets you review and
organize your changes before committing, creating a clean, understandable history where each
commit represents one logical change.  

a) Think about the work you did in this assignment. You created README.md, .gitignore, and
hw3a-solution.md. Why was it valuable to commit the README and .gitignore together
first, then commit hw3a-solution.md separately later? What would have been lost if you’d
committed everything  

- It was valuable to commit README and .gitignore together because they are both part of setting up the project. If I included hw3a-solution, it would make it more difficult to find where the assignment setup ended and where the actual assignment work started. Now, this is easy because the commits are seperated.

b) Imagine you’re working on a homework assignment over several days. You:  

• Write code to load data  

• Start working on a new analysis function (half-finished)  

• Fix a typo in a comment  

• Update your README  

Which of these changes should you commit now, and which should you wait on? Why? How
does staging help you make this decision  

- I would start by committing the code to load data, the fixed typo, and the updated README. I would start with these, because they are all complete and finished. I would most likely avoid committing the half finished analysis function, since committing something incomplete might add confusion later. Staging helps with this decision because it allows me to specify which files go into each commit instead of all of them at once.

c) Explain how git status helps you make decisions about what to stage and commit. When
in your workflow should you use it?  

- git status lets the user see everything that is currently in their repository including what has been modified and staged. In doing so, it allows you to get an idea of what might need to be updated in you repository if something hasn't been updated or clearly shown prior to your commit. This will allow you to make sure you haven't left anyhing important out of your repository.

#### **Question 2: Local vs. Remote Repositories**
You experienced both local repositories (on your computer) and remote repositories (on GitHub).  

a) Git is described as a “distributed” version control system. Based on your experience with
class_repo and my_repo, explain what this means. How is it different from just storing files
in Google Drive or Dropbox?  

- I think it is different because if you update a file in dropbox or google drive, because it overwrites the file for everybody. However, with git, you have the ability to control what you choose to commit or update. Also, this is all done locally with Git, whereas google drive and dropbox use the cloud. This allows me to make changes on my computer and push them to github when I am ready. To do this on drive or dropbox, you would have to download a local copy, change it, then reupload the updated version as a new file.

b) You can work on your local repository (my_repo) even without an internet connection - making
commits, viewing history, etc. Then later you can git push to sync with GitHub. Explain
why this architecture is valuable for developers. What workflows does it enable?  

- This architecture is valuable to the developer because it allows them to work anywhere as long as they have access to their computer. As a result, they don't need an internet connection and could make updates in a variety of unique situations. If there is a group development project, the team can split up the work among the different branches of the repository and work locally, and once they have created their code, they can push it to github and pull other developers' work.

c) Describe the relationship between git clone, git pull, and git push. Why can you pull
from class_repo but not push to it, while your my_repo allows both  

- git clone creates a full copy of the remote repository from github on my local device. This lets me update it and pull changes from guthub or push my changes to the repository on github. This does not work for the class_repo, because it is a read only repo that we are not authorized to push to.

#### **Question 3: Professional Portfolio**
You’ve created a public repository on GitHub that will 
be visible to potential employers or collaborators.  

a) Throughout the remainder of this course, you’ll add more work to this repository. What
should you consider when deciding what to commit? How do you balance showing your work
process (including mistakes and iterations) versus presenting polished final product?  

- This is an interesting question and something that I have already been thinking about. When deciding what to commit, I will consider the amount of work it took me as well as the difficulty level. If a code change is small and somewhat trivial, I will most likely avoid committing it. When I am trying to show a balanced work process, I think it is okay to show mistakes, but the mistake as well as why it is important should be clearly explained in the repository. Overall, I would want it to accurately depict my learning process, without showing any disorganization or lack of effort in my work.  

b) Your README.md is the first thing people see when they visit your repository. What makes
a README effective for a portfolio repository versus a README for an open-source project
someone might want to use?  

- I think for a portfolio repository it is important to answer the higher level questions of why you made the code, what problem it solves, and what you learned during the process. This is because your github repository should show personal growth to outside observers. For an open-source project readme, you will be communicating information to other developers. As a result, it should probably be more technical and focused on how the code actually operates as well as how it can be improved.

c) Reflect on the value of building this public portfolio during your coursework rather than
waiting until you’re job searching. What habits should you develop now to make this portfolio
valuable later?  

- The value of building the repository now is that I can more accurately depict what I have done and what I am working on currently. It would be much more difficult to do this at some later date, because I may not have a handle on what I did. By working on it now, I can continuously improve and refine it to make it look good for future employers. In regard to good habits, I should create clear commits, update readme files, and create clear comments throughout my code.
13
ts??
ision?ng at once?terials?ved?
