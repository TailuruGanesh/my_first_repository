
## What is GIT ?
Git is an Open Source tool for tracking my files in the project repository.  Its one of the Version Control Systems (VSC). Its used for Source Code management. 

## What is GITHUB?
TODO, how is it related to GIT


### GITHUB Alternatives
TODO atleast 4

### GIT Alternatives
TODO , its a VCS 2



## GIT Configuration:

To track who did the changes to the files, so we need to set Git username, email. 
To push the files to a remote (a server where our source code is hosted/stored) we also need to set up the authentication method to that remote hosting. (Example : GitHub)

```bash
 git config --global user.email "you@example.com"
 git config --global user.name "Your Name"

```

## GIT Commands
### Help
 `git --help` is used to get a description of all the major commands of git

### Clone

### Initialization:
`git init` is used to Initialize an empty Git repository in current directory. 
- It'll create a directory called `.git` in my current directory. 
- Wherever the `.git` directory exist, it is considered as the root of the project. 
- the `.git` folder contains files that are required for the git software to track the project files (.i.e., our source code)

### Status:
`git status` is used to  check the status of my current source code with my git repo. 
- It contains
	- current branch that we are working on , 
	- new commits yet to be pushed to remote,
	- Changes not staged for commit,
	- Untracked files, 
	- Changes to be committed.

### Add to Tracking
`git add` is used to add files to git tracking, until we add the new files using this command , they are not tracked by our git.
#### Add Single File
`git add <FILE_NAME>` 

#### Add All Files that are new or has changes
`git add .`  or `git add -A`  where -A is for ALL








### Commit

`git commit` is used to commit files with changes to a repository.
#### GIT Commit Message:
After every git commit we need to mention why we are doing the commit, I mean why we are backing up the files at the point.  

For example, I wrote a program which has 5 steps, I completed my program till 3rd step after a lot of trail and error , and now till my step3 my program is proper , I want to make sure that my code is till now is safe and secure. so I'll do a commit with message as 'working code till step 3' so incase I do some mess up in later stages I can always come back to my commit and continue from there. 

Usually the `git commit`  command, opens an editor for us to enter a message , we can skip this two step process by adding the message to `git commit` command like
	`git commit -m 'Message_HERE'` . 



### History (Log)
`git log` is used to see changes in the git repository


### Switch to a branch

`git checkout <branch_name>` is used to switch to an existing branch in the git repo 

- if we want to create a new branch if there is no branch existing then we used the command with an argument to the parameter `-b` 
	`git checkout -b <new_branch_name>` 
	This will create a new branch from current branch (latest changes from current branch)
- If you want to create new branch from existing branch
	`git checkout -b <new branch name> <existing branch name>`
- If you want to create a new branch from an existing commit
	`git checkout -b <new branch name> <existing commit id/hash>`
	you can get commit id/hash from `git log` command.


### List Branches

 `git branch -a` is used to list all branches available locally



### PUSH

#### force push 
### Fetch
- Only fetches the tracking information from Remote and stores in local for comparision but automatically merge it with corresponding local branch
### Merge

Merges the files that are fetched to current local branch
### Pull

Pull will do two commands at once, that is Fetch + Merge

### Fetch


### Add Remote 
`git remote add origin <remote hosted repo url that ends with .git>`

where `git remote add` is the command , `origin` is the name(varaible ) for the remote we assigned , it can be anything. we need to give this name to remote because we can add multiple remotes. 




