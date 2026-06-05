# Git_Learning
I just have learned about the git na fthe github. How to use thw git in the real world projects and keep track of them and puah the code to the github.




# **INTODUCTION**:

>  **Git** is ==a distributed version control system that tracks changes in computer files and coordinates work among multiple developers==. It functions like a "checkpoint" or snapshot system, allowing you to save different versions of your project, collaborate without overriding others' work, and easily revert to previous states if mistakes occur.

>  ==**Linus Torvalds**==, the creator of the Linux operating system, created Git in **April 2005**.

>  The Linux kernel development team had been using a proprietary source control tool called ==**BitKeeper**==. When a licensing dispute occurred and the tool's free-of-charge status was revoked, Torvalds needed a new tool immediately
![[Git.png]]


## **Git Init:**  
   
  >The `git init` command is used to initialize a new repository. The instructor emphasizes that this should only be run **once per project** to create the necessary hidden `.git` directory, which houses the repository's internal tracking mechanisms. 

## **Tracking Status:** 

  >By using `git status`, you can verify whether a folder is being tracked by Git. After initialization, the output changes from an error message to a confirmation that the directory is now under Git's management .

## **Workflow Philosophy:**
   
  >The core takeaway is that Git is a powerful tool for managing version history, and understanding these foundational commands allows developers to maintain clean and reliable project workflows without needing to rely on trial-and-error. 
# **Git Commit and Log:**


![[git intro.png]]

![[git initiatio preccess.png]]

## **Before Commit:** 

> Before you can commit you have to initialise the directory you are going to tell hit to track so just run
```sh
git init 
```
> after that you run 
```sh
git status 
```
> You make a habit to run this command `git status` to run this command often to see what are you doing and what is you error and everything.

> Then you have to add the file in the git staging area 
```sh 
git add .
```
for add evrything in the staging area 

- To add the files you are want to add in the area run 
```sh 
git add filename1 filename2 
```

- then commit the file 
```sh 
git commit 
```

### git add user.name:
```sh
    git config  --global user.name "user_name"
```

### git add user.mail:
```sh
    git config  --global user.email "usser_mail"
``` 

### change the code editor from git commit:
   
  > because the default code editor for the git commiit command is vim and it will be little bit hard to understand and to code in that editor. So we will use the visual studio code.

```sh
    git config --global core.editor "code --wait"
``` 

![[gitlog.png]]


## **COMMIT:** 
		
>   git commit -m "a good descriptive message
    git status
    Repeat 2-3 times
    git log of commits with commit hash)

## **ATOMIC COMMIT:** 
   >keep commits centric to one feture, one component or
   >
   >on fix. Focused on one thing		
   >> 
   >> 1. Present or Past coummit message
   >> 2. Depends {Present Tense, Imperative}
   >> 3. give order to code base
   >> 4. Don't Care

   ```sh 
   git config -- global code. editor " code git-- wait"
   ```
   >>(for configuration file )
   >>change default editor to Vs Code


![[git commit.png]]



## **gitlog:**

> it shows the git trakeing info like your user.name, user.mail and the 
  commit id something like `421425b538ca1b26538480649881233d3dd7a5a8`

there is a command called the 
```sh
git log --oneline
```

it just show the less info that you vscode and other git graph visualizer will show you and that will be enough for you. 

# **gitingnore:**

> the gitignore is the file which the git does not keep track.

> to use the gitignore you have to create a file called `.gitignore`
  or you can just write the command 

```sh
touch .gitignore
```

> then in the file you have to write the file names in the directory that you are willing not to keep track by the git 

# **Branch:**

## master branch:

>   This is thee branch which is created at the start when you init a directory. 

![[Brach.png]]

to see all the branches
```sh
git branch 
```

## **New Brach:**

to make a new branch
```sh 
git branch branch_name
```

to go to the branch 
```sh
git checkout branch_name
```

  > You can work on the different branches and without interfering into another. This is very helpful when working in a team or working in a very big own project (like website, app, etc)

  > Like when you are in your master branch it will not show you the file of your other branches so you can do the work hassal free. 
  
![[git_branch_command.png]]  

## **Git Brach Merge:**




![[Git_branch_merge_concept.png]]


