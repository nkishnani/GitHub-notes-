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




## Branches : The backbone of the GitHub workflow







## Setting up Git & GitHub on your computer

There are two options available for using Git / GitHub on your computer:

1. Install [GitHub for Desktop](https://desktop.github.com). 
   - GitHub for Desktop allows you to pull from, edit, and push to repositories stored in GitHub. 
   - This option does not require the use of the command line, and therefore the next section is not needed for you to use GitHub.
2. Open your terminal.
   - `git config --global user.email [**YOUR EMAIL**]` 
   - `git config --global user.name [**YOUR DISPLAY NAME**]`

## The Git workflow & command-line commands for Git 

![image](https://github.com/nkishnani/Notes/blob/master/git_github/git_work_flow.png)



- `git init` : allows the working directory to be tracked via Git.
- `git add` : serves as the staging command. Adding a file indicates that these changes are about to be committed to the branch you are in.
- 



## More resources

- [Git Cheat Sheet ](http://files.zeroturnaround.com/pdf/zt_git_cheat_sheet.pdf)

- [Harvard's CS50 lecture on Git](https://www.youtube.com/watch?v=MJUJ4wbFm_A)
