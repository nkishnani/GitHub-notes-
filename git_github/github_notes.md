# Git & [Github](https://github.com) 

Many thanks to [Brian Hung](https://github.com/brianhung) for his help in navigating both Git and Markdown. This is being edited on [Typora](https://typora.io), a minimalist Markdown editor.



![Image](https://spin.atomicobject.com/wp-content/uploads/20171003153036/github-logo.png)



## What is Git?

- Git is a **DVCS**, or distributed version control software. Git allows developers to keep track of different versions of their code, enabling them to revert back to previous versions if needed. Further, Git is useful for software collaboration as all contributors to a project are able to view all changes that other developers are making in real time. 
- A recent [StackOverflow poll](https://insights.stackoverflow.com/survey/2018/) found that Git is used by ~70% of developers worldwide, making it the most popular DVCS. 
- Version control software is used to enhance the software development environment. When multiple people are working on several files for a project, there is a high likelihood for overlapping work and a lack of clarity on responsibilities. Git aims to fix this.
- Git does this by allowing for all developers in a project to be able to see all changes being made to the files in the project, or **respository**. All changes are tracked via Git, and versions of the files can be seen or reverted to at all times.

## What is GitHub?

*This is a question that I had for many months* 😛

- GitHub is a hosting platform for Git repositories (folders of files that are tracked via Git).
- Using GitHub you can make new projects, add contributors, and efficiently develop your codebase.
- GitHub has also branched off into other sectors - for example, GitHub pages allows you to maintain a website (HTML code) by committing and pushing changes directly from a GitHub repository (i.e. *your_ website_name*.github.io)



### The Basics

- To review, Git is a version control protocol, and GitHub is a server to host projects that are being tracked via Git. 

- Version control via Git is a 3-step process: staging,  committing, and pushing. 

  ![image](https://github.com/nkishnani/Notes/blob/master/git_github/git_work_flow.png)



  - When **staging**, you are indicating to Git that the file(s) being staged has changes that are going to need to be tracked. 
  - When **committing**, you are documenting the changes made and saving the current version of the file.
  - When **pushing**, you are uploading the commits you have made to a server (either locally or more commonly, to GitHub).

## Branches : The backbone of the GitHub workflow

![image](https://wac-cdn.atlassian.com/dam/jcr:83323200-3c57-4c29-9b7e-e67e98745427/Branch-1.png?cdnVersion=jw)



- Branching are the essence of collaboration in the Git and GitHub environment. Imagine you're working with a partner on a file. Your partner can make their own branch (copy of the current state of the file, like the green nodes) and begin working on their portion of the project. Once they have completed their work, you both can look it over and decide to `merge`	and update the state of the main file.
- Branches can be created for each collaborator, and each branch and its contents (commits) can be seen by all other collaborators.



### Forks and Pull Requests

<p align="center">
  <img src="https://github-images.s3.amazonaws.com/help/bootcamp/Bootcamp-Fork.png">
</p>

- If you want to make a copy of someone else's repository but don't want to changes that you make to be reflected on the original you can **fork** the project. 
- Once you are done tinkering with the project and you want to propose the changes you amde to the author, you can file a **pull request**, which informs the author of the changes and gives them the option to include your commits in the original project. 
- Forks and pull requests illustrate yet another feature within GitHub that streamlines collaboration in software development. 



## Setting up Git & GitHub on your computer

There are two options available for using Git / GitHub on your computer:

1. Install [GitHub for Desktop](https://desktop.github.com). 
   - GitHub for Desktop allows you to pull from, edit, and push to repositories stored in GitHub. 
   - This option does not require the use of the command line, and therefore the next section is not needed for you to use GitHub.
2. Open your terminal.
   - `git config --global user.email [**YOUR EMAIL**]` 
   - `git config --global user.name [**YOUR DISPLAY NAME**]`

## The Command Line

- `git init` : allows the working directory to be tracked via Git.



- `git add` : serves as the staging command. Adding a file indicates that these changes are about to be committed to the branch you are in.



- `git commit -m "<COMMIT MESSAGE>"`: commits the changes to the files currently staged and links it with a message detailing the changes. Commits are tracked like checkpoints on the current branch you are working on.



- `git status`: gives a breakdown of the files currently staged, and the files that have been altered but not committed yet. 



- `git log`: gives a breakdown of times and meesages of each commit on the branch you are working on.



- `git diff`: gives a breakdown of the differences between the file you are currently working and the state of that file based on the last commit.


- `git branch <NEW BRANCH NAME> : creates new branch 
    - `git branch -a`: lists all local branches within the current repository.

- `git checkout <BRANCH NAME>`: switches to specified branch.

    - `git checkout -b <NEW BRANCH NAME> : creates new branch and switches to it 
    - `git checkout -b <NEW BRANCH NAME> <EXISTING BRANCH NAME> : creates new branch with specific HEAD and checks it out

- `git merge <MERGING BRANCH NAME>`: merges current branch with specified branch.

- `git fetch`: gets the latest changes from origin repo without merging.

- `git pull`: get the latest changes from origin repo and merges them.

- `git rest <FILE NAME>`: unstages file but retains changes.

- `git reset --hard`: reverts everything to state at last commit.

- `git status` : allows you to check which branch you are currently as well as how current the current branch is in relation to the HEAD (where you branched off of)

- `git log` : gives record of commits on current branch

## More resources

- [Git Cheat Sheet ](http://files.zeroturnaround.com/pdf/zt_git_cheat_sheet.pdf)

- [Harvard's CS50 lecture on Git](https://www.youtube.com/watch?v=MJUJ4wbFm_A)
